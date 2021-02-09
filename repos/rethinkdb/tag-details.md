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
$ docker pull rethinkdb@sha256:ff28f747a8183811cd42d74a3108d61d17a7ec763d8c12ad6326ae52d8451ad1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9ef47668dc41835e4b510ff3c1a0ab24f49eaf624a06f4279a72285999b628f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43da69a11fa66e371f467faff34759709b0e5be912143f3d939c925495acba12`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 10:01:21 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:24 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 09 Feb 2021 10:01:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 09 Feb 2021 10:01:33 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:33 GMT
VOLUME [/data]
# Tue, 09 Feb 2021 10:01:33 GMT
WORKDIR /data
# Tue, 09 Feb 2021 10:01:34 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 09 Feb 2021 10:01:34 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba91f7729f259daac39bd3811894b8eb41e413868b9dbc849b075a091ddfab`  
		Last Modified: Tue, 09 Feb 2021 10:02:37 GMT  
		Size: 6.7 MB (6689002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70800ce8bb800c48858ed7b5ff88cac5dcc2ee0656bb66cdaee2c9f94e0d639a`  
		Last Modified: Tue, 09 Feb 2021 10:02:32 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f9c3fcb993740acdaaef14ba45efa51fad022d25880ec2b637992a58f6e2`  
		Last Modified: Tue, 09 Feb 2021 10:02:38 GMT  
		Size: 18.0 MB (17990777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4be2b06f4e8bb25cc27cbdfa252e7dd775d539450c90410f2127256feab50c7`  
		Last Modified: Tue, 09 Feb 2021 10:02:33 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4`

```console
$ docker pull rethinkdb@sha256:ff28f747a8183811cd42d74a3108d61d17a7ec763d8c12ad6326ae52d8451ad1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9ef47668dc41835e4b510ff3c1a0ab24f49eaf624a06f4279a72285999b628f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43da69a11fa66e371f467faff34759709b0e5be912143f3d939c925495acba12`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 10:01:21 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:24 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 09 Feb 2021 10:01:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 09 Feb 2021 10:01:33 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:33 GMT
VOLUME [/data]
# Tue, 09 Feb 2021 10:01:33 GMT
WORKDIR /data
# Tue, 09 Feb 2021 10:01:34 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 09 Feb 2021 10:01:34 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba91f7729f259daac39bd3811894b8eb41e413868b9dbc849b075a091ddfab`  
		Last Modified: Tue, 09 Feb 2021 10:02:37 GMT  
		Size: 6.7 MB (6689002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70800ce8bb800c48858ed7b5ff88cac5dcc2ee0656bb66cdaee2c9f94e0d639a`  
		Last Modified: Tue, 09 Feb 2021 10:02:32 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f9c3fcb993740acdaaef14ba45efa51fad022d25880ec2b637992a58f6e2`  
		Last Modified: Tue, 09 Feb 2021 10:02:38 GMT  
		Size: 18.0 MB (17990777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4be2b06f4e8bb25cc27cbdfa252e7dd775d539450c90410f2127256feab50c7`  
		Last Modified: Tue, 09 Feb 2021 10:02:33 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0`

```console
$ docker pull rethinkdb@sha256:8ce8b91c6652715547740d156ff44869987ebc04ecbed580040cafcde7914c72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0` - linux; amd64

```console
$ docker pull rethinkdb@sha256:3a415f1d5e452128f29ea87f90ae899f874d844399f8c25770a2e97768dcbde4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51779059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96674cb0f04e2159c73d1c5e039e3ac949bb9bcba75787f875b16b43eaa8fadd`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 10:01:21 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:47 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 09 Feb 2021 10:01:47 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Tue, 09 Feb 2021 10:01:58 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:58 GMT
VOLUME [/data]
# Tue, 09 Feb 2021 10:01:59 GMT
WORKDIR /data
# Tue, 09 Feb 2021 10:01:59 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 09 Feb 2021 10:02:00 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba91f7729f259daac39bd3811894b8eb41e413868b9dbc849b075a091ddfab`  
		Last Modified: Tue, 09 Feb 2021 10:02:37 GMT  
		Size: 6.7 MB (6689002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede96e68258f7f4b1b603352672cf80c2aaa51a640b0593b006c5cde5491c660`  
		Last Modified: Tue, 09 Feb 2021 10:02:52 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e076aad5b9b349354adbfd07a5613bd46540d9ee41ec013313487a13ac042f4`  
		Last Modified: Tue, 09 Feb 2021 10:02:59 GMT  
		Size: 18.0 MB (17992210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec607f89dc554c7b43bba7a0e630413018e912d0e6c60fec2e31029dc6838cd`  
		Last Modified: Tue, 09 Feb 2021 10:02:53 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-buster-slim`

```console
$ docker pull rethinkdb@sha256:8ce8b91c6652715547740d156ff44869987ebc04ecbed580040cafcde7914c72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:3a415f1d5e452128f29ea87f90ae899f874d844399f8c25770a2e97768dcbde4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51779059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96674cb0f04e2159c73d1c5e039e3ac949bb9bcba75787f875b16b43eaa8fadd`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 10:01:21 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:47 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 09 Feb 2021 10:01:47 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Tue, 09 Feb 2021 10:01:58 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:58 GMT
VOLUME [/data]
# Tue, 09 Feb 2021 10:01:59 GMT
WORKDIR /data
# Tue, 09 Feb 2021 10:01:59 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 09 Feb 2021 10:02:00 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba91f7729f259daac39bd3811894b8eb41e413868b9dbc849b075a091ddfab`  
		Last Modified: Tue, 09 Feb 2021 10:02:37 GMT  
		Size: 6.7 MB (6689002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede96e68258f7f4b1b603352672cf80c2aaa51a640b0593b006c5cde5491c660`  
		Last Modified: Tue, 09 Feb 2021 10:02:52 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e076aad5b9b349354adbfd07a5613bd46540d9ee41ec013313487a13ac042f4`  
		Last Modified: Tue, 09 Feb 2021 10:02:59 GMT  
		Size: 18.0 MB (17992210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec607f89dc554c7b43bba7a0e630413018e912d0e6c60fec2e31029dc6838cd`  
		Last Modified: Tue, 09 Feb 2021 10:02:53 GMT  
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
$ docker pull rethinkdb@sha256:ff28f747a8183811cd42d74a3108d61d17a7ec763d8c12ad6326ae52d8451ad1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9ef47668dc41835e4b510ff3c1a0ab24f49eaf624a06f4279a72285999b628f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43da69a11fa66e371f467faff34759709b0e5be912143f3d939c925495acba12`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 10:01:21 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:24 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 09 Feb 2021 10:01:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 09 Feb 2021 10:01:33 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:33 GMT
VOLUME [/data]
# Tue, 09 Feb 2021 10:01:33 GMT
WORKDIR /data
# Tue, 09 Feb 2021 10:01:34 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 09 Feb 2021 10:01:34 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba91f7729f259daac39bd3811894b8eb41e413868b9dbc849b075a091ddfab`  
		Last Modified: Tue, 09 Feb 2021 10:02:37 GMT  
		Size: 6.7 MB (6689002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70800ce8bb800c48858ed7b5ff88cac5dcc2ee0656bb66cdaee2c9f94e0d639a`  
		Last Modified: Tue, 09 Feb 2021 10:02:32 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f9c3fcb993740acdaaef14ba45efa51fad022d25880ec2b637992a58f6e2`  
		Last Modified: Tue, 09 Feb 2021 10:02:38 GMT  
		Size: 18.0 MB (17990777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4be2b06f4e8bb25cc27cbdfa252e7dd775d539450c90410f2127256feab50c7`  
		Last Modified: Tue, 09 Feb 2021 10:02:33 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1-buster-slim`

```console
$ docker pull rethinkdb@sha256:ff28f747a8183811cd42d74a3108d61d17a7ec763d8c12ad6326ae52d8451ad1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9ef47668dc41835e4b510ff3c1a0ab24f49eaf624a06f4279a72285999b628f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43da69a11fa66e371f467faff34759709b0e5be912143f3d939c925495acba12`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 10:01:21 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:24 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 09 Feb 2021 10:01:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 09 Feb 2021 10:01:33 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:33 GMT
VOLUME [/data]
# Tue, 09 Feb 2021 10:01:33 GMT
WORKDIR /data
# Tue, 09 Feb 2021 10:01:34 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 09 Feb 2021 10:01:34 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba91f7729f259daac39bd3811894b8eb41e413868b9dbc849b075a091ddfab`  
		Last Modified: Tue, 09 Feb 2021 10:02:37 GMT  
		Size: 6.7 MB (6689002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70800ce8bb800c48858ed7b5ff88cac5dcc2ee0656bb66cdaee2c9f94e0d639a`  
		Last Modified: Tue, 09 Feb 2021 10:02:32 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f9c3fcb993740acdaaef14ba45efa51fad022d25880ec2b637992a58f6e2`  
		Last Modified: Tue, 09 Feb 2021 10:02:38 GMT  
		Size: 18.0 MB (17990777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4be2b06f4e8bb25cc27cbdfa252e7dd775d539450c90410f2127256feab50c7`  
		Last Modified: Tue, 09 Feb 2021 10:02:33 GMT  
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
$ docker pull rethinkdb@sha256:ff28f747a8183811cd42d74a3108d61d17a7ec763d8c12ad6326ae52d8451ad1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9ef47668dc41835e4b510ff3c1a0ab24f49eaf624a06f4279a72285999b628f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43da69a11fa66e371f467faff34759709b0e5be912143f3d939c925495acba12`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 10:01:21 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:24 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 09 Feb 2021 10:01:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 09 Feb 2021 10:01:33 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:33 GMT
VOLUME [/data]
# Tue, 09 Feb 2021 10:01:33 GMT
WORKDIR /data
# Tue, 09 Feb 2021 10:01:34 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 09 Feb 2021 10:01:34 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba91f7729f259daac39bd3811894b8eb41e413868b9dbc849b075a091ddfab`  
		Last Modified: Tue, 09 Feb 2021 10:02:37 GMT  
		Size: 6.7 MB (6689002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70800ce8bb800c48858ed7b5ff88cac5dcc2ee0656bb66cdaee2c9f94e0d639a`  
		Last Modified: Tue, 09 Feb 2021 10:02:32 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f9c3fcb993740acdaaef14ba45efa51fad022d25880ec2b637992a58f6e2`  
		Last Modified: Tue, 09 Feb 2021 10:02:38 GMT  
		Size: 18.0 MB (17990777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4be2b06f4e8bb25cc27cbdfa252e7dd775d539450c90410f2127256feab50c7`  
		Last Modified: Tue, 09 Feb 2021 10:02:33 GMT  
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
$ docker pull rethinkdb@sha256:ff28f747a8183811cd42d74a3108d61d17a7ec763d8c12ad6326ae52d8451ad1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9ef47668dc41835e4b510ff3c1a0ab24f49eaf624a06f4279a72285999b628f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43da69a11fa66e371f467faff34759709b0e5be912143f3d939c925495acba12`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 10:01:21 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:24 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 09 Feb 2021 10:01:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 09 Feb 2021 10:01:33 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:33 GMT
VOLUME [/data]
# Tue, 09 Feb 2021 10:01:33 GMT
WORKDIR /data
# Tue, 09 Feb 2021 10:01:34 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 09 Feb 2021 10:01:34 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba91f7729f259daac39bd3811894b8eb41e413868b9dbc849b075a091ddfab`  
		Last Modified: Tue, 09 Feb 2021 10:02:37 GMT  
		Size: 6.7 MB (6689002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70800ce8bb800c48858ed7b5ff88cac5dcc2ee0656bb66cdaee2c9f94e0d639a`  
		Last Modified: Tue, 09 Feb 2021 10:02:32 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f9c3fcb993740acdaaef14ba45efa51fad022d25880ec2b637992a58f6e2`  
		Last Modified: Tue, 09 Feb 2021 10:02:38 GMT  
		Size: 18.0 MB (17990777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4be2b06f4e8bb25cc27cbdfa252e7dd775d539450c90410f2127256feab50c7`  
		Last Modified: Tue, 09 Feb 2021 10:02:33 GMT  
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
$ docker pull rethinkdb@sha256:ff28f747a8183811cd42d74a3108d61d17a7ec763d8c12ad6326ae52d8451ad1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9ef47668dc41835e4b510ff3c1a0ab24f49eaf624a06f4279a72285999b628f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43da69a11fa66e371f467faff34759709b0e5be912143f3d939c925495acba12`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 10:01:21 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:24 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 09 Feb 2021 10:01:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 09 Feb 2021 10:01:33 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:33 GMT
VOLUME [/data]
# Tue, 09 Feb 2021 10:01:33 GMT
WORKDIR /data
# Tue, 09 Feb 2021 10:01:34 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 09 Feb 2021 10:01:34 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba91f7729f259daac39bd3811894b8eb41e413868b9dbc849b075a091ddfab`  
		Last Modified: Tue, 09 Feb 2021 10:02:37 GMT  
		Size: 6.7 MB (6689002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70800ce8bb800c48858ed7b5ff88cac5dcc2ee0656bb66cdaee2c9f94e0d639a`  
		Last Modified: Tue, 09 Feb 2021 10:02:32 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f9c3fcb993740acdaaef14ba45efa51fad022d25880ec2b637992a58f6e2`  
		Last Modified: Tue, 09 Feb 2021 10:02:38 GMT  
		Size: 18.0 MB (17990777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4be2b06f4e8bb25cc27cbdfa252e7dd775d539450c90410f2127256feab50c7`  
		Last Modified: Tue, 09 Feb 2021 10:02:33 GMT  
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
$ docker pull rethinkdb@sha256:ff28f747a8183811cd42d74a3108d61d17a7ec763d8c12ad6326ae52d8451ad1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:latest` - linux; amd64

```console
$ docker pull rethinkdb@sha256:9ef47668dc41835e4b510ff3c1a0ab24f49eaf624a06f4279a72285999b628f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43da69a11fa66e371f467faff34759709b0e5be912143f3d939c925495acba12`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 10:01:21 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:24 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 09 Feb 2021 10:01:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 09 Feb 2021 10:01:33 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 10:01:33 GMT
VOLUME [/data]
# Tue, 09 Feb 2021 10:01:33 GMT
WORKDIR /data
# Tue, 09 Feb 2021 10:01:34 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 09 Feb 2021 10:01:34 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dba91f7729f259daac39bd3811894b8eb41e413868b9dbc849b075a091ddfab`  
		Last Modified: Tue, 09 Feb 2021 10:02:37 GMT  
		Size: 6.7 MB (6689002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70800ce8bb800c48858ed7b5ff88cac5dcc2ee0656bb66cdaee2c9f94e0d639a`  
		Last Modified: Tue, 09 Feb 2021 10:02:32 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3f9c3fcb993740acdaaef14ba45efa51fad022d25880ec2b637992a58f6e2`  
		Last Modified: Tue, 09 Feb 2021 10:02:38 GMT  
		Size: 18.0 MB (17990777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4be2b06f4e8bb25cc27cbdfa252e7dd775d539450c90410f2127256feab50c7`  
		Last Modified: Tue, 09 Feb 2021 10:02:33 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
