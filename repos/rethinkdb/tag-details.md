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
$ docker pull rethinkdb@sha256:2fd3b70663c04a742cb05a38cd006f838dd03f598b53e0905fe416e6ce9c8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2` - linux; amd64

```console
$ docker pull rethinkdb@sha256:d06b5c006ea5bed1913283910e0045f0c2144d0f968fb4b46ccaf0947cb99b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f37e5daf5bdf21d3a3cdd583213b0bb7dabf6dfdcdc12e2231cfc39551af5b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:29:01 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:04 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 12 May 2021 17:29:05 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 12 May 2021 17:29:12 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:12 GMT
VOLUME [/data]
# Wed, 12 May 2021 17:29:12 GMT
WORKDIR /data
# Wed, 12 May 2021 17:29:13 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 12 May 2021 17:29:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b31dbb3d3e7721a2f9cb1ed29dcb1b960873ee852b122ca3cab6e6300154d`  
		Last Modified: Wed, 12 May 2021 17:29:58 GMT  
		Size: 6.7 MB (6690387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5695ae0ed6c7809de5b3cc650a24848ef3ddc7fdd2ee8b43b12255cdf1bd204`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0722ed38c905f6d03f45d75ddf2dd6209c84e9100a8b3e2aed1e9b702dba81`  
		Last Modified: Wed, 12 May 2021 17:29:59 GMT  
		Size: 18.0 MB (17991761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f89003a5ba016395930174176b5e32e83c894225e40329527289ad7238bf8f`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-buster-slim`

```console
$ docker pull rethinkdb@sha256:2fd3b70663c04a742cb05a38cd006f838dd03f598b53e0905fe416e6ce9c8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:d06b5c006ea5bed1913283910e0045f0c2144d0f968fb4b46ccaf0947cb99b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f37e5daf5bdf21d3a3cdd583213b0bb7dabf6dfdcdc12e2231cfc39551af5b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:29:01 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:04 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 12 May 2021 17:29:05 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 12 May 2021 17:29:12 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:12 GMT
VOLUME [/data]
# Wed, 12 May 2021 17:29:12 GMT
WORKDIR /data
# Wed, 12 May 2021 17:29:13 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 12 May 2021 17:29:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b31dbb3d3e7721a2f9cb1ed29dcb1b960873ee852b122ca3cab6e6300154d`  
		Last Modified: Wed, 12 May 2021 17:29:58 GMT  
		Size: 6.7 MB (6690387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5695ae0ed6c7809de5b3cc650a24848ef3ddc7fdd2ee8b43b12255cdf1bd204`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0722ed38c905f6d03f45d75ddf2dd6209c84e9100a8b3e2aed1e9b702dba81`  
		Last Modified: Wed, 12 May 2021 17:29:59 GMT  
		Size: 18.0 MB (17991761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f89003a5ba016395930174176b5e32e83c894225e40329527289ad7238bf8f`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-centos`

```console
$ docker pull rethinkdb@sha256:b64ea5554c79140250dcb1b9890a403d81dda0562b8b747a9f8f03507fafa6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull rethinkdb@sha256:2fd3b70663c04a742cb05a38cd006f838dd03f598b53e0905fe416e6ce9c8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4` - linux; amd64

```console
$ docker pull rethinkdb@sha256:d06b5c006ea5bed1913283910e0045f0c2144d0f968fb4b46ccaf0947cb99b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f37e5daf5bdf21d3a3cdd583213b0bb7dabf6dfdcdc12e2231cfc39551af5b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:29:01 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:04 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 12 May 2021 17:29:05 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 12 May 2021 17:29:12 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:12 GMT
VOLUME [/data]
# Wed, 12 May 2021 17:29:12 GMT
WORKDIR /data
# Wed, 12 May 2021 17:29:13 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 12 May 2021 17:29:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b31dbb3d3e7721a2f9cb1ed29dcb1b960873ee852b122ca3cab6e6300154d`  
		Last Modified: Wed, 12 May 2021 17:29:58 GMT  
		Size: 6.7 MB (6690387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5695ae0ed6c7809de5b3cc650a24848ef3ddc7fdd2ee8b43b12255cdf1bd204`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0722ed38c905f6d03f45d75ddf2dd6209c84e9100a8b3e2aed1e9b702dba81`  
		Last Modified: Wed, 12 May 2021 17:29:59 GMT  
		Size: 18.0 MB (17991761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f89003a5ba016395930174176b5e32e83c894225e40329527289ad7238bf8f`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-buster-slim`

```console
$ docker pull rethinkdb@sha256:2fd3b70663c04a742cb05a38cd006f838dd03f598b53e0905fe416e6ce9c8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:d06b5c006ea5bed1913283910e0045f0c2144d0f968fb4b46ccaf0947cb99b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f37e5daf5bdf21d3a3cdd583213b0bb7dabf6dfdcdc12e2231cfc39551af5b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:29:01 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:04 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 12 May 2021 17:29:05 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 12 May 2021 17:29:12 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:12 GMT
VOLUME [/data]
# Wed, 12 May 2021 17:29:12 GMT
WORKDIR /data
# Wed, 12 May 2021 17:29:13 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 12 May 2021 17:29:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b31dbb3d3e7721a2f9cb1ed29dcb1b960873ee852b122ca3cab6e6300154d`  
		Last Modified: Wed, 12 May 2021 17:29:58 GMT  
		Size: 6.7 MB (6690387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5695ae0ed6c7809de5b3cc650a24848ef3ddc7fdd2ee8b43b12255cdf1bd204`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0722ed38c905f6d03f45d75ddf2dd6209c84e9100a8b3e2aed1e9b702dba81`  
		Last Modified: Wed, 12 May 2021 17:29:59 GMT  
		Size: 18.0 MB (17991761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f89003a5ba016395930174176b5e32e83c894225e40329527289ad7238bf8f`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-centos`

```console
$ docker pull rethinkdb@sha256:b64ea5554c79140250dcb1b9890a403d81dda0562b8b747a9f8f03507fafa6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull rethinkdb@sha256:b7f991833ac2e42126c6f8524068fed49437d24c44a1f0f56b2971c9db0afb05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4.0` - linux; amd64

```console
$ docker pull rethinkdb@sha256:e8f63e59970344af9c809076adc84dcaf26afe897b260e905afdd68a4618225e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51831981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe4e32db149c753d82c273cc631ecb9c3ce1dabf9faea3a02f1f4338134ee36d`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:29:01 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:24 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 12 May 2021 17:29:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Wed, 12 May 2021 17:29:31 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:31 GMT
VOLUME [/data]
# Wed, 12 May 2021 17:29:32 GMT
WORKDIR /data
# Wed, 12 May 2021 17:29:32 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 12 May 2021 17:29:32 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b31dbb3d3e7721a2f9cb1ed29dcb1b960873ee852b122ca3cab6e6300154d`  
		Last Modified: Wed, 12 May 2021 17:29:58 GMT  
		Size: 6.7 MB (6690387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab5b1bbff0da5dc7ccaf62cbe1c0ba8d37d2c39f6cff56e32db321d48f1d7d8`  
		Last Modified: Wed, 12 May 2021 17:30:26 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b7f267a8d8b5140d18db76dea9f954b888ab1eea95edddb187252bf336faa`  
		Last Modified: Wed, 12 May 2021 17:30:30 GMT  
		Size: 18.0 MB (17992942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d9960d37f6972cb7a76020daa32e8d0c07d5e99b69f651018987440db2b684`  
		Last Modified: Wed, 12 May 2021 17:30:26 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-buster-slim`

```console
$ docker pull rethinkdb@sha256:b7f991833ac2e42126c6f8524068fed49437d24c44a1f0f56b2971c9db0afb05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4.0-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:e8f63e59970344af9c809076adc84dcaf26afe897b260e905afdd68a4618225e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51831981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe4e32db149c753d82c273cc631ecb9c3ce1dabf9faea3a02f1f4338134ee36d`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:29:01 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:24 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 12 May 2021 17:29:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Wed, 12 May 2021 17:29:31 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:31 GMT
VOLUME [/data]
# Wed, 12 May 2021 17:29:32 GMT
WORKDIR /data
# Wed, 12 May 2021 17:29:32 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 12 May 2021 17:29:32 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b31dbb3d3e7721a2f9cb1ed29dcb1b960873ee852b122ca3cab6e6300154d`  
		Last Modified: Wed, 12 May 2021 17:29:58 GMT  
		Size: 6.7 MB (6690387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab5b1bbff0da5dc7ccaf62cbe1c0ba8d37d2c39f6cff56e32db321d48f1d7d8`  
		Last Modified: Wed, 12 May 2021 17:30:26 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291b7f267a8d8b5140d18db76dea9f954b888ab1eea95edddb187252bf336faa`  
		Last Modified: Wed, 12 May 2021 17:30:30 GMT  
		Size: 18.0 MB (17992942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d9960d37f6972cb7a76020daa32e8d0c07d5e99b69f651018987440db2b684`  
		Last Modified: Wed, 12 May 2021 17:30:26 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-centos`

```console
$ docker pull rethinkdb@sha256:11d9649e49b7e3b68d5d28e3e3959b055a6f7639bab3bc810e8afe96c6e7cc01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull rethinkdb@sha256:2fd3b70663c04a742cb05a38cd006f838dd03f598b53e0905fe416e6ce9c8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4.1` - linux; amd64

```console
$ docker pull rethinkdb@sha256:d06b5c006ea5bed1913283910e0045f0c2144d0f968fb4b46ccaf0947cb99b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f37e5daf5bdf21d3a3cdd583213b0bb7dabf6dfdcdc12e2231cfc39551af5b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:29:01 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:04 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 12 May 2021 17:29:05 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 12 May 2021 17:29:12 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:12 GMT
VOLUME [/data]
# Wed, 12 May 2021 17:29:12 GMT
WORKDIR /data
# Wed, 12 May 2021 17:29:13 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 12 May 2021 17:29:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b31dbb3d3e7721a2f9cb1ed29dcb1b960873ee852b122ca3cab6e6300154d`  
		Last Modified: Wed, 12 May 2021 17:29:58 GMT  
		Size: 6.7 MB (6690387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5695ae0ed6c7809de5b3cc650a24848ef3ddc7fdd2ee8b43b12255cdf1bd204`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0722ed38c905f6d03f45d75ddf2dd6209c84e9100a8b3e2aed1e9b702dba81`  
		Last Modified: Wed, 12 May 2021 17:29:59 GMT  
		Size: 18.0 MB (17991761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f89003a5ba016395930174176b5e32e83c894225e40329527289ad7238bf8f`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1-buster-slim`

```console
$ docker pull rethinkdb@sha256:2fd3b70663c04a742cb05a38cd006f838dd03f598b53e0905fe416e6ce9c8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4.1-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:d06b5c006ea5bed1913283910e0045f0c2144d0f968fb4b46ccaf0947cb99b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f37e5daf5bdf21d3a3cdd583213b0bb7dabf6dfdcdc12e2231cfc39551af5b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:29:01 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:04 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 12 May 2021 17:29:05 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 12 May 2021 17:29:12 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:12 GMT
VOLUME [/data]
# Wed, 12 May 2021 17:29:12 GMT
WORKDIR /data
# Wed, 12 May 2021 17:29:13 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 12 May 2021 17:29:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b31dbb3d3e7721a2f9cb1ed29dcb1b960873ee852b122ca3cab6e6300154d`  
		Last Modified: Wed, 12 May 2021 17:29:58 GMT  
		Size: 6.7 MB (6690387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5695ae0ed6c7809de5b3cc650a24848ef3ddc7fdd2ee8b43b12255cdf1bd204`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0722ed38c905f6d03f45d75ddf2dd6209c84e9100a8b3e2aed1e9b702dba81`  
		Last Modified: Wed, 12 May 2021 17:29:59 GMT  
		Size: 18.0 MB (17991761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f89003a5ba016395930174176b5e32e83c894225e40329527289ad7238bf8f`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1-centos`

```console
$ docker pull rethinkdb@sha256:b64ea5554c79140250dcb1b9890a403d81dda0562b8b747a9f8f03507fafa6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull rethinkdb@sha256:2fd3b70663c04a742cb05a38cd006f838dd03f598b53e0905fe416e6ce9c8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:d06b5c006ea5bed1913283910e0045f0c2144d0f968fb4b46ccaf0947cb99b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f37e5daf5bdf21d3a3cdd583213b0bb7dabf6dfdcdc12e2231cfc39551af5b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:29:01 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:04 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 12 May 2021 17:29:05 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 12 May 2021 17:29:12 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:12 GMT
VOLUME [/data]
# Wed, 12 May 2021 17:29:12 GMT
WORKDIR /data
# Wed, 12 May 2021 17:29:13 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 12 May 2021 17:29:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b31dbb3d3e7721a2f9cb1ed29dcb1b960873ee852b122ca3cab6e6300154d`  
		Last Modified: Wed, 12 May 2021 17:29:58 GMT  
		Size: 6.7 MB (6690387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5695ae0ed6c7809de5b3cc650a24848ef3ddc7fdd2ee8b43b12255cdf1bd204`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0722ed38c905f6d03f45d75ddf2dd6209c84e9100a8b3e2aed1e9b702dba81`  
		Last Modified: Wed, 12 May 2021 17:29:59 GMT  
		Size: 18.0 MB (17991761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f89003a5ba016395930174176b5e32e83c894225e40329527289ad7238bf8f`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:centos`

```console
$ docker pull rethinkdb@sha256:b64ea5554c79140250dcb1b9890a403d81dda0562b8b747a9f8f03507fafa6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull rethinkdb@sha256:2fd3b70663c04a742cb05a38cd006f838dd03f598b53e0905fe416e6ce9c8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:latest` - linux; amd64

```console
$ docker pull rethinkdb@sha256:d06b5c006ea5bed1913283910e0045f0c2144d0f968fb4b46ccaf0947cb99b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f37e5daf5bdf21d3a3cdd583213b0bb7dabf6dfdcdc12e2231cfc39551af5b0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:29:01 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:04 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 12 May 2021 17:29:05 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Wed, 12 May 2021 17:29:12 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:29:12 GMT
VOLUME [/data]
# Wed, 12 May 2021 17:29:12 GMT
WORKDIR /data
# Wed, 12 May 2021 17:29:13 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 12 May 2021 17:29:13 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b31dbb3d3e7721a2f9cb1ed29dcb1b960873ee852b122ca3cab6e6300154d`  
		Last Modified: Wed, 12 May 2021 17:29:58 GMT  
		Size: 6.7 MB (6690387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5695ae0ed6c7809de5b3cc650a24848ef3ddc7fdd2ee8b43b12255cdf1bd204`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0722ed38c905f6d03f45d75ddf2dd6209c84e9100a8b3e2aed1e9b702dba81`  
		Last Modified: Wed, 12 May 2021 17:29:59 GMT  
		Size: 18.0 MB (17991761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f89003a5ba016395930174176b5e32e83c894225e40329527289ad7238bf8f`  
		Last Modified: Wed, 12 May 2021 17:29:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
