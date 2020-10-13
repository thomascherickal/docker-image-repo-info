<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rethinkdb`

-	[`rethinkdb:2`](#rethinkdb2)
-	[`rethinkdb:2.4`](#rethinkdb24)
-	[`rethinkdb:2.4.0`](#rethinkdb240)
-	[`rethinkdb:2.4.0-buster-slim`](#rethinkdb240-buster-slim)
-	[`rethinkdb:2.4.0-centos`](#rethinkdb240-centos)
-	[`rethinkdb:2.4.1`](#rethinkdb241)
-	[`rethinkdb:2.4.1-buster-slim`](#rethinkdb241-buster-slim)
-	[`rethinkdb:2.4.1-centos`](#rethinkdb241-centos)
-	[`rethinkdb:2.4-buster-slim`](#rethinkdb24-buster-slim)
-	[`rethinkdb:2.4-centos`](#rethinkdb24-centos)
-	[`rethinkdb:2-buster-slim`](#rethinkdb2-buster-slim)
-	[`rethinkdb:2-centos`](#rethinkdb2-centos)
-	[`rethinkdb:buster-slim`](#rethinkdbbuster-slim)
-	[`rethinkdb:centos`](#rethinkdbcentos)
-	[`rethinkdb:latest`](#rethinkdblatest)

## `rethinkdb:2`

```console
$ docker pull rethinkdb@sha256:7e85ad23b6382fbb83af993a65b37ef60a7e57a38195482ebd6c7e3634f74bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2` - linux; amd64

```console
$ docker pull rethinkdb@sha256:82ab41f04983eb23c0cbccc2d5ecfb111c31b140b65d6fade4c2dfbd10b9d027
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51754789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc02d43272252404086d84ffbb128e9f8ebcbef2bb3b685a6f5f141a7e72c764`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:04:35 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Oct 2020 22:04:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 13 Oct 2020 22:04:45 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:46 GMT
VOLUME [/data]
# Tue, 13 Oct 2020 22:04:46 GMT
WORKDIR /data
# Tue, 13 Oct 2020 22:04:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Oct 2020 22:04:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ff2d863f5cb64cbf6e74cad8f981b6b9b5a3dfd323a549059ed3fe391221`  
		Last Modified: Tue, 13 Oct 2020 22:05:23 GMT  
		Size: 6.7 MB (6669162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e76d8854d8cc50116145a95caaaedc2d267de5c7680bd1ce2e695d5180de76`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84795ccb1d288c022adb90fd10839a7de78e636e0546c739e3dad1055cee0e4f`  
		Last Modified: Tue, 13 Oct 2020 22:05:27 GMT  
		Size: 18.0 MB (17990695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71976fa1d68a93d177f7529f95d65759cf1f0b6035e836d149fcda592c9b80b`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4`

```console
$ docker pull rethinkdb@sha256:7e85ad23b6382fbb83af993a65b37ef60a7e57a38195482ebd6c7e3634f74bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4` - linux; amd64

```console
$ docker pull rethinkdb@sha256:82ab41f04983eb23c0cbccc2d5ecfb111c31b140b65d6fade4c2dfbd10b9d027
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51754789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc02d43272252404086d84ffbb128e9f8ebcbef2bb3b685a6f5f141a7e72c764`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:04:35 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Oct 2020 22:04:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 13 Oct 2020 22:04:45 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:46 GMT
VOLUME [/data]
# Tue, 13 Oct 2020 22:04:46 GMT
WORKDIR /data
# Tue, 13 Oct 2020 22:04:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Oct 2020 22:04:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ff2d863f5cb64cbf6e74cad8f981b6b9b5a3dfd323a549059ed3fe391221`  
		Last Modified: Tue, 13 Oct 2020 22:05:23 GMT  
		Size: 6.7 MB (6669162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e76d8854d8cc50116145a95caaaedc2d267de5c7680bd1ce2e695d5180de76`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84795ccb1d288c022adb90fd10839a7de78e636e0546c739e3dad1055cee0e4f`  
		Last Modified: Tue, 13 Oct 2020 22:05:27 GMT  
		Size: 18.0 MB (17990695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71976fa1d68a93d177f7529f95d65759cf1f0b6035e836d149fcda592c9b80b`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0`

```console
$ docker pull rethinkdb@sha256:fc61fc0181399d3a394b02dbba2f348dfe32011e51f07dd446c96c6ad2492934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9e297a9af0c706c7321a4b2d1c7df8df06c97f2e317a80eefa7cb8cbf6bc5fe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51756115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba6736ea0ea199b08cff1b5cd9878d0bb471ca5a4409957719bc3f0f12ac322`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:04:35 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:56 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Oct 2020 22:04:57 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Tue, 13 Oct 2020 22:05:06 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:05:06 GMT
VOLUME [/data]
# Tue, 13 Oct 2020 22:05:06 GMT
WORKDIR /data
# Tue, 13 Oct 2020 22:05:06 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Oct 2020 22:05:07 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ff2d863f5cb64cbf6e74cad8f981b6b9b5a3dfd323a549059ed3fe391221`  
		Last Modified: Tue, 13 Oct 2020 22:05:23 GMT  
		Size: 6.7 MB (6669162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e846dad4351fb8c0149ffd8d984bdbe7d498f75601c765b09f5f9673bacaa15d`  
		Last Modified: Tue, 13 Oct 2020 22:05:39 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0715a3e5cea651021435b1a0dbd006bf00c768b22d182112657f04d24b110654`  
		Last Modified: Tue, 13 Oct 2020 22:05:43 GMT  
		Size: 18.0 MB (17992022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c3d029b6e94d01d05c501c16d2053770145139185f077b23650562e50022b4`  
		Last Modified: Tue, 13 Oct 2020 22:05:39 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-buster-slim`

```console
$ docker pull rethinkdb@sha256:fc61fc0181399d3a394b02dbba2f348dfe32011e51f07dd446c96c6ad2492934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9e297a9af0c706c7321a4b2d1c7df8df06c97f2e317a80eefa7cb8cbf6bc5fe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51756115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba6736ea0ea199b08cff1b5cd9878d0bb471ca5a4409957719bc3f0f12ac322`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:04:35 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:56 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Oct 2020 22:04:57 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Tue, 13 Oct 2020 22:05:06 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:05:06 GMT
VOLUME [/data]
# Tue, 13 Oct 2020 22:05:06 GMT
WORKDIR /data
# Tue, 13 Oct 2020 22:05:06 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Oct 2020 22:05:07 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ff2d863f5cb64cbf6e74cad8f981b6b9b5a3dfd323a549059ed3fe391221`  
		Last Modified: Tue, 13 Oct 2020 22:05:23 GMT  
		Size: 6.7 MB (6669162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e846dad4351fb8c0149ffd8d984bdbe7d498f75601c765b09f5f9673bacaa15d`  
		Last Modified: Tue, 13 Oct 2020 22:05:39 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0715a3e5cea651021435b1a0dbd006bf00c768b22d182112657f04d24b110654`  
		Last Modified: Tue, 13 Oct 2020 22:05:43 GMT  
		Size: 18.0 MB (17992022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c3d029b6e94d01d05c501c16d2053770145139185f077b23650562e50022b4`  
		Last Modified: Tue, 13 Oct 2020 22:05:39 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-centos`

```console
$ docker pull rethinkdb@sha256:115347ac348bbd0c47964b9d4752eee50a939ef89800bfa8c913b57155c84bdb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:b75b236e0d67b1d8c7f7d3800179cabd1ec330719a7d51c9155fce82fd4231eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97239408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc4c32f9f785547d2206f4d058e96229d571c31d6a714d32570dbf672ce015ed`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 19:00:22 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0
# Mon, 10 Aug 2020 19:00:23 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 14 Aug 2020 21:13:36 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 14 Aug 2020 21:13:36 GMT
VOLUME [/data]
# Fri, 14 Aug 2020 21:13:37 GMT
WORKDIR /data
# Fri, 14 Aug 2020 21:13:37 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 14 Aug 2020 21:13:37 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692940a286c0d3f1beadabb7a212a6e1678d9c0e303ac94a5bf35eb3734cadb2`  
		Last Modified: Fri, 14 Aug 2020 21:14:24 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481ff4bec25e8a9c3995aa160e716057e6833426bc14c40925c0c9153efa3758`  
		Last Modified: Fri, 14 Aug 2020 21:14:29 GMT  
		Size: 22.4 MB (22370928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be9a2117906713867ccadcfe5b95b109d1b8f5788bb2fed8736ddcae099972b`  
		Last Modified: Fri, 14 Aug 2020 21:14:24 GMT  
		Size: 91.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1`

```console
$ docker pull rethinkdb@sha256:7e85ad23b6382fbb83af993a65b37ef60a7e57a38195482ebd6c7e3634f74bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1` - linux; amd64

```console
$ docker pull rethinkdb@sha256:82ab41f04983eb23c0cbccc2d5ecfb111c31b140b65d6fade4c2dfbd10b9d027
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51754789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc02d43272252404086d84ffbb128e9f8ebcbef2bb3b685a6f5f141a7e72c764`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:04:35 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Oct 2020 22:04:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 13 Oct 2020 22:04:45 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:46 GMT
VOLUME [/data]
# Tue, 13 Oct 2020 22:04:46 GMT
WORKDIR /data
# Tue, 13 Oct 2020 22:04:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Oct 2020 22:04:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ff2d863f5cb64cbf6e74cad8f981b6b9b5a3dfd323a549059ed3fe391221`  
		Last Modified: Tue, 13 Oct 2020 22:05:23 GMT  
		Size: 6.7 MB (6669162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e76d8854d8cc50116145a95caaaedc2d267de5c7680bd1ce2e695d5180de76`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84795ccb1d288c022adb90fd10839a7de78e636e0546c739e3dad1055cee0e4f`  
		Last Modified: Tue, 13 Oct 2020 22:05:27 GMT  
		Size: 18.0 MB (17990695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71976fa1d68a93d177f7529f95d65759cf1f0b6035e836d149fcda592c9b80b`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1-buster-slim`

```console
$ docker pull rethinkdb@sha256:7e85ad23b6382fbb83af993a65b37ef60a7e57a38195482ebd6c7e3634f74bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:82ab41f04983eb23c0cbccc2d5ecfb111c31b140b65d6fade4c2dfbd10b9d027
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51754789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc02d43272252404086d84ffbb128e9f8ebcbef2bb3b685a6f5f141a7e72c764`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:04:35 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Oct 2020 22:04:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 13 Oct 2020 22:04:45 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:46 GMT
VOLUME [/data]
# Tue, 13 Oct 2020 22:04:46 GMT
WORKDIR /data
# Tue, 13 Oct 2020 22:04:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Oct 2020 22:04:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ff2d863f5cb64cbf6e74cad8f981b6b9b5a3dfd323a549059ed3fe391221`  
		Last Modified: Tue, 13 Oct 2020 22:05:23 GMT  
		Size: 6.7 MB (6669162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e76d8854d8cc50116145a95caaaedc2d267de5c7680bd1ce2e695d5180de76`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84795ccb1d288c022adb90fd10839a7de78e636e0546c739e3dad1055cee0e4f`  
		Last Modified: Tue, 13 Oct 2020 22:05:27 GMT  
		Size: 18.0 MB (17990695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71976fa1d68a93d177f7529f95d65759cf1f0b6035e836d149fcda592c9b80b`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1-centos`

```console
$ docker pull rethinkdb@sha256:ff373e004421806fce99fb671c77cc5501f94033e7b71e098217b06527a6c848
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:1657b2cdf8aa6349ee420f6dd13742464a5f10f6c9afa7452f21bc77dadb6680
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97241933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc67788580c45d661eca9eee275f454bad6b9f39847268008a4d3b32f6e5c7e6`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 14 Aug 2020 21:12:58 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Fri, 14 Aug 2020 21:12:59 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 14 Aug 2020 21:13:11 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 14 Aug 2020 21:13:12 GMT
VOLUME [/data]
# Fri, 14 Aug 2020 21:13:12 GMT
WORKDIR /data
# Fri, 14 Aug 2020 21:13:12 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 14 Aug 2020 21:13:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab244016302f983bd67f48b1617ff02399bff6c698eb9fbe14e9fb697cce3d27`  
		Last Modified: Fri, 14 Aug 2020 21:14:13 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afcadaf6949665a0a4e3476e4aea8716dfe440805296483f5d251343e3b7aad`  
		Last Modified: Fri, 14 Aug 2020 21:14:18 GMT  
		Size: 22.4 MB (22373453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f5e734cc4ca195caee21f22078178255473a5f345528d5bf12d82d2fb8b1e0`  
		Last Modified: Fri, 14 Aug 2020 21:14:13 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-buster-slim`

```console
$ docker pull rethinkdb@sha256:7e85ad23b6382fbb83af993a65b37ef60a7e57a38195482ebd6c7e3634f74bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:82ab41f04983eb23c0cbccc2d5ecfb111c31b140b65d6fade4c2dfbd10b9d027
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51754789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc02d43272252404086d84ffbb128e9f8ebcbef2bb3b685a6f5f141a7e72c764`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:04:35 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Oct 2020 22:04:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 13 Oct 2020 22:04:45 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:46 GMT
VOLUME [/data]
# Tue, 13 Oct 2020 22:04:46 GMT
WORKDIR /data
# Tue, 13 Oct 2020 22:04:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Oct 2020 22:04:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ff2d863f5cb64cbf6e74cad8f981b6b9b5a3dfd323a549059ed3fe391221`  
		Last Modified: Tue, 13 Oct 2020 22:05:23 GMT  
		Size: 6.7 MB (6669162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e76d8854d8cc50116145a95caaaedc2d267de5c7680bd1ce2e695d5180de76`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84795ccb1d288c022adb90fd10839a7de78e636e0546c739e3dad1055cee0e4f`  
		Last Modified: Tue, 13 Oct 2020 22:05:27 GMT  
		Size: 18.0 MB (17990695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71976fa1d68a93d177f7529f95d65759cf1f0b6035e836d149fcda592c9b80b`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-centos`

```console
$ docker pull rethinkdb@sha256:ff373e004421806fce99fb671c77cc5501f94033e7b71e098217b06527a6c848
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:1657b2cdf8aa6349ee420f6dd13742464a5f10f6c9afa7452f21bc77dadb6680
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97241933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc67788580c45d661eca9eee275f454bad6b9f39847268008a4d3b32f6e5c7e6`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 14 Aug 2020 21:12:58 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Fri, 14 Aug 2020 21:12:59 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 14 Aug 2020 21:13:11 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 14 Aug 2020 21:13:12 GMT
VOLUME [/data]
# Fri, 14 Aug 2020 21:13:12 GMT
WORKDIR /data
# Fri, 14 Aug 2020 21:13:12 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 14 Aug 2020 21:13:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab244016302f983bd67f48b1617ff02399bff6c698eb9fbe14e9fb697cce3d27`  
		Last Modified: Fri, 14 Aug 2020 21:14:13 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afcadaf6949665a0a4e3476e4aea8716dfe440805296483f5d251343e3b7aad`  
		Last Modified: Fri, 14 Aug 2020 21:14:18 GMT  
		Size: 22.4 MB (22373453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f5e734cc4ca195caee21f22078178255473a5f345528d5bf12d82d2fb8b1e0`  
		Last Modified: Fri, 14 Aug 2020 21:14:13 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-buster-slim`

```console
$ docker pull rethinkdb@sha256:7e85ad23b6382fbb83af993a65b37ef60a7e57a38195482ebd6c7e3634f74bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:82ab41f04983eb23c0cbccc2d5ecfb111c31b140b65d6fade4c2dfbd10b9d027
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51754789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc02d43272252404086d84ffbb128e9f8ebcbef2bb3b685a6f5f141a7e72c764`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:04:35 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Oct 2020 22:04:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 13 Oct 2020 22:04:45 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:46 GMT
VOLUME [/data]
# Tue, 13 Oct 2020 22:04:46 GMT
WORKDIR /data
# Tue, 13 Oct 2020 22:04:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Oct 2020 22:04:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ff2d863f5cb64cbf6e74cad8f981b6b9b5a3dfd323a549059ed3fe391221`  
		Last Modified: Tue, 13 Oct 2020 22:05:23 GMT  
		Size: 6.7 MB (6669162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e76d8854d8cc50116145a95caaaedc2d267de5c7680bd1ce2e695d5180de76`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84795ccb1d288c022adb90fd10839a7de78e636e0546c739e3dad1055cee0e4f`  
		Last Modified: Tue, 13 Oct 2020 22:05:27 GMT  
		Size: 18.0 MB (17990695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71976fa1d68a93d177f7529f95d65759cf1f0b6035e836d149fcda592c9b80b`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-centos`

```console
$ docker pull rethinkdb@sha256:ff373e004421806fce99fb671c77cc5501f94033e7b71e098217b06527a6c848
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:1657b2cdf8aa6349ee420f6dd13742464a5f10f6c9afa7452f21bc77dadb6680
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97241933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc67788580c45d661eca9eee275f454bad6b9f39847268008a4d3b32f6e5c7e6`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 14 Aug 2020 21:12:58 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Fri, 14 Aug 2020 21:12:59 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 14 Aug 2020 21:13:11 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 14 Aug 2020 21:13:12 GMT
VOLUME [/data]
# Fri, 14 Aug 2020 21:13:12 GMT
WORKDIR /data
# Fri, 14 Aug 2020 21:13:12 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 14 Aug 2020 21:13:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab244016302f983bd67f48b1617ff02399bff6c698eb9fbe14e9fb697cce3d27`  
		Last Modified: Fri, 14 Aug 2020 21:14:13 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afcadaf6949665a0a4e3476e4aea8716dfe440805296483f5d251343e3b7aad`  
		Last Modified: Fri, 14 Aug 2020 21:14:18 GMT  
		Size: 22.4 MB (22373453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f5e734cc4ca195caee21f22078178255473a5f345528d5bf12d82d2fb8b1e0`  
		Last Modified: Fri, 14 Aug 2020 21:14:13 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:buster-slim`

```console
$ docker pull rethinkdb@sha256:7e85ad23b6382fbb83af993a65b37ef60a7e57a38195482ebd6c7e3634f74bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:82ab41f04983eb23c0cbccc2d5ecfb111c31b140b65d6fade4c2dfbd10b9d027
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51754789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc02d43272252404086d84ffbb128e9f8ebcbef2bb3b685a6f5f141a7e72c764`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:04:35 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Oct 2020 22:04:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 13 Oct 2020 22:04:45 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:46 GMT
VOLUME [/data]
# Tue, 13 Oct 2020 22:04:46 GMT
WORKDIR /data
# Tue, 13 Oct 2020 22:04:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Oct 2020 22:04:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ff2d863f5cb64cbf6e74cad8f981b6b9b5a3dfd323a549059ed3fe391221`  
		Last Modified: Tue, 13 Oct 2020 22:05:23 GMT  
		Size: 6.7 MB (6669162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e76d8854d8cc50116145a95caaaedc2d267de5c7680bd1ce2e695d5180de76`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84795ccb1d288c022adb90fd10839a7de78e636e0546c739e3dad1055cee0e4f`  
		Last Modified: Tue, 13 Oct 2020 22:05:27 GMT  
		Size: 18.0 MB (17990695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71976fa1d68a93d177f7529f95d65759cf1f0b6035e836d149fcda592c9b80b`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:centos`

```console
$ docker pull rethinkdb@sha256:ff373e004421806fce99fb671c77cc5501f94033e7b71e098217b06527a6c848
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:1657b2cdf8aa6349ee420f6dd13742464a5f10f6c9afa7452f21bc77dadb6680
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97241933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc67788580c45d661eca9eee275f454bad6b9f39847268008a4d3b32f6e5c7e6`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Mon, 10 Aug 2020 18:19:49 GMT
ADD file:538afc0c5c964ce0dde0141953a4dcf03c2d993c5989c92e7fee418e9305e2a3 in / 
# Mon, 10 Aug 2020 18:19:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809
# Mon, 10 Aug 2020 18:19:49 GMT
CMD ["/bin/bash"]
# Fri, 14 Aug 2020 21:12:58 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Fri, 14 Aug 2020 21:12:59 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 14 Aug 2020 21:13:11 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 14 Aug 2020 21:13:12 GMT
VOLUME [/data]
# Fri, 14 Aug 2020 21:13:12 GMT
WORKDIR /data
# Fri, 14 Aug 2020 21:13:12 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 14 Aug 2020 21:13:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:3c72a8ed68140139e483fe7368ae4d9651422749e91483557cbd5ecf99a96110`  
		Last Modified: Mon, 10 Aug 2020 18:21:27 GMT  
		Size: 74.9 MB (74868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab244016302f983bd67f48b1617ff02399bff6c698eb9fbe14e9fb697cce3d27`  
		Last Modified: Fri, 14 Aug 2020 21:14:13 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afcadaf6949665a0a4e3476e4aea8716dfe440805296483f5d251343e3b7aad`  
		Last Modified: Fri, 14 Aug 2020 21:14:18 GMT  
		Size: 22.4 MB (22373453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f5e734cc4ca195caee21f22078178255473a5f345528d5bf12d82d2fb8b1e0`  
		Last Modified: Fri, 14 Aug 2020 21:14:13 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:latest`

```console
$ docker pull rethinkdb@sha256:7e85ad23b6382fbb83af993a65b37ef60a7e57a38195482ebd6c7e3634f74bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:latest` - linux; amd64

```console
$ docker pull rethinkdb@sha256:82ab41f04983eb23c0cbccc2d5ecfb111c31b140b65d6fade4c2dfbd10b9d027
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51754789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc02d43272252404086d84ffbb128e9f8ebcbef2bb3b685a6f5f141a7e72c764`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:04:35 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Oct 2020 22:04:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 13 Oct 2020 22:04:45 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:04:46 GMT
VOLUME [/data]
# Tue, 13 Oct 2020 22:04:46 GMT
WORKDIR /data
# Tue, 13 Oct 2020 22:04:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Oct 2020 22:04:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8ff2d863f5cb64cbf6e74cad8f981b6b9b5a3dfd323a549059ed3fe391221`  
		Last Modified: Tue, 13 Oct 2020 22:05:23 GMT  
		Size: 6.7 MB (6669162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e76d8854d8cc50116145a95caaaedc2d267de5c7680bd1ce2e695d5180de76`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84795ccb1d288c022adb90fd10839a7de78e636e0546c739e3dad1055cee0e4f`  
		Last Modified: Tue, 13 Oct 2020 22:05:27 GMT  
		Size: 18.0 MB (17990695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71976fa1d68a93d177f7529f95d65759cf1f0b6035e836d149fcda592c9b80b`  
		Last Modified: Tue, 13 Oct 2020 22:05:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
