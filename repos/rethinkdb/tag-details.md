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
$ docker pull rethinkdb@sha256:a8fffec3603d1e783241621f7d4c38a832c3d8c72b864fdf53a16832f36f923b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2` - linux; amd64

```console
$ docker pull rethinkdb@sha256:89ba9d77b9679711ea2fbe2477559928cd797abe9d254277bb6ef174f8d06522
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51770925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306135cbdefaca7b1cca2add3b26c78860c574bcc1987854d9d555037bac689`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 18:51:56 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:00 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 12 Jan 2021 18:52:00 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 12 Jan 2021 18:52:09 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:10 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 18:52:10 GMT
WORKDIR /data
# Tue, 12 Jan 2021 18:52:10 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 12 Jan 2021 18:52:10 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742cc0ee20ecb3c5f1baf61e368bb7680f504920f45e94feb08c039083721630`  
		Last Modified: Tue, 12 Jan 2021 18:53:03 GMT  
		Size: 6.7 MB (6669370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2d02d25f25a0e5dfc4612ac26de45286ae76de0b2af90e673cd3ea90f7ca9`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c448e71024af56b5a9295387b2361b8fcc53ec2c6d216698b1d91fa89dfe6cb1`  
		Last Modified: Tue, 12 Jan 2021 18:53:05 GMT  
		Size: 18.0 MB (17990781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8882dba2ce6aabd7c249d1a05395fbf06f39877174db31da4073707a735e02b3`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4`

```console
$ docker pull rethinkdb@sha256:a8fffec3603d1e783241621f7d4c38a832c3d8c72b864fdf53a16832f36f923b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4` - linux; amd64

```console
$ docker pull rethinkdb@sha256:89ba9d77b9679711ea2fbe2477559928cd797abe9d254277bb6ef174f8d06522
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51770925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306135cbdefaca7b1cca2add3b26c78860c574bcc1987854d9d555037bac689`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 18:51:56 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:00 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 12 Jan 2021 18:52:00 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 12 Jan 2021 18:52:09 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:10 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 18:52:10 GMT
WORKDIR /data
# Tue, 12 Jan 2021 18:52:10 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 12 Jan 2021 18:52:10 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742cc0ee20ecb3c5f1baf61e368bb7680f504920f45e94feb08c039083721630`  
		Last Modified: Tue, 12 Jan 2021 18:53:03 GMT  
		Size: 6.7 MB (6669370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2d02d25f25a0e5dfc4612ac26de45286ae76de0b2af90e673cd3ea90f7ca9`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c448e71024af56b5a9295387b2361b8fcc53ec2c6d216698b1d91fa89dfe6cb1`  
		Last Modified: Tue, 12 Jan 2021 18:53:05 GMT  
		Size: 18.0 MB (17990781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8882dba2ce6aabd7c249d1a05395fbf06f39877174db31da4073707a735e02b3`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0`

```console
$ docker pull rethinkdb@sha256:c115a65b49aaf27638807bef351f89fcb58b94934a47588bfafe3e2849b6dd36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0` - linux; amd64

```console
$ docker pull rethinkdb@sha256:d805a677d44aafdcc935ecd551994d99ddb6cb6222edddd061c365360ff3764b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51772287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b77b60d7e89b561a9b0340f59d072850cc93001f89818d598498f754a63d562`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 18:51:56 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:22 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 12 Jan 2021 18:52:22 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Tue, 12 Jan 2021 18:52:31 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:31 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 18:52:32 GMT
WORKDIR /data
# Tue, 12 Jan 2021 18:52:32 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 12 Jan 2021 18:52:32 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742cc0ee20ecb3c5f1baf61e368bb7680f504920f45e94feb08c039083721630`  
		Last Modified: Tue, 12 Jan 2021 18:53:03 GMT  
		Size: 6.7 MB (6669370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752c5113305a2acacf5c29ba36468f410174c89134e61e4858a1a867ce3df315`  
		Last Modified: Tue, 12 Jan 2021 18:53:22 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc63f93b76e34c54c37a73d50aba1a330309f2a8ba27cf3d54b0cc033838d87`  
		Last Modified: Tue, 12 Jan 2021 18:53:25 GMT  
		Size: 18.0 MB (17992144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73314e21afadc54582fe1ae934bb6a9120efdbb93d25bae033174eca90b7c458`  
		Last Modified: Tue, 12 Jan 2021 18:53:22 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-buster-slim`

```console
$ docker pull rethinkdb@sha256:c115a65b49aaf27638807bef351f89fcb58b94934a47588bfafe3e2849b6dd36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:d805a677d44aafdcc935ecd551994d99ddb6cb6222edddd061c365360ff3764b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51772287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b77b60d7e89b561a9b0340f59d072850cc93001f89818d598498f754a63d562`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 18:51:56 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:22 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 12 Jan 2021 18:52:22 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Tue, 12 Jan 2021 18:52:31 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:31 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 18:52:32 GMT
WORKDIR /data
# Tue, 12 Jan 2021 18:52:32 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 12 Jan 2021 18:52:32 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742cc0ee20ecb3c5f1baf61e368bb7680f504920f45e94feb08c039083721630`  
		Last Modified: Tue, 12 Jan 2021 18:53:03 GMT  
		Size: 6.7 MB (6669370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752c5113305a2acacf5c29ba36468f410174c89134e61e4858a1a867ce3df315`  
		Last Modified: Tue, 12 Jan 2021 18:53:22 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc63f93b76e34c54c37a73d50aba1a330309f2a8ba27cf3d54b0cc033838d87`  
		Last Modified: Tue, 12 Jan 2021 18:53:25 GMT  
		Size: 18.0 MB (17992144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73314e21afadc54582fe1ae934bb6a9120efdbb93d25bae033174eca90b7c458`  
		Last Modified: Tue, 12 Jan 2021 18:53:22 GMT  
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
$ docker pull rethinkdb@sha256:a8fffec3603d1e783241621f7d4c38a832c3d8c72b864fdf53a16832f36f923b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1` - linux; amd64

```console
$ docker pull rethinkdb@sha256:89ba9d77b9679711ea2fbe2477559928cd797abe9d254277bb6ef174f8d06522
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51770925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306135cbdefaca7b1cca2add3b26c78860c574bcc1987854d9d555037bac689`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 18:51:56 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:00 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 12 Jan 2021 18:52:00 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 12 Jan 2021 18:52:09 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:10 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 18:52:10 GMT
WORKDIR /data
# Tue, 12 Jan 2021 18:52:10 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 12 Jan 2021 18:52:10 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742cc0ee20ecb3c5f1baf61e368bb7680f504920f45e94feb08c039083721630`  
		Last Modified: Tue, 12 Jan 2021 18:53:03 GMT  
		Size: 6.7 MB (6669370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2d02d25f25a0e5dfc4612ac26de45286ae76de0b2af90e673cd3ea90f7ca9`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c448e71024af56b5a9295387b2361b8fcc53ec2c6d216698b1d91fa89dfe6cb1`  
		Last Modified: Tue, 12 Jan 2021 18:53:05 GMT  
		Size: 18.0 MB (17990781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8882dba2ce6aabd7c249d1a05395fbf06f39877174db31da4073707a735e02b3`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.1-buster-slim`

```console
$ docker pull rethinkdb@sha256:a8fffec3603d1e783241621f7d4c38a832c3d8c72b864fdf53a16832f36f923b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.1-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:89ba9d77b9679711ea2fbe2477559928cd797abe9d254277bb6ef174f8d06522
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51770925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306135cbdefaca7b1cca2add3b26c78860c574bcc1987854d9d555037bac689`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 18:51:56 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:00 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 12 Jan 2021 18:52:00 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 12 Jan 2021 18:52:09 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:10 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 18:52:10 GMT
WORKDIR /data
# Tue, 12 Jan 2021 18:52:10 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 12 Jan 2021 18:52:10 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742cc0ee20ecb3c5f1baf61e368bb7680f504920f45e94feb08c039083721630`  
		Last Modified: Tue, 12 Jan 2021 18:53:03 GMT  
		Size: 6.7 MB (6669370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2d02d25f25a0e5dfc4612ac26de45286ae76de0b2af90e673cd3ea90f7ca9`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c448e71024af56b5a9295387b2361b8fcc53ec2c6d216698b1d91fa89dfe6cb1`  
		Last Modified: Tue, 12 Jan 2021 18:53:05 GMT  
		Size: 18.0 MB (17990781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8882dba2ce6aabd7c249d1a05395fbf06f39877174db31da4073707a735e02b3`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
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
$ docker pull rethinkdb@sha256:a8fffec3603d1e783241621f7d4c38a832c3d8c72b864fdf53a16832f36f923b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:89ba9d77b9679711ea2fbe2477559928cd797abe9d254277bb6ef174f8d06522
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51770925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306135cbdefaca7b1cca2add3b26c78860c574bcc1987854d9d555037bac689`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 18:51:56 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:00 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 12 Jan 2021 18:52:00 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 12 Jan 2021 18:52:09 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:10 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 18:52:10 GMT
WORKDIR /data
# Tue, 12 Jan 2021 18:52:10 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 12 Jan 2021 18:52:10 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742cc0ee20ecb3c5f1baf61e368bb7680f504920f45e94feb08c039083721630`  
		Last Modified: Tue, 12 Jan 2021 18:53:03 GMT  
		Size: 6.7 MB (6669370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2d02d25f25a0e5dfc4612ac26de45286ae76de0b2af90e673cd3ea90f7ca9`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c448e71024af56b5a9295387b2361b8fcc53ec2c6d216698b1d91fa89dfe6cb1`  
		Last Modified: Tue, 12 Jan 2021 18:53:05 GMT  
		Size: 18.0 MB (17990781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8882dba2ce6aabd7c249d1a05395fbf06f39877174db31da4073707a735e02b3`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
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
$ docker pull rethinkdb@sha256:a8fffec3603d1e783241621f7d4c38a832c3d8c72b864fdf53a16832f36f923b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:89ba9d77b9679711ea2fbe2477559928cd797abe9d254277bb6ef174f8d06522
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51770925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306135cbdefaca7b1cca2add3b26c78860c574bcc1987854d9d555037bac689`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 18:51:56 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:00 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 12 Jan 2021 18:52:00 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 12 Jan 2021 18:52:09 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:10 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 18:52:10 GMT
WORKDIR /data
# Tue, 12 Jan 2021 18:52:10 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 12 Jan 2021 18:52:10 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742cc0ee20ecb3c5f1baf61e368bb7680f504920f45e94feb08c039083721630`  
		Last Modified: Tue, 12 Jan 2021 18:53:03 GMT  
		Size: 6.7 MB (6669370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2d02d25f25a0e5dfc4612ac26de45286ae76de0b2af90e673cd3ea90f7ca9`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c448e71024af56b5a9295387b2361b8fcc53ec2c6d216698b1d91fa89dfe6cb1`  
		Last Modified: Tue, 12 Jan 2021 18:53:05 GMT  
		Size: 18.0 MB (17990781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8882dba2ce6aabd7c249d1a05395fbf06f39877174db31da4073707a735e02b3`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
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
$ docker pull rethinkdb@sha256:a8fffec3603d1e783241621f7d4c38a832c3d8c72b864fdf53a16832f36f923b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:89ba9d77b9679711ea2fbe2477559928cd797abe9d254277bb6ef174f8d06522
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51770925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306135cbdefaca7b1cca2add3b26c78860c574bcc1987854d9d555037bac689`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 18:51:56 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:00 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 12 Jan 2021 18:52:00 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 12 Jan 2021 18:52:09 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:10 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 18:52:10 GMT
WORKDIR /data
# Tue, 12 Jan 2021 18:52:10 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 12 Jan 2021 18:52:10 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742cc0ee20ecb3c5f1baf61e368bb7680f504920f45e94feb08c039083721630`  
		Last Modified: Tue, 12 Jan 2021 18:53:03 GMT  
		Size: 6.7 MB (6669370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2d02d25f25a0e5dfc4612ac26de45286ae76de0b2af90e673cd3ea90f7ca9`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c448e71024af56b5a9295387b2361b8fcc53ec2c6d216698b1d91fa89dfe6cb1`  
		Last Modified: Tue, 12 Jan 2021 18:53:05 GMT  
		Size: 18.0 MB (17990781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8882dba2ce6aabd7c249d1a05395fbf06f39877174db31da4073707a735e02b3`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
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
$ docker pull rethinkdb@sha256:a8fffec3603d1e783241621f7d4c38a832c3d8c72b864fdf53a16832f36f923b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:latest` - linux; amd64

```console
$ docker pull rethinkdb@sha256:89ba9d77b9679711ea2fbe2477559928cd797abe9d254277bb6ef174f8d06522
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51770925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2306135cbdefaca7b1cca2add3b26c78860c574bcc1987854d9d555037bac689`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 18:51:56 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:00 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A3A8C6692E6E3F69B3FE81D85E93F801BB43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 12 Jan 2021 18:52:00 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.1~0buster
# Tue, 12 Jan 2021 18:52:09 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 18:52:10 GMT
VOLUME [/data]
# Tue, 12 Jan 2021 18:52:10 GMT
WORKDIR /data
# Tue, 12 Jan 2021 18:52:10 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 12 Jan 2021 18:52:10 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742cc0ee20ecb3c5f1baf61e368bb7680f504920f45e94feb08c039083721630`  
		Last Modified: Tue, 12 Jan 2021 18:53:03 GMT  
		Size: 6.7 MB (6669370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2d02d25f25a0e5dfc4612ac26de45286ae76de0b2af90e673cd3ea90f7ca9`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 2.6 KB (2612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c448e71024af56b5a9295387b2361b8fcc53ec2c6d216698b1d91fa89dfe6cb1`  
		Last Modified: Tue, 12 Jan 2021 18:53:05 GMT  
		Size: 18.0 MB (17990781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8882dba2ce6aabd7c249d1a05395fbf06f39877174db31da4073707a735e02b3`  
		Last Modified: Tue, 12 Jan 2021 18:53:01 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
