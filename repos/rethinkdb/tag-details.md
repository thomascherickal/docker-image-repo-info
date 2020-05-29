<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rethinkdb`

-	[`rethinkdb:2`](#rethinkdb2)
-	[`rethinkdb:2.4`](#rethinkdb24)
-	[`rethinkdb:2.4.0`](#rethinkdb240)
-	[`rethinkdb:2.4.0-buster-slim`](#rethinkdb240-buster-slim)
-	[`rethinkdb:2.4.0-centos`](#rethinkdb240-centos)
-	[`rethinkdb:2.4-buster-slim`](#rethinkdb24-buster-slim)
-	[`rethinkdb:2.4-centos`](#rethinkdb24-centos)
-	[`rethinkdb:2-buster-slim`](#rethinkdb2-buster-slim)
-	[`rethinkdb:2-centos`](#rethinkdb2-centos)
-	[`rethinkdb:buster-slim`](#rethinkdbbuster-slim)
-	[`rethinkdb:centos`](#rethinkdbcentos)
-	[`rethinkdb:latest`](#rethinkdblatest)

## `rethinkdb:2`

```console
$ docker pull rethinkdb@sha256:63bdac5aa30ea52505f4baf8ee0c8b26e12d460cbf603ec6904fa9ab60a8aa81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2` - linux; amd64

```console
$ docker pull rethinkdb@sha256:63487ef450fe9a6619e215461fa5f6c97fb329b3577dd3aab6b914bd75eaa19f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51763334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ccb19f89ce22f0fe7e41c57f2287d1a57513136fa36f5b75abaedd6572e0b2f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 29 May 2020 21:20:36 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 29 May 2020 21:20:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Fri, 29 May 2020 21:20:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:46 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:20:46 GMT
WORKDIR /data
# Fri, 29 May 2020 21:20:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:20:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bbb42f3811a4c02b1c4215f0931baa5e7fd47f7fee958f5a6df4eaf484b513`  
		Last Modified: Fri, 29 May 2020 21:21:15 GMT  
		Size: 6.7 MB (6669801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e549bc572ab8ed4af16254f062de89f9a16ad863d45cc0d7376fa281f371aef`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82a54f8493424eb4636699476754b60fd40544d6c4a0be22d9d98201ec6a492`  
		Last Modified: Fri, 29 May 2020 21:21:19 GMT  
		Size: 18.0 MB (17992073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db2f23689c74580c5a35e7baae3f5a2734bb5650037e85252f8e46dfadbc66e`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4`

```console
$ docker pull rethinkdb@sha256:63bdac5aa30ea52505f4baf8ee0c8b26e12d460cbf603ec6904fa9ab60a8aa81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4` - linux; amd64

```console
$ docker pull rethinkdb@sha256:63487ef450fe9a6619e215461fa5f6c97fb329b3577dd3aab6b914bd75eaa19f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51763334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ccb19f89ce22f0fe7e41c57f2287d1a57513136fa36f5b75abaedd6572e0b2f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 29 May 2020 21:20:36 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 29 May 2020 21:20:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Fri, 29 May 2020 21:20:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:46 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:20:46 GMT
WORKDIR /data
# Fri, 29 May 2020 21:20:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:20:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bbb42f3811a4c02b1c4215f0931baa5e7fd47f7fee958f5a6df4eaf484b513`  
		Last Modified: Fri, 29 May 2020 21:21:15 GMT  
		Size: 6.7 MB (6669801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e549bc572ab8ed4af16254f062de89f9a16ad863d45cc0d7376fa281f371aef`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82a54f8493424eb4636699476754b60fd40544d6c4a0be22d9d98201ec6a492`  
		Last Modified: Fri, 29 May 2020 21:21:19 GMT  
		Size: 18.0 MB (17992073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db2f23689c74580c5a35e7baae3f5a2734bb5650037e85252f8e46dfadbc66e`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0`

```console
$ docker pull rethinkdb@sha256:63bdac5aa30ea52505f4baf8ee0c8b26e12d460cbf603ec6904fa9ab60a8aa81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0` - linux; amd64

```console
$ docker pull rethinkdb@sha256:63487ef450fe9a6619e215461fa5f6c97fb329b3577dd3aab6b914bd75eaa19f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51763334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ccb19f89ce22f0fe7e41c57f2287d1a57513136fa36f5b75abaedd6572e0b2f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 29 May 2020 21:20:36 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 29 May 2020 21:20:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Fri, 29 May 2020 21:20:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:46 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:20:46 GMT
WORKDIR /data
# Fri, 29 May 2020 21:20:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:20:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bbb42f3811a4c02b1c4215f0931baa5e7fd47f7fee958f5a6df4eaf484b513`  
		Last Modified: Fri, 29 May 2020 21:21:15 GMT  
		Size: 6.7 MB (6669801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e549bc572ab8ed4af16254f062de89f9a16ad863d45cc0d7376fa281f371aef`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82a54f8493424eb4636699476754b60fd40544d6c4a0be22d9d98201ec6a492`  
		Last Modified: Fri, 29 May 2020 21:21:19 GMT  
		Size: 18.0 MB (17992073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db2f23689c74580c5a35e7baae3f5a2734bb5650037e85252f8e46dfadbc66e`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-buster-slim`

```console
$ docker pull rethinkdb@sha256:63bdac5aa30ea52505f4baf8ee0c8b26e12d460cbf603ec6904fa9ab60a8aa81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:63487ef450fe9a6619e215461fa5f6c97fb329b3577dd3aab6b914bd75eaa19f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51763334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ccb19f89ce22f0fe7e41c57f2287d1a57513136fa36f5b75abaedd6572e0b2f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 29 May 2020 21:20:36 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 29 May 2020 21:20:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Fri, 29 May 2020 21:20:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:46 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:20:46 GMT
WORKDIR /data
# Fri, 29 May 2020 21:20:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:20:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bbb42f3811a4c02b1c4215f0931baa5e7fd47f7fee958f5a6df4eaf484b513`  
		Last Modified: Fri, 29 May 2020 21:21:15 GMT  
		Size: 6.7 MB (6669801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e549bc572ab8ed4af16254f062de89f9a16ad863d45cc0d7376fa281f371aef`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82a54f8493424eb4636699476754b60fd40544d6c4a0be22d9d98201ec6a492`  
		Last Modified: Fri, 29 May 2020 21:21:19 GMT  
		Size: 18.0 MB (17992073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db2f23689c74580c5a35e7baae3f5a2734bb5650037e85252f8e46dfadbc66e`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.0-centos`

```console
$ docker pull rethinkdb@sha256:337f58133036b1801a3a7d89bdc95e6834412fb9880ada8c0fee4c77fa715202
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4.0-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:bc4ee01c40db894fa929843c6280fb3a88ef1caef3cb5065fb5170f5e2e803e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95607040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91b14dfd2a34098405da55563bbe36675c5c7f603c1ad7fb5e493ddd0678ed`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 15 Jan 2020 01:19:50 GMT
ADD file:aa54047c80ba30064fe59adf4c978a929f38480be77af9ac644074bd5288ef18 in / 
# Sat, 18 Jan 2020 00:26:46 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200114 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-01-14 00:00:00-08:00
# Sat, 18 Jan 2020 00:26:46 GMT
CMD ["/bin/bash"]
# Fri, 29 May 2020 21:20:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0
# Fri, 29 May 2020 21:20:53 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 29 May 2020 21:21:03 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 29 May 2020 21:21:03 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:21:03 GMT
WORKDIR /data
# Fri, 29 May 2020 21:21:03 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:21:04 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:8a29a15cefaeccf6545f7ecf11298f9672d2f0cdaf9e357a95133ac3ad3e1f07`  
		Last Modified: Wed, 15 Jan 2020 01:22:13 GMT  
		Size: 73.2 MB (73228446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ed52937dd359254212cec2ba560de303b45166cf96a4a59cf855672ffb8ae`  
		Last Modified: Fri, 29 May 2020 21:21:26 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5334e1e32012e4ef609fb934b7f8787325c38faf02a52b8dd225f98ccb3e19be`  
		Last Modified: Fri, 29 May 2020 21:21:29 GMT  
		Size: 22.4 MB (22378234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb6c71258fb5509731722064a7e271e891874f38c2f91c87e78614fb1b7e164`  
		Last Modified: Fri, 29 May 2020 21:21:26 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-buster-slim`

```console
$ docker pull rethinkdb@sha256:63bdac5aa30ea52505f4baf8ee0c8b26e12d460cbf603ec6904fa9ab60a8aa81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:63487ef450fe9a6619e215461fa5f6c97fb329b3577dd3aab6b914bd75eaa19f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51763334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ccb19f89ce22f0fe7e41c57f2287d1a57513136fa36f5b75abaedd6572e0b2f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 29 May 2020 21:20:36 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 29 May 2020 21:20:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Fri, 29 May 2020 21:20:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:46 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:20:46 GMT
WORKDIR /data
# Fri, 29 May 2020 21:20:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:20:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bbb42f3811a4c02b1c4215f0931baa5e7fd47f7fee958f5a6df4eaf484b513`  
		Last Modified: Fri, 29 May 2020 21:21:15 GMT  
		Size: 6.7 MB (6669801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e549bc572ab8ed4af16254f062de89f9a16ad863d45cc0d7376fa281f371aef`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82a54f8493424eb4636699476754b60fd40544d6c4a0be22d9d98201ec6a492`  
		Last Modified: Fri, 29 May 2020 21:21:19 GMT  
		Size: 18.0 MB (17992073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db2f23689c74580c5a35e7baae3f5a2734bb5650037e85252f8e46dfadbc66e`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-centos`

```console
$ docker pull rethinkdb@sha256:337f58133036b1801a3a7d89bdc95e6834412fb9880ada8c0fee4c77fa715202
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2.4-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:bc4ee01c40db894fa929843c6280fb3a88ef1caef3cb5065fb5170f5e2e803e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95607040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91b14dfd2a34098405da55563bbe36675c5c7f603c1ad7fb5e493ddd0678ed`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 15 Jan 2020 01:19:50 GMT
ADD file:aa54047c80ba30064fe59adf4c978a929f38480be77af9ac644074bd5288ef18 in / 
# Sat, 18 Jan 2020 00:26:46 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200114 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-01-14 00:00:00-08:00
# Sat, 18 Jan 2020 00:26:46 GMT
CMD ["/bin/bash"]
# Fri, 29 May 2020 21:20:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0
# Fri, 29 May 2020 21:20:53 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 29 May 2020 21:21:03 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 29 May 2020 21:21:03 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:21:03 GMT
WORKDIR /data
# Fri, 29 May 2020 21:21:03 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:21:04 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:8a29a15cefaeccf6545f7ecf11298f9672d2f0cdaf9e357a95133ac3ad3e1f07`  
		Last Modified: Wed, 15 Jan 2020 01:22:13 GMT  
		Size: 73.2 MB (73228446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ed52937dd359254212cec2ba560de303b45166cf96a4a59cf855672ffb8ae`  
		Last Modified: Fri, 29 May 2020 21:21:26 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5334e1e32012e4ef609fb934b7f8787325c38faf02a52b8dd225f98ccb3e19be`  
		Last Modified: Fri, 29 May 2020 21:21:29 GMT  
		Size: 22.4 MB (22378234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb6c71258fb5509731722064a7e271e891874f38c2f91c87e78614fb1b7e164`  
		Last Modified: Fri, 29 May 2020 21:21:26 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-buster-slim`

```console
$ docker pull rethinkdb@sha256:63bdac5aa30ea52505f4baf8ee0c8b26e12d460cbf603ec6904fa9ab60a8aa81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:63487ef450fe9a6619e215461fa5f6c97fb329b3577dd3aab6b914bd75eaa19f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51763334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ccb19f89ce22f0fe7e41c57f2287d1a57513136fa36f5b75abaedd6572e0b2f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 29 May 2020 21:20:36 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 29 May 2020 21:20:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Fri, 29 May 2020 21:20:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:46 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:20:46 GMT
WORKDIR /data
# Fri, 29 May 2020 21:20:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:20:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bbb42f3811a4c02b1c4215f0931baa5e7fd47f7fee958f5a6df4eaf484b513`  
		Last Modified: Fri, 29 May 2020 21:21:15 GMT  
		Size: 6.7 MB (6669801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e549bc572ab8ed4af16254f062de89f9a16ad863d45cc0d7376fa281f371aef`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82a54f8493424eb4636699476754b60fd40544d6c4a0be22d9d98201ec6a492`  
		Last Modified: Fri, 29 May 2020 21:21:19 GMT  
		Size: 18.0 MB (17992073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db2f23689c74580c5a35e7baae3f5a2734bb5650037e85252f8e46dfadbc66e`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-centos`

```console
$ docker pull rethinkdb@sha256:337f58133036b1801a3a7d89bdc95e6834412fb9880ada8c0fee4c77fa715202
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:bc4ee01c40db894fa929843c6280fb3a88ef1caef3cb5065fb5170f5e2e803e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95607040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91b14dfd2a34098405da55563bbe36675c5c7f603c1ad7fb5e493ddd0678ed`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 15 Jan 2020 01:19:50 GMT
ADD file:aa54047c80ba30064fe59adf4c978a929f38480be77af9ac644074bd5288ef18 in / 
# Sat, 18 Jan 2020 00:26:46 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200114 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-01-14 00:00:00-08:00
# Sat, 18 Jan 2020 00:26:46 GMT
CMD ["/bin/bash"]
# Fri, 29 May 2020 21:20:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0
# Fri, 29 May 2020 21:20:53 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 29 May 2020 21:21:03 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 29 May 2020 21:21:03 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:21:03 GMT
WORKDIR /data
# Fri, 29 May 2020 21:21:03 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:21:04 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:8a29a15cefaeccf6545f7ecf11298f9672d2f0cdaf9e357a95133ac3ad3e1f07`  
		Last Modified: Wed, 15 Jan 2020 01:22:13 GMT  
		Size: 73.2 MB (73228446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ed52937dd359254212cec2ba560de303b45166cf96a4a59cf855672ffb8ae`  
		Last Modified: Fri, 29 May 2020 21:21:26 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5334e1e32012e4ef609fb934b7f8787325c38faf02a52b8dd225f98ccb3e19be`  
		Last Modified: Fri, 29 May 2020 21:21:29 GMT  
		Size: 22.4 MB (22378234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb6c71258fb5509731722064a7e271e891874f38c2f91c87e78614fb1b7e164`  
		Last Modified: Fri, 29 May 2020 21:21:26 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:buster-slim`

```console
$ docker pull rethinkdb@sha256:63bdac5aa30ea52505f4baf8ee0c8b26e12d460cbf603ec6904fa9ab60a8aa81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:buster-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:63487ef450fe9a6619e215461fa5f6c97fb329b3577dd3aab6b914bd75eaa19f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51763334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ccb19f89ce22f0fe7e41c57f2287d1a57513136fa36f5b75abaedd6572e0b2f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 29 May 2020 21:20:36 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 29 May 2020 21:20:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Fri, 29 May 2020 21:20:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:46 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:20:46 GMT
WORKDIR /data
# Fri, 29 May 2020 21:20:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:20:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bbb42f3811a4c02b1c4215f0931baa5e7fd47f7fee958f5a6df4eaf484b513`  
		Last Modified: Fri, 29 May 2020 21:21:15 GMT  
		Size: 6.7 MB (6669801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e549bc572ab8ed4af16254f062de89f9a16ad863d45cc0d7376fa281f371aef`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82a54f8493424eb4636699476754b60fd40544d6c4a0be22d9d98201ec6a492`  
		Last Modified: Fri, 29 May 2020 21:21:19 GMT  
		Size: 18.0 MB (17992073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db2f23689c74580c5a35e7baae3f5a2734bb5650037e85252f8e46dfadbc66e`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:centos`

```console
$ docker pull rethinkdb@sha256:337f58133036b1801a3a7d89bdc95e6834412fb9880ada8c0fee4c77fa715202
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:bc4ee01c40db894fa929843c6280fb3a88ef1caef3cb5065fb5170f5e2e803e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95607040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91b14dfd2a34098405da55563bbe36675c5c7f603c1ad7fb5e493ddd0678ed`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 15 Jan 2020 01:19:50 GMT
ADD file:aa54047c80ba30064fe59adf4c978a929f38480be77af9ac644074bd5288ef18 in / 
# Sat, 18 Jan 2020 00:26:46 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200114 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-01-14 00:00:00-08:00
# Sat, 18 Jan 2020 00:26:46 GMT
CMD ["/bin/bash"]
# Fri, 29 May 2020 21:20:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0
# Fri, 29 May 2020 21:20:53 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 29 May 2020 21:21:03 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 29 May 2020 21:21:03 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:21:03 GMT
WORKDIR /data
# Fri, 29 May 2020 21:21:03 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:21:04 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:8a29a15cefaeccf6545f7ecf11298f9672d2f0cdaf9e357a95133ac3ad3e1f07`  
		Last Modified: Wed, 15 Jan 2020 01:22:13 GMT  
		Size: 73.2 MB (73228446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ed52937dd359254212cec2ba560de303b45166cf96a4a59cf855672ffb8ae`  
		Last Modified: Fri, 29 May 2020 21:21:26 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5334e1e32012e4ef609fb934b7f8787325c38faf02a52b8dd225f98ccb3e19be`  
		Last Modified: Fri, 29 May 2020 21:21:29 GMT  
		Size: 22.4 MB (22378234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb6c71258fb5509731722064a7e271e891874f38c2f91c87e78614fb1b7e164`  
		Last Modified: Fri, 29 May 2020 21:21:26 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:latest`

```console
$ docker pull rethinkdb@sha256:63bdac5aa30ea52505f4baf8ee0c8b26e12d460cbf603ec6904fa9ab60a8aa81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:latest` - linux; amd64

```console
$ docker pull rethinkdb@sha256:63487ef450fe9a6619e215461fa5f6c97fb329b3577dd3aab6b914bd75eaa19f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51763334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ccb19f89ce22f0fe7e41c57f2287d1a57513136fa36f5b75abaedd6572e0b2f`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 29 May 2020 21:20:36 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:37 GMT
RUN apt-key adv --keyserver keys.gnupg.net --recv-keys "539A 3A8C 6692 E6E3 F69B 3FE8 1D85 E93F 801B B43F"     && echo "deb https://download.rethinkdb.com/repository/debian-buster buster main" > /etc/apt/sources.list.d/rethinkdb.list
# Fri, 29 May 2020 21:20:37 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0~0buster
# Fri, 29 May 2020 21:20:46 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 May 2020 21:20:46 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:20:46 GMT
WORKDIR /data
# Fri, 29 May 2020 21:20:46 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:20:46 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bbb42f3811a4c02b1c4215f0931baa5e7fd47f7fee958f5a6df4eaf484b513`  
		Last Modified: Fri, 29 May 2020 21:21:15 GMT  
		Size: 6.7 MB (6669801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e549bc572ab8ed4af16254f062de89f9a16ad863d45cc0d7376fa281f371aef`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 2.6 KB (2611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82a54f8493424eb4636699476754b60fd40544d6c4a0be22d9d98201ec6a492`  
		Last Modified: Fri, 29 May 2020 21:21:19 GMT  
		Size: 18.0 MB (17992073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db2f23689c74580c5a35e7baae3f5a2734bb5650037e85252f8e46dfadbc66e`  
		Last Modified: Fri, 29 May 2020 21:21:14 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
