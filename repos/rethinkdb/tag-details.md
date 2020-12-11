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
$ docker pull rethinkdb@sha256:cbbf15433fcb52100a23f4bb7be59a831a73cd0ca0ee321d6ffda36e959ddc85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2` - linux; amd64

```console
$ docker pull rethinkdb@sha256:e82e2a47850cb2fdaa67e62cd0b9805866dea32f42c2a6f6c40af22b486a9da6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51762155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47f7a611e908cbbaea401dd1423f89fd680405fe2de65529d34a05fbb903b6f8`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:30:12 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:30 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 11 Dec 2020 21:30:31 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Fri, 11 Dec 2020 21:30:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:42 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 21:30:43 GMT
WORKDIR /data
# Fri, 11 Dec 2020 21:30:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 11 Dec 2020 21:30:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2d9849117186723077e69c1d532fbe0d0dbf06bc77065e1d34bd912f884f4`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 6.7 MB (6669373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8e70d4772bbd48835bc5a140ebc5dc90235f3b4448ab04531119b5df9bd6e8`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85305ef524422b25dfbeae6ff5c198a9357be5eb61deec68d082163c56c1b63c`  
		Last Modified: Fri, 11 Dec 2020 21:31:40 GMT  
		Size: 18.0 MB (17990776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b866d19c595dd1c274ae2513eb6029b36a45b7fa1177a9660e92ca91c7cc3a86`  
		Last Modified: Fri, 11 Dec 2020 21:31:37 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4`

```console
$ docker pull rethinkdb@sha256:cbbf15433fcb52100a23f4bb7be59a831a73cd0ca0ee321d6ffda36e959ddc85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4` - linux; amd64

```console
$ docker pull rethinkdb@sha256:e82e2a47850cb2fdaa67e62cd0b9805866dea32f42c2a6f6c40af22b486a9da6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51762155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47f7a611e908cbbaea401dd1423f89fd680405fe2de65529d34a05fbb903b6f8`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:30:12 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:30 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 11 Dec 2020 21:30:31 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Fri, 11 Dec 2020 21:30:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:42 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 21:30:43 GMT
WORKDIR /data
# Fri, 11 Dec 2020 21:30:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 11 Dec 2020 21:30:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2d9849117186723077e69c1d532fbe0d0dbf06bc77065e1d34bd912f884f4`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 6.7 MB (6669373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8e70d4772bbd48835bc5a140ebc5dc90235f3b4448ab04531119b5df9bd6e8`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85305ef524422b25dfbeae6ff5c198a9357be5eb61deec68d082163c56c1b63c`  
		Last Modified: Fri, 11 Dec 2020 21:31:40 GMT  
		Size: 18.0 MB (17990776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b866d19c595dd1c274ae2513eb6029b36a45b7fa1177a9660e92ca91c7cc3a86`  
		Last Modified: Fri, 11 Dec 2020 21:31:37 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0`

```console
$ docker pull rethinkdb@sha256:fcbe81179f3aa6ca69b817447789a7430fa894176bf1ee6620ef205bfdb45537
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9bbd4175beb8d8b20dfe523ef1644e49b4bf8f9011b35fffd03c9b07ff1cf752
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51763549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e60129f21041396713ad3574cc7162da1d7cb2cafbe80bc31f9a16707470f5a`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:30:12 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:57 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 11 Dec 2020 21:30:58 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Fri, 11 Dec 2020 21:31:06 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:31:06 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 21:31:07 GMT
WORKDIR /data
# Fri, 11 Dec 2020 21:31:07 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 11 Dec 2020 21:31:07 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2d9849117186723077e69c1d532fbe0d0dbf06bc77065e1d34bd912f884f4`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 6.7 MB (6669373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d8ca6d40198376bdc1e0cbf6b35ef64c9475d4f910babad9dac5d3564497bd`  
		Last Modified: Fri, 11 Dec 2020 21:31:54 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4a876b18f25d912625b82f840afaf1a3ae884a36a97d92fbf5c8ad1af67314`  
		Last Modified: Fri, 11 Dec 2020 21:31:59 GMT  
		Size: 18.0 MB (17992177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574ec29edb9386e0174bab7bbfd4bf3cb70ef588edcb0a85d90ea8ba5d73da48`  
		Last Modified: Fri, 11 Dec 2020 21:31:53 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-buster-slim`

```console
$ docker pull rethinkdb@sha256:fcbe81179f3aa6ca69b817447789a7430fa894176bf1ee6620ef205bfdb45537
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9bbd4175beb8d8b20dfe523ef1644e49b4bf8f9011b35fffd03c9b07ff1cf752
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51763549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e60129f21041396713ad3574cc7162da1d7cb2cafbe80bc31f9a16707470f5a`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:30:12 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:57 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 11 Dec 2020 21:30:58 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Fri, 11 Dec 2020 21:31:06 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:31:06 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 21:31:07 GMT
WORKDIR /data
# Fri, 11 Dec 2020 21:31:07 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 11 Dec 2020 21:31:07 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2d9849117186723077e69c1d532fbe0d0dbf06bc77065e1d34bd912f884f4`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 6.7 MB (6669373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d8ca6d40198376bdc1e0cbf6b35ef64c9475d4f910babad9dac5d3564497bd`  
		Last Modified: Fri, 11 Dec 2020 21:31:54 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4a876b18f25d912625b82f840afaf1a3ae884a36a97d92fbf5c8ad1af67314`  
		Last Modified: Fri, 11 Dec 2020 21:31:59 GMT  
		Size: 18.0 MB (17992177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574ec29edb9386e0174bab7bbfd4bf3cb70ef588edcb0a85d90ea8ba5d73da48`  
		Last Modified: Fri, 11 Dec 2020 21:31:53 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-centos`

```console
$ docker pull rethinkdb@sha256:7c38966f6109abc28bf7d6a760f61738b3700ff909ae29f3fcdcdb9ebd901bf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:ce5736a722cb1b0fd0d6b79921cbc40e4a5cb81d12c3f1b3b95e067abfae50c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97512373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67bb51549074acf5d2f9fea2523c6679c9e3b0c0338a5daa404b9d3f65d588b8`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:56:12 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0
# Tue, 08 Dec 2020 00:56:13 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Tue, 08 Dec 2020 00:56:22 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Tue, 08 Dec 2020 00:56:22 GMT
VOLUME [/data]
# Tue, 08 Dec 2020 00:56:23 GMT
WORKDIR /data
# Tue, 08 Dec 2020 00:56:23 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 08 Dec 2020 00:56:23 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f040b4714648b6f92a7ee925071efaef18aba5be86b9caed7d53946866eb9598`  
		Last Modified: Tue, 08 Dec 2020 00:56:50 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4455d10560e81b3e86bef5719a82016dea5f5188d72b93dd3ddeb68aa93412fe`  
		Last Modified: Tue, 08 Dec 2020 00:56:54 GMT  
		Size: 22.3 MB (22330013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fe62d29608f5241c3782f3eda19fbdbf98d2e3da5d762b11155384799d1e38`  
		Last Modified: Tue, 08 Dec 2020 00:56:50 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1`

```console
$ docker pull rethinkdb@sha256:cbbf15433fcb52100a23f4bb7be59a831a73cd0ca0ee321d6ffda36e959ddc85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1` - linux; amd64

```console
$ docker pull rethinkdb@sha256:e82e2a47850cb2fdaa67e62cd0b9805866dea32f42c2a6f6c40af22b486a9da6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51762155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47f7a611e908cbbaea401dd1423f89fd680405fe2de65529d34a05fbb903b6f8`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:30:12 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:30 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 11 Dec 2020 21:30:31 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Fri, 11 Dec 2020 21:30:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:42 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 21:30:43 GMT
WORKDIR /data
# Fri, 11 Dec 2020 21:30:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 11 Dec 2020 21:30:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2d9849117186723077e69c1d532fbe0d0dbf06bc77065e1d34bd912f884f4`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 6.7 MB (6669373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8e70d4772bbd48835bc5a140ebc5dc90235f3b4448ab04531119b5df9bd6e8`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85305ef524422b25dfbeae6ff5c198a9357be5eb61deec68d082163c56c1b63c`  
		Last Modified: Fri, 11 Dec 2020 21:31:40 GMT  
		Size: 18.0 MB (17990776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b866d19c595dd1c274ae2513eb6029b36a45b7fa1177a9660e92ca91c7cc3a86`  
		Last Modified: Fri, 11 Dec 2020 21:31:37 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1-buster-slim`

```console
$ docker pull rethinkdb@sha256:cbbf15433fcb52100a23f4bb7be59a831a73cd0ca0ee321d6ffda36e959ddc85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:e82e2a47850cb2fdaa67e62cd0b9805866dea32f42c2a6f6c40af22b486a9da6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51762155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47f7a611e908cbbaea401dd1423f89fd680405fe2de65529d34a05fbb903b6f8`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:30:12 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:30 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 11 Dec 2020 21:30:31 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Fri, 11 Dec 2020 21:30:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:42 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 21:30:43 GMT
WORKDIR /data
# Fri, 11 Dec 2020 21:30:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 11 Dec 2020 21:30:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2d9849117186723077e69c1d532fbe0d0dbf06bc77065e1d34bd912f884f4`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 6.7 MB (6669373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8e70d4772bbd48835bc5a140ebc5dc90235f3b4448ab04531119b5df9bd6e8`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85305ef524422b25dfbeae6ff5c198a9357be5eb61deec68d082163c56c1b63c`  
		Last Modified: Fri, 11 Dec 2020 21:31:40 GMT  
		Size: 18.0 MB (17990776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b866d19c595dd1c274ae2513eb6029b36a45b7fa1177a9660e92ca91c7cc3a86`  
		Last Modified: Fri, 11 Dec 2020 21:31:37 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1-centos`

```console
$ docker pull rethinkdb@sha256:675a7224e465eccf67748eb9747bf0a44c00e53ab1a9764cd57d1d650c6b7209
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a9ab5edeaa46c3b0cf02bdf15f5d9503c510bad64ade43b9487911612086c635
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97511761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cb58d00fcf7cc3361f0035e54d47062c0ce389f12ad5e44b81134e9152e0aab`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:55:52 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Tue, 08 Dec 2020 00:55:53 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Tue, 08 Dec 2020 00:56:03 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Tue, 08 Dec 2020 00:56:03 GMT
VOLUME [/data]
# Tue, 08 Dec 2020 00:56:03 GMT
WORKDIR /data
# Tue, 08 Dec 2020 00:56:03 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 08 Dec 2020 00:56:04 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec050a263eb1b536df655a3f4d2382bd757fe1c35f03b832d7d0ba2e7dfa7cfa`  
		Last Modified: Tue, 08 Dec 2020 00:56:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79bd86fa34f79229b182548217853bb74036f4923de9f2d0aa40c56f3978542`  
		Last Modified: Tue, 08 Dec 2020 00:56:43 GMT  
		Size: 22.3 MB (22329404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37c9f29738a7bfc5fe4dcd5cdb902c80495514ea9e8f43c8cf1b264315b090f`  
		Last Modified: Tue, 08 Dec 2020 00:56:38 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-buster-slim`

```console
$ docker pull rethinkdb@sha256:cbbf15433fcb52100a23f4bb7be59a831a73cd0ca0ee321d6ffda36e959ddc85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:e82e2a47850cb2fdaa67e62cd0b9805866dea32f42c2a6f6c40af22b486a9da6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51762155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47f7a611e908cbbaea401dd1423f89fd680405fe2de65529d34a05fbb903b6f8`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:30:12 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:30 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 11 Dec 2020 21:30:31 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Fri, 11 Dec 2020 21:30:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:42 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 21:30:43 GMT
WORKDIR /data
# Fri, 11 Dec 2020 21:30:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 11 Dec 2020 21:30:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2d9849117186723077e69c1d532fbe0d0dbf06bc77065e1d34bd912f884f4`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 6.7 MB (6669373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8e70d4772bbd48835bc5a140ebc5dc90235f3b4448ab04531119b5df9bd6e8`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85305ef524422b25dfbeae6ff5c198a9357be5eb61deec68d082163c56c1b63c`  
		Last Modified: Fri, 11 Dec 2020 21:31:40 GMT  
		Size: 18.0 MB (17990776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b866d19c595dd1c274ae2513eb6029b36a45b7fa1177a9660e92ca91c7cc3a86`  
		Last Modified: Fri, 11 Dec 2020 21:31:37 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-centos`

```console
$ docker pull rethinkdb@sha256:675a7224e465eccf67748eb9747bf0a44c00e53ab1a9764cd57d1d650c6b7209
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a9ab5edeaa46c3b0cf02bdf15f5d9503c510bad64ade43b9487911612086c635
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97511761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cb58d00fcf7cc3361f0035e54d47062c0ce389f12ad5e44b81134e9152e0aab`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:55:52 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Tue, 08 Dec 2020 00:55:53 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Tue, 08 Dec 2020 00:56:03 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Tue, 08 Dec 2020 00:56:03 GMT
VOLUME [/data]
# Tue, 08 Dec 2020 00:56:03 GMT
WORKDIR /data
# Tue, 08 Dec 2020 00:56:03 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 08 Dec 2020 00:56:04 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec050a263eb1b536df655a3f4d2382bd757fe1c35f03b832d7d0ba2e7dfa7cfa`  
		Last Modified: Tue, 08 Dec 2020 00:56:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79bd86fa34f79229b182548217853bb74036f4923de9f2d0aa40c56f3978542`  
		Last Modified: Tue, 08 Dec 2020 00:56:43 GMT  
		Size: 22.3 MB (22329404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37c9f29738a7bfc5fe4dcd5cdb902c80495514ea9e8f43c8cf1b264315b090f`  
		Last Modified: Tue, 08 Dec 2020 00:56:38 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-buster-slim`

```console
$ docker pull rethinkdb@sha256:cbbf15433fcb52100a23f4bb7be59a831a73cd0ca0ee321d6ffda36e959ddc85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:e82e2a47850cb2fdaa67e62cd0b9805866dea32f42c2a6f6c40af22b486a9da6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51762155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47f7a611e908cbbaea401dd1423f89fd680405fe2de65529d34a05fbb903b6f8`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:30:12 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:30 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 11 Dec 2020 21:30:31 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Fri, 11 Dec 2020 21:30:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:42 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 21:30:43 GMT
WORKDIR /data
# Fri, 11 Dec 2020 21:30:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 11 Dec 2020 21:30:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2d9849117186723077e69c1d532fbe0d0dbf06bc77065e1d34bd912f884f4`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 6.7 MB (6669373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8e70d4772bbd48835bc5a140ebc5dc90235f3b4448ab04531119b5df9bd6e8`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85305ef524422b25dfbeae6ff5c198a9357be5eb61deec68d082163c56c1b63c`  
		Last Modified: Fri, 11 Dec 2020 21:31:40 GMT  
		Size: 18.0 MB (17990776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b866d19c595dd1c274ae2513eb6029b36a45b7fa1177a9660e92ca91c7cc3a86`  
		Last Modified: Fri, 11 Dec 2020 21:31:37 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-centos`

```console
$ docker pull rethinkdb@sha256:675a7224e465eccf67748eb9747bf0a44c00e53ab1a9764cd57d1d650c6b7209
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a9ab5edeaa46c3b0cf02bdf15f5d9503c510bad64ade43b9487911612086c635
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97511761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cb58d00fcf7cc3361f0035e54d47062c0ce389f12ad5e44b81134e9152e0aab`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:55:52 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Tue, 08 Dec 2020 00:55:53 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Tue, 08 Dec 2020 00:56:03 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Tue, 08 Dec 2020 00:56:03 GMT
VOLUME [/data]
# Tue, 08 Dec 2020 00:56:03 GMT
WORKDIR /data
# Tue, 08 Dec 2020 00:56:03 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 08 Dec 2020 00:56:04 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec050a263eb1b536df655a3f4d2382bd757fe1c35f03b832d7d0ba2e7dfa7cfa`  
		Last Modified: Tue, 08 Dec 2020 00:56:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79bd86fa34f79229b182548217853bb74036f4923de9f2d0aa40c56f3978542`  
		Last Modified: Tue, 08 Dec 2020 00:56:43 GMT  
		Size: 22.3 MB (22329404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37c9f29738a7bfc5fe4dcd5cdb902c80495514ea9e8f43c8cf1b264315b090f`  
		Last Modified: Tue, 08 Dec 2020 00:56:38 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:buster-slim`

```console
$ docker pull rethinkdb@sha256:cbbf15433fcb52100a23f4bb7be59a831a73cd0ca0ee321d6ffda36e959ddc85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:e82e2a47850cb2fdaa67e62cd0b9805866dea32f42c2a6f6c40af22b486a9da6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51762155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47f7a611e908cbbaea401dd1423f89fd680405fe2de65529d34a05fbb903b6f8`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:30:12 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:30 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 11 Dec 2020 21:30:31 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Fri, 11 Dec 2020 21:30:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:42 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 21:30:43 GMT
WORKDIR /data
# Fri, 11 Dec 2020 21:30:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 11 Dec 2020 21:30:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2d9849117186723077e69c1d532fbe0d0dbf06bc77065e1d34bd912f884f4`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 6.7 MB (6669373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8e70d4772bbd48835bc5a140ebc5dc90235f3b4448ab04531119b5df9bd6e8`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85305ef524422b25dfbeae6ff5c198a9357be5eb61deec68d082163c56c1b63c`  
		Last Modified: Fri, 11 Dec 2020 21:31:40 GMT  
		Size: 18.0 MB (17990776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b866d19c595dd1c274ae2513eb6029b36a45b7fa1177a9660e92ca91c7cc3a86`  
		Last Modified: Fri, 11 Dec 2020 21:31:37 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:centos`

```console
$ docker pull rethinkdb@sha256:675a7224e465eccf67748eb9747bf0a44c00e53ab1a9764cd57d1d650c6b7209
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:a9ab5edeaa46c3b0cf02bdf15f5d9503c510bad64ade43b9487911612086c635
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97511761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cb58d00fcf7cc3361f0035e54d47062c0ce389f12ad5e44b81134e9152e0aab`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Tue, 08 Dec 2020 00:55:52 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Tue, 08 Dec 2020 00:55:53 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Tue, 08 Dec 2020 00:56:03 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Tue, 08 Dec 2020 00:56:03 GMT
VOLUME [/data]
# Tue, 08 Dec 2020 00:56:03 GMT
WORKDIR /data
# Tue, 08 Dec 2020 00:56:03 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 08 Dec 2020 00:56:04 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec050a263eb1b536df655a3f4d2382bd757fe1c35f03b832d7d0ba2e7dfa7cfa`  
		Last Modified: Tue, 08 Dec 2020 00:56:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79bd86fa34f79229b182548217853bb74036f4923de9f2d0aa40c56f3978542`  
		Last Modified: Tue, 08 Dec 2020 00:56:43 GMT  
		Size: 22.3 MB (22329404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37c9f29738a7bfc5fe4dcd5cdb902c80495514ea9e8f43c8cf1b264315b090f`  
		Last Modified: Tue, 08 Dec 2020 00:56:38 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:latest`

```console
$ docker pull rethinkdb@sha256:cbbf15433fcb52100a23f4bb7be59a831a73cd0ca0ee321d6ffda36e959ddc85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:latest` - linux; amd64

```console
$ docker pull rethinkdb@sha256:e82e2a47850cb2fdaa67e62cd0b9805866dea32f42c2a6f6c40af22b486a9da6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51762155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47f7a611e908cbbaea401dd1423f89fd680405fe2de65529d34a05fbb903b6f8`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:30:12 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:30 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 11 Dec 2020 21:30:31 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Fri, 11 Dec 2020 21:30:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:30:42 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 21:30:43 GMT
WORKDIR /data
# Fri, 11 Dec 2020 21:30:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 11 Dec 2020 21:30:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2d9849117186723077e69c1d532fbe0d0dbf06bc77065e1d34bd912f884f4`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 6.7 MB (6669373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8e70d4772bbd48835bc5a140ebc5dc90235f3b4448ab04531119b5df9bd6e8`  
		Last Modified: Fri, 11 Dec 2020 21:31:38 GMT  
		Size: 2.6 KB (2618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85305ef524422b25dfbeae6ff5c198a9357be5eb61deec68d082163c56c1b63c`  
		Last Modified: Fri, 11 Dec 2020 21:31:40 GMT  
		Size: 18.0 MB (17990776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b866d19c595dd1c274ae2513eb6029b36a45b7fa1177a9660e92ca91c7cc3a86`  
		Last Modified: Fri, 11 Dec 2020 21:31:37 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
