<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rethinkdb`

-	[`rethinkdb:2`](#rethinkdb2)
-	[`rethinkdb:2-buster-slim`](#rethinkdb2-buster-slim)
-	[`rethinkdb:2-centos`](#rethinkdb2-centos)
-	[`rethinkdb:2.4`](#rethinkdb24)
-	[`rethinkdb:2.4-buster-slim`](#rethinkdb24-buster-slim)
-	[`rethinkdb:2.4-centos`](#rethinkdb24-centos)
-	[`rethinkdb:2.4.0`](#rethinkdb240)
-	[`rethinkdb:2.4.0-buster-slim`](#rethinkdb240-buster-slim)
-	[`rethinkdb:2.4.0-centos`](#rethinkdb240-centos)
-	[`rethinkdb:2.4.1`](#rethinkdb241)
-	[`rethinkdb:2.4.1-buster-slim`](#rethinkdb241-buster-slim)
-	[`rethinkdb:2.4.1-centos`](#rethinkdb241-centos)
-	[`rethinkdb:buster-slim`](#rethinkdbbuster-slim)
-	[`rethinkdb:centos`](#rethinkdbcentos)
-	[`rethinkdb:latest`](#rethinkdblatest)

## `rethinkdb:2`

```console
$ docker pull rethinkdb@sha256:ef228aaa7f72799c143b5eecc5a0fa2bfabfdaea31ceefa5bb27b7da25645290
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2` - linux; amd64

```console
$ docker pull rethinkdb@sha256:87b9e743d853c86cd2998223eb8badb5852a2de294d02f186d3f15b5314b71fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51824125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4250c5b26ae2ca851263ba2ebaa677466e42fed8cf45ebe581945d0bc3fc1f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:10:24 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:27 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 10 Apr 2021 17:10:28 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Sat, 10 Apr 2021 17:10:34 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:35 GMT
VOLUME [/data]
# Sat, 10 Apr 2021 17:10:35 GMT
WORKDIR /data
# Sat, 10 Apr 2021 17:10:35 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 10 Apr 2021 17:10:35 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e36f66c1815fb7b7ac84f2e19aaad0b7a00fdb61921150d29feab40023fde1c`  
		Last Modified: Sat, 10 Apr 2021 17:11:23 GMT  
		Size: 6.7 MB (6690291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b4f8dfad448c8753fff951042f3d7f0346ad2cd3a116cfbb39d3b0db993c`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fcc47b42337170ffdce3d5d3edc1913ae6d1f4d0960f973b0bcbc609f4f79`  
		Last Modified: Sat, 10 Apr 2021 17:11:19 GMT  
		Size: 18.0 MB (17991722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef48c89b3b8060a67e31c4182e08fba291533418ea7829341843ce728f24ab4`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-buster-slim`

```console
$ docker pull rethinkdb@sha256:ef228aaa7f72799c143b5eecc5a0fa2bfabfdaea31ceefa5bb27b7da25645290
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:87b9e743d853c86cd2998223eb8badb5852a2de294d02f186d3f15b5314b71fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51824125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4250c5b26ae2ca851263ba2ebaa677466e42fed8cf45ebe581945d0bc3fc1f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:10:24 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:27 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 10 Apr 2021 17:10:28 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Sat, 10 Apr 2021 17:10:34 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:35 GMT
VOLUME [/data]
# Sat, 10 Apr 2021 17:10:35 GMT
WORKDIR /data
# Sat, 10 Apr 2021 17:10:35 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 10 Apr 2021 17:10:35 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e36f66c1815fb7b7ac84f2e19aaad0b7a00fdb61921150d29feab40023fde1c`  
		Last Modified: Sat, 10 Apr 2021 17:11:23 GMT  
		Size: 6.7 MB (6690291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b4f8dfad448c8753fff951042f3d7f0346ad2cd3a116cfbb39d3b0db993c`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fcc47b42337170ffdce3d5d3edc1913ae6d1f4d0960f973b0bcbc609f4f79`  
		Last Modified: Sat, 10 Apr 2021 17:11:19 GMT  
		Size: 18.0 MB (17991722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef48c89b3b8060a67e31c4182e08fba291533418ea7829341843ce728f24ab4`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-centos`

```console
$ docker pull rethinkdb@sha256:b64ea5554c79140250dcb1b9890a403d81dda0562b8b747a9f8f03507fafa6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:19543b769d6fc6364ebf7e49586a5393f1e4aea8c846b1b66becd6309be84b9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97511790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c64b1fd4d8d7be12e58683646b567a9b21e435a629175801f20ace09eed40b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Fri, 12 Mar 2021 22:06:09 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Fri, 12 Mar 2021 22:06:11 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 12 Mar 2021 22:06:23 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 12 Mar 2021 22:06:23 GMT
VOLUME [/data]
# Fri, 12 Mar 2021 22:06:24 GMT
WORKDIR /data
# Fri, 12 Mar 2021 22:06:24 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 12 Mar 2021 22:06:24 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae1e6677aefac3d9eae873c0dcf112163e1d7c02e8b1c6440876d95a5fa448d`  
		Last Modified: Fri, 12 Mar 2021 22:07:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308bfa96e4023aefc38b6afabf4bab16585c81dca08a9846cf82a86d1ab02186`  
		Last Modified: Fri, 12 Mar 2021 22:07:56 GMT  
		Size: 22.3 MB (22329396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c75a151438cb5b472c183e238e3ce14e21bbab2ba06c6ca56bc5bffc489866`  
		Last Modified: Fri, 12 Mar 2021 22:07:51 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4`

```console
$ docker pull rethinkdb@sha256:ef228aaa7f72799c143b5eecc5a0fa2bfabfdaea31ceefa5bb27b7da25645290
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4` - linux; amd64

```console
$ docker pull rethinkdb@sha256:87b9e743d853c86cd2998223eb8badb5852a2de294d02f186d3f15b5314b71fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51824125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4250c5b26ae2ca851263ba2ebaa677466e42fed8cf45ebe581945d0bc3fc1f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:10:24 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:27 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 10 Apr 2021 17:10:28 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Sat, 10 Apr 2021 17:10:34 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:35 GMT
VOLUME [/data]
# Sat, 10 Apr 2021 17:10:35 GMT
WORKDIR /data
# Sat, 10 Apr 2021 17:10:35 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 10 Apr 2021 17:10:35 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e36f66c1815fb7b7ac84f2e19aaad0b7a00fdb61921150d29feab40023fde1c`  
		Last Modified: Sat, 10 Apr 2021 17:11:23 GMT  
		Size: 6.7 MB (6690291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b4f8dfad448c8753fff951042f3d7f0346ad2cd3a116cfbb39d3b0db993c`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fcc47b42337170ffdce3d5d3edc1913ae6d1f4d0960f973b0bcbc609f4f79`  
		Last Modified: Sat, 10 Apr 2021 17:11:19 GMT  
		Size: 18.0 MB (17991722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef48c89b3b8060a67e31c4182e08fba291533418ea7829341843ce728f24ab4`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-buster-slim`

```console
$ docker pull rethinkdb@sha256:ef228aaa7f72799c143b5eecc5a0fa2bfabfdaea31ceefa5bb27b7da25645290
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:87b9e743d853c86cd2998223eb8badb5852a2de294d02f186d3f15b5314b71fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51824125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4250c5b26ae2ca851263ba2ebaa677466e42fed8cf45ebe581945d0bc3fc1f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:10:24 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:27 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 10 Apr 2021 17:10:28 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Sat, 10 Apr 2021 17:10:34 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:35 GMT
VOLUME [/data]
# Sat, 10 Apr 2021 17:10:35 GMT
WORKDIR /data
# Sat, 10 Apr 2021 17:10:35 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 10 Apr 2021 17:10:35 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e36f66c1815fb7b7ac84f2e19aaad0b7a00fdb61921150d29feab40023fde1c`  
		Last Modified: Sat, 10 Apr 2021 17:11:23 GMT  
		Size: 6.7 MB (6690291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b4f8dfad448c8753fff951042f3d7f0346ad2cd3a116cfbb39d3b0db993c`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fcc47b42337170ffdce3d5d3edc1913ae6d1f4d0960f973b0bcbc609f4f79`  
		Last Modified: Sat, 10 Apr 2021 17:11:19 GMT  
		Size: 18.0 MB (17991722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef48c89b3b8060a67e31c4182e08fba291533418ea7829341843ce728f24ab4`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-centos`

```console
$ docker pull rethinkdb@sha256:b64ea5554c79140250dcb1b9890a403d81dda0562b8b747a9f8f03507fafa6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:19543b769d6fc6364ebf7e49586a5393f1e4aea8c846b1b66becd6309be84b9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97511790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c64b1fd4d8d7be12e58683646b567a9b21e435a629175801f20ace09eed40b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Fri, 12 Mar 2021 22:06:09 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Fri, 12 Mar 2021 22:06:11 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 12 Mar 2021 22:06:23 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 12 Mar 2021 22:06:23 GMT
VOLUME [/data]
# Fri, 12 Mar 2021 22:06:24 GMT
WORKDIR /data
# Fri, 12 Mar 2021 22:06:24 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 12 Mar 2021 22:06:24 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae1e6677aefac3d9eae873c0dcf112163e1d7c02e8b1c6440876d95a5fa448d`  
		Last Modified: Fri, 12 Mar 2021 22:07:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308bfa96e4023aefc38b6afabf4bab16585c81dca08a9846cf82a86d1ab02186`  
		Last Modified: Fri, 12 Mar 2021 22:07:56 GMT  
		Size: 22.3 MB (22329396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c75a151438cb5b472c183e238e3ce14e21bbab2ba06c6ca56bc5bffc489866`  
		Last Modified: Fri, 12 Mar 2021 22:07:51 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0`

```console
$ docker pull rethinkdb@sha256:f6aeb4ebcaa15d1a041e2fb4fbafc55d335b1eacdd6654640b1e4f8c0b869371
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0` - linux; amd64

```console
$ docker pull rethinkdb@sha256:36b43b32b6c1f6532618095a389a5a082d2ceb85b7087595b83c36550a02041b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51825340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6618deb8f49b90d8cead8cf0aa461a64cf7a354f5d2112c8bea7329413bbcaff`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:10:24 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:45 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 10 Apr 2021 17:10:45 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Sat, 10 Apr 2021 17:10:52 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:52 GMT
VOLUME [/data]
# Sat, 10 Apr 2021 17:10:52 GMT
WORKDIR /data
# Sat, 10 Apr 2021 17:10:53 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 10 Apr 2021 17:10:53 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e36f66c1815fb7b7ac84f2e19aaad0b7a00fdb61921150d29feab40023fde1c`  
		Last Modified: Sat, 10 Apr 2021 17:11:23 GMT  
		Size: 6.7 MB (6690291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a53b6eaad13ee614860644809935e3fe3fa06afeca1898b2fa365fcbef2a4d`  
		Last Modified: Sat, 10 Apr 2021 17:11:50 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf502fc8c73279227aa932d715132f41351addaa2a746a1e83713a7105b01204`  
		Last Modified: Sat, 10 Apr 2021 17:11:55 GMT  
		Size: 18.0 MB (17992934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cbd5635e7e96a1112c9ac58415f9fd3429d084ff1e5f0bf14f985e18aa435a`  
		Last Modified: Sat, 10 Apr 2021 17:11:50 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-buster-slim`

```console
$ docker pull rethinkdb@sha256:f6aeb4ebcaa15d1a041e2fb4fbafc55d335b1eacdd6654640b1e4f8c0b869371
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:36b43b32b6c1f6532618095a389a5a082d2ceb85b7087595b83c36550a02041b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51825340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6618deb8f49b90d8cead8cf0aa461a64cf7a354f5d2112c8bea7329413bbcaff`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:10:24 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:45 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 10 Apr 2021 17:10:45 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Sat, 10 Apr 2021 17:10:52 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:52 GMT
VOLUME [/data]
# Sat, 10 Apr 2021 17:10:52 GMT
WORKDIR /data
# Sat, 10 Apr 2021 17:10:53 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 10 Apr 2021 17:10:53 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e36f66c1815fb7b7ac84f2e19aaad0b7a00fdb61921150d29feab40023fde1c`  
		Last Modified: Sat, 10 Apr 2021 17:11:23 GMT  
		Size: 6.7 MB (6690291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a53b6eaad13ee614860644809935e3fe3fa06afeca1898b2fa365fcbef2a4d`  
		Last Modified: Sat, 10 Apr 2021 17:11:50 GMT  
		Size: 2.6 KB (2615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf502fc8c73279227aa932d715132f41351addaa2a746a1e83713a7105b01204`  
		Last Modified: Sat, 10 Apr 2021 17:11:55 GMT  
		Size: 18.0 MB (17992934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cbd5635e7e96a1112c9ac58415f9fd3429d084ff1e5f0bf14f985e18aa435a`  
		Last Modified: Sat, 10 Apr 2021 17:11:50 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-centos`

```console
$ docker pull rethinkdb@sha256:11d9649e49b7e3b68d5d28e3e3959b055a6f7639bab3bc810e8afe96c6e7cc01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:17689662917e7af14d2bebf46cd6890ee8badf9b74e8e8b1480ec0b6bde5a29a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97512200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f93c64f13e16520ee2f13c350b04b364d79f12de5f07eb0ab11357643807bf`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Fri, 12 Mar 2021 22:06:50 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0
# Fri, 12 Mar 2021 22:06:51 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 12 Mar 2021 22:06:59 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 12 Mar 2021 22:06:59 GMT
VOLUME [/data]
# Fri, 12 Mar 2021 22:07:00 GMT
WORKDIR /data
# Fri, 12 Mar 2021 22:07:00 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 12 Mar 2021 22:07:00 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25076e20c46678ae755ba6afa36d6d81841dc318bbf67e12e1dc65a61830d747`  
		Last Modified: Fri, 12 Mar 2021 22:08:28 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a6c1b31a4042d1cd7786c6f48d8c3d4f0c4694af26eef0a12a818bfb31e040`  
		Last Modified: Fri, 12 Mar 2021 22:08:32 GMT  
		Size: 22.3 MB (22329806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b305cc56442aaa917ad4c80c57d1d01db071a009e92c3a8f5129445a25b4eb`  
		Last Modified: Fri, 12 Mar 2021 22:08:28 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1`

```console
$ docker pull rethinkdb@sha256:ef228aaa7f72799c143b5eecc5a0fa2bfabfdaea31ceefa5bb27b7da25645290
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1` - linux; amd64

```console
$ docker pull rethinkdb@sha256:87b9e743d853c86cd2998223eb8badb5852a2de294d02f186d3f15b5314b71fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51824125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4250c5b26ae2ca851263ba2ebaa677466e42fed8cf45ebe581945d0bc3fc1f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:10:24 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:27 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 10 Apr 2021 17:10:28 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Sat, 10 Apr 2021 17:10:34 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:35 GMT
VOLUME [/data]
# Sat, 10 Apr 2021 17:10:35 GMT
WORKDIR /data
# Sat, 10 Apr 2021 17:10:35 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 10 Apr 2021 17:10:35 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e36f66c1815fb7b7ac84f2e19aaad0b7a00fdb61921150d29feab40023fde1c`  
		Last Modified: Sat, 10 Apr 2021 17:11:23 GMT  
		Size: 6.7 MB (6690291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b4f8dfad448c8753fff951042f3d7f0346ad2cd3a116cfbb39d3b0db993c`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fcc47b42337170ffdce3d5d3edc1913ae6d1f4d0960f973b0bcbc609f4f79`  
		Last Modified: Sat, 10 Apr 2021 17:11:19 GMT  
		Size: 18.0 MB (17991722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef48c89b3b8060a67e31c4182e08fba291533418ea7829341843ce728f24ab4`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1-buster-slim`

```console
$ docker pull rethinkdb@sha256:ef228aaa7f72799c143b5eecc5a0fa2bfabfdaea31ceefa5bb27b7da25645290
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:87b9e743d853c86cd2998223eb8badb5852a2de294d02f186d3f15b5314b71fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51824125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4250c5b26ae2ca851263ba2ebaa677466e42fed8cf45ebe581945d0bc3fc1f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:10:24 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:27 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 10 Apr 2021 17:10:28 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Sat, 10 Apr 2021 17:10:34 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:35 GMT
VOLUME [/data]
# Sat, 10 Apr 2021 17:10:35 GMT
WORKDIR /data
# Sat, 10 Apr 2021 17:10:35 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 10 Apr 2021 17:10:35 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e36f66c1815fb7b7ac84f2e19aaad0b7a00fdb61921150d29feab40023fde1c`  
		Last Modified: Sat, 10 Apr 2021 17:11:23 GMT  
		Size: 6.7 MB (6690291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b4f8dfad448c8753fff951042f3d7f0346ad2cd3a116cfbb39d3b0db993c`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fcc47b42337170ffdce3d5d3edc1913ae6d1f4d0960f973b0bcbc609f4f79`  
		Last Modified: Sat, 10 Apr 2021 17:11:19 GMT  
		Size: 18.0 MB (17991722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef48c89b3b8060a67e31c4182e08fba291533418ea7829341843ce728f24ab4`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1-centos`

```console
$ docker pull rethinkdb@sha256:b64ea5554c79140250dcb1b9890a403d81dda0562b8b747a9f8f03507fafa6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:19543b769d6fc6364ebf7e49586a5393f1e4aea8c846b1b66becd6309be84b9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97511790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c64b1fd4d8d7be12e58683646b567a9b21e435a629175801f20ace09eed40b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Fri, 12 Mar 2021 22:06:09 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Fri, 12 Mar 2021 22:06:11 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 12 Mar 2021 22:06:23 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 12 Mar 2021 22:06:23 GMT
VOLUME [/data]
# Fri, 12 Mar 2021 22:06:24 GMT
WORKDIR /data
# Fri, 12 Mar 2021 22:06:24 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 12 Mar 2021 22:06:24 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae1e6677aefac3d9eae873c0dcf112163e1d7c02e8b1c6440876d95a5fa448d`  
		Last Modified: Fri, 12 Mar 2021 22:07:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308bfa96e4023aefc38b6afabf4bab16585c81dca08a9846cf82a86d1ab02186`  
		Last Modified: Fri, 12 Mar 2021 22:07:56 GMT  
		Size: 22.3 MB (22329396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c75a151438cb5b472c183e238e3ce14e21bbab2ba06c6ca56bc5bffc489866`  
		Last Modified: Fri, 12 Mar 2021 22:07:51 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:buster-slim`

```console
$ docker pull rethinkdb@sha256:ef228aaa7f72799c143b5eecc5a0fa2bfabfdaea31ceefa5bb27b7da25645290
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:87b9e743d853c86cd2998223eb8badb5852a2de294d02f186d3f15b5314b71fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51824125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4250c5b26ae2ca851263ba2ebaa677466e42fed8cf45ebe581945d0bc3fc1f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:10:24 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:27 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 10 Apr 2021 17:10:28 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Sat, 10 Apr 2021 17:10:34 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:35 GMT
VOLUME [/data]
# Sat, 10 Apr 2021 17:10:35 GMT
WORKDIR /data
# Sat, 10 Apr 2021 17:10:35 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 10 Apr 2021 17:10:35 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e36f66c1815fb7b7ac84f2e19aaad0b7a00fdb61921150d29feab40023fde1c`  
		Last Modified: Sat, 10 Apr 2021 17:11:23 GMT  
		Size: 6.7 MB (6690291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b4f8dfad448c8753fff951042f3d7f0346ad2cd3a116cfbb39d3b0db993c`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fcc47b42337170ffdce3d5d3edc1913ae6d1f4d0960f973b0bcbc609f4f79`  
		Last Modified: Sat, 10 Apr 2021 17:11:19 GMT  
		Size: 18.0 MB (17991722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef48c89b3b8060a67e31c4182e08fba291533418ea7829341843ce728f24ab4`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:centos`

```console
$ docker pull rethinkdb@sha256:b64ea5554c79140250dcb1b9890a403d81dda0562b8b747a9f8f03507fafa6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:19543b769d6fc6364ebf7e49586a5393f1e4aea8c846b1b66becd6309be84b9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97511790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c64b1fd4d8d7be12e58683646b567a9b21e435a629175801f20ace09eed40b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Fri, 12 Mar 2021 22:06:09 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Fri, 12 Mar 2021 22:06:11 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 12 Mar 2021 22:06:23 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 12 Mar 2021 22:06:23 GMT
VOLUME [/data]
# Fri, 12 Mar 2021 22:06:24 GMT
WORKDIR /data
# Fri, 12 Mar 2021 22:06:24 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 12 Mar 2021 22:06:24 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae1e6677aefac3d9eae873c0dcf112163e1d7c02e8b1c6440876d95a5fa448d`  
		Last Modified: Fri, 12 Mar 2021 22:07:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308bfa96e4023aefc38b6afabf4bab16585c81dca08a9846cf82a86d1ab02186`  
		Last Modified: Fri, 12 Mar 2021 22:07:56 GMT  
		Size: 22.3 MB (22329396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c75a151438cb5b472c183e238e3ce14e21bbab2ba06c6ca56bc5bffc489866`  
		Last Modified: Fri, 12 Mar 2021 22:07:51 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:latest`

```console
$ docker pull rethinkdb@sha256:ef228aaa7f72799c143b5eecc5a0fa2bfabfdaea31ceefa5bb27b7da25645290
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:latest` - linux; amd64

```console
$ docker pull rethinkdb@sha256:87b9e743d853c86cd2998223eb8badb5852a2de294d02f186d3f15b5314b71fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51824125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4250c5b26ae2ca851263ba2ebaa677466e42fed8cf45ebe581945d0bc3fc1f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:10:24 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:27 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 10 Apr 2021 17:10:28 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Sat, 10 Apr 2021 17:10:34 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:10:35 GMT
VOLUME [/data]
# Sat, 10 Apr 2021 17:10:35 GMT
WORKDIR /data
# Sat, 10 Apr 2021 17:10:35 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 10 Apr 2021 17:10:35 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e36f66c1815fb7b7ac84f2e19aaad0b7a00fdb61921150d29feab40023fde1c`  
		Last Modified: Sat, 10 Apr 2021 17:11:23 GMT  
		Size: 6.7 MB (6690291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b4f8dfad448c8753fff951042f3d7f0346ad2cd3a116cfbb39d3b0db993c`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fcc47b42337170ffdce3d5d3edc1913ae6d1f4d0960f973b0bcbc609f4f79`  
		Last Modified: Sat, 10 Apr 2021 17:11:19 GMT  
		Size: 18.0 MB (17991722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef48c89b3b8060a67e31c4182e08fba291533418ea7829341843ce728f24ab4`  
		Last Modified: Sat, 10 Apr 2021 17:11:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
