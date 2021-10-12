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
$ docker pull rethinkdb@sha256:0dba02987090e751b491d9ebd70890c37690f4eed1b81972f86deea1d7db8c63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:4f8964161ce484c16f65c8c6e206dd758793adf06c53993eac651bdb9c1649ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105945035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76992aa3ff22017132fc0d31a6c2cd470a5d8929b7cd7e71356d4421052abf03`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 19:49:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Wed, 15 Sep 2021 19:49:38 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Wed, 15 Sep 2021 19:49:48 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Wed, 15 Sep 2021 19:49:48 GMT
VOLUME [/data]
# Wed, 15 Sep 2021 19:49:49 GMT
WORKDIR /data
# Wed, 15 Sep 2021 19:49:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 15 Sep 2021 19:49:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14535878a922d6f2b6784f3df0b1171a760b89f733accf8864763f80ce565fc`  
		Last Modified: Wed, 15 Sep 2021 19:50:34 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83765c84b45bb249242f550b991fa45fdc0417c90860657ca7a763a28f23d652`  
		Last Modified: Wed, 15 Sep 2021 19:50:39 GMT  
		Size: 22.4 MB (22426554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee5a6d0670eea07ae2e798a19685994d7486109329162bdcdbc1da3b739967e`  
		Last Modified: Wed, 15 Sep 2021 19:50:34 GMT  
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
$ docker pull rethinkdb@sha256:0dba02987090e751b491d9ebd70890c37690f4eed1b81972f86deea1d7db8c63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:4f8964161ce484c16f65c8c6e206dd758793adf06c53993eac651bdb9c1649ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105945035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76992aa3ff22017132fc0d31a6c2cd470a5d8929b7cd7e71356d4421052abf03`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 19:49:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Wed, 15 Sep 2021 19:49:38 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Wed, 15 Sep 2021 19:49:48 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Wed, 15 Sep 2021 19:49:48 GMT
VOLUME [/data]
# Wed, 15 Sep 2021 19:49:49 GMT
WORKDIR /data
# Wed, 15 Sep 2021 19:49:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 15 Sep 2021 19:49:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14535878a922d6f2b6784f3df0b1171a760b89f733accf8864763f80ce565fc`  
		Last Modified: Wed, 15 Sep 2021 19:50:34 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83765c84b45bb249242f550b991fa45fdc0417c90860657ca7a763a28f23d652`  
		Last Modified: Wed, 15 Sep 2021 19:50:39 GMT  
		Size: 22.4 MB (22426554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee5a6d0670eea07ae2e798a19685994d7486109329162bdcdbc1da3b739967e`  
		Last Modified: Wed, 15 Sep 2021 19:50:34 GMT  
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
$ docker pull rethinkdb@sha256:127baddfaa5980d32d72b1a183b099c5fc09f6850f885a07a66f5aff9dfc94cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4.0-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:2f1d63134244dce7a18047fc9c336f030018106de165f20cb96b056fe15932d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105953941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09bfa082b6e23579424f3636f1834d60760851cc31e2ad3a83341f4ede584925`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 19:50:11 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0
# Wed, 15 Sep 2021 19:50:12 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Wed, 15 Sep 2021 19:50:21 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Wed, 15 Sep 2021 19:50:21 GMT
VOLUME [/data]
# Wed, 15 Sep 2021 19:50:21 GMT
WORKDIR /data
# Wed, 15 Sep 2021 19:50:21 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 15 Sep 2021 19:50:22 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a1f1af6786baf62588680bf55b34e33915e42145ba9f756d8e4500a6a9b8fd`  
		Last Modified: Wed, 15 Sep 2021 19:50:54 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a986b4447aa452122bf1f57003844972c0d061ef017a8031fd2729663065a7d`  
		Last Modified: Wed, 15 Sep 2021 19:50:57 GMT  
		Size: 22.4 MB (22435460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da5fd37ada27938e8214f8bcb8cd867404c2cc05616094e992032cd96042ee0`  
		Last Modified: Wed, 15 Sep 2021 19:50:54 GMT  
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
$ docker pull rethinkdb@sha256:0dba02987090e751b491d9ebd70890c37690f4eed1b81972f86deea1d7db8c63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4.1-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:4f8964161ce484c16f65c8c6e206dd758793adf06c53993eac651bdb9c1649ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105945035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76992aa3ff22017132fc0d31a6c2cd470a5d8929b7cd7e71356d4421052abf03`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 19:49:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Wed, 15 Sep 2021 19:49:38 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Wed, 15 Sep 2021 19:49:48 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Wed, 15 Sep 2021 19:49:48 GMT
VOLUME [/data]
# Wed, 15 Sep 2021 19:49:49 GMT
WORKDIR /data
# Wed, 15 Sep 2021 19:49:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 15 Sep 2021 19:49:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14535878a922d6f2b6784f3df0b1171a760b89f733accf8864763f80ce565fc`  
		Last Modified: Wed, 15 Sep 2021 19:50:34 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83765c84b45bb249242f550b991fa45fdc0417c90860657ca7a763a28f23d652`  
		Last Modified: Wed, 15 Sep 2021 19:50:39 GMT  
		Size: 22.4 MB (22426554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee5a6d0670eea07ae2e798a19685994d7486109329162bdcdbc1da3b739967e`  
		Last Modified: Wed, 15 Sep 2021 19:50:34 GMT  
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
$ docker pull rethinkdb@sha256:0dba02987090e751b491d9ebd70890c37690f4eed1b81972f86deea1d7db8c63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:4f8964161ce484c16f65c8c6e206dd758793adf06c53993eac651bdb9c1649ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105945035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76992aa3ff22017132fc0d31a6c2cd470a5d8929b7cd7e71356d4421052abf03`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 19:49:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1
# Wed, 15 Sep 2021 19:49:38 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Wed, 15 Sep 2021 19:49:48 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Wed, 15 Sep 2021 19:49:48 GMT
VOLUME [/data]
# Wed, 15 Sep 2021 19:49:49 GMT
WORKDIR /data
# Wed, 15 Sep 2021 19:49:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 15 Sep 2021 19:49:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14535878a922d6f2b6784f3df0b1171a760b89f733accf8864763f80ce565fc`  
		Last Modified: Wed, 15 Sep 2021 19:50:34 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83765c84b45bb249242f550b991fa45fdc0417c90860657ca7a763a28f23d652`  
		Last Modified: Wed, 15 Sep 2021 19:50:39 GMT  
		Size: 22.4 MB (22426554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee5a6d0670eea07ae2e798a19685994d7486109329162bdcdbc1da3b739967e`  
		Last Modified: Wed, 15 Sep 2021 19:50:34 GMT  
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
