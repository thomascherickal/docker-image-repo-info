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
$ docker pull buildpack-deps@sha256:498c3e1c24d8bf3c692c0ed7d8afeaba649e5990abea41ce76bc88a5144f7c3e
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
$ docker pull buildpack-deps@sha256:2608204439da09756cf236495eabd8abf170fee83470c3afdb8caa3ceb104ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.1 MB (272077462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982da4d9dfdd4bd047eb685a31015aa7dd1f57402c4e78d9fe24f42a1d82eb21`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:02 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:10 GMT
ADD file:9e750ebbbf7e47a121d153e6699006776ea61b04b6c8e31556600483a020f617 in / 
# Wed, 11 Oct 2023 18:03:10 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 06:17:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:21:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b743c812db4b2a4cb933b4107dd5408c786d034c3bcff4d162d02e20587dce07`  
		Last Modified: Fri, 13 Oct 2023 06:40:38 GMT  
		Size: 27.3 MB (27340045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e717ff89b8bce5f5201b6827c6ed6615c39f2b52f5b0e8ca3d659d049b51e6`  
		Last Modified: Wed, 15 Nov 2023 06:23:55 GMT  
		Size: 9.6 MB (9645467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3cadc26010e0f011e17572f55422b03f3cc9dd1729864eba62145f0aeacf76`  
		Last Modified: Wed, 15 Nov 2023 06:24:12 GMT  
		Size: 45.0 MB (44982339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651e35dbc14e3494cc43e42663e48327f408cfde12d19c632c44377b1654e9a1`  
		Last Modified: Wed, 15 Nov 2023 06:24:41 GMT  
		Size: 190.1 MB (190109611 bytes)  
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
$ docker pull buildpack-deps@sha256:2c2946cb3e2a5c8a960b0c37413e3ff648f830a750a8ee2b3553ac1257c9638c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.0 MB (257957931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce82b60021dc7fb1c62212e9c71ec596bd448c6623a4d6188ca2df6fe8d956b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:34 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:36 GMT
ADD file:8ceb0028af8276b03b6c88b19445f30165a41791919c756e1434da6ded4387db in / 
# Wed, 11 Oct 2023 18:03:36 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:24:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:27:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:82cdc38d6d4a8f105e5928c09fada25b62831433ea5f6e4c51bda4c9ecbd9702`  
		Last Modified: Wed, 15 Nov 2023 05:29:56 GMT  
		Size: 27.6 MB (27617854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25054bfcd5aaaaab9a8b81261f4b5a2752bc79e2ef9670be2543ea4ca8151408`  
		Last Modified: Wed, 15 Nov 2023 05:29:53 GMT  
		Size: 9.7 MB (9696878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692f488bb8b766464b4e25f6f72ccf92efc432f0c10df1d1003061838b729d85`  
		Last Modified: Wed, 15 Nov 2023 05:30:09 GMT  
		Size: 45.6 MB (45572317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b65bd5cf9be92580539ab8bd5dce75b179cc8d5b9be1a70fa8247b133f4a0d`  
		Last Modified: Wed, 15 Nov 2023 05:30:35 GMT  
		Size: 175.1 MB (175070882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10-curl`

```console
$ docker pull buildpack-deps@sha256:fdd84b5fb072cd9015e72499e405b6c2ee6071d354e22f49309744b75abe40a0
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
$ docker pull buildpack-deps@sha256:d649d5fa7ae482f135330be776368c49ff5d30b7336734c39ad94af9a6064874
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36985512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16ce70cb7143b41128b73de1bc7c1520314ceae722ab6e435381a4fd31188a78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:02 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:10 GMT
ADD file:9e750ebbbf7e47a121d153e6699006776ea61b04b6c8e31556600483a020f617 in / 
# Wed, 11 Oct 2023 18:03:10 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 06:17:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b743c812db4b2a4cb933b4107dd5408c786d034c3bcff4d162d02e20587dce07`  
		Last Modified: Fri, 13 Oct 2023 06:40:38 GMT  
		Size: 27.3 MB (27340045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e717ff89b8bce5f5201b6827c6ed6615c39f2b52f5b0e8ca3d659d049b51e6`  
		Last Modified: Wed, 15 Nov 2023 06:23:55 GMT  
		Size: 9.6 MB (9645467 bytes)  
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
$ docker pull buildpack-deps@sha256:e3fb9abd82bd63f435954245545251574327c9881255d2db0ca53940bda40d64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37314732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64946e8ba5952759944b3513696715ee3fc336e4cb5f02dced4113a84b7fb861`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:34 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:36 GMT
ADD file:8ceb0028af8276b03b6c88b19445f30165a41791919c756e1434da6ded4387db in / 
# Wed, 11 Oct 2023 18:03:36 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:82cdc38d6d4a8f105e5928c09fada25b62831433ea5f6e4c51bda4c9ecbd9702`  
		Last Modified: Wed, 15 Nov 2023 05:29:56 GMT  
		Size: 27.6 MB (27617854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25054bfcd5aaaaab9a8b81261f4b5a2752bc79e2ef9670be2543ea4ca8151408`  
		Last Modified: Wed, 15 Nov 2023 05:29:53 GMT  
		Size: 9.7 MB (9696878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10-scm`

```console
$ docker pull buildpack-deps@sha256:27f45ae4542018ae28469a9738efc4351c50cfbd8ef2638d4e22f131701dbbec
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
$ docker pull buildpack-deps@sha256:cf087be5e86a4c17a523c29b076e9f0fe429f185a1485b4288e664384784dfcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81967851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab16779c759dc820ef4e5a74d5ce02ee78fa337b3a8e604f11ef1f752d8f4001`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:02 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:10 GMT
ADD file:9e750ebbbf7e47a121d153e6699006776ea61b04b6c8e31556600483a020f617 in / 
# Wed, 11 Oct 2023 18:03:10 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 06:17:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b743c812db4b2a4cb933b4107dd5408c786d034c3bcff4d162d02e20587dce07`  
		Last Modified: Fri, 13 Oct 2023 06:40:38 GMT  
		Size: 27.3 MB (27340045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e717ff89b8bce5f5201b6827c6ed6615c39f2b52f5b0e8ca3d659d049b51e6`  
		Last Modified: Wed, 15 Nov 2023 06:23:55 GMT  
		Size: 9.6 MB (9645467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3cadc26010e0f011e17572f55422b03f3cc9dd1729864eba62145f0aeacf76`  
		Last Modified: Wed, 15 Nov 2023 06:24:12 GMT  
		Size: 45.0 MB (44982339 bytes)  
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
$ docker pull buildpack-deps@sha256:a91a88d92cebe1e06032a2e91eca9eed7764f96574bf8209a0e634b723902068
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82887049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f810d9541dc377d4af2da31b65e5188e4419926498729a02895e8664cdb624`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:34 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:36 GMT
ADD file:8ceb0028af8276b03b6c88b19445f30165a41791919c756e1434da6ded4387db in / 
# Wed, 11 Oct 2023 18:03:36 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:24:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:82cdc38d6d4a8f105e5928c09fada25b62831433ea5f6e4c51bda4c9ecbd9702`  
		Last Modified: Wed, 15 Nov 2023 05:29:56 GMT  
		Size: 27.6 MB (27617854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25054bfcd5aaaaab9a8b81261f4b5a2752bc79e2ef9670be2543ea4ca8151408`  
		Last Modified: Wed, 15 Nov 2023 05:29:53 GMT  
		Size: 9.7 MB (9696878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692f488bb8b766464b4e25f6f72ccf92efc432f0c10df1d1003061838b729d85`  
		Last Modified: Wed, 15 Nov 2023 05:30:09 GMT  
		Size: 45.6 MB (45572317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:1fe9f803a37577bc063b88c1ab063c620ebbea8ed3b451b95dde19a19ceaac10
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
$ docker pull buildpack-deps@sha256:227ea9bc7dd964b6592406f4447f91cdaf529d06dbe9980626edf3455d79bc37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316029661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316e91cadc40ed25984ede1f07ab85dbe4913f989cd383e3b3511c486c119a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:42 GMT
ADD file:e217c81e321b5371a29bea20d4b2802fa8223262c92dbffd268ec38c8951181c in / 
# Tue, 21 Nov 2023 05:00:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:14:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:16:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6ffd672cfa56bc540c641f8f5c7b5216716ae5d6336d6698ebdf8fb8cae06e0`  
		Last Modified: Tue, 21 Nov 2023 05:03:32 GMT  
		Size: 47.4 MB (47355729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e04f9270e7bd9277315236c8f83ecc5537fd0907204e9c9f75a2464091a59`  
		Last Modified: Tue, 21 Nov 2023 06:24:19 GMT  
		Size: 22.7 MB (22727407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7466297e667840b4907e1e017052f34ebebba91fb7a476d17a10259cf5a264fc`  
		Last Modified: Tue, 21 Nov 2023 06:24:41 GMT  
		Size: 61.6 MB (61561534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8128c2db4bac59c665360b03846fbc4d0013d87270dad0af442499ef7088c34`  
		Last Modified: Tue, 21 Nov 2023 06:25:23 GMT  
		Size: 184.4 MB (184384991 bytes)  
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
$ docker pull buildpack-deps@sha256:ff34a667d81db5798aaf33085e09a789e13a45e7b48e804c87809631102b0ec7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.0 MB (362952942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b6ecc5afbeef5b86b674ec0993915e6bb01b89f9c44f901050856f10a1bf0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:23:59 GMT
ADD file:209097c8dfcefec7951851d25bc9e8c1d56aefed076c682c5f2e077cc05aeaf8 in / 
# Tue, 21 Nov 2023 04:24:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:53:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:56:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d694a6aceb98c067febf569d227d6249cd8d39b11dead73e4840d07861a25e9`  
		Last Modified: Tue, 21 Nov 2023 04:28:27 GMT  
		Size: 53.6 MB (53575858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71d255e683d12334b12df8a9e23692d03ce5d514a74efe4553f12269885d87`  
		Last Modified: Tue, 21 Nov 2023 07:06:46 GMT  
		Size: 25.7 MB (25698746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a54ea75827017eaea7b7055d8fca97c313c72d7a237502105b83ab018bd5ad`  
		Last Modified: Tue, 21 Nov 2023 07:07:08 GMT  
		Size: 69.6 MB (69584187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e986f224599c525ac40be9636489d408b4daff891bb3567a7986f6ae5c817cc1`  
		Last Modified: Tue, 21 Nov 2023 07:07:49 GMT  
		Size: 214.1 MB (214094151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d1822d31d3c58472a93084eaa39396b37585eb538479e3ca57d5e2e50d7470c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318217378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0dcda8469adc1e80e5b8779671680724ff22c47c0c87e7d0658d100902caa19`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:00 GMT
ADD file:8bb55d91755618d4e84d57150867ddbe9513d01cf9543fa953cf7cd1745397ac in / 
# Tue, 21 Nov 2023 05:04:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:06:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:07:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7318387eb66a53962a6ff8f603919b1f2eebd63059538ee442fb3f3643d79fd1`  
		Last Modified: Tue, 21 Nov 2023 05:10:07 GMT  
		Size: 47.9 MB (47943002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a20203ebe78a0c1643a97475f1f406b6af2dedd0e14005e4ca4bbeca0470d21`  
		Last Modified: Tue, 21 Nov 2023 06:16:17 GMT  
		Size: 24.0 MB (24045086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c99a00cc05c2b6ae13b5a9c1b8997b9915ab687454a9fcd00d485bbb2d9a5d`  
		Last Modified: Tue, 21 Nov 2023 06:16:33 GMT  
		Size: 63.1 MB (63132875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cf7e37f4b53af6dfd3bdea89a2078a221738e8eeade3f46428f3def3e4c97c`  
		Last Modified: Tue, 21 Nov 2023 06:17:01 GMT  
		Size: 183.1 MB (183096415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:d53c880810f72ba3a0b875b502506201f5059fb6649867ded0721135ff0b76f5
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
$ docker pull buildpack-deps@sha256:f8e864b6759c58dd553d3638f996a6918822de02ea1c443cc92559e7e7cfdad4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70083136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f201a632265b71438164333d2c732c7918b180c004463264455c253dcc1afc98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:42 GMT
ADD file:e217c81e321b5371a29bea20d4b2802fa8223262c92dbffd268ec38c8951181c in / 
# Tue, 21 Nov 2023 05:00:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:14:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6ffd672cfa56bc540c641f8f5c7b5216716ae5d6336d6698ebdf8fb8cae06e0`  
		Last Modified: Tue, 21 Nov 2023 05:03:32 GMT  
		Size: 47.4 MB (47355729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e04f9270e7bd9277315236c8f83ecc5537fd0907204e9c9f75a2464091a59`  
		Last Modified: Tue, 21 Nov 2023 06:24:19 GMT  
		Size: 22.7 MB (22727407 bytes)  
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
$ docker pull buildpack-deps@sha256:784282fea3a27c11b3c8668acf83fdf5fa1f805e2c648264766bd6bedda9f057
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79274604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:927ae87f00aa3f0f3b5f1fccbc2848eda2dec7b3d1754259fdd0af08c5485cf4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:23:59 GMT
ADD file:209097c8dfcefec7951851d25bc9e8c1d56aefed076c682c5f2e077cc05aeaf8 in / 
# Tue, 21 Nov 2023 04:24:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d694a6aceb98c067febf569d227d6249cd8d39b11dead73e4840d07861a25e9`  
		Last Modified: Tue, 21 Nov 2023 04:28:27 GMT  
		Size: 53.6 MB (53575858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71d255e683d12334b12df8a9e23692d03ce5d514a74efe4553f12269885d87`  
		Last Modified: Tue, 21 Nov 2023 07:06:46 GMT  
		Size: 25.7 MB (25698746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:56dea1f8a449f195ffdd426569472adfdcbb657344ea182789923be11c8b79f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71988088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba3cde7adf1be7b7277ab9b2cd62cc5ea051cb781184b34e1645be1f946290f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:00 GMT
ADD file:8bb55d91755618d4e84d57150867ddbe9513d01cf9543fa953cf7cd1745397ac in / 
# Tue, 21 Nov 2023 05:04:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7318387eb66a53962a6ff8f603919b1f2eebd63059538ee442fb3f3643d79fd1`  
		Last Modified: Tue, 21 Nov 2023 05:10:07 GMT  
		Size: 47.9 MB (47943002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a20203ebe78a0c1643a97475f1f406b6af2dedd0e14005e4ca4bbeca0470d21`  
		Last Modified: Tue, 21 Nov 2023 06:16:17 GMT  
		Size: 24.0 MB (24045086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:c99b8a43be556e5b407214a5ea1801af92a581294119cc772136046613486699
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
$ docker pull buildpack-deps@sha256:adec01003a17f6b964516dc2082a5c112ef7132fd914810661c01e4fde930972
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131644670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3bc44cf636b514c0c186654ac43d24bd92f970d9fdcd2dca3b0516e058959c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:42 GMT
ADD file:e217c81e321b5371a29bea20d4b2802fa8223262c92dbffd268ec38c8951181c in / 
# Tue, 21 Nov 2023 05:00:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:14:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6ffd672cfa56bc540c641f8f5c7b5216716ae5d6336d6698ebdf8fb8cae06e0`  
		Last Modified: Tue, 21 Nov 2023 05:03:32 GMT  
		Size: 47.4 MB (47355729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e04f9270e7bd9277315236c8f83ecc5537fd0907204e9c9f75a2464091a59`  
		Last Modified: Tue, 21 Nov 2023 06:24:19 GMT  
		Size: 22.7 MB (22727407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7466297e667840b4907e1e017052f34ebebba91fb7a476d17a10259cf5a264fc`  
		Last Modified: Tue, 21 Nov 2023 06:24:41 GMT  
		Size: 61.6 MB (61561534 bytes)  
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
$ docker pull buildpack-deps@sha256:ad518e13047a2bffa7358d6ed80141ee89918b12549d94563fe33dfe97693f63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148858791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1afccc4310e63668ea2fa68e7ed2114f91aa1c4023a673f0dbd3cb0d533ddd7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:23:59 GMT
ADD file:209097c8dfcefec7951851d25bc9e8c1d56aefed076c682c5f2e077cc05aeaf8 in / 
# Tue, 21 Nov 2023 04:24:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:53:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d694a6aceb98c067febf569d227d6249cd8d39b11dead73e4840d07861a25e9`  
		Last Modified: Tue, 21 Nov 2023 04:28:27 GMT  
		Size: 53.6 MB (53575858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71d255e683d12334b12df8a9e23692d03ce5d514a74efe4553f12269885d87`  
		Last Modified: Tue, 21 Nov 2023 07:06:46 GMT  
		Size: 25.7 MB (25698746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a54ea75827017eaea7b7055d8fca97c313c72d7a237502105b83ab018bd5ad`  
		Last Modified: Tue, 21 Nov 2023 07:07:08 GMT  
		Size: 69.6 MB (69584187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a1788f5a7099541c5a0691f88050070dd6e2d5f4b0c97777b19ed32f799c64e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135120963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f2372afa7eb1de18c0332fe8e706503fe4a85393e04c4f9b30e3689e074ea3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:00 GMT
ADD file:8bb55d91755618d4e84d57150867ddbe9513d01cf9543fa953cf7cd1745397ac in / 
# Tue, 21 Nov 2023 05:04:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:06:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7318387eb66a53962a6ff8f603919b1f2eebd63059538ee442fb3f3643d79fd1`  
		Last Modified: Tue, 21 Nov 2023 05:10:07 GMT  
		Size: 47.9 MB (47943002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a20203ebe78a0c1643a97475f1f406b6af2dedd0e14005e4ca4bbeca0470d21`  
		Last Modified: Tue, 21 Nov 2023 06:16:17 GMT  
		Size: 24.0 MB (24045086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c99a00cc05c2b6ae13b5a9c1b8997b9915ab687454a9fcd00d485bbb2d9a5d`  
		Last Modified: Tue, 21 Nov 2023 06:16:33 GMT  
		Size: 63.1 MB (63132875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:88347aed575e413e0481c58be6a945efaad368794a5e9fad50ca25b9af707572
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
$ docker pull buildpack-deps@sha256:ae9a24d7f122f6bb717deadca505fcf45d667cf620c18141389e1053a3b30e56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295366852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcd98698dc1524eaaa3470b3a83094eaf1c56bb354485bbb12afaa247f8b9825`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:16:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:16:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:18:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaa95caafdd4a91609c9997495068a1afc54f385cc3d198e197fac2e00499aa`  
		Last Modified: Tue, 21 Nov 2023 06:25:36 GMT  
		Size: 15.4 MB (15374754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108e54afb4786d49e6af3732141dc10a011b5f0c4496f4e0fdeec608d057a602`  
		Last Modified: Tue, 21 Nov 2023 06:25:55 GMT  
		Size: 52.3 MB (52331159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17dc578bd3fc3acc1b5fcb610b28a09e3d8c99af82c12672e7ccaf00a3e89a8`  
		Last Modified: Tue, 21 Nov 2023 06:26:30 GMT  
		Size: 175.1 MB (175098018 bytes)  
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
$ docker pull buildpack-deps@sha256:7733751255f51040ad326e2d497c3d6aabe11a8ed24f783c9636ab12482f2ea1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330807464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c9fbbaaeb6eea31291adf92f760e668048a0a46665f6b4aea3f842b280bc4d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:56:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:57:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:58:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1736e334b1e250eaca590180779f3cbbdea68af8d960e1795174a8524fe6517`  
		Last Modified: Tue, 21 Nov 2023 07:08:03 GMT  
		Size: 16.8 MB (16765413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaf6761a16c321d5d91b3da652f34fb1b7bde7c3cd21ef5adab0f5622b5abf6`  
		Last Modified: Tue, 21 Nov 2023 07:08:22 GMT  
		Size: 58.9 MB (58866450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071a148a4e40b127789a1fa17ce9bddefefb7832718f122f278a3521df2a87d8`  
		Last Modified: Tue, 21 Nov 2023 07:08:59 GMT  
		Size: 196.2 MB (196245923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d21eb43ffae9bddb2833bb2cc089a45a2657ceb129fbc1efe82596c29ef7a606
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295896976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d4523cd15fcda2a1659bf2e046932979faa9852aae1b3abfb45dc8067736010`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:08:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:08:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:09:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c193fc0604e913e07c3d3f12254414b0f8e42234edfd55788c347f10cebf6ea`  
		Last Modified: Tue, 21 Nov 2023 06:17:13 GMT  
		Size: 15.6 MB (15640102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818038e8ab94615d4f37c021912371b8c12b7678bedbb8ec6d6ab7f1831fae84`  
		Last Modified: Tue, 21 Nov 2023 06:17:26 GMT  
		Size: 54.1 MB (54065995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e80e3f19dd08ea1b9709c3e94f513a117ed8eecd4e17bbd3c4c34659f2fdda0`  
		Last Modified: Tue, 21 Nov 2023 06:17:52 GMT  
		Size: 172.9 MB (172894483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:93b8e7182f485542bcc738f7823ed1c606d6b021710574b72e4295b2410f20bd
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
$ docker pull buildpack-deps@sha256:c23abea3a5efc4debae1f1bec6e3158668a82b6c8df371a6e258a248c29b4777
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67937675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55717d14d3b04b67807a055241a5179bd8e274e358f0d53f6e9a50525d39ddf1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:16:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaa95caafdd4a91609c9997495068a1afc54f385cc3d198e197fac2e00499aa`  
		Last Modified: Tue, 21 Nov 2023 06:25:36 GMT  
		Size: 15.4 MB (15374754 bytes)  
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
$ docker pull buildpack-deps@sha256:96b66b231fd64c79e68c691f1433a4bae3e42a85f281bae68f9d92ca74757725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75695091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8889c736f84811847c5c858939a4798aed2d8b76097caa4c6d78166be76e0a32`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:56:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1736e334b1e250eaca590180779f3cbbdea68af8d960e1795174a8524fe6517`  
		Last Modified: Tue, 21 Nov 2023 07:08:03 GMT  
		Size: 16.8 MB (16765413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9e358f5a8c9afb1a2a92c448a0ead789ae73f7a3f08d60828c77a609488c14ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68936498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d58ad62e6f20633b36173add8ac4f67db4f318b98538e0af575671b1d23053f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:08:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c193fc0604e913e07c3d3f12254414b0f8e42234edfd55788c347f10cebf6ea`  
		Last Modified: Tue, 21 Nov 2023 06:17:13 GMT  
		Size: 15.6 MB (15640102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:bdca2ea7609e632bd8ff53bee7a1ef75f0d185fac4b58cece8d6911b01aeb3b1
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
$ docker pull buildpack-deps@sha256:5c03f01bdf5926079d1994296d2e246e6a915901c7a8ead0d550ddd0cfa0ab47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120268834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152f5629b5b5f0683836ffcc6a235a1b1c8d58fbc5eded7e367eb2c3721e17e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:16:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:16:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaa95caafdd4a91609c9997495068a1afc54f385cc3d198e197fac2e00499aa`  
		Last Modified: Tue, 21 Nov 2023 06:25:36 GMT  
		Size: 15.4 MB (15374754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108e54afb4786d49e6af3732141dc10a011b5f0c4496f4e0fdeec608d057a602`  
		Last Modified: Tue, 21 Nov 2023 06:25:55 GMT  
		Size: 52.3 MB (52331159 bytes)  
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
$ docker pull buildpack-deps@sha256:c0b321f4ed509ca9b8a6fd514c00b095650f350fa88bc41aebed430c8e630183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134561541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad50681818836003e815808939eaf0bbcf38f7bb74d0ba6c1c0a98ea2023e54`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:56:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:57:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1736e334b1e250eaca590180779f3cbbdea68af8d960e1795174a8524fe6517`  
		Last Modified: Tue, 21 Nov 2023 07:08:03 GMT  
		Size: 16.8 MB (16765413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaf6761a16c321d5d91b3da652f34fb1b7bde7c3cd21ef5adab0f5622b5abf6`  
		Last Modified: Tue, 21 Nov 2023 07:08:22 GMT  
		Size: 58.9 MB (58866450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3c98e3cfb95c8dfddbcf6a9c7c2ab92065e9739358e1198121f0eb6058e38cc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123002493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f01b8fe57da07ed806d6e7abc328bee8c0693bd626282085fffbe8c7c8ab436d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:08:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:08:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c193fc0604e913e07c3d3f12254414b0f8e42234edfd55788c347f10cebf6ea`  
		Last Modified: Tue, 21 Nov 2023 06:17:13 GMT  
		Size: 15.6 MB (15640102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818038e8ab94615d4f37c021912371b8c12b7678bedbb8ec6d6ab7f1831fae84`  
		Last Modified: Tue, 21 Nov 2023 06:17:26 GMT  
		Size: 54.1 MB (54065995 bytes)  
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
$ docker pull buildpack-deps@sha256:d53c880810f72ba3a0b875b502506201f5059fb6649867ded0721135ff0b76f5
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
$ docker pull buildpack-deps@sha256:f8e864b6759c58dd553d3638f996a6918822de02ea1c443cc92559e7e7cfdad4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70083136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f201a632265b71438164333d2c732c7918b180c004463264455c253dcc1afc98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:42 GMT
ADD file:e217c81e321b5371a29bea20d4b2802fa8223262c92dbffd268ec38c8951181c in / 
# Tue, 21 Nov 2023 05:00:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:14:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6ffd672cfa56bc540c641f8f5c7b5216716ae5d6336d6698ebdf8fb8cae06e0`  
		Last Modified: Tue, 21 Nov 2023 05:03:32 GMT  
		Size: 47.4 MB (47355729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e04f9270e7bd9277315236c8f83ecc5537fd0907204e9c9f75a2464091a59`  
		Last Modified: Tue, 21 Nov 2023 06:24:19 GMT  
		Size: 22.7 MB (22727407 bytes)  
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
$ docker pull buildpack-deps@sha256:784282fea3a27c11b3c8668acf83fdf5fa1f805e2c648264766bd6bedda9f057
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79274604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:927ae87f00aa3f0f3b5f1fccbc2848eda2dec7b3d1754259fdd0af08c5485cf4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:23:59 GMT
ADD file:209097c8dfcefec7951851d25bc9e8c1d56aefed076c682c5f2e077cc05aeaf8 in / 
# Tue, 21 Nov 2023 04:24:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d694a6aceb98c067febf569d227d6249cd8d39b11dead73e4840d07861a25e9`  
		Last Modified: Tue, 21 Nov 2023 04:28:27 GMT  
		Size: 53.6 MB (53575858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71d255e683d12334b12df8a9e23692d03ce5d514a74efe4553f12269885d87`  
		Last Modified: Tue, 21 Nov 2023 07:06:46 GMT  
		Size: 25.7 MB (25698746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:56dea1f8a449f195ffdd426569472adfdcbb657344ea182789923be11c8b79f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71988088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba3cde7adf1be7b7277ab9b2cd62cc5ea051cb781184b34e1645be1f946290f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:00 GMT
ADD file:8bb55d91755618d4e84d57150867ddbe9513d01cf9543fa953cf7cd1745397ac in / 
# Tue, 21 Nov 2023 05:04:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7318387eb66a53962a6ff8f603919b1f2eebd63059538ee442fb3f3643d79fd1`  
		Last Modified: Tue, 21 Nov 2023 05:10:07 GMT  
		Size: 47.9 MB (47943002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a20203ebe78a0c1643a97475f1f406b6af2dedd0e14005e4ca4bbeca0470d21`  
		Last Modified: Tue, 21 Nov 2023 06:16:17 GMT  
		Size: 24.0 MB (24045086 bytes)  
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
$ docker pull buildpack-deps@sha256:1fe9f803a37577bc063b88c1ab063c620ebbea8ed3b451b95dde19a19ceaac10
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
$ docker pull buildpack-deps@sha256:227ea9bc7dd964b6592406f4447f91cdaf529d06dbe9980626edf3455d79bc37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316029661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316e91cadc40ed25984ede1f07ab85dbe4913f989cd383e3b3511c486c119a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:42 GMT
ADD file:e217c81e321b5371a29bea20d4b2802fa8223262c92dbffd268ec38c8951181c in / 
# Tue, 21 Nov 2023 05:00:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:14:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:16:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6ffd672cfa56bc540c641f8f5c7b5216716ae5d6336d6698ebdf8fb8cae06e0`  
		Last Modified: Tue, 21 Nov 2023 05:03:32 GMT  
		Size: 47.4 MB (47355729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e04f9270e7bd9277315236c8f83ecc5537fd0907204e9c9f75a2464091a59`  
		Last Modified: Tue, 21 Nov 2023 06:24:19 GMT  
		Size: 22.7 MB (22727407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7466297e667840b4907e1e017052f34ebebba91fb7a476d17a10259cf5a264fc`  
		Last Modified: Tue, 21 Nov 2023 06:24:41 GMT  
		Size: 61.6 MB (61561534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8128c2db4bac59c665360b03846fbc4d0013d87270dad0af442499ef7088c34`  
		Last Modified: Tue, 21 Nov 2023 06:25:23 GMT  
		Size: 184.4 MB (184384991 bytes)  
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
$ docker pull buildpack-deps@sha256:ff34a667d81db5798aaf33085e09a789e13a45e7b48e804c87809631102b0ec7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.0 MB (362952942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b6ecc5afbeef5b86b674ec0993915e6bb01b89f9c44f901050856f10a1bf0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:23:59 GMT
ADD file:209097c8dfcefec7951851d25bc9e8c1d56aefed076c682c5f2e077cc05aeaf8 in / 
# Tue, 21 Nov 2023 04:24:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:53:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:56:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d694a6aceb98c067febf569d227d6249cd8d39b11dead73e4840d07861a25e9`  
		Last Modified: Tue, 21 Nov 2023 04:28:27 GMT  
		Size: 53.6 MB (53575858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71d255e683d12334b12df8a9e23692d03ce5d514a74efe4553f12269885d87`  
		Last Modified: Tue, 21 Nov 2023 07:06:46 GMT  
		Size: 25.7 MB (25698746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a54ea75827017eaea7b7055d8fca97c313c72d7a237502105b83ab018bd5ad`  
		Last Modified: Tue, 21 Nov 2023 07:07:08 GMT  
		Size: 69.6 MB (69584187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e986f224599c525ac40be9636489d408b4daff891bb3567a7986f6ae5c817cc1`  
		Last Modified: Tue, 21 Nov 2023 07:07:49 GMT  
		Size: 214.1 MB (214094151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d1822d31d3c58472a93084eaa39396b37585eb538479e3ca57d5e2e50d7470c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318217378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0dcda8469adc1e80e5b8779671680724ff22c47c0c87e7d0658d100902caa19`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:00 GMT
ADD file:8bb55d91755618d4e84d57150867ddbe9513d01cf9543fa953cf7cd1745397ac in / 
# Tue, 21 Nov 2023 05:04:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:06:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:07:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7318387eb66a53962a6ff8f603919b1f2eebd63059538ee442fb3f3643d79fd1`  
		Last Modified: Tue, 21 Nov 2023 05:10:07 GMT  
		Size: 47.9 MB (47943002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a20203ebe78a0c1643a97475f1f406b6af2dedd0e14005e4ca4bbeca0470d21`  
		Last Modified: Tue, 21 Nov 2023 06:16:17 GMT  
		Size: 24.0 MB (24045086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c99a00cc05c2b6ae13b5a9c1b8997b9915ab687454a9fcd00d485bbb2d9a5d`  
		Last Modified: Tue, 21 Nov 2023 06:16:33 GMT  
		Size: 63.1 MB (63132875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cf7e37f4b53af6dfd3bdea89a2078a221738e8eeade3f46428f3def3e4c97c`  
		Last Modified: Tue, 21 Nov 2023 06:17:01 GMT  
		Size: 183.1 MB (183096415 bytes)  
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
$ docker pull buildpack-deps@sha256:498c3e1c24d8bf3c692c0ed7d8afeaba649e5990abea41ce76bc88a5144f7c3e
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
$ docker pull buildpack-deps@sha256:2608204439da09756cf236495eabd8abf170fee83470c3afdb8caa3ceb104ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.1 MB (272077462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982da4d9dfdd4bd047eb685a31015aa7dd1f57402c4e78d9fe24f42a1d82eb21`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:02 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:10 GMT
ADD file:9e750ebbbf7e47a121d153e6699006776ea61b04b6c8e31556600483a020f617 in / 
# Wed, 11 Oct 2023 18:03:10 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 06:17:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:21:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b743c812db4b2a4cb933b4107dd5408c786d034c3bcff4d162d02e20587dce07`  
		Last Modified: Fri, 13 Oct 2023 06:40:38 GMT  
		Size: 27.3 MB (27340045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e717ff89b8bce5f5201b6827c6ed6615c39f2b52f5b0e8ca3d659d049b51e6`  
		Last Modified: Wed, 15 Nov 2023 06:23:55 GMT  
		Size: 9.6 MB (9645467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3cadc26010e0f011e17572f55422b03f3cc9dd1729864eba62145f0aeacf76`  
		Last Modified: Wed, 15 Nov 2023 06:24:12 GMT  
		Size: 45.0 MB (44982339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651e35dbc14e3494cc43e42663e48327f408cfde12d19c632c44377b1654e9a1`  
		Last Modified: Wed, 15 Nov 2023 06:24:41 GMT  
		Size: 190.1 MB (190109611 bytes)  
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
$ docker pull buildpack-deps@sha256:2c2946cb3e2a5c8a960b0c37413e3ff648f830a750a8ee2b3553ac1257c9638c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.0 MB (257957931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce82b60021dc7fb1c62212e9c71ec596bd448c6623a4d6188ca2df6fe8d956b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:34 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:36 GMT
ADD file:8ceb0028af8276b03b6c88b19445f30165a41791919c756e1434da6ded4387db in / 
# Wed, 11 Oct 2023 18:03:36 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:24:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:27:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:82cdc38d6d4a8f105e5928c09fada25b62831433ea5f6e4c51bda4c9ecbd9702`  
		Last Modified: Wed, 15 Nov 2023 05:29:56 GMT  
		Size: 27.6 MB (27617854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25054bfcd5aaaaab9a8b81261f4b5a2752bc79e2ef9670be2543ea4ca8151408`  
		Last Modified: Wed, 15 Nov 2023 05:29:53 GMT  
		Size: 9.7 MB (9696878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692f488bb8b766464b4e25f6f72ccf92efc432f0c10df1d1003061838b729d85`  
		Last Modified: Wed, 15 Nov 2023 05:30:09 GMT  
		Size: 45.6 MB (45572317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b65bd5cf9be92580539ab8bd5dce75b179cc8d5b9be1a70fa8247b133f4a0d`  
		Last Modified: Wed, 15 Nov 2023 05:30:35 GMT  
		Size: 175.1 MB (175070882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic-curl`

```console
$ docker pull buildpack-deps@sha256:fdd84b5fb072cd9015e72499e405b6c2ee6071d354e22f49309744b75abe40a0
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
$ docker pull buildpack-deps@sha256:d649d5fa7ae482f135330be776368c49ff5d30b7336734c39ad94af9a6064874
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36985512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16ce70cb7143b41128b73de1bc7c1520314ceae722ab6e435381a4fd31188a78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:02 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:10 GMT
ADD file:9e750ebbbf7e47a121d153e6699006776ea61b04b6c8e31556600483a020f617 in / 
# Wed, 11 Oct 2023 18:03:10 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 06:17:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b743c812db4b2a4cb933b4107dd5408c786d034c3bcff4d162d02e20587dce07`  
		Last Modified: Fri, 13 Oct 2023 06:40:38 GMT  
		Size: 27.3 MB (27340045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e717ff89b8bce5f5201b6827c6ed6615c39f2b52f5b0e8ca3d659d049b51e6`  
		Last Modified: Wed, 15 Nov 2023 06:23:55 GMT  
		Size: 9.6 MB (9645467 bytes)  
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
$ docker pull buildpack-deps@sha256:e3fb9abd82bd63f435954245545251574327c9881255d2db0ca53940bda40d64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37314732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64946e8ba5952759944b3513696715ee3fc336e4cb5f02dced4113a84b7fb861`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:34 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:36 GMT
ADD file:8ceb0028af8276b03b6c88b19445f30165a41791919c756e1434da6ded4387db in / 
# Wed, 11 Oct 2023 18:03:36 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:82cdc38d6d4a8f105e5928c09fada25b62831433ea5f6e4c51bda4c9ecbd9702`  
		Last Modified: Wed, 15 Nov 2023 05:29:56 GMT  
		Size: 27.6 MB (27617854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25054bfcd5aaaaab9a8b81261f4b5a2752bc79e2ef9670be2543ea4ca8151408`  
		Last Modified: Wed, 15 Nov 2023 05:29:53 GMT  
		Size: 9.7 MB (9696878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic-scm`

```console
$ docker pull buildpack-deps@sha256:27f45ae4542018ae28469a9738efc4351c50cfbd8ef2638d4e22f131701dbbec
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
$ docker pull buildpack-deps@sha256:cf087be5e86a4c17a523c29b076e9f0fe429f185a1485b4288e664384784dfcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81967851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab16779c759dc820ef4e5a74d5ce02ee78fa337b3a8e604f11ef1f752d8f4001`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:02 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:10 GMT
ADD file:9e750ebbbf7e47a121d153e6699006776ea61b04b6c8e31556600483a020f617 in / 
# Wed, 11 Oct 2023 18:03:10 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 06:17:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b743c812db4b2a4cb933b4107dd5408c786d034c3bcff4d162d02e20587dce07`  
		Last Modified: Fri, 13 Oct 2023 06:40:38 GMT  
		Size: 27.3 MB (27340045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e717ff89b8bce5f5201b6827c6ed6615c39f2b52f5b0e8ca3d659d049b51e6`  
		Last Modified: Wed, 15 Nov 2023 06:23:55 GMT  
		Size: 9.6 MB (9645467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3cadc26010e0f011e17572f55422b03f3cc9dd1729864eba62145f0aeacf76`  
		Last Modified: Wed, 15 Nov 2023 06:24:12 GMT  
		Size: 45.0 MB (44982339 bytes)  
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
$ docker pull buildpack-deps@sha256:a91a88d92cebe1e06032a2e91eca9eed7764f96574bf8209a0e634b723902068
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82887049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f810d9541dc377d4af2da31b65e5188e4419926498729a02895e8664cdb624`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:34 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:36 GMT
ADD file:8ceb0028af8276b03b6c88b19445f30165a41791919c756e1434da6ded4387db in / 
# Wed, 11 Oct 2023 18:03:36 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:24:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:82cdc38d6d4a8f105e5928c09fada25b62831433ea5f6e4c51bda4c9ecbd9702`  
		Last Modified: Wed, 15 Nov 2023 05:29:56 GMT  
		Size: 27.6 MB (27617854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25054bfcd5aaaaab9a8b81261f4b5a2752bc79e2ef9670be2543ea4ca8151408`  
		Last Modified: Wed, 15 Nov 2023 05:29:53 GMT  
		Size: 9.7 MB (9696878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692f488bb8b766464b4e25f6f72ccf92efc432f0c10df1d1003061838b729d85`  
		Last Modified: Wed, 15 Nov 2023 05:30:09 GMT  
		Size: 45.6 MB (45572317 bytes)  
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
$ docker pull buildpack-deps@sha256:88347aed575e413e0481c58be6a945efaad368794a5e9fad50ca25b9af707572
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
$ docker pull buildpack-deps@sha256:ae9a24d7f122f6bb717deadca505fcf45d667cf620c18141389e1053a3b30e56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295366852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcd98698dc1524eaaa3470b3a83094eaf1c56bb354485bbb12afaa247f8b9825`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:16:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:16:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:18:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaa95caafdd4a91609c9997495068a1afc54f385cc3d198e197fac2e00499aa`  
		Last Modified: Tue, 21 Nov 2023 06:25:36 GMT  
		Size: 15.4 MB (15374754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108e54afb4786d49e6af3732141dc10a011b5f0c4496f4e0fdeec608d057a602`  
		Last Modified: Tue, 21 Nov 2023 06:25:55 GMT  
		Size: 52.3 MB (52331159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17dc578bd3fc3acc1b5fcb610b28a09e3d8c99af82c12672e7ccaf00a3e89a8`  
		Last Modified: Tue, 21 Nov 2023 06:26:30 GMT  
		Size: 175.1 MB (175098018 bytes)  
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
$ docker pull buildpack-deps@sha256:7733751255f51040ad326e2d497c3d6aabe11a8ed24f783c9636ab12482f2ea1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330807464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c9fbbaaeb6eea31291adf92f760e668048a0a46665f6b4aea3f842b280bc4d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:56:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:57:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:58:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1736e334b1e250eaca590180779f3cbbdea68af8d960e1795174a8524fe6517`  
		Last Modified: Tue, 21 Nov 2023 07:08:03 GMT  
		Size: 16.8 MB (16765413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaf6761a16c321d5d91b3da652f34fb1b7bde7c3cd21ef5adab0f5622b5abf6`  
		Last Modified: Tue, 21 Nov 2023 07:08:22 GMT  
		Size: 58.9 MB (58866450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071a148a4e40b127789a1fa17ce9bddefefb7832718f122f278a3521df2a87d8`  
		Last Modified: Tue, 21 Nov 2023 07:08:59 GMT  
		Size: 196.2 MB (196245923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d21eb43ffae9bddb2833bb2cc089a45a2657ceb129fbc1efe82596c29ef7a606
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295896976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d4523cd15fcda2a1659bf2e046932979faa9852aae1b3abfb45dc8067736010`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:08:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:08:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:09:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c193fc0604e913e07c3d3f12254414b0f8e42234edfd55788c347f10cebf6ea`  
		Last Modified: Tue, 21 Nov 2023 06:17:13 GMT  
		Size: 15.6 MB (15640102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818038e8ab94615d4f37c021912371b8c12b7678bedbb8ec6d6ab7f1831fae84`  
		Last Modified: Tue, 21 Nov 2023 06:17:26 GMT  
		Size: 54.1 MB (54065995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e80e3f19dd08ea1b9709c3e94f513a117ed8eecd4e17bbd3c4c34659f2fdda0`  
		Last Modified: Tue, 21 Nov 2023 06:17:52 GMT  
		Size: 172.9 MB (172894483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:93b8e7182f485542bcc738f7823ed1c606d6b021710574b72e4295b2410f20bd
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
$ docker pull buildpack-deps@sha256:c23abea3a5efc4debae1f1bec6e3158668a82b6c8df371a6e258a248c29b4777
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67937675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55717d14d3b04b67807a055241a5179bd8e274e358f0d53f6e9a50525d39ddf1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:16:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaa95caafdd4a91609c9997495068a1afc54f385cc3d198e197fac2e00499aa`  
		Last Modified: Tue, 21 Nov 2023 06:25:36 GMT  
		Size: 15.4 MB (15374754 bytes)  
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
$ docker pull buildpack-deps@sha256:96b66b231fd64c79e68c691f1433a4bae3e42a85f281bae68f9d92ca74757725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75695091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8889c736f84811847c5c858939a4798aed2d8b76097caa4c6d78166be76e0a32`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:56:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1736e334b1e250eaca590180779f3cbbdea68af8d960e1795174a8524fe6517`  
		Last Modified: Tue, 21 Nov 2023 07:08:03 GMT  
		Size: 16.8 MB (16765413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9e358f5a8c9afb1a2a92c448a0ead789ae73f7a3f08d60828c77a609488c14ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68936498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d58ad62e6f20633b36173add8ac4f67db4f318b98538e0af575671b1d23053f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:08:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c193fc0604e913e07c3d3f12254414b0f8e42234edfd55788c347f10cebf6ea`  
		Last Modified: Tue, 21 Nov 2023 06:17:13 GMT  
		Size: 15.6 MB (15640102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:bdca2ea7609e632bd8ff53bee7a1ef75f0d185fac4b58cece8d6911b01aeb3b1
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
$ docker pull buildpack-deps@sha256:5c03f01bdf5926079d1994296d2e246e6a915901c7a8ead0d550ddd0cfa0ab47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120268834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152f5629b5b5f0683836ffcc6a235a1b1c8d58fbc5eded7e367eb2c3721e17e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:16:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:16:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaa95caafdd4a91609c9997495068a1afc54f385cc3d198e197fac2e00499aa`  
		Last Modified: Tue, 21 Nov 2023 06:25:36 GMT  
		Size: 15.4 MB (15374754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108e54afb4786d49e6af3732141dc10a011b5f0c4496f4e0fdeec608d057a602`  
		Last Modified: Tue, 21 Nov 2023 06:25:55 GMT  
		Size: 52.3 MB (52331159 bytes)  
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
$ docker pull buildpack-deps@sha256:c0b321f4ed509ca9b8a6fd514c00b095650f350fa88bc41aebed430c8e630183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134561541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad50681818836003e815808939eaf0bbcf38f7bb74d0ba6c1c0a98ea2023e54`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:56:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:57:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1736e334b1e250eaca590180779f3cbbdea68af8d960e1795174a8524fe6517`  
		Last Modified: Tue, 21 Nov 2023 07:08:03 GMT  
		Size: 16.8 MB (16765413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaf6761a16c321d5d91b3da652f34fb1b7bde7c3cd21ef5adab0f5622b5abf6`  
		Last Modified: Tue, 21 Nov 2023 07:08:22 GMT  
		Size: 58.9 MB (58866450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3c98e3cfb95c8dfddbcf6a9c7c2ab92065e9739358e1198121f0eb6058e38cc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123002493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f01b8fe57da07ed806d6e7abc328bee8c0693bd626282085fffbe8c7c8ab436d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:08:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:08:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c193fc0604e913e07c3d3f12254414b0f8e42234edfd55788c347f10cebf6ea`  
		Last Modified: Tue, 21 Nov 2023 06:17:13 GMT  
		Size: 15.6 MB (15640102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818038e8ab94615d4f37c021912371b8c12b7678bedbb8ec6d6ab7f1831fae84`  
		Last Modified: Tue, 21 Nov 2023 06:17:26 GMT  
		Size: 54.1 MB (54065995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:c99b8a43be556e5b407214a5ea1801af92a581294119cc772136046613486699
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
$ docker pull buildpack-deps@sha256:adec01003a17f6b964516dc2082a5c112ef7132fd914810661c01e4fde930972
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131644670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3bc44cf636b514c0c186654ac43d24bd92f970d9fdcd2dca3b0516e058959c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:42 GMT
ADD file:e217c81e321b5371a29bea20d4b2802fa8223262c92dbffd268ec38c8951181c in / 
# Tue, 21 Nov 2023 05:00:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:14:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6ffd672cfa56bc540c641f8f5c7b5216716ae5d6336d6698ebdf8fb8cae06e0`  
		Last Modified: Tue, 21 Nov 2023 05:03:32 GMT  
		Size: 47.4 MB (47355729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e04f9270e7bd9277315236c8f83ecc5537fd0907204e9c9f75a2464091a59`  
		Last Modified: Tue, 21 Nov 2023 06:24:19 GMT  
		Size: 22.7 MB (22727407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7466297e667840b4907e1e017052f34ebebba91fb7a476d17a10259cf5a264fc`  
		Last Modified: Tue, 21 Nov 2023 06:24:41 GMT  
		Size: 61.6 MB (61561534 bytes)  
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
$ docker pull buildpack-deps@sha256:ad518e13047a2bffa7358d6ed80141ee89918b12549d94563fe33dfe97693f63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148858791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1afccc4310e63668ea2fa68e7ed2114f91aa1c4023a673f0dbd3cb0d533ddd7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:23:59 GMT
ADD file:209097c8dfcefec7951851d25bc9e8c1d56aefed076c682c5f2e077cc05aeaf8 in / 
# Tue, 21 Nov 2023 04:24:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:53:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d694a6aceb98c067febf569d227d6249cd8d39b11dead73e4840d07861a25e9`  
		Last Modified: Tue, 21 Nov 2023 04:28:27 GMT  
		Size: 53.6 MB (53575858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71d255e683d12334b12df8a9e23692d03ce5d514a74efe4553f12269885d87`  
		Last Modified: Tue, 21 Nov 2023 07:06:46 GMT  
		Size: 25.7 MB (25698746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a54ea75827017eaea7b7055d8fca97c313c72d7a237502105b83ab018bd5ad`  
		Last Modified: Tue, 21 Nov 2023 07:07:08 GMT  
		Size: 69.6 MB (69584187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a1788f5a7099541c5a0691f88050070dd6e2d5f4b0c97777b19ed32f799c64e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135120963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f2372afa7eb1de18c0332fe8e706503fe4a85393e04c4f9b30e3689e074ea3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:00 GMT
ADD file:8bb55d91755618d4e84d57150867ddbe9513d01cf9543fa953cf7cd1745397ac in / 
# Tue, 21 Nov 2023 05:04:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:06:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7318387eb66a53962a6ff8f603919b1f2eebd63059538ee442fb3f3643d79fd1`  
		Last Modified: Tue, 21 Nov 2023 05:10:07 GMT  
		Size: 47.9 MB (47943002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a20203ebe78a0c1643a97475f1f406b6af2dedd0e14005e4ca4bbeca0470d21`  
		Last Modified: Tue, 21 Nov 2023 06:16:17 GMT  
		Size: 24.0 MB (24045086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c99a00cc05c2b6ae13b5a9c1b8997b9915ab687454a9fcd00d485bbb2d9a5d`  
		Last Modified: Tue, 21 Nov 2023 06:16:33 GMT  
		Size: 63.1 MB (63132875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:b64036ac9f9e82d6152e2397921cccb86cdf7aa797d13de79f61d3301955ceee
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
$ docker pull buildpack-deps@sha256:fcf7edb8ce652541065efcbc0f507104b809f1e99b8353836e0713ff4525e41d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.9 MB (348901354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e89ade2f919c3a4ff65a0eb3b9f73bc2ae64a6ba48b4f89ea808f2dfdaab921a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:33 GMT
ADD file:b1618939ac80f9d3256d12ed22ac3e37f61dc396e5370e7a4013561a073af181 in / 
# Tue, 21 Nov 2023 05:01:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:19:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:19:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:21:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:228b88d8d39e27fa3bddca63f14715a5dec3e5c3de7b5b5a892c00385ea38d2b`  
		Last Modified: Tue, 21 Nov 2023 05:05:36 GMT  
		Size: 47.2 MB (47196697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df76a43e2f790a0c0d3fd4795cae7a8d79b43803710d103b38936a70bbe216`  
		Last Modified: Tue, 21 Nov 2023 06:26:42 GMT  
		Size: 25.9 MB (25892928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df8da3dad66ffd081a2a6a2a79c62c577b4c8f5b7751d2718f24e60791eae1e`  
		Last Modified: Tue, 21 Nov 2023 06:27:02 GMT  
		Size: 63.0 MB (63027803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada4fcce692f91cb6588fc68ccf3c8e63e6e26a568c586b8fd8af47793481bd9`  
		Last Modified: Tue, 21 Nov 2023 06:27:42 GMT  
		Size: 212.8 MB (212783926 bytes)  
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
$ docker pull buildpack-deps@sha256:1766ed0c020a64b0c0245a19f9ba7a951551f98147642a9acf6ede2115229dca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.4 MB (393372396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e24823afdd39ee710bbbc971c39d0aa4ff7fb43aebaf6a79c893b045539c7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:25:27 GMT
ADD file:a20f125b82438597a2805558ad08c66dbc68ff26fb4af210ce31e903d1d46127 in / 
# Tue, 21 Nov 2023 04:25:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:59:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:02:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:700801ea1c1b3b29b8d88a2f8f9405af55e151c6a84cab4b448b09ce5f2e432c`  
		Last Modified: Tue, 21 Nov 2023 04:30:48 GMT  
		Size: 53.4 MB (53423841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978542d765f76211993ce7a733e45289127bc6a8dcd47683860c44cd31e03925`  
		Last Modified: Tue, 21 Nov 2023 07:09:13 GMT  
		Size: 30.0 MB (30010990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fb001517f3aa634674774ca44ff1ee072157218fcd0522c1630479101d895`  
		Last Modified: Tue, 21 Nov 2023 07:09:33 GMT  
		Size: 70.9 MB (70920797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b31909696ac928d37c89a4769a0d196f1f4641efdd73d46c6a365e9c76eea9b`  
		Last Modified: Tue, 21 Nov 2023 07:10:21 GMT  
		Size: 239.0 MB (239016768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:cd9775eccbc9ffcd297a1818f606c97ed2ad5ca30801aac383fd3ff85ac44fab
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.6 MB (415648463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:872ff0980fc3f2e38808c31811962bbb2b3158891d22903ae44c81b2c9ab8eb4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:02 GMT
ADD file:6edb177cc4c3fc7c02043410bba7fabbbaa23493a2e0444ac13e281f6fd7d209 in / 
# Tue, 21 Nov 2023 04:09:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 04:35:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 04:42:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9197643899c29fb1e411101ee2f4e677b44704d5c2c8ce98f7567cb7f7a6cf58`  
		Last Modified: Tue, 21 Nov 2023 04:12:00 GMT  
		Size: 48.2 MB (48206696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0617cf6ad3eec888f08f7b773880b515adb1cae0586b8aa6f4b5f40076079dd`  
		Last Modified: Tue, 21 Nov 2023 04:43:06 GMT  
		Size: 26.8 MB (26784568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e112439f28d2102590bea4e42209332ea3595b8c9789016a1e8b479e123bee`  
		Last Modified: Tue, 21 Nov 2023 04:44:20 GMT  
		Size: 64.7 MB (64702623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b281221811c330e1fa4440fa0722c3b2f9601f5f9016ab7e7d8f32cdda28633`  
		Last Modified: Tue, 21 Nov 2023 04:49:49 GMT  
		Size: 276.0 MB (275954576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c93fc2e94d1d3a26456ef129ab582ef7d63a767ab8762db8940202c77f1388df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.1 MB (355072174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc793a1658b88281067a4063d6ed988d648fdb13eb5611f6e42534971d82b3da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:06:09 GMT
ADD file:38bf5e0509c54c17377ce5928ac13833ab7953cb7ff56a92265b9835fad4a7ef in / 
# Tue, 21 Nov 2023 05:06:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:10:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:12:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89d47f76a96d7ec8b86acac59109c329b28ddeee28c3c0b2ae9c6f275a50a136`  
		Last Modified: Tue, 21 Nov 2023 05:11:22 GMT  
		Size: 49.2 MB (49228111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd42e8e3bd2b6546f326a1d59a7ec0be9e7ece5e7885fd1749571be27caa1ba2`  
		Last Modified: Tue, 21 Nov 2023 06:18:03 GMT  
		Size: 28.0 MB (28032511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21db908a00e81480eebf3fad2c4e13874394ba9f9978d3ea7677d3be28b4fb`  
		Last Modified: Tue, 21 Nov 2023 06:18:18 GMT  
		Size: 66.5 MB (66490545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d423dea4ea04d9998b72e9dca146ee1f13e78ec50b02fa0de85998fc82032b`  
		Last Modified: Tue, 21 Nov 2023 06:18:48 GMT  
		Size: 211.3 MB (211321007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:8d7693e4c73bfb146460b441c69670413b9f765cd92ae0a2371828d1e0fe345f
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
$ docker pull buildpack-deps@sha256:c2083dcfe7e41b3bb14edc1e4c5d008973dd762ba4cec2830ebbddbb2f98ca9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73089625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1359faa3d45cb9604477049d17de32d2cb1490b072e28d9b1ae3ebd36b86c2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:33 GMT
ADD file:b1618939ac80f9d3256d12ed22ac3e37f61dc396e5370e7a4013561a073af181 in / 
# Tue, 21 Nov 2023 05:01:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:19:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:228b88d8d39e27fa3bddca63f14715a5dec3e5c3de7b5b5a892c00385ea38d2b`  
		Last Modified: Tue, 21 Nov 2023 05:05:36 GMT  
		Size: 47.2 MB (47196697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df76a43e2f790a0c0d3fd4795cae7a8d79b43803710d103b38936a70bbe216`  
		Last Modified: Tue, 21 Nov 2023 06:26:42 GMT  
		Size: 25.9 MB (25892928 bytes)  
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
$ docker pull buildpack-deps@sha256:bf7b2c6f20aeaa97efb86336a12338247f96a743fa032cbb6e848100e365d25e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83434831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e185b08bc814b3731dcb7aa4ef80f272175c6d3715e08afb5a280d02f76715`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:25:27 GMT
ADD file:a20f125b82438597a2805558ad08c66dbc68ff26fb4af210ce31e903d1d46127 in / 
# Tue, 21 Nov 2023 04:25:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:59:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:700801ea1c1b3b29b8d88a2f8f9405af55e151c6a84cab4b448b09ce5f2e432c`  
		Last Modified: Tue, 21 Nov 2023 04:30:48 GMT  
		Size: 53.4 MB (53423841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978542d765f76211993ce7a733e45289127bc6a8dcd47683860c44cd31e03925`  
		Last Modified: Tue, 21 Nov 2023 07:09:13 GMT  
		Size: 30.0 MB (30010990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:d47d61fd7d6f36e367a86f12fb809a0caa3ca64d6514b9d4a264184bcdc171f9
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74991264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c519b4d73993379f707098d265c9b5132d01092cdf180e2bb22b72f3163cef07`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:02 GMT
ADD file:6edb177cc4c3fc7c02043410bba7fabbbaa23493a2e0444ac13e281f6fd7d209 in / 
# Tue, 21 Nov 2023 04:09:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9197643899c29fb1e411101ee2f4e677b44704d5c2c8ce98f7567cb7f7a6cf58`  
		Last Modified: Tue, 21 Nov 2023 04:12:00 GMT  
		Size: 48.2 MB (48206696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0617cf6ad3eec888f08f7b773880b515adb1cae0586b8aa6f4b5f40076079dd`  
		Last Modified: Tue, 21 Nov 2023 04:43:06 GMT  
		Size: 26.8 MB (26784568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:132caa5f4dfbbce1e1f7a982aa07300d03415c825ae2ba80361c5c01a31e8332
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.3 MB (77260622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84e28664175d244c1cd5e4e6f02cccb38f1c27e640751ef1722a1529d588c2a9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:06:09 GMT
ADD file:38bf5e0509c54c17377ce5928ac13833ab7953cb7ff56a92265b9835fad4a7ef in / 
# Tue, 21 Nov 2023 05:06:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:10:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89d47f76a96d7ec8b86acac59109c329b28ddeee28c3c0b2ae9c6f275a50a136`  
		Last Modified: Tue, 21 Nov 2023 05:11:22 GMT  
		Size: 49.2 MB (49228111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd42e8e3bd2b6546f326a1d59a7ec0be9e7ece5e7885fd1749571be27caa1ba2`  
		Last Modified: Tue, 21 Nov 2023 06:18:03 GMT  
		Size: 28.0 MB (28032511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:dd82e7d82d39f837e964e0a02ec7acd4b7c87412144bc6b05940f154ec67d818
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
$ docker pull buildpack-deps@sha256:a14fff4df4cffc72ece82f02fb56f4d17fa776812b43c4c2cf6a19a9b4c87db3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136117428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2bafb9025c11df5f43acb3bedb814be855b4fd0db9041333997866bd26b03b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:33 GMT
ADD file:b1618939ac80f9d3256d12ed22ac3e37f61dc396e5370e7a4013561a073af181 in / 
# Tue, 21 Nov 2023 05:01:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:19:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:19:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:228b88d8d39e27fa3bddca63f14715a5dec3e5c3de7b5b5a892c00385ea38d2b`  
		Last Modified: Tue, 21 Nov 2023 05:05:36 GMT  
		Size: 47.2 MB (47196697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df76a43e2f790a0c0d3fd4795cae7a8d79b43803710d103b38936a70bbe216`  
		Last Modified: Tue, 21 Nov 2023 06:26:42 GMT  
		Size: 25.9 MB (25892928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df8da3dad66ffd081a2a6a2a79c62c577b4c8f5b7751d2718f24e60791eae1e`  
		Last Modified: Tue, 21 Nov 2023 06:27:02 GMT  
		Size: 63.0 MB (63027803 bytes)  
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
$ docker pull buildpack-deps@sha256:24a7862e93585787852dbaecc311fe50c85ca997c602ae777a5a40f37264db6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154355628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f839951b7a1ec1855581f34657a10b0e452a76662c147f9893fb5b4b1355743a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:25:27 GMT
ADD file:a20f125b82438597a2805558ad08c66dbc68ff26fb4af210ce31e903d1d46127 in / 
# Tue, 21 Nov 2023 04:25:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:59:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:700801ea1c1b3b29b8d88a2f8f9405af55e151c6a84cab4b448b09ce5f2e432c`  
		Last Modified: Tue, 21 Nov 2023 04:30:48 GMT  
		Size: 53.4 MB (53423841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978542d765f76211993ce7a733e45289127bc6a8dcd47683860c44cd31e03925`  
		Last Modified: Tue, 21 Nov 2023 07:09:13 GMT  
		Size: 30.0 MB (30010990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fb001517f3aa634674774ca44ff1ee072157218fcd0522c1630479101d895`  
		Last Modified: Tue, 21 Nov 2023 07:09:33 GMT  
		Size: 70.9 MB (70920797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:33c5e15d08ce712b59fb3c301d86849d093fabbed9d042e2dfd606d54cb3405a
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139693887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77b886411896315e38d59726c286243652452815642a349f1633769e908c0c92`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:02 GMT
ADD file:6edb177cc4c3fc7c02043410bba7fabbbaa23493a2e0444ac13e281f6fd7d209 in / 
# Tue, 21 Nov 2023 04:09:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 04:35:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9197643899c29fb1e411101ee2f4e677b44704d5c2c8ce98f7567cb7f7a6cf58`  
		Last Modified: Tue, 21 Nov 2023 04:12:00 GMT  
		Size: 48.2 MB (48206696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0617cf6ad3eec888f08f7b773880b515adb1cae0586b8aa6f4b5f40076079dd`  
		Last Modified: Tue, 21 Nov 2023 04:43:06 GMT  
		Size: 26.8 MB (26784568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e112439f28d2102590bea4e42209332ea3595b8c9789016a1e8b479e123bee`  
		Last Modified: Tue, 21 Nov 2023 04:44:20 GMT  
		Size: 64.7 MB (64702623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1769e0bcb2fe395e6ae63c7c91bdeee37003e88269a8db80d927a4fc64840f8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.8 MB (143751167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47000f61dc60af3bdb834e3d3470c752ac2e6269191cb531d5f7264a413791e8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:06:09 GMT
ADD file:38bf5e0509c54c17377ce5928ac13833ab7953cb7ff56a92265b9835fad4a7ef in / 
# Tue, 21 Nov 2023 05:06:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:10:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89d47f76a96d7ec8b86acac59109c329b28ddeee28c3c0b2ae9c6f275a50a136`  
		Last Modified: Tue, 21 Nov 2023 05:11:22 GMT  
		Size: 49.2 MB (49228111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd42e8e3bd2b6546f326a1d59a7ec0be9e7ece5e7885fd1749571be27caa1ba2`  
		Last Modified: Tue, 21 Nov 2023 06:18:03 GMT  
		Size: 28.0 MB (28032511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21db908a00e81480eebf3fad2c4e13874394ba9f9978d3ea7677d3be28b4fb`  
		Last Modified: Tue, 21 Nov 2023 06:18:18 GMT  
		Size: 66.5 MB (66490545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:1fe9f803a37577bc063b88c1ab063c620ebbea8ed3b451b95dde19a19ceaac10
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
$ docker pull buildpack-deps@sha256:227ea9bc7dd964b6592406f4447f91cdaf529d06dbe9980626edf3455d79bc37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316029661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316e91cadc40ed25984ede1f07ab85dbe4913f989cd383e3b3511c486c119a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:42 GMT
ADD file:e217c81e321b5371a29bea20d4b2802fa8223262c92dbffd268ec38c8951181c in / 
# Tue, 21 Nov 2023 05:00:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:14:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:16:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6ffd672cfa56bc540c641f8f5c7b5216716ae5d6336d6698ebdf8fb8cae06e0`  
		Last Modified: Tue, 21 Nov 2023 05:03:32 GMT  
		Size: 47.4 MB (47355729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e04f9270e7bd9277315236c8f83ecc5537fd0907204e9c9f75a2464091a59`  
		Last Modified: Tue, 21 Nov 2023 06:24:19 GMT  
		Size: 22.7 MB (22727407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7466297e667840b4907e1e017052f34ebebba91fb7a476d17a10259cf5a264fc`  
		Last Modified: Tue, 21 Nov 2023 06:24:41 GMT  
		Size: 61.6 MB (61561534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8128c2db4bac59c665360b03846fbc4d0013d87270dad0af442499ef7088c34`  
		Last Modified: Tue, 21 Nov 2023 06:25:23 GMT  
		Size: 184.4 MB (184384991 bytes)  
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
$ docker pull buildpack-deps@sha256:ff34a667d81db5798aaf33085e09a789e13a45e7b48e804c87809631102b0ec7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.0 MB (362952942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b6ecc5afbeef5b86b674ec0993915e6bb01b89f9c44f901050856f10a1bf0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:23:59 GMT
ADD file:209097c8dfcefec7951851d25bc9e8c1d56aefed076c682c5f2e077cc05aeaf8 in / 
# Tue, 21 Nov 2023 04:24:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:53:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:56:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d694a6aceb98c067febf569d227d6249cd8d39b11dead73e4840d07861a25e9`  
		Last Modified: Tue, 21 Nov 2023 04:28:27 GMT  
		Size: 53.6 MB (53575858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71d255e683d12334b12df8a9e23692d03ce5d514a74efe4553f12269885d87`  
		Last Modified: Tue, 21 Nov 2023 07:06:46 GMT  
		Size: 25.7 MB (25698746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a54ea75827017eaea7b7055d8fca97c313c72d7a237502105b83ab018bd5ad`  
		Last Modified: Tue, 21 Nov 2023 07:07:08 GMT  
		Size: 69.6 MB (69584187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e986f224599c525ac40be9636489d408b4daff891bb3567a7986f6ae5c817cc1`  
		Last Modified: Tue, 21 Nov 2023 07:07:49 GMT  
		Size: 214.1 MB (214094151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d1822d31d3c58472a93084eaa39396b37585eb538479e3ca57d5e2e50d7470c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318217378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0dcda8469adc1e80e5b8779671680724ff22c47c0c87e7d0658d100902caa19`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:00 GMT
ADD file:8bb55d91755618d4e84d57150867ddbe9513d01cf9543fa953cf7cd1745397ac in / 
# Tue, 21 Nov 2023 05:04:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:06:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:07:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7318387eb66a53962a6ff8f603919b1f2eebd63059538ee442fb3f3643d79fd1`  
		Last Modified: Tue, 21 Nov 2023 05:10:07 GMT  
		Size: 47.9 MB (47943002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a20203ebe78a0c1643a97475f1f406b6af2dedd0e14005e4ca4bbeca0470d21`  
		Last Modified: Tue, 21 Nov 2023 06:16:17 GMT  
		Size: 24.0 MB (24045086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c99a00cc05c2b6ae13b5a9c1b8997b9915ab687454a9fcd00d485bbb2d9a5d`  
		Last Modified: Tue, 21 Nov 2023 06:16:33 GMT  
		Size: 63.1 MB (63132875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cf7e37f4b53af6dfd3bdea89a2078a221738e8eeade3f46428f3def3e4c97c`  
		Last Modified: Tue, 21 Nov 2023 06:17:01 GMT  
		Size: 183.1 MB (183096415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:d53c880810f72ba3a0b875b502506201f5059fb6649867ded0721135ff0b76f5
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
$ docker pull buildpack-deps@sha256:f8e864b6759c58dd553d3638f996a6918822de02ea1c443cc92559e7e7cfdad4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70083136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f201a632265b71438164333d2c732c7918b180c004463264455c253dcc1afc98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:42 GMT
ADD file:e217c81e321b5371a29bea20d4b2802fa8223262c92dbffd268ec38c8951181c in / 
# Tue, 21 Nov 2023 05:00:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:14:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6ffd672cfa56bc540c641f8f5c7b5216716ae5d6336d6698ebdf8fb8cae06e0`  
		Last Modified: Tue, 21 Nov 2023 05:03:32 GMT  
		Size: 47.4 MB (47355729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e04f9270e7bd9277315236c8f83ecc5537fd0907204e9c9f75a2464091a59`  
		Last Modified: Tue, 21 Nov 2023 06:24:19 GMT  
		Size: 22.7 MB (22727407 bytes)  
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
$ docker pull buildpack-deps@sha256:784282fea3a27c11b3c8668acf83fdf5fa1f805e2c648264766bd6bedda9f057
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79274604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:927ae87f00aa3f0f3b5f1fccbc2848eda2dec7b3d1754259fdd0af08c5485cf4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:23:59 GMT
ADD file:209097c8dfcefec7951851d25bc9e8c1d56aefed076c682c5f2e077cc05aeaf8 in / 
# Tue, 21 Nov 2023 04:24:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d694a6aceb98c067febf569d227d6249cd8d39b11dead73e4840d07861a25e9`  
		Last Modified: Tue, 21 Nov 2023 04:28:27 GMT  
		Size: 53.6 MB (53575858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71d255e683d12334b12df8a9e23692d03ce5d514a74efe4553f12269885d87`  
		Last Modified: Tue, 21 Nov 2023 07:06:46 GMT  
		Size: 25.7 MB (25698746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:56dea1f8a449f195ffdd426569472adfdcbb657344ea182789923be11c8b79f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71988088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba3cde7adf1be7b7277ab9b2cd62cc5ea051cb781184b34e1645be1f946290f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:00 GMT
ADD file:8bb55d91755618d4e84d57150867ddbe9513d01cf9543fa953cf7cd1745397ac in / 
# Tue, 21 Nov 2023 05:04:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7318387eb66a53962a6ff8f603919b1f2eebd63059538ee442fb3f3643d79fd1`  
		Last Modified: Tue, 21 Nov 2023 05:10:07 GMT  
		Size: 47.9 MB (47943002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a20203ebe78a0c1643a97475f1f406b6af2dedd0e14005e4ca4bbeca0470d21`  
		Last Modified: Tue, 21 Nov 2023 06:16:17 GMT  
		Size: 24.0 MB (24045086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:c99b8a43be556e5b407214a5ea1801af92a581294119cc772136046613486699
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
$ docker pull buildpack-deps@sha256:adec01003a17f6b964516dc2082a5c112ef7132fd914810661c01e4fde930972
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131644670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3bc44cf636b514c0c186654ac43d24bd92f970d9fdcd2dca3b0516e058959c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:42 GMT
ADD file:e217c81e321b5371a29bea20d4b2802fa8223262c92dbffd268ec38c8951181c in / 
# Tue, 21 Nov 2023 05:00:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:14:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6ffd672cfa56bc540c641f8f5c7b5216716ae5d6336d6698ebdf8fb8cae06e0`  
		Last Modified: Tue, 21 Nov 2023 05:03:32 GMT  
		Size: 47.4 MB (47355729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e04f9270e7bd9277315236c8f83ecc5537fd0907204e9c9f75a2464091a59`  
		Last Modified: Tue, 21 Nov 2023 06:24:19 GMT  
		Size: 22.7 MB (22727407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7466297e667840b4907e1e017052f34ebebba91fb7a476d17a10259cf5a264fc`  
		Last Modified: Tue, 21 Nov 2023 06:24:41 GMT  
		Size: 61.6 MB (61561534 bytes)  
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
$ docker pull buildpack-deps@sha256:ad518e13047a2bffa7358d6ed80141ee89918b12549d94563fe33dfe97693f63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148858791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1afccc4310e63668ea2fa68e7ed2114f91aa1c4023a673f0dbd3cb0d533ddd7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:23:59 GMT
ADD file:209097c8dfcefec7951851d25bc9e8c1d56aefed076c682c5f2e077cc05aeaf8 in / 
# Tue, 21 Nov 2023 04:24:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:53:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d694a6aceb98c067febf569d227d6249cd8d39b11dead73e4840d07861a25e9`  
		Last Modified: Tue, 21 Nov 2023 04:28:27 GMT  
		Size: 53.6 MB (53575858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71d255e683d12334b12df8a9e23692d03ce5d514a74efe4553f12269885d87`  
		Last Modified: Tue, 21 Nov 2023 07:06:46 GMT  
		Size: 25.7 MB (25698746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a54ea75827017eaea7b7055d8fca97c313c72d7a237502105b83ab018bd5ad`  
		Last Modified: Tue, 21 Nov 2023 07:07:08 GMT  
		Size: 69.6 MB (69584187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a1788f5a7099541c5a0691f88050070dd6e2d5f4b0c97777b19ed32f799c64e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135120963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f2372afa7eb1de18c0332fe8e706503fe4a85393e04c4f9b30e3689e074ea3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:00 GMT
ADD file:8bb55d91755618d4e84d57150867ddbe9513d01cf9543fa953cf7cd1745397ac in / 
# Tue, 21 Nov 2023 05:04:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:06:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7318387eb66a53962a6ff8f603919b1f2eebd63059538ee442fb3f3643d79fd1`  
		Last Modified: Tue, 21 Nov 2023 05:10:07 GMT  
		Size: 47.9 MB (47943002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a20203ebe78a0c1643a97475f1f406b6af2dedd0e14005e4ca4bbeca0470d21`  
		Last Modified: Tue, 21 Nov 2023 06:16:17 GMT  
		Size: 24.0 MB (24045086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c99a00cc05c2b6ae13b5a9c1b8997b9915ab687454a9fcd00d485bbb2d9a5d`  
		Last Modified: Tue, 21 Nov 2023 06:16:33 GMT  
		Size: 63.1 MB (63132875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:7db9a67390ff0f4b734d20a28702170dc292a6c6bb0f11f08b5c78a8bf71f157
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
$ docker pull buildpack-deps@sha256:e4159d16939a5804c07e4dd959b0c9dcaddbc3744d9e3d04b0f1963bd11b989d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.7 MB (347687227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00c1f4c60036b1a9b1fab9754a256090009d8c3722fe8d0473c3b62f4e20e428`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:02:24 GMT
ADD file:b3c8930f9373d4b494084a470670d4cc731173a6b8f430173b03a3352a74180b in / 
# Tue, 21 Nov 2023 05:02:24 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:22:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:23:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9f882881657ea279897d7d6f0016a79c0e107f1eb6d1fbcfeb6c31891d0af0`  
		Last Modified: Tue, 21 Nov 2023 05:07:16 GMT  
		Size: 47.2 MB (47222272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13edd38987d456d8e87f699a7a27f33d76ba9ad1e72d127632cccf39db11078`  
		Last Modified: Tue, 21 Nov 2023 06:27:56 GMT  
		Size: 24.8 MB (24757246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eeb03a8240f153b8290020f4477589eab862383b6104a427817ada174625af9`  
		Last Modified: Tue, 21 Nov 2023 06:28:15 GMT  
		Size: 63.0 MB (63026793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211e51dfd6f73198b06c3e486450d2339a25e5b62b650b88fd94e54420d115fe`  
		Last Modified: Tue, 21 Nov 2023 06:29:00 GMT  
		Size: 212.7 MB (212680916 bytes)  
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
$ docker pull buildpack-deps@sha256:b2e27262ab28153789fa0690506b74172e483469bcf54e531d38a75b4dc470a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.2 MB (377166522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcbee65158084b93c96a37687ed9010fa6173adea090417e413b34468b86b146`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 06:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:16:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9f358858592f5e90a4632a64fcf6ddf202edaa456ab82e9ee3179bcd65f13a`  
		Last Modified: Wed, 15 Nov 2023 06:22:50 GMT  
		Size: 25.8 MB (25827983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945297878d74e2e2c19a6a94a85622c203ecece7a80062df11aa21c95b4cbace`  
		Last Modified: Wed, 15 Nov 2023 06:23:06 GMT  
		Size: 65.6 MB (65609297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c643ecec1685aebb7183262bb6877f888a3954564374f4b2da8cd655ab204f2`  
		Last Modified: Wed, 15 Nov 2023 06:23:37 GMT  
		Size: 236.2 MB (236234015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:dc366815e1bee218bfc5028b9b8b34382e4c63912ad23e4a66741ae8e321a39c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.8 MB (391761890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14431b06174dd9effe045e6123d9fe4244a1894951a16f106cc77063c14cf147`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 07:50:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 07:51:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 07:53:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45aae569aec31ff4357ae059a8e608470587e67c959acb2daee68188b4a1d72`  
		Last Modified: Wed, 15 Nov 2023 07:54:12 GMT  
		Size: 27.3 MB (27304463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21f7b2672fa2cfcfbb88d236a9d3c18479bd05f2cfc6504481d3006ee65214`  
		Last Modified: Wed, 15 Nov 2023 07:54:36 GMT  
		Size: 67.3 MB (67270819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02783d09b275fdf784fe78459529f7b1a4f0303b00ea8242e1841a65c913861`  
		Last Modified: Wed, 15 Nov 2023 07:55:35 GMT  
		Size: 246.7 MB (246720235 bytes)  
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
$ docker pull buildpack-deps@sha256:f7122304c08fa3322fb619c28b1d079afd3d5d1ae28d49a7c9e5e054c1b641aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.1 MB (392079404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd296328898f802900eb913bb6523c2ceecf64df4a720940a7c51218cce74b7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:26:49 GMT
ADD file:dc6f1d4d555ba3f35237b7e67b320c18ac6e1c8d12a95eedb8a5230f42402844 in / 
# Tue, 21 Nov 2023 04:26:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:03:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:05:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c7e2ccd81c8e1fab8cf4a7e3dcfcc9c9057946f10830bacc66f9e35e00b25e3`  
		Last Modified: Tue, 21 Nov 2023 04:32:41 GMT  
		Size: 53.4 MB (53437879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da93de48b4e366a300fc98f49a68981fa34793ac393d57b3adda3769aff47f`  
		Last Modified: Tue, 21 Nov 2023 07:10:36 GMT  
		Size: 28.8 MB (28814830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09699f0245492a67f8cf23ca1a57b1830e534c2904c0101f5032102ad5f2c4c1`  
		Last Modified: Tue, 21 Nov 2023 07:10:57 GMT  
		Size: 70.9 MB (70922067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67883ae22a135174fd28adf25d7ee6ae5e6bce0ed0f2184e2e8693a052f4d849`  
		Last Modified: Tue, 21 Nov 2023 07:11:43 GMT  
		Size: 238.9 MB (238904628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fc3c7f7fdec6e003481bbeb0997f6daa643394d8da369bd4790ac484bf03a5bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.5 MB (353469255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c09c825610f278f9458ee2308b22e1fb54a3e9f39fe8f41b26fcba0d3d2b866a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:07:59 GMT
ADD file:d0b90d4f8aa4259bbd6e1887bf2da65394e444995622363495d2e13ad00154bf in / 
# Tue, 21 Nov 2023 05:08:07 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:12:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:13:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b094bae18b4460a8208634d7220fba165e3979b123ddcbdd060fb9c73c37f2b`  
		Last Modified: Tue, 21 Nov 2023 05:12:26 GMT  
		Size: 49.0 MB (48970235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e58498ddda5b5285e62304a232a3204b2c0d769172de15744b3afdda3b07cb`  
		Last Modified: Tue, 21 Nov 2023 06:18:57 GMT  
		Size: 26.8 MB (26829362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09114f0213626e79784208aa286e09335b4ba1f291eb0eca1b085809f09d3a4`  
		Last Modified: Tue, 21 Nov 2023 06:19:11 GMT  
		Size: 66.5 MB (66490948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258f4a65c94de18a1fd53de8a964d1e72298a66a44688d4fcc60dd699744a8ae`  
		Last Modified: Tue, 21 Nov 2023 06:19:41 GMT  
		Size: 211.2 MB (211178710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:d45682fe48133a66ef3b5d2a535b87687296abd7a0f00917ad9264053e63091d
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
$ docker pull buildpack-deps@sha256:a7da9b745838c041278c9aeba2fbb2ca1837a9530b6f96239c8f5c58d6b963ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71979518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffd2c0fa32747f25861583e129cca4b26127abcc0f95d20b84cbe0118c62cefc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:02:24 GMT
ADD file:b3c8930f9373d4b494084a470670d4cc731173a6b8f430173b03a3352a74180b in / 
# Tue, 21 Nov 2023 05:02:24 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:22:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9f882881657ea279897d7d6f0016a79c0e107f1eb6d1fbcfeb6c31891d0af0`  
		Last Modified: Tue, 21 Nov 2023 05:07:16 GMT  
		Size: 47.2 MB (47222272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13edd38987d456d8e87f699a7a27f33d76ba9ad1e72d127632cccf39db11078`  
		Last Modified: Tue, 21 Nov 2023 06:27:56 GMT  
		Size: 24.8 MB (24757246 bytes)  
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
$ docker pull buildpack-deps@sha256:57ab995ed8f689c7931c0a83b6f2b948ace8c98a21555e6f297fde5918bf4996
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75323210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905f2ed7423347e36afbd048bfece66a4d84b57c278a57d081648102e9399b77`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 06:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9f358858592f5e90a4632a64fcf6ddf202edaa456ab82e9ee3179bcd65f13a`  
		Last Modified: Wed, 15 Nov 2023 06:22:50 GMT  
		Size: 25.8 MB (25827983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8c6c188fd23ca22f501be40067c2957e2a3a5d1f7f4c18b0bfd7e2bdf9455fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77770836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f98cf6f937c6e49091148e07808fcb8d6c74b67e7a76d289068b9d3fdb2e89`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 07:50:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45aae569aec31ff4357ae059a8e608470587e67c959acb2daee68188b4a1d72`  
		Last Modified: Wed, 15 Nov 2023 07:54:12 GMT  
		Size: 27.3 MB (27304463 bytes)  
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
$ docker pull buildpack-deps@sha256:965f912e338611b668babc493a452d7633aada0b922596c5ef12cc6e50e27a3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82252709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76bdba459863fec3e91bd7c853b0ea34383073b319aa7a132424943ec736438d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:26:49 GMT
ADD file:dc6f1d4d555ba3f35237b7e67b320c18ac6e1c8d12a95eedb8a5230f42402844 in / 
# Tue, 21 Nov 2023 04:26:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:03:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c7e2ccd81c8e1fab8cf4a7e3dcfcc9c9057946f10830bacc66f9e35e00b25e3`  
		Last Modified: Tue, 21 Nov 2023 04:32:41 GMT  
		Size: 53.4 MB (53437879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da93de48b4e366a300fc98f49a68981fa34793ac393d57b3adda3769aff47f`  
		Last Modified: Tue, 21 Nov 2023 07:10:36 GMT  
		Size: 28.8 MB (28814830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3cec0b4b3003b6e8ca7b66e3ea1180aacfef23d35fe6903a4accc9f2e403d199
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75799597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31893a587eeb03b3917a1a1c908f5d45b32756818b46d56b8e081ce5579ba7f1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:07:59 GMT
ADD file:d0b90d4f8aa4259bbd6e1887bf2da65394e444995622363495d2e13ad00154bf in / 
# Tue, 21 Nov 2023 05:08:07 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b094bae18b4460a8208634d7220fba165e3979b123ddcbdd060fb9c73c37f2b`  
		Last Modified: Tue, 21 Nov 2023 05:12:26 GMT  
		Size: 49.0 MB (48970235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e58498ddda5b5285e62304a232a3204b2c0d769172de15744b3afdda3b07cb`  
		Last Modified: Tue, 21 Nov 2023 06:18:57 GMT  
		Size: 26.8 MB (26829362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:8379a6d16f139d251f0ae3b4a28e81077eb45e62a893a4832250166eb3466c58
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
$ docker pull buildpack-deps@sha256:1d4213b5ecd42e4e5d502fa5018177bd7bb7a3f432a8efda32f3fcf3e25470a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135006311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbf22d4e85d7661a17d70059b767ea7b7860e81f80d7c21d4e3894acfc178b9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:02:24 GMT
ADD file:b3c8930f9373d4b494084a470670d4cc731173a6b8f430173b03a3352a74180b in / 
# Tue, 21 Nov 2023 05:02:24 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:22:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9f882881657ea279897d7d6f0016a79c0e107f1eb6d1fbcfeb6c31891d0af0`  
		Last Modified: Tue, 21 Nov 2023 05:07:16 GMT  
		Size: 47.2 MB (47222272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13edd38987d456d8e87f699a7a27f33d76ba9ad1e72d127632cccf39db11078`  
		Last Modified: Tue, 21 Nov 2023 06:27:56 GMT  
		Size: 24.8 MB (24757246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eeb03a8240f153b8290020f4477589eab862383b6104a427817ada174625af9`  
		Last Modified: Tue, 21 Nov 2023 06:28:15 GMT  
		Size: 63.0 MB (63026793 bytes)  
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
$ docker pull buildpack-deps@sha256:996ba0fb550a4858251501430c769432e96b323ab0b37fece0320e74ca51d64e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.9 MB (140932507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd12d0b0c131a48bd2384a168b67b7974f1533250aa34782f5a4e6a43c24a523`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 06:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9f358858592f5e90a4632a64fcf6ddf202edaa456ab82e9ee3179bcd65f13a`  
		Last Modified: Wed, 15 Nov 2023 06:22:50 GMT  
		Size: 25.8 MB (25827983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945297878d74e2e2c19a6a94a85622c203ecece7a80062df11aa21c95b4cbace`  
		Last Modified: Wed, 15 Nov 2023 06:23:06 GMT  
		Size: 65.6 MB (65609297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6a71927e5c8018db89d04ec95f5d9c4a5ddaeadec1a6b19a620de50b9e3381de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.0 MB (145041655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769c21d85929a1dbb4f206fbca8a9aefcf988596b5655c3a1486b1997768bbc5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 07:50:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 07:51:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45aae569aec31ff4357ae059a8e608470587e67c959acb2daee68188b4a1d72`  
		Last Modified: Wed, 15 Nov 2023 07:54:12 GMT  
		Size: 27.3 MB (27304463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21f7b2672fa2cfcfbb88d236a9d3c18479bd05f2cfc6504481d3006ee65214`  
		Last Modified: Wed, 15 Nov 2023 07:54:36 GMT  
		Size: 67.3 MB (67270819 bytes)  
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
$ docker pull buildpack-deps@sha256:d10b4a6b3ef635a2b679169bacda8ac4b674df60ae3371a03c8a1f5cc86e7a93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.2 MB (153174776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897ba107c9d649eae78c14111b541fbffa91311376657fbeebbcb7275085fe88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:26:49 GMT
ADD file:dc6f1d4d555ba3f35237b7e67b320c18ac6e1c8d12a95eedb8a5230f42402844 in / 
# Tue, 21 Nov 2023 04:26:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:03:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c7e2ccd81c8e1fab8cf4a7e3dcfcc9c9057946f10830bacc66f9e35e00b25e3`  
		Last Modified: Tue, 21 Nov 2023 04:32:41 GMT  
		Size: 53.4 MB (53437879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da93de48b4e366a300fc98f49a68981fa34793ac393d57b3adda3769aff47f`  
		Last Modified: Tue, 21 Nov 2023 07:10:36 GMT  
		Size: 28.8 MB (28814830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09699f0245492a67f8cf23ca1a57b1830e534c2904c0101f5032102ad5f2c4c1`  
		Last Modified: Tue, 21 Nov 2023 07:10:57 GMT  
		Size: 70.9 MB (70922067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c1151634c7e3a017b784f1eb9a20d31ca5b19e61af07410c71d068ffca257b06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142290545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:585f78d00d4e7d5176cfb4e20e019ad8271fa52f40eae6313924bd54827c4bde`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:07:59 GMT
ADD file:d0b90d4f8aa4259bbd6e1887bf2da65394e444995622363495d2e13ad00154bf in / 
# Tue, 21 Nov 2023 05:08:07 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:12:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b094bae18b4460a8208634d7220fba165e3979b123ddcbdd060fb9c73c37f2b`  
		Last Modified: Tue, 21 Nov 2023 05:12:26 GMT  
		Size: 49.0 MB (48970235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e58498ddda5b5285e62304a232a3204b2c0d769172de15744b3afdda3b07cb`  
		Last Modified: Tue, 21 Nov 2023 06:18:57 GMT  
		Size: 26.8 MB (26829362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09114f0213626e79784208aa286e09335b4ba1f291eb0eca1b085809f09d3a4`  
		Last Modified: Tue, 21 Nov 2023 06:19:11 GMT  
		Size: 66.5 MB (66490948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:trixie`

```console
$ docker pull buildpack-deps@sha256:7db9a67390ff0f4b734d20a28702170dc292a6c6bb0f11f08b5c78a8bf71f157
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
$ docker pull buildpack-deps@sha256:e4159d16939a5804c07e4dd959b0c9dcaddbc3744d9e3d04b0f1963bd11b989d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.7 MB (347687227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00c1f4c60036b1a9b1fab9754a256090009d8c3722fe8d0473c3b62f4e20e428`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:02:24 GMT
ADD file:b3c8930f9373d4b494084a470670d4cc731173a6b8f430173b03a3352a74180b in / 
# Tue, 21 Nov 2023 05:02:24 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:22:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:23:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9f882881657ea279897d7d6f0016a79c0e107f1eb6d1fbcfeb6c31891d0af0`  
		Last Modified: Tue, 21 Nov 2023 05:07:16 GMT  
		Size: 47.2 MB (47222272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13edd38987d456d8e87f699a7a27f33d76ba9ad1e72d127632cccf39db11078`  
		Last Modified: Tue, 21 Nov 2023 06:27:56 GMT  
		Size: 24.8 MB (24757246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eeb03a8240f153b8290020f4477589eab862383b6104a427817ada174625af9`  
		Last Modified: Tue, 21 Nov 2023 06:28:15 GMT  
		Size: 63.0 MB (63026793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211e51dfd6f73198b06c3e486450d2339a25e5b62b650b88fd94e54420d115fe`  
		Last Modified: Tue, 21 Nov 2023 06:29:00 GMT  
		Size: 212.7 MB (212680916 bytes)  
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
$ docker pull buildpack-deps@sha256:b2e27262ab28153789fa0690506b74172e483469bcf54e531d38a75b4dc470a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.2 MB (377166522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcbee65158084b93c96a37687ed9010fa6173adea090417e413b34468b86b146`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 06:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:16:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9f358858592f5e90a4632a64fcf6ddf202edaa456ab82e9ee3179bcd65f13a`  
		Last Modified: Wed, 15 Nov 2023 06:22:50 GMT  
		Size: 25.8 MB (25827983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945297878d74e2e2c19a6a94a85622c203ecece7a80062df11aa21c95b4cbace`  
		Last Modified: Wed, 15 Nov 2023 06:23:06 GMT  
		Size: 65.6 MB (65609297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c643ecec1685aebb7183262bb6877f888a3954564374f4b2da8cd655ab204f2`  
		Last Modified: Wed, 15 Nov 2023 06:23:37 GMT  
		Size: 236.2 MB (236234015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; 386

```console
$ docker pull buildpack-deps@sha256:dc366815e1bee218bfc5028b9b8b34382e4c63912ad23e4a66741ae8e321a39c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.8 MB (391761890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14431b06174dd9effe045e6123d9fe4244a1894951a16f106cc77063c14cf147`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 07:50:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 07:51:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 07:53:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45aae569aec31ff4357ae059a8e608470587e67c959acb2daee68188b4a1d72`  
		Last Modified: Wed, 15 Nov 2023 07:54:12 GMT  
		Size: 27.3 MB (27304463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21f7b2672fa2cfcfbb88d236a9d3c18479bd05f2cfc6504481d3006ee65214`  
		Last Modified: Wed, 15 Nov 2023 07:54:36 GMT  
		Size: 67.3 MB (67270819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02783d09b275fdf784fe78459529f7b1a4f0303b00ea8242e1841a65c913861`  
		Last Modified: Wed, 15 Nov 2023 07:55:35 GMT  
		Size: 246.7 MB (246720235 bytes)  
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
$ docker pull buildpack-deps@sha256:f7122304c08fa3322fb619c28b1d079afd3d5d1ae28d49a7c9e5e054c1b641aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.1 MB (392079404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd296328898f802900eb913bb6523c2ceecf64df4a720940a7c51218cce74b7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:26:49 GMT
ADD file:dc6f1d4d555ba3f35237b7e67b320c18ac6e1c8d12a95eedb8a5230f42402844 in / 
# Tue, 21 Nov 2023 04:26:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:03:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:05:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c7e2ccd81c8e1fab8cf4a7e3dcfcc9c9057946f10830bacc66f9e35e00b25e3`  
		Last Modified: Tue, 21 Nov 2023 04:32:41 GMT  
		Size: 53.4 MB (53437879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da93de48b4e366a300fc98f49a68981fa34793ac393d57b3adda3769aff47f`  
		Last Modified: Tue, 21 Nov 2023 07:10:36 GMT  
		Size: 28.8 MB (28814830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09699f0245492a67f8cf23ca1a57b1830e534c2904c0101f5032102ad5f2c4c1`  
		Last Modified: Tue, 21 Nov 2023 07:10:57 GMT  
		Size: 70.9 MB (70922067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67883ae22a135174fd28adf25d7ee6ae5e6bce0ed0f2184e2e8693a052f4d849`  
		Last Modified: Tue, 21 Nov 2023 07:11:43 GMT  
		Size: 238.9 MB (238904628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fc3c7f7fdec6e003481bbeb0997f6daa643394d8da369bd4790ac484bf03a5bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.5 MB (353469255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c09c825610f278f9458ee2308b22e1fb54a3e9f39fe8f41b26fcba0d3d2b866a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:07:59 GMT
ADD file:d0b90d4f8aa4259bbd6e1887bf2da65394e444995622363495d2e13ad00154bf in / 
# Tue, 21 Nov 2023 05:08:07 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:12:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:13:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b094bae18b4460a8208634d7220fba165e3979b123ddcbdd060fb9c73c37f2b`  
		Last Modified: Tue, 21 Nov 2023 05:12:26 GMT  
		Size: 49.0 MB (48970235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e58498ddda5b5285e62304a232a3204b2c0d769172de15744b3afdda3b07cb`  
		Last Modified: Tue, 21 Nov 2023 06:18:57 GMT  
		Size: 26.8 MB (26829362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09114f0213626e79784208aa286e09335b4ba1f291eb0eca1b085809f09d3a4`  
		Last Modified: Tue, 21 Nov 2023 06:19:11 GMT  
		Size: 66.5 MB (66490948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258f4a65c94de18a1fd53de8a964d1e72298a66a44688d4fcc60dd699744a8ae`  
		Last Modified: Tue, 21 Nov 2023 06:19:41 GMT  
		Size: 211.2 MB (211178710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:trixie-curl`

```console
$ docker pull buildpack-deps@sha256:d45682fe48133a66ef3b5d2a535b87687296abd7a0f00917ad9264053e63091d
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
$ docker pull buildpack-deps@sha256:a7da9b745838c041278c9aeba2fbb2ca1837a9530b6f96239c8f5c58d6b963ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71979518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffd2c0fa32747f25861583e129cca4b26127abcc0f95d20b84cbe0118c62cefc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:02:24 GMT
ADD file:b3c8930f9373d4b494084a470670d4cc731173a6b8f430173b03a3352a74180b in / 
# Tue, 21 Nov 2023 05:02:24 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:22:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9f882881657ea279897d7d6f0016a79c0e107f1eb6d1fbcfeb6c31891d0af0`  
		Last Modified: Tue, 21 Nov 2023 05:07:16 GMT  
		Size: 47.2 MB (47222272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13edd38987d456d8e87f699a7a27f33d76ba9ad1e72d127632cccf39db11078`  
		Last Modified: Tue, 21 Nov 2023 06:27:56 GMT  
		Size: 24.8 MB (24757246 bytes)  
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
$ docker pull buildpack-deps@sha256:57ab995ed8f689c7931c0a83b6f2b948ace8c98a21555e6f297fde5918bf4996
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75323210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905f2ed7423347e36afbd048bfece66a4d84b57c278a57d081648102e9399b77`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 06:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9f358858592f5e90a4632a64fcf6ddf202edaa456ab82e9ee3179bcd65f13a`  
		Last Modified: Wed, 15 Nov 2023 06:22:50 GMT  
		Size: 25.8 MB (25827983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8c6c188fd23ca22f501be40067c2957e2a3a5d1f7f4c18b0bfd7e2bdf9455fba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77770836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f98cf6f937c6e49091148e07808fcb8d6c74b67e7a76d289068b9d3fdb2e89`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 07:50:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45aae569aec31ff4357ae059a8e608470587e67c959acb2daee68188b4a1d72`  
		Last Modified: Wed, 15 Nov 2023 07:54:12 GMT  
		Size: 27.3 MB (27304463 bytes)  
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
$ docker pull buildpack-deps@sha256:965f912e338611b668babc493a452d7633aada0b922596c5ef12cc6e50e27a3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82252709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76bdba459863fec3e91bd7c853b0ea34383073b319aa7a132424943ec736438d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:26:49 GMT
ADD file:dc6f1d4d555ba3f35237b7e67b320c18ac6e1c8d12a95eedb8a5230f42402844 in / 
# Tue, 21 Nov 2023 04:26:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:03:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c7e2ccd81c8e1fab8cf4a7e3dcfcc9c9057946f10830bacc66f9e35e00b25e3`  
		Last Modified: Tue, 21 Nov 2023 04:32:41 GMT  
		Size: 53.4 MB (53437879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da93de48b4e366a300fc98f49a68981fa34793ac393d57b3adda3769aff47f`  
		Last Modified: Tue, 21 Nov 2023 07:10:36 GMT  
		Size: 28.8 MB (28814830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3cec0b4b3003b6e8ca7b66e3ea1180aacfef23d35fe6903a4accc9f2e403d199
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75799597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31893a587eeb03b3917a1a1c908f5d45b32756818b46d56b8e081ce5579ba7f1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:07:59 GMT
ADD file:d0b90d4f8aa4259bbd6e1887bf2da65394e444995622363495d2e13ad00154bf in / 
# Tue, 21 Nov 2023 05:08:07 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b094bae18b4460a8208634d7220fba165e3979b123ddcbdd060fb9c73c37f2b`  
		Last Modified: Tue, 21 Nov 2023 05:12:26 GMT  
		Size: 49.0 MB (48970235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e58498ddda5b5285e62304a232a3204b2c0d769172de15744b3afdda3b07cb`  
		Last Modified: Tue, 21 Nov 2023 06:18:57 GMT  
		Size: 26.8 MB (26829362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:trixie-scm`

```console
$ docker pull buildpack-deps@sha256:8379a6d16f139d251f0ae3b4a28e81077eb45e62a893a4832250166eb3466c58
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
$ docker pull buildpack-deps@sha256:1d4213b5ecd42e4e5d502fa5018177bd7bb7a3f432a8efda32f3fcf3e25470a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135006311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbf22d4e85d7661a17d70059b767ea7b7860e81f80d7c21d4e3894acfc178b9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:02:24 GMT
ADD file:b3c8930f9373d4b494084a470670d4cc731173a6b8f430173b03a3352a74180b in / 
# Tue, 21 Nov 2023 05:02:24 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:22:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0e9f882881657ea279897d7d6f0016a79c0e107f1eb6d1fbcfeb6c31891d0af0`  
		Last Modified: Tue, 21 Nov 2023 05:07:16 GMT  
		Size: 47.2 MB (47222272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13edd38987d456d8e87f699a7a27f33d76ba9ad1e72d127632cccf39db11078`  
		Last Modified: Tue, 21 Nov 2023 06:27:56 GMT  
		Size: 24.8 MB (24757246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eeb03a8240f153b8290020f4477589eab862383b6104a427817ada174625af9`  
		Last Modified: Tue, 21 Nov 2023 06:28:15 GMT  
		Size: 63.0 MB (63026793 bytes)  
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
$ docker pull buildpack-deps@sha256:996ba0fb550a4858251501430c769432e96b323ab0b37fece0320e74ca51d64e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.9 MB (140932507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd12d0b0c131a48bd2384a168b67b7974f1533250aa34782f5a4e6a43c24a523`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 06:14:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 06:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9f358858592f5e90a4632a64fcf6ddf202edaa456ab82e9ee3179bcd65f13a`  
		Last Modified: Wed, 15 Nov 2023 06:22:50 GMT  
		Size: 25.8 MB (25827983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945297878d74e2e2c19a6a94a85622c203ecece7a80062df11aa21c95b4cbace`  
		Last Modified: Wed, 15 Nov 2023 06:23:06 GMT  
		Size: 65.6 MB (65609297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6a71927e5c8018db89d04ec95f5d9c4a5ddaeadec1a6b19a620de50b9e3381de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.0 MB (145041655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769c21d85929a1dbb4f206fbca8a9aefcf988596b5655c3a1486b1997768bbc5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 07:50:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 07:51:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45aae569aec31ff4357ae059a8e608470587e67c959acb2daee68188b4a1d72`  
		Last Modified: Wed, 15 Nov 2023 07:54:12 GMT  
		Size: 27.3 MB (27304463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea21f7b2672fa2cfcfbb88d236a9d3c18479bd05f2cfc6504481d3006ee65214`  
		Last Modified: Wed, 15 Nov 2023 07:54:36 GMT  
		Size: 67.3 MB (67270819 bytes)  
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
$ docker pull buildpack-deps@sha256:d10b4a6b3ef635a2b679169bacda8ac4b674df60ae3371a03c8a1f5cc86e7a93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.2 MB (153174776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897ba107c9d649eae78c14111b541fbffa91311376657fbeebbcb7275085fe88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:26:49 GMT
ADD file:dc6f1d4d555ba3f35237b7e67b320c18ac6e1c8d12a95eedb8a5230f42402844 in / 
# Tue, 21 Nov 2023 04:26:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:03:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:03:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c7e2ccd81c8e1fab8cf4a7e3dcfcc9c9057946f10830bacc66f9e35e00b25e3`  
		Last Modified: Tue, 21 Nov 2023 04:32:41 GMT  
		Size: 53.4 MB (53437879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da93de48b4e366a300fc98f49a68981fa34793ac393d57b3adda3769aff47f`  
		Last Modified: Tue, 21 Nov 2023 07:10:36 GMT  
		Size: 28.8 MB (28814830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09699f0245492a67f8cf23ca1a57b1830e534c2904c0101f5032102ad5f2c4c1`  
		Last Modified: Tue, 21 Nov 2023 07:10:57 GMT  
		Size: 70.9 MB (70922067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c1151634c7e3a017b784f1eb9a20d31ca5b19e61af07410c71d068ffca257b06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142290545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:585f78d00d4e7d5176cfb4e20e019ad8271fa52f40eae6313924bd54827c4bde`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:07:59 GMT
ADD file:d0b90d4f8aa4259bbd6e1887bf2da65394e444995622363495d2e13ad00154bf in / 
# Tue, 21 Nov 2023 05:08:07 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:12:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b094bae18b4460a8208634d7220fba165e3979b123ddcbdd060fb9c73c37f2b`  
		Last Modified: Tue, 21 Nov 2023 05:12:26 GMT  
		Size: 49.0 MB (48970235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e58498ddda5b5285e62304a232a3204b2c0d769172de15744b3afdda3b07cb`  
		Last Modified: Tue, 21 Nov 2023 06:18:57 GMT  
		Size: 26.8 MB (26829362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09114f0213626e79784208aa286e09335b4ba1f291eb0eca1b085809f09d3a4`  
		Last Modified: Tue, 21 Nov 2023 06:19:11 GMT  
		Size: 66.5 MB (66490948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:b64036ac9f9e82d6152e2397921cccb86cdf7aa797d13de79f61d3301955ceee
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
$ docker pull buildpack-deps@sha256:fcf7edb8ce652541065efcbc0f507104b809f1e99b8353836e0713ff4525e41d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.9 MB (348901354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e89ade2f919c3a4ff65a0eb3b9f73bc2ae64a6ba48b4f89ea808f2dfdaab921a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:33 GMT
ADD file:b1618939ac80f9d3256d12ed22ac3e37f61dc396e5370e7a4013561a073af181 in / 
# Tue, 21 Nov 2023 05:01:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:19:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:19:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:21:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:228b88d8d39e27fa3bddca63f14715a5dec3e5c3de7b5b5a892c00385ea38d2b`  
		Last Modified: Tue, 21 Nov 2023 05:05:36 GMT  
		Size: 47.2 MB (47196697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df76a43e2f790a0c0d3fd4795cae7a8d79b43803710d103b38936a70bbe216`  
		Last Modified: Tue, 21 Nov 2023 06:26:42 GMT  
		Size: 25.9 MB (25892928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df8da3dad66ffd081a2a6a2a79c62c577b4c8f5b7751d2718f24e60791eae1e`  
		Last Modified: Tue, 21 Nov 2023 06:27:02 GMT  
		Size: 63.0 MB (63027803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada4fcce692f91cb6588fc68ccf3c8e63e6e26a568c586b8fd8af47793481bd9`  
		Last Modified: Tue, 21 Nov 2023 06:27:42 GMT  
		Size: 212.8 MB (212783926 bytes)  
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
$ docker pull buildpack-deps@sha256:1766ed0c020a64b0c0245a19f9ba7a951551f98147642a9acf6ede2115229dca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.4 MB (393372396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e24823afdd39ee710bbbc971c39d0aa4ff7fb43aebaf6a79c893b045539c7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:25:27 GMT
ADD file:a20f125b82438597a2805558ad08c66dbc68ff26fb4af210ce31e903d1d46127 in / 
# Tue, 21 Nov 2023 04:25:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:59:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:02:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:700801ea1c1b3b29b8d88a2f8f9405af55e151c6a84cab4b448b09ce5f2e432c`  
		Last Modified: Tue, 21 Nov 2023 04:30:48 GMT  
		Size: 53.4 MB (53423841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978542d765f76211993ce7a733e45289127bc6a8dcd47683860c44cd31e03925`  
		Last Modified: Tue, 21 Nov 2023 07:09:13 GMT  
		Size: 30.0 MB (30010990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fb001517f3aa634674774ca44ff1ee072157218fcd0522c1630479101d895`  
		Last Modified: Tue, 21 Nov 2023 07:09:33 GMT  
		Size: 70.9 MB (70920797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b31909696ac928d37c89a4769a0d196f1f4641efdd73d46c6a365e9c76eea9b`  
		Last Modified: Tue, 21 Nov 2023 07:10:21 GMT  
		Size: 239.0 MB (239016768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:cd9775eccbc9ffcd297a1818f606c97ed2ad5ca30801aac383fd3ff85ac44fab
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.6 MB (415648463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:872ff0980fc3f2e38808c31811962bbb2b3158891d22903ae44c81b2c9ab8eb4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:02 GMT
ADD file:6edb177cc4c3fc7c02043410bba7fabbbaa23493a2e0444ac13e281f6fd7d209 in / 
# Tue, 21 Nov 2023 04:09:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 04:35:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 04:42:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9197643899c29fb1e411101ee2f4e677b44704d5c2c8ce98f7567cb7f7a6cf58`  
		Last Modified: Tue, 21 Nov 2023 04:12:00 GMT  
		Size: 48.2 MB (48206696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0617cf6ad3eec888f08f7b773880b515adb1cae0586b8aa6f4b5f40076079dd`  
		Last Modified: Tue, 21 Nov 2023 04:43:06 GMT  
		Size: 26.8 MB (26784568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e112439f28d2102590bea4e42209332ea3595b8c9789016a1e8b479e123bee`  
		Last Modified: Tue, 21 Nov 2023 04:44:20 GMT  
		Size: 64.7 MB (64702623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b281221811c330e1fa4440fa0722c3b2f9601f5f9016ab7e7d8f32cdda28633`  
		Last Modified: Tue, 21 Nov 2023 04:49:49 GMT  
		Size: 276.0 MB (275954576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c93fc2e94d1d3a26456ef129ab582ef7d63a767ab8762db8940202c77f1388df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.1 MB (355072174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc793a1658b88281067a4063d6ed988d648fdb13eb5611f6e42534971d82b3da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:06:09 GMT
ADD file:38bf5e0509c54c17377ce5928ac13833ab7953cb7ff56a92265b9835fad4a7ef in / 
# Tue, 21 Nov 2023 05:06:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:10:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:12:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89d47f76a96d7ec8b86acac59109c329b28ddeee28c3c0b2ae9c6f275a50a136`  
		Last Modified: Tue, 21 Nov 2023 05:11:22 GMT  
		Size: 49.2 MB (49228111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd42e8e3bd2b6546f326a1d59a7ec0be9e7ece5e7885fd1749571be27caa1ba2`  
		Last Modified: Tue, 21 Nov 2023 06:18:03 GMT  
		Size: 28.0 MB (28032511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21db908a00e81480eebf3fad2c4e13874394ba9f9978d3ea7677d3be28b4fb`  
		Last Modified: Tue, 21 Nov 2023 06:18:18 GMT  
		Size: 66.5 MB (66490545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d423dea4ea04d9998b72e9dca146ee1f13e78ec50b02fa0de85998fc82032b`  
		Last Modified: Tue, 21 Nov 2023 06:18:48 GMT  
		Size: 211.3 MB (211321007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:8d7693e4c73bfb146460b441c69670413b9f765cd92ae0a2371828d1e0fe345f
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
$ docker pull buildpack-deps@sha256:c2083dcfe7e41b3bb14edc1e4c5d008973dd762ba4cec2830ebbddbb2f98ca9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73089625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1359faa3d45cb9604477049d17de32d2cb1490b072e28d9b1ae3ebd36b86c2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:33 GMT
ADD file:b1618939ac80f9d3256d12ed22ac3e37f61dc396e5370e7a4013561a073af181 in / 
# Tue, 21 Nov 2023 05:01:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:19:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:228b88d8d39e27fa3bddca63f14715a5dec3e5c3de7b5b5a892c00385ea38d2b`  
		Last Modified: Tue, 21 Nov 2023 05:05:36 GMT  
		Size: 47.2 MB (47196697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df76a43e2f790a0c0d3fd4795cae7a8d79b43803710d103b38936a70bbe216`  
		Last Modified: Tue, 21 Nov 2023 06:26:42 GMT  
		Size: 25.9 MB (25892928 bytes)  
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
$ docker pull buildpack-deps@sha256:bf7b2c6f20aeaa97efb86336a12338247f96a743fa032cbb6e848100e365d25e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83434831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e185b08bc814b3731dcb7aa4ef80f272175c6d3715e08afb5a280d02f76715`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:25:27 GMT
ADD file:a20f125b82438597a2805558ad08c66dbc68ff26fb4af210ce31e903d1d46127 in / 
# Tue, 21 Nov 2023 04:25:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:59:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:700801ea1c1b3b29b8d88a2f8f9405af55e151c6a84cab4b448b09ce5f2e432c`  
		Last Modified: Tue, 21 Nov 2023 04:30:48 GMT  
		Size: 53.4 MB (53423841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978542d765f76211993ce7a733e45289127bc6a8dcd47683860c44cd31e03925`  
		Last Modified: Tue, 21 Nov 2023 07:09:13 GMT  
		Size: 30.0 MB (30010990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:d47d61fd7d6f36e367a86f12fb809a0caa3ca64d6514b9d4a264184bcdc171f9
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74991264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c519b4d73993379f707098d265c9b5132d01092cdf180e2bb22b72f3163cef07`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:02 GMT
ADD file:6edb177cc4c3fc7c02043410bba7fabbbaa23493a2e0444ac13e281f6fd7d209 in / 
# Tue, 21 Nov 2023 04:09:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9197643899c29fb1e411101ee2f4e677b44704d5c2c8ce98f7567cb7f7a6cf58`  
		Last Modified: Tue, 21 Nov 2023 04:12:00 GMT  
		Size: 48.2 MB (48206696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0617cf6ad3eec888f08f7b773880b515adb1cae0586b8aa6f4b5f40076079dd`  
		Last Modified: Tue, 21 Nov 2023 04:43:06 GMT  
		Size: 26.8 MB (26784568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:132caa5f4dfbbce1e1f7a982aa07300d03415c825ae2ba80361c5c01a31e8332
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.3 MB (77260622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84e28664175d244c1cd5e4e6f02cccb38f1c27e640751ef1722a1529d588c2a9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:06:09 GMT
ADD file:38bf5e0509c54c17377ce5928ac13833ab7953cb7ff56a92265b9835fad4a7ef in / 
# Tue, 21 Nov 2023 05:06:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:10:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89d47f76a96d7ec8b86acac59109c329b28ddeee28c3c0b2ae9c6f275a50a136`  
		Last Modified: Tue, 21 Nov 2023 05:11:22 GMT  
		Size: 49.2 MB (49228111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd42e8e3bd2b6546f326a1d59a7ec0be9e7ece5e7885fd1749571be27caa1ba2`  
		Last Modified: Tue, 21 Nov 2023 06:18:03 GMT  
		Size: 28.0 MB (28032511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:dd82e7d82d39f837e964e0a02ec7acd4b7c87412144bc6b05940f154ec67d818
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
$ docker pull buildpack-deps@sha256:a14fff4df4cffc72ece82f02fb56f4d17fa776812b43c4c2cf6a19a9b4c87db3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136117428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2bafb9025c11df5f43acb3bedb814be855b4fd0db9041333997866bd26b03b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:33 GMT
ADD file:b1618939ac80f9d3256d12ed22ac3e37f61dc396e5370e7a4013561a073af181 in / 
# Tue, 21 Nov 2023 05:01:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:19:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:19:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:228b88d8d39e27fa3bddca63f14715a5dec3e5c3de7b5b5a892c00385ea38d2b`  
		Last Modified: Tue, 21 Nov 2023 05:05:36 GMT  
		Size: 47.2 MB (47196697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df76a43e2f790a0c0d3fd4795cae7a8d79b43803710d103b38936a70bbe216`  
		Last Modified: Tue, 21 Nov 2023 06:26:42 GMT  
		Size: 25.9 MB (25892928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df8da3dad66ffd081a2a6a2a79c62c577b4c8f5b7751d2718f24e60791eae1e`  
		Last Modified: Tue, 21 Nov 2023 06:27:02 GMT  
		Size: 63.0 MB (63027803 bytes)  
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
$ docker pull buildpack-deps@sha256:24a7862e93585787852dbaecc311fe50c85ca997c602ae777a5a40f37264db6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154355628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f839951b7a1ec1855581f34657a10b0e452a76662c147f9893fb5b4b1355743a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:25:27 GMT
ADD file:a20f125b82438597a2805558ad08c66dbc68ff26fb4af210ce31e903d1d46127 in / 
# Tue, 21 Nov 2023 04:25:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:59:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:700801ea1c1b3b29b8d88a2f8f9405af55e151c6a84cab4b448b09ce5f2e432c`  
		Last Modified: Tue, 21 Nov 2023 04:30:48 GMT  
		Size: 53.4 MB (53423841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978542d765f76211993ce7a733e45289127bc6a8dcd47683860c44cd31e03925`  
		Last Modified: Tue, 21 Nov 2023 07:09:13 GMT  
		Size: 30.0 MB (30010990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fb001517f3aa634674774ca44ff1ee072157218fcd0522c1630479101d895`  
		Last Modified: Tue, 21 Nov 2023 07:09:33 GMT  
		Size: 70.9 MB (70920797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:33c5e15d08ce712b59fb3c301d86849d093fabbed9d042e2dfd606d54cb3405a
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139693887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77b886411896315e38d59726c286243652452815642a349f1633769e908c0c92`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:02 GMT
ADD file:6edb177cc4c3fc7c02043410bba7fabbbaa23493a2e0444ac13e281f6fd7d209 in / 
# Tue, 21 Nov 2023 04:09:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 04:35:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9197643899c29fb1e411101ee2f4e677b44704d5c2c8ce98f7567cb7f7a6cf58`  
		Last Modified: Tue, 21 Nov 2023 04:12:00 GMT  
		Size: 48.2 MB (48206696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0617cf6ad3eec888f08f7b773880b515adb1cae0586b8aa6f4b5f40076079dd`  
		Last Modified: Tue, 21 Nov 2023 04:43:06 GMT  
		Size: 26.8 MB (26784568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e112439f28d2102590bea4e42209332ea3595b8c9789016a1e8b479e123bee`  
		Last Modified: Tue, 21 Nov 2023 04:44:20 GMT  
		Size: 64.7 MB (64702623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1769e0bcb2fe395e6ae63c7c91bdeee37003e88269a8db80d927a4fc64840f8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.8 MB (143751167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47000f61dc60af3bdb834e3d3470c752ac2e6269191cb531d5f7264a413791e8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:06:09 GMT
ADD file:38bf5e0509c54c17377ce5928ac13833ab7953cb7ff56a92265b9835fad4a7ef in / 
# Tue, 21 Nov 2023 05:06:14 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:10:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:89d47f76a96d7ec8b86acac59109c329b28ddeee28c3c0b2ae9c6f275a50a136`  
		Last Modified: Tue, 21 Nov 2023 05:11:22 GMT  
		Size: 49.2 MB (49228111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd42e8e3bd2b6546f326a1d59a7ec0be9e7ece5e7885fd1749571be27caa1ba2`  
		Last Modified: Tue, 21 Nov 2023 06:18:03 GMT  
		Size: 28.0 MB (28032511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21db908a00e81480eebf3fad2c4e13874394ba9f9978d3ea7677d3be28b4fb`  
		Last Modified: Tue, 21 Nov 2023 06:18:18 GMT  
		Size: 66.5 MB (66490545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
