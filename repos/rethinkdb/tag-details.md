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
$ docker pull rethinkdb@sha256:17401c1edbafb8cc807fdc44016e556de7b686c35d86045fa1a4234b5857281d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a5b1c585ce5a5c45ae362bb92f1eea1a653f4326acfce1f76f26231a26722d25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51768068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5dd5b23cd2539cb34f37912ecc325d0cf53b2a905def5ac15dcb9a4ace4144f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:22:30 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:34 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 18 Nov 2020 12:22:34 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 18 Nov 2020 12:22:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:47 GMT
VOLUME [/data]
# Wed, 18 Nov 2020 12:22:47 GMT
WORKDIR /data
# Wed, 18 Nov 2020 12:22:47 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 18 Nov 2020 12:22:48 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447f5e1357f860f3451dcd3ab5cfe3c128cd2fece1ee9a36d64ad1609b4b5c3`  
		Last Modified: Wed, 18 Nov 2020 12:23:49 GMT  
		Size: 6.7 MB (6669182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e01b054557acaca0b77b081da248dd2c131f0976518577554f266a5cdf3cc3`  
		Last Modified: Wed, 18 Nov 2020 12:23:47 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e161d64e52b40a0973d2b765dd9d1fe8e69f825cccbc28eb1b76aed57c764d98`  
		Last Modified: Wed, 18 Nov 2020 12:23:51 GMT  
		Size: 18.0 MB (17990696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a53590d415b928b049c7903ed1b598541c171689418d6b6b775e94c49548d`  
		Last Modified: Wed, 18 Nov 2020 12:23:48 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4`

```console
$ docker pull rethinkdb@sha256:17401c1edbafb8cc807fdc44016e556de7b686c35d86045fa1a4234b5857281d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a5b1c585ce5a5c45ae362bb92f1eea1a653f4326acfce1f76f26231a26722d25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51768068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5dd5b23cd2539cb34f37912ecc325d0cf53b2a905def5ac15dcb9a4ace4144f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:22:30 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:34 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 18 Nov 2020 12:22:34 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 18 Nov 2020 12:22:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:47 GMT
VOLUME [/data]
# Wed, 18 Nov 2020 12:22:47 GMT
WORKDIR /data
# Wed, 18 Nov 2020 12:22:47 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 18 Nov 2020 12:22:48 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447f5e1357f860f3451dcd3ab5cfe3c128cd2fece1ee9a36d64ad1609b4b5c3`  
		Last Modified: Wed, 18 Nov 2020 12:23:49 GMT  
		Size: 6.7 MB (6669182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e01b054557acaca0b77b081da248dd2c131f0976518577554f266a5cdf3cc3`  
		Last Modified: Wed, 18 Nov 2020 12:23:47 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e161d64e52b40a0973d2b765dd9d1fe8e69f825cccbc28eb1b76aed57c764d98`  
		Last Modified: Wed, 18 Nov 2020 12:23:51 GMT  
		Size: 18.0 MB (17990696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a53590d415b928b049c7903ed1b598541c171689418d6b6b775e94c49548d`  
		Last Modified: Wed, 18 Nov 2020 12:23:48 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0`

```console
$ docker pull rethinkdb@sha256:050f2b26eb24fbf7ffedb03729f129bb69017d5914225234b1aad92794fc4b5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0` - linux; amd64

```console
$ docker pull rethinkdb@sha256:116efebe920037a490e59edad8f0c0a9631449905587ed6c527a201875993dea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51769486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b34aba053e7c6bb15302f412b9775fd1427f3783a372f6624bfc7254acf2f437`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:22:30 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:23:05 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 18 Nov 2020 12:23:05 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Wed, 18 Nov 2020 12:23:18 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:23:18 GMT
VOLUME [/data]
# Wed, 18 Nov 2020 12:23:19 GMT
WORKDIR /data
# Wed, 18 Nov 2020 12:23:19 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 18 Nov 2020 12:23:19 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447f5e1357f860f3451dcd3ab5cfe3c128cd2fece1ee9a36d64ad1609b4b5c3`  
		Last Modified: Wed, 18 Nov 2020 12:23:49 GMT  
		Size: 6.7 MB (6669182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09288e1a9e2d051d96ce5861c59a8c00e5627e1f8db8d62752cf5788600af284`  
		Last Modified: Wed, 18 Nov 2020 12:24:03 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79682743e7e2ce6c87a2198b22608f58c7cd1e194e8c77599dbfabcc69b387ab`  
		Last Modified: Wed, 18 Nov 2020 12:24:06 GMT  
		Size: 18.0 MB (17992108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7fcee731c9ac6895659e6e080dfe464a8c6eda260c76bb5cc39e7d519e4231`  
		Last Modified: Wed, 18 Nov 2020 12:24:02 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-buster-slim`

```console
$ docker pull rethinkdb@sha256:050f2b26eb24fbf7ffedb03729f129bb69017d5914225234b1aad92794fc4b5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:116efebe920037a490e59edad8f0c0a9631449905587ed6c527a201875993dea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51769486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b34aba053e7c6bb15302f412b9775fd1427f3783a372f6624bfc7254acf2f437`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:22:30 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:23:05 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 18 Nov 2020 12:23:05 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Wed, 18 Nov 2020 12:23:18 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:23:18 GMT
VOLUME [/data]
# Wed, 18 Nov 2020 12:23:19 GMT
WORKDIR /data
# Wed, 18 Nov 2020 12:23:19 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 18 Nov 2020 12:23:19 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447f5e1357f860f3451dcd3ab5cfe3c128cd2fece1ee9a36d64ad1609b4b5c3`  
		Last Modified: Wed, 18 Nov 2020 12:23:49 GMT  
		Size: 6.7 MB (6669182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09288e1a9e2d051d96ce5861c59a8c00e5627e1f8db8d62752cf5788600af284`  
		Last Modified: Wed, 18 Nov 2020 12:24:03 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79682743e7e2ce6c87a2198b22608f58c7cd1e194e8c77599dbfabcc69b387ab`  
		Last Modified: Wed, 18 Nov 2020 12:24:06 GMT  
		Size: 18.0 MB (17992108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7fcee731c9ac6895659e6e080dfe464a8c6eda260c76bb5cc39e7d519e4231`  
		Last Modified: Wed, 18 Nov 2020 12:24:02 GMT  
		Size: 93.0 B  
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
$ docker pull rethinkdb@sha256:17401c1edbafb8cc807fdc44016e556de7b686c35d86045fa1a4234b5857281d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a5b1c585ce5a5c45ae362bb92f1eea1a653f4326acfce1f76f26231a26722d25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51768068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5dd5b23cd2539cb34f37912ecc325d0cf53b2a905def5ac15dcb9a4ace4144f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:22:30 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:34 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 18 Nov 2020 12:22:34 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 18 Nov 2020 12:22:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:47 GMT
VOLUME [/data]
# Wed, 18 Nov 2020 12:22:47 GMT
WORKDIR /data
# Wed, 18 Nov 2020 12:22:47 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 18 Nov 2020 12:22:48 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447f5e1357f860f3451dcd3ab5cfe3c128cd2fece1ee9a36d64ad1609b4b5c3`  
		Last Modified: Wed, 18 Nov 2020 12:23:49 GMT  
		Size: 6.7 MB (6669182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e01b054557acaca0b77b081da248dd2c131f0976518577554f266a5cdf3cc3`  
		Last Modified: Wed, 18 Nov 2020 12:23:47 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e161d64e52b40a0973d2b765dd9d1fe8e69f825cccbc28eb1b76aed57c764d98`  
		Last Modified: Wed, 18 Nov 2020 12:23:51 GMT  
		Size: 18.0 MB (17990696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a53590d415b928b049c7903ed1b598541c171689418d6b6b775e94c49548d`  
		Last Modified: Wed, 18 Nov 2020 12:23:48 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1-buster-slim`

```console
$ docker pull rethinkdb@sha256:17401c1edbafb8cc807fdc44016e556de7b686c35d86045fa1a4234b5857281d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a5b1c585ce5a5c45ae362bb92f1eea1a653f4326acfce1f76f26231a26722d25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51768068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5dd5b23cd2539cb34f37912ecc325d0cf53b2a905def5ac15dcb9a4ace4144f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:22:30 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:34 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 18 Nov 2020 12:22:34 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 18 Nov 2020 12:22:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:47 GMT
VOLUME [/data]
# Wed, 18 Nov 2020 12:22:47 GMT
WORKDIR /data
# Wed, 18 Nov 2020 12:22:47 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 18 Nov 2020 12:22:48 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447f5e1357f860f3451dcd3ab5cfe3c128cd2fece1ee9a36d64ad1609b4b5c3`  
		Last Modified: Wed, 18 Nov 2020 12:23:49 GMT  
		Size: 6.7 MB (6669182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e01b054557acaca0b77b081da248dd2c131f0976518577554f266a5cdf3cc3`  
		Last Modified: Wed, 18 Nov 2020 12:23:47 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e161d64e52b40a0973d2b765dd9d1fe8e69f825cccbc28eb1b76aed57c764d98`  
		Last Modified: Wed, 18 Nov 2020 12:23:51 GMT  
		Size: 18.0 MB (17990696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a53590d415b928b049c7903ed1b598541c171689418d6b6b775e94c49548d`  
		Last Modified: Wed, 18 Nov 2020 12:23:48 GMT  
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
$ docker pull rethinkdb@sha256:17401c1edbafb8cc807fdc44016e556de7b686c35d86045fa1a4234b5857281d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a5b1c585ce5a5c45ae362bb92f1eea1a653f4326acfce1f76f26231a26722d25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51768068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5dd5b23cd2539cb34f37912ecc325d0cf53b2a905def5ac15dcb9a4ace4144f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:22:30 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:34 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 18 Nov 2020 12:22:34 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 18 Nov 2020 12:22:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:47 GMT
VOLUME [/data]
# Wed, 18 Nov 2020 12:22:47 GMT
WORKDIR /data
# Wed, 18 Nov 2020 12:22:47 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 18 Nov 2020 12:22:48 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447f5e1357f860f3451dcd3ab5cfe3c128cd2fece1ee9a36d64ad1609b4b5c3`  
		Last Modified: Wed, 18 Nov 2020 12:23:49 GMT  
		Size: 6.7 MB (6669182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e01b054557acaca0b77b081da248dd2c131f0976518577554f266a5cdf3cc3`  
		Last Modified: Wed, 18 Nov 2020 12:23:47 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e161d64e52b40a0973d2b765dd9d1fe8e69f825cccbc28eb1b76aed57c764d98`  
		Last Modified: Wed, 18 Nov 2020 12:23:51 GMT  
		Size: 18.0 MB (17990696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a53590d415b928b049c7903ed1b598541c171689418d6b6b775e94c49548d`  
		Last Modified: Wed, 18 Nov 2020 12:23:48 GMT  
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
$ docker pull rethinkdb@sha256:17401c1edbafb8cc807fdc44016e556de7b686c35d86045fa1a4234b5857281d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a5b1c585ce5a5c45ae362bb92f1eea1a653f4326acfce1f76f26231a26722d25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51768068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5dd5b23cd2539cb34f37912ecc325d0cf53b2a905def5ac15dcb9a4ace4144f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:22:30 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:34 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 18 Nov 2020 12:22:34 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 18 Nov 2020 12:22:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:47 GMT
VOLUME [/data]
# Wed, 18 Nov 2020 12:22:47 GMT
WORKDIR /data
# Wed, 18 Nov 2020 12:22:47 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 18 Nov 2020 12:22:48 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447f5e1357f860f3451dcd3ab5cfe3c128cd2fece1ee9a36d64ad1609b4b5c3`  
		Last Modified: Wed, 18 Nov 2020 12:23:49 GMT  
		Size: 6.7 MB (6669182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e01b054557acaca0b77b081da248dd2c131f0976518577554f266a5cdf3cc3`  
		Last Modified: Wed, 18 Nov 2020 12:23:47 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e161d64e52b40a0973d2b765dd9d1fe8e69f825cccbc28eb1b76aed57c764d98`  
		Last Modified: Wed, 18 Nov 2020 12:23:51 GMT  
		Size: 18.0 MB (17990696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a53590d415b928b049c7903ed1b598541c171689418d6b6b775e94c49548d`  
		Last Modified: Wed, 18 Nov 2020 12:23:48 GMT  
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
$ docker pull rethinkdb@sha256:17401c1edbafb8cc807fdc44016e556de7b686c35d86045fa1a4234b5857281d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a5b1c585ce5a5c45ae362bb92f1eea1a653f4326acfce1f76f26231a26722d25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51768068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5dd5b23cd2539cb34f37912ecc325d0cf53b2a905def5ac15dcb9a4ace4144f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:22:30 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:34 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 18 Nov 2020 12:22:34 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 18 Nov 2020 12:22:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:47 GMT
VOLUME [/data]
# Wed, 18 Nov 2020 12:22:47 GMT
WORKDIR /data
# Wed, 18 Nov 2020 12:22:47 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 18 Nov 2020 12:22:48 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447f5e1357f860f3451dcd3ab5cfe3c128cd2fece1ee9a36d64ad1609b4b5c3`  
		Last Modified: Wed, 18 Nov 2020 12:23:49 GMT  
		Size: 6.7 MB (6669182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e01b054557acaca0b77b081da248dd2c131f0976518577554f266a5cdf3cc3`  
		Last Modified: Wed, 18 Nov 2020 12:23:47 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e161d64e52b40a0973d2b765dd9d1fe8e69f825cccbc28eb1b76aed57c764d98`  
		Last Modified: Wed, 18 Nov 2020 12:23:51 GMT  
		Size: 18.0 MB (17990696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a53590d415b928b049c7903ed1b598541c171689418d6b6b775e94c49548d`  
		Last Modified: Wed, 18 Nov 2020 12:23:48 GMT  
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
$ docker pull rethinkdb@sha256:17401c1edbafb8cc807fdc44016e556de7b686c35d86045fa1a4234b5857281d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:latest` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a5b1c585ce5a5c45ae362bb92f1eea1a653f4326acfce1f76f26231a26722d25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51768068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5dd5b23cd2539cb34f37912ecc325d0cf53b2a905def5ac15dcb9a4ace4144f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:22:30 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:34 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 18 Nov 2020 12:22:34 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 18 Nov 2020 12:22:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:22:47 GMT
VOLUME [/data]
# Wed, 18 Nov 2020 12:22:47 GMT
WORKDIR /data
# Wed, 18 Nov 2020 12:22:47 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 18 Nov 2020 12:22:48 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447f5e1357f860f3451dcd3ab5cfe3c128cd2fece1ee9a36d64ad1609b4b5c3`  
		Last Modified: Wed, 18 Nov 2020 12:23:49 GMT  
		Size: 6.7 MB (6669182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e01b054557acaca0b77b081da248dd2c131f0976518577554f266a5cdf3cc3`  
		Last Modified: Wed, 18 Nov 2020 12:23:47 GMT  
		Size: 2.6 KB (2613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e161d64e52b40a0973d2b765dd9d1fe8e69f825cccbc28eb1b76aed57c764d98`  
		Last Modified: Wed, 18 Nov 2020 12:23:51 GMT  
		Size: 18.0 MB (17990696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a53590d415b928b049c7903ed1b598541c171689418d6b6b775e94c49548d`  
		Last Modified: Wed, 18 Nov 2020 12:23:48 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
