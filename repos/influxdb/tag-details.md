<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `influxdb`

-	[`influxdb:1.8`](#influxdb18)
-	[`influxdb:1.8-alpine`](#influxdb18-alpine)
-	[`influxdb:1.8-data`](#influxdb18-data)
-	[`influxdb:1.8-data-alpine`](#influxdb18-data-alpine)
-	[`influxdb:1.8-meta`](#influxdb18-meta)
-	[`influxdb:1.8-meta-alpine`](#influxdb18-meta-alpine)
-	[`influxdb:1.8.10`](#influxdb1810)
-	[`influxdb:1.8.10-alpine`](#influxdb1810-alpine)
-	[`influxdb:1.8.10-data`](#influxdb1810-data)
-	[`influxdb:1.8.10-data-alpine`](#influxdb1810-data-alpine)
-	[`influxdb:1.8.10-meta`](#influxdb1810-meta)
-	[`influxdb:1.8.10-meta-alpine`](#influxdb1810-meta-alpine)
-	[`influxdb:1.9-data`](#influxdb19-data)
-	[`influxdb:1.9-data-alpine`](#influxdb19-data-alpine)
-	[`influxdb:1.9-meta`](#influxdb19-meta)
-	[`influxdb:1.9-meta-alpine`](#influxdb19-meta-alpine)
-	[`influxdb:1.9.7-data`](#influxdb197-data)
-	[`influxdb:1.9.7-data-alpine`](#influxdb197-data-alpine)
-	[`influxdb:1.9.7-meta`](#influxdb197-meta)
-	[`influxdb:1.9.7-meta-alpine`](#influxdb197-meta-alpine)
-	[`influxdb:2.0`](#influxdb20)
-	[`influxdb:2.0-alpine`](#influxdb20-alpine)
-	[`influxdb:2.0.9`](#influxdb209)
-	[`influxdb:2.0.9-alpine`](#influxdb209-alpine)
-	[`influxdb:2.1`](#influxdb21)
-	[`influxdb:2.1-alpine`](#influxdb21-alpine)
-	[`influxdb:2.1.1`](#influxdb211)
-	[`influxdb:2.1.1-alpine`](#influxdb211-alpine)
-	[`influxdb:2.2`](#influxdb22)
-	[`influxdb:2.2-alpine`](#influxdb22-alpine)
-	[`influxdb:2.2.0`](#influxdb220)
-	[`influxdb:2.2.0-alpine`](#influxdb220-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:f9d7a1374648cd9b4d0d4052d8d1f0bb5236ccba37f210de4d6a3a1f217c4d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:7d8b8dbd35ea4437b8400a803ca83ed36bd1319d9bf5d7dbbfea352f76d86300
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115967857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7bb9814d084c5be76a7bd442b84d37f0619b028f5af3f54bca681582ad8ad82`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:38:23 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 11 May 2022 20:38:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 11 May 2022 20:38:28 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 11 May 2022 20:38:28 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:38:28 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 20:38:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 11 May 2022 20:38:29 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 11 May 2022 20:38:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:38:29 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565d52697dc7657483e66de35859480ec0bb9fdce45fd76e1512042633b2b15`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28747fe7e9af0d9216b9b75b26043f8458a5dcabf09dd82393d67569f883b768`  
		Last Modified: Wed, 11 May 2022 20:40:52 GMT  
		Size: 54.9 MB (54890081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8f1499a548411daa7f09ca42a45c304cda353b7c359b389f7843045db5de26`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47d1fb1db8b9b97893850db180f93e6b108be6d9c604e19de87b6603f0c5a9b`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16910a4bdbe0f8a2a65b247087104053cd1b5f7eca03af047b66b2c9c5e5fa3`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:28475519e1645995a9ad38a53a319499245102e6ab0c79cd818a1e12db43e098
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107651847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7492aaee2a0b81914c9438fd0d4fd01908522ea656e042c749e64cc988590f0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:54:33 GMT
ADD file:c679388ac7a37037465302aea3117354d9746d0c50c056e826b5c8c58aea5138 in / 
# Wed, 11 May 2022 01:54:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:33:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 12 May 2022 15:42:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 12 May 2022 15:42:11 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 12 May 2022 15:42:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 12 May 2022 15:42:27 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 12 May 2022 15:42:27 GMT
EXPOSE 8086
# Thu, 12 May 2022 15:42:28 GMT
VOLUME [/var/lib/influxdb]
# Thu, 12 May 2022 15:42:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 12 May 2022 15:42:29 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 12 May 2022 15:42:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 May 2022 15:42:29 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:629c5b996bdb9cea71f1d194d7a244d4aba271133bad4f5b88bfe38c4626349a`  
		Last Modified: Wed, 11 May 2022 02:11:17 GMT  
		Size: 42.2 MB (42151163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbf25ac5d0e3ca11a0fb961c2ac0f897f1982389c85b6e31ee0fa63a0293cc0`  
		Last Modified: Wed, 11 May 2022 03:55:11 GMT  
		Size: 10.0 MB (9956859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a3f9738e27d03b85306ba8927ec41f0ffd375d26fc501906f097e639a1047f`  
		Last Modified: Wed, 11 May 2022 03:55:08 GMT  
		Size: 3.9 MB (3921810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8ba85498aa9ec14d6356681a65e5518b0339fb2f69ea60e8116206d91b7b1f`  
		Last Modified: Thu, 12 May 2022 15:42:50 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2706d770f31bf25c5a5bb2c674a061746a32751a92dc83031e117e44ff8dd6e2`  
		Last Modified: Thu, 12 May 2022 15:43:18 GMT  
		Size: 51.6 MB (51617444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09adb5a1ae0f8d3a375a6b8a0405a2b150b9c27d4672243158eeed487c668e3`  
		Last Modified: Thu, 12 May 2022 15:42:50 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fe9e86bdd84f915f593a7ad9d9fef249c44e68378a4e88ba881d2127251feb`  
		Last Modified: Thu, 12 May 2022 15:42:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa68e5c988497e3f94258a0ce40343cad0bd045180907cea242c8d3573c34606`  
		Last Modified: Thu, 12 May 2022 15:42:50 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:12437d507e19d0ed02a5e9fc6047016219bc700a772c8375c00a51ab1b677354
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108543647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d494ca50234a24e19cbddea857d07e7a9045957adf975fcafd37240fec8763`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 00:49:08 GMT
ADD file:8949016fba61b18207f5a2309fc974562080c5cc80d1eb82adb35c4fa03f6f05 in / 
# Wed, 11 May 2022 00:49:09 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:29:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:30:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:48:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 19:48:13 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 11 May 2022 19:48:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 11 May 2022 19:48:21 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 11 May 2022 19:48:21 GMT
EXPOSE 8086
# Wed, 11 May 2022 19:48:22 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 19:48:24 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 11 May 2022 19:48:25 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 11 May 2022 19:48:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:48:26 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:139065d8f4553df403babda56f830c32aa1f3e57f18d2145a3179468921a4bb8`  
		Last Modified: Wed, 11 May 2022 00:57:26 GMT  
		Size: 43.2 MB (43212478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0acfd1725613d968a54b7fbfe1f70f24b8a0dad792ad3cb28349035f7736fe`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 10.2 MB (10217776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002c314192ef0350d2ac1d1e49b4fddbc49dbcdc609e56e0e2567ee2dd37f0bc`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 3.9 MB (3874525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e7249575734137345484e5fb7d160f9549c007fa5de438ac8242aa60c0b0bd`  
		Last Modified: Wed, 11 May 2022 19:51:22 GMT  
		Size: 2.8 KB (2823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd577c441cd1ad63dace2ddc48b2fc8d70323482327babdd32bbadc77719b81`  
		Last Modified: Wed, 11 May 2022 19:51:28 GMT  
		Size: 51.2 MB (51234330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81086768af5803909208fb6f79d0fbf6fbf22e9af7d600d7ca3f8387f93e127f`  
		Last Modified: Wed, 11 May 2022 19:51:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1654bdca69813aac0376a220c1f34244ccc3c4e720a6647d6004423bd7c6cf0`  
		Last Modified: Wed, 11 May 2022 19:51:22 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd66fcd846237eeca7ed9df5ac610e45acc75f56c92916d4d60d58231b1316c`  
		Last Modified: Wed, 11 May 2022 19:51:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:9b54e97bda0ad56d352d7b0f30f0838a7804786af3dcf9902f2facb20cdc8c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:da9e53019e9e915278d9b6a199a64cc8486e13528411101f75385bb7f2e709a1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58955359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33508e3d62d57b814452b7f7b3c08050f7fbd3890283f8078e4a6979ca58299`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:02:50 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 10:03:30 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 05 Apr 2022 10:03:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 10:03:38 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 05 Apr 2022 10:03:38 GMT
EXPOSE 8086
# Tue, 05 Apr 2022 10:03:38 GMT
VOLUME [/var/lib/influxdb]
# Tue, 05 Apr 2022 10:03:38 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 05 Apr 2022 10:03:38 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 05 Apr 2022 10:03:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 10:03:39 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a82c2bf0b07bc97e48386998fdb52307a711c8cde52325fb999e1b7a0f0073`  
		Last Modified: Tue, 05 Apr 2022 10:06:22 GMT  
		Size: 1.5 MB (1475485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c92e0e1b5e3133d942ce0fc2b295ac44f364c5d1d17b60fd452b00d16327c6`  
		Last Modified: Tue, 05 Apr 2022 10:07:22 GMT  
		Size: 54.7 MB (54659608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694e17e1c591b62f9b5418e23aba661b8e50ca089d198a5324be12c4fb3cc771`  
		Last Modified: Tue, 05 Apr 2022 10:07:15 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d046f1f7638fc6b5b400ed626934ab027a265996965cf13474e1dc8d21bde4b4`  
		Last Modified: Tue, 05 Apr 2022 10:07:14 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862c4c27d4c5aea4da583ac392bed4175d995bbacbd71ecc116d6b77d44a1aa3`  
		Last Modified: Tue, 05 Apr 2022 10:07:15 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:5b0b5c4d626c6486c1bd33a598500229e30086e622103392e582c08f5af2c961
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:b1490b4e0037c9ec65d02818851e0229ccaad0c3c1d0300418e4142a731258d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117786946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d87cf020fc2a813256c8a935cc37c72fdc75869a998b4a87cf875891e2032044`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:38:33 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 11 May 2022 20:38:39 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 11 May 2022 20:38:40 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 11 May 2022 20:38:40 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:38:40 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 20:38:40 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 11 May 2022 20:38:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 11 May 2022 20:38:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:38:40 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565d52697dc7657483e66de35859480ec0bb9fdce45fd76e1512042633b2b15`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3623f788a4d6e2cd10a137d1b81983e5a858e33ad4bf4cad01f47d90b8084200`  
		Last Modified: Wed, 11 May 2022 20:41:10 GMT  
		Size: 56.7 MB (56709115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242df9a8b2f790b9a34d5f6b7a55989913b076aa27425f3709b3ebaab620ffbc`  
		Last Modified: Wed, 11 May 2022 20:41:02 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b27dbc8850d0b6695b7b1d943292c56a290cf4786773c0e32e8639d16e4bd7`  
		Last Modified: Wed, 11 May 2022 20:41:02 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433d58cd840d19993e454795631954fac3097458b2b862700b9954bd383b1e4a`  
		Last Modified: Wed, 11 May 2022 20:41:02 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:5b6f51f9283101e2260d04e4ec6e97e6ac6b42906de0330d245556207485ff9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ffe5860e830f75f1ecc06f6d9ef5131783a4009bf8c178a202b221b7090991d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60799475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c51bbfae48c946a370eace3f872988f7daf93c3ee3586f383c6165ed132c4760`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:02:50 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 10:03:43 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 07 Apr 2022 22:22:53 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 07 Apr 2022 22:22:54 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 07 Apr 2022 22:22:54 GMT
EXPOSE 8086
# Thu, 07 Apr 2022 22:22:54 GMT
VOLUME [/var/lib/influxdb]
# Thu, 07 Apr 2022 22:22:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 07 Apr 2022 22:22:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 07 Apr 2022 22:22:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:22:54 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a82c2bf0b07bc97e48386998fdb52307a711c8cde52325fb999e1b7a0f0073`  
		Last Modified: Tue, 05 Apr 2022 10:06:22 GMT  
		Size: 1.5 MB (1475485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d253e65fc0c40504c5ab7ed8891c7535ce694e62e9b315612518257a49a27e`  
		Last Modified: Thu, 07 Apr 2022 22:24:53 GMT  
		Size: 56.5 MB (56503671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c14b9a988386b736ef6a259676adf189b9aee692453b5a41173a23bd2aed93e`  
		Last Modified: Thu, 07 Apr 2022 22:24:46 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1e32c4578db25e99bb2f5fbd9bae12550160681dd612559a2fdb24774b6636`  
		Last Modified: Thu, 07 Apr 2022 22:24:46 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3641a605f831a5d23969cb82df4b923d91d0377459df0169f7c92d5a15449a9`  
		Last Modified: Thu, 07 Apr 2022 22:24:46 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:52cf241438911f68b82ca627dfb338fc09a90a0712e43a48bde0f923674c8d04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ced01456b4cd44c84a41de62ef164e2cdf38dd0ee474bbf67827aae43c764b0e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84493544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:470881da7fcdba67ecb9b682507e53aeb5518826856bb316132641238a2ef278`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:38:33 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 11 May 2022 20:38:48 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 11 May 2022 20:38:49 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 11 May 2022 20:38:49 GMT
EXPOSE 8091
# Wed, 11 May 2022 20:38:49 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 20:38:49 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 11 May 2022 20:38:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:38:49 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565d52697dc7657483e66de35859480ec0bb9fdce45fd76e1512042633b2b15`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c80c146b168e3ced16a4c687940031768c8750b3c972237b2b742b0e09410f1`  
		Last Modified: Wed, 11 May 2022 20:41:26 GMT  
		Size: 23.4 MB (23416916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c721d0e8c99466248351dc4cc8f1dd68923ab2ac35bb71198d63b20edfa1c203`  
		Last Modified: Wed, 11 May 2022 20:41:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbcc734429c05067742043f9ff495038a02f7be5ad26dfa0f2ca63de9b559d6`  
		Last Modified: Wed, 11 May 2022 20:41:23 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:008db7d140fce00d44cb0f11b4e04a8d5c151222c18e20f1a6e3c40432c1b6c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:06b3c6c7fdaaae61c386be3b2db8debdb79dc029c86b28fb2ddd57b7a813cca9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27587601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c59c3a9d5137ca189bf5be3e9b530b46a594f7e9911d79fb7ce49a68802cbdd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:02:50 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 10:03:43 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 07 Apr 2022 22:23:04 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 07 Apr 2022 22:23:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 07 Apr 2022 22:23:04 GMT
EXPOSE 8091
# Thu, 07 Apr 2022 22:23:04 GMT
VOLUME [/var/lib/influxdb]
# Thu, 07 Apr 2022 22:23:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 07 Apr 2022 22:23:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:23:05 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a82c2bf0b07bc97e48386998fdb52307a711c8cde52325fb999e1b7a0f0073`  
		Last Modified: Tue, 05 Apr 2022 10:06:22 GMT  
		Size: 1.5 MB (1475485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef0611ecd34d60d54d119ad0d5b217bf9bb505143a9a76d79a71588306f6962`  
		Last Modified: Thu, 07 Apr 2022 22:25:10 GMT  
		Size: 23.3 MB (23292997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03800bc1786c31a63f2ce29355aa6c75587b563883515d7db2faec592fe0bcc5`  
		Last Modified: Thu, 07 Apr 2022 22:25:07 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56614b1a615f4516c69895cb7e68ac004819d3dd52ffe4766c55c5686847eff`  
		Last Modified: Thu, 07 Apr 2022 22:25:07 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10`

```console
$ docker pull influxdb@sha256:f9d7a1374648cd9b4d0d4052d8d1f0bb5236ccba37f210de4d6a3a1f217c4d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:7d8b8dbd35ea4437b8400a803ca83ed36bd1319d9bf5d7dbbfea352f76d86300
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115967857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7bb9814d084c5be76a7bd442b84d37f0619b028f5af3f54bca681582ad8ad82`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:38:23 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 11 May 2022 20:38:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 11 May 2022 20:38:28 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 11 May 2022 20:38:28 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:38:28 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 20:38:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 11 May 2022 20:38:29 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 11 May 2022 20:38:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:38:29 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565d52697dc7657483e66de35859480ec0bb9fdce45fd76e1512042633b2b15`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28747fe7e9af0d9216b9b75b26043f8458a5dcabf09dd82393d67569f883b768`  
		Last Modified: Wed, 11 May 2022 20:40:52 GMT  
		Size: 54.9 MB (54890081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8f1499a548411daa7f09ca42a45c304cda353b7c359b389f7843045db5de26`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47d1fb1db8b9b97893850db180f93e6b108be6d9c604e19de87b6603f0c5a9b`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16910a4bdbe0f8a2a65b247087104053cd1b5f7eca03af047b66b2c9c5e5fa3`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:28475519e1645995a9ad38a53a319499245102e6ab0c79cd818a1e12db43e098
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107651847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7492aaee2a0b81914c9438fd0d4fd01908522ea656e042c749e64cc988590f0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:54:33 GMT
ADD file:c679388ac7a37037465302aea3117354d9746d0c50c056e826b5c8c58aea5138 in / 
# Wed, 11 May 2022 01:54:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:33:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 12 May 2022 15:42:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 12 May 2022 15:42:11 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 12 May 2022 15:42:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 12 May 2022 15:42:27 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 12 May 2022 15:42:27 GMT
EXPOSE 8086
# Thu, 12 May 2022 15:42:28 GMT
VOLUME [/var/lib/influxdb]
# Thu, 12 May 2022 15:42:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 12 May 2022 15:42:29 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 12 May 2022 15:42:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 May 2022 15:42:29 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:629c5b996bdb9cea71f1d194d7a244d4aba271133bad4f5b88bfe38c4626349a`  
		Last Modified: Wed, 11 May 2022 02:11:17 GMT  
		Size: 42.2 MB (42151163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbf25ac5d0e3ca11a0fb961c2ac0f897f1982389c85b6e31ee0fa63a0293cc0`  
		Last Modified: Wed, 11 May 2022 03:55:11 GMT  
		Size: 10.0 MB (9956859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a3f9738e27d03b85306ba8927ec41f0ffd375d26fc501906f097e639a1047f`  
		Last Modified: Wed, 11 May 2022 03:55:08 GMT  
		Size: 3.9 MB (3921810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8ba85498aa9ec14d6356681a65e5518b0339fb2f69ea60e8116206d91b7b1f`  
		Last Modified: Thu, 12 May 2022 15:42:50 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2706d770f31bf25c5a5bb2c674a061746a32751a92dc83031e117e44ff8dd6e2`  
		Last Modified: Thu, 12 May 2022 15:43:18 GMT  
		Size: 51.6 MB (51617444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09adb5a1ae0f8d3a375a6b8a0405a2b150b9c27d4672243158eeed487c668e3`  
		Last Modified: Thu, 12 May 2022 15:42:50 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fe9e86bdd84f915f593a7ad9d9fef249c44e68378a4e88ba881d2127251feb`  
		Last Modified: Thu, 12 May 2022 15:42:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa68e5c988497e3f94258a0ce40343cad0bd045180907cea242c8d3573c34606`  
		Last Modified: Thu, 12 May 2022 15:42:50 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:12437d507e19d0ed02a5e9fc6047016219bc700a772c8375c00a51ab1b677354
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108543647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d494ca50234a24e19cbddea857d07e7a9045957adf975fcafd37240fec8763`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 00:49:08 GMT
ADD file:8949016fba61b18207f5a2309fc974562080c5cc80d1eb82adb35c4fa03f6f05 in / 
# Wed, 11 May 2022 00:49:09 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:29:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:30:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:48:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 19:48:13 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 11 May 2022 19:48:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 11 May 2022 19:48:21 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 11 May 2022 19:48:21 GMT
EXPOSE 8086
# Wed, 11 May 2022 19:48:22 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 19:48:24 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 11 May 2022 19:48:25 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 11 May 2022 19:48:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:48:26 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:139065d8f4553df403babda56f830c32aa1f3e57f18d2145a3179468921a4bb8`  
		Last Modified: Wed, 11 May 2022 00:57:26 GMT  
		Size: 43.2 MB (43212478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0acfd1725613d968a54b7fbfe1f70f24b8a0dad792ad3cb28349035f7736fe`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 10.2 MB (10217776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002c314192ef0350d2ac1d1e49b4fddbc49dbcdc609e56e0e2567ee2dd37f0bc`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 3.9 MB (3874525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e7249575734137345484e5fb7d160f9549c007fa5de438ac8242aa60c0b0bd`  
		Last Modified: Wed, 11 May 2022 19:51:22 GMT  
		Size: 2.8 KB (2823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd577c441cd1ad63dace2ddc48b2fc8d70323482327babdd32bbadc77719b81`  
		Last Modified: Wed, 11 May 2022 19:51:28 GMT  
		Size: 51.2 MB (51234330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81086768af5803909208fb6f79d0fbf6fbf22e9af7d600d7ca3f8387f93e127f`  
		Last Modified: Wed, 11 May 2022 19:51:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1654bdca69813aac0376a220c1f34244ccc3c4e720a6647d6004423bd7c6cf0`  
		Last Modified: Wed, 11 May 2022 19:51:22 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd66fcd846237eeca7ed9df5ac610e45acc75f56c92916d4d60d58231b1316c`  
		Last Modified: Wed, 11 May 2022 19:51:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-alpine`

```console
$ docker pull influxdb@sha256:9b54e97bda0ad56d352d7b0f30f0838a7804786af3dcf9902f2facb20cdc8c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:da9e53019e9e915278d9b6a199a64cc8486e13528411101f75385bb7f2e709a1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58955359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33508e3d62d57b814452b7f7b3c08050f7fbd3890283f8078e4a6979ca58299`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:02:50 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 10:03:30 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 05 Apr 2022 10:03:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 10:03:38 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 05 Apr 2022 10:03:38 GMT
EXPOSE 8086
# Tue, 05 Apr 2022 10:03:38 GMT
VOLUME [/var/lib/influxdb]
# Tue, 05 Apr 2022 10:03:38 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 05 Apr 2022 10:03:38 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 05 Apr 2022 10:03:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 10:03:39 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a82c2bf0b07bc97e48386998fdb52307a711c8cde52325fb999e1b7a0f0073`  
		Last Modified: Tue, 05 Apr 2022 10:06:22 GMT  
		Size: 1.5 MB (1475485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c92e0e1b5e3133d942ce0fc2b295ac44f364c5d1d17b60fd452b00d16327c6`  
		Last Modified: Tue, 05 Apr 2022 10:07:22 GMT  
		Size: 54.7 MB (54659608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694e17e1c591b62f9b5418e23aba661b8e50ca089d198a5324be12c4fb3cc771`  
		Last Modified: Tue, 05 Apr 2022 10:07:15 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d046f1f7638fc6b5b400ed626934ab027a265996965cf13474e1dc8d21bde4b4`  
		Last Modified: Tue, 05 Apr 2022 10:07:14 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862c4c27d4c5aea4da583ac392bed4175d995bbacbd71ecc116d6b77d44a1aa3`  
		Last Modified: Tue, 05 Apr 2022 10:07:15 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data`

```console
$ docker pull influxdb@sha256:5b0b5c4d626c6486c1bd33a598500229e30086e622103392e582c08f5af2c961
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:b1490b4e0037c9ec65d02818851e0229ccaad0c3c1d0300418e4142a731258d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117786946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d87cf020fc2a813256c8a935cc37c72fdc75869a998b4a87cf875891e2032044`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:38:33 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 11 May 2022 20:38:39 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 11 May 2022 20:38:40 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 11 May 2022 20:38:40 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:38:40 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 20:38:40 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 11 May 2022 20:38:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 11 May 2022 20:38:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:38:40 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565d52697dc7657483e66de35859480ec0bb9fdce45fd76e1512042633b2b15`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3623f788a4d6e2cd10a137d1b81983e5a858e33ad4bf4cad01f47d90b8084200`  
		Last Modified: Wed, 11 May 2022 20:41:10 GMT  
		Size: 56.7 MB (56709115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242df9a8b2f790b9a34d5f6b7a55989913b076aa27425f3709b3ebaab620ffbc`  
		Last Modified: Wed, 11 May 2022 20:41:02 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b27dbc8850d0b6695b7b1d943292c56a290cf4786773c0e32e8639d16e4bd7`  
		Last Modified: Wed, 11 May 2022 20:41:02 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433d58cd840d19993e454795631954fac3097458b2b862700b9954bd383b1e4a`  
		Last Modified: Wed, 11 May 2022 20:41:02 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data-alpine`

```console
$ docker pull influxdb@sha256:5b6f51f9283101e2260d04e4ec6e97e6ac6b42906de0330d245556207485ff9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ffe5860e830f75f1ecc06f6d9ef5131783a4009bf8c178a202b221b7090991d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60799475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c51bbfae48c946a370eace3f872988f7daf93c3ee3586f383c6165ed132c4760`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:02:50 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 10:03:43 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 07 Apr 2022 22:22:53 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 07 Apr 2022 22:22:54 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 07 Apr 2022 22:22:54 GMT
EXPOSE 8086
# Thu, 07 Apr 2022 22:22:54 GMT
VOLUME [/var/lib/influxdb]
# Thu, 07 Apr 2022 22:22:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 07 Apr 2022 22:22:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 07 Apr 2022 22:22:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:22:54 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a82c2bf0b07bc97e48386998fdb52307a711c8cde52325fb999e1b7a0f0073`  
		Last Modified: Tue, 05 Apr 2022 10:06:22 GMT  
		Size: 1.5 MB (1475485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d253e65fc0c40504c5ab7ed8891c7535ce694e62e9b315612518257a49a27e`  
		Last Modified: Thu, 07 Apr 2022 22:24:53 GMT  
		Size: 56.5 MB (56503671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c14b9a988386b736ef6a259676adf189b9aee692453b5a41173a23bd2aed93e`  
		Last Modified: Thu, 07 Apr 2022 22:24:46 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1e32c4578db25e99bb2f5fbd9bae12550160681dd612559a2fdb24774b6636`  
		Last Modified: Thu, 07 Apr 2022 22:24:46 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3641a605f831a5d23969cb82df4b923d91d0377459df0169f7c92d5a15449a9`  
		Last Modified: Thu, 07 Apr 2022 22:24:46 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta`

```console
$ docker pull influxdb@sha256:52cf241438911f68b82ca627dfb338fc09a90a0712e43a48bde0f923674c8d04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ced01456b4cd44c84a41de62ef164e2cdf38dd0ee474bbf67827aae43c764b0e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84493544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:470881da7fcdba67ecb9b682507e53aeb5518826856bb316132641238a2ef278`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:38:33 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 11 May 2022 20:38:48 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 11 May 2022 20:38:49 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 11 May 2022 20:38:49 GMT
EXPOSE 8091
# Wed, 11 May 2022 20:38:49 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 20:38:49 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 11 May 2022 20:38:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:38:49 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565d52697dc7657483e66de35859480ec0bb9fdce45fd76e1512042633b2b15`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c80c146b168e3ced16a4c687940031768c8750b3c972237b2b742b0e09410f1`  
		Last Modified: Wed, 11 May 2022 20:41:26 GMT  
		Size: 23.4 MB (23416916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c721d0e8c99466248351dc4cc8f1dd68923ab2ac35bb71198d63b20edfa1c203`  
		Last Modified: Wed, 11 May 2022 20:41:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbcc734429c05067742043f9ff495038a02f7be5ad26dfa0f2ca63de9b559d6`  
		Last Modified: Wed, 11 May 2022 20:41:23 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta-alpine`

```console
$ docker pull influxdb@sha256:008db7d140fce00d44cb0f11b4e04a8d5c151222c18e20f1a6e3c40432c1b6c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:06b3c6c7fdaaae61c386be3b2db8debdb79dc029c86b28fb2ddd57b7a813cca9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27587601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c59c3a9d5137ca189bf5be3e9b530b46a594f7e9911d79fb7ce49a68802cbdd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:02:50 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 10:03:43 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 07 Apr 2022 22:23:04 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 07 Apr 2022 22:23:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 07 Apr 2022 22:23:04 GMT
EXPOSE 8091
# Thu, 07 Apr 2022 22:23:04 GMT
VOLUME [/var/lib/influxdb]
# Thu, 07 Apr 2022 22:23:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 07 Apr 2022 22:23:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:23:05 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a82c2bf0b07bc97e48386998fdb52307a711c8cde52325fb999e1b7a0f0073`  
		Last Modified: Tue, 05 Apr 2022 10:06:22 GMT  
		Size: 1.5 MB (1475485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef0611ecd34d60d54d119ad0d5b217bf9bb505143a9a76d79a71588306f6962`  
		Last Modified: Thu, 07 Apr 2022 22:25:10 GMT  
		Size: 23.3 MB (23292997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03800bc1786c31a63f2ce29355aa6c75587b563883515d7db2faec592fe0bcc5`  
		Last Modified: Thu, 07 Apr 2022 22:25:07 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56614b1a615f4516c69895cb7e68ac004819d3dd52ffe4766c55c5686847eff`  
		Last Modified: Thu, 07 Apr 2022 22:25:07 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data`

```console
$ docker pull influxdb@sha256:92dd787fb1b132355be5b51840dfcdad82f5f2596f9e527f31b2238b9b93588d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:da6f860af069a8f643e280986e5de823e6dc07dee00e4bb7afa0c5d409354709
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88681981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca83c232cf10aad75b3b9206bb75d45a784421a835b79a40ee9b44fb123a6fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:38:53 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Wed, 11 May 2022 20:38:58 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 11 May 2022 20:38:58 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 11 May 2022 20:38:58 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:38:58 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 20:38:58 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 11 May 2022 20:38:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 11 May 2022 20:38:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:38:59 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565d52697dc7657483e66de35859480ec0bb9fdce45fd76e1512042633b2b15`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f83cbc5f262349c458bf31cd1e6bb691ef072c638331ce75b1dc2e149fb0a8`  
		Last Modified: Wed, 11 May 2022 20:41:44 GMT  
		Size: 27.6 MB (27604148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044dec5cc25e4bbdaf9d8f87b2386dc7be50bbf168a5c4b6a3452269daadf7c9`  
		Last Modified: Wed, 11 May 2022 20:41:39 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3058b5f89140be57c63374d2d9146cf30541fbc91adb67b9b955d92aa513034d`  
		Last Modified: Wed, 11 May 2022 20:41:39 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e942527cac317c2589da3125159e6a824647dc3ac65ac9214211257930a4e9c`  
		Last Modified: Wed, 11 May 2022 20:41:39 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:d8934ee0edc69812dae63ed9b474eb91d650ca8c460605bbc305dbc18c3cb014
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:fcdb1822869fea2ae4d731fd9ef53bc6b7cc591649a0c19870c5dc331e725798
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.9 MB (31863241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fba23542f7a038ace18c55398d146c9e474a0c1d4580ddc36feded2f14f6de3f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:02:50 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 10:04:06 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Thu, 07 Apr 2022 22:23:13 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 07 Apr 2022 22:23:14 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 07 Apr 2022 22:23:14 GMT
EXPOSE 8086
# Thu, 07 Apr 2022 22:23:14 GMT
VOLUME [/var/lib/influxdb]
# Thu, 07 Apr 2022 22:23:14 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 07 Apr 2022 22:23:14 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 07 Apr 2022 22:23:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:23:14 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a82c2bf0b07bc97e48386998fdb52307a711c8cde52325fb999e1b7a0f0073`  
		Last Modified: Tue, 05 Apr 2022 10:06:22 GMT  
		Size: 1.5 MB (1475485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87330db054b158b6242dfa37ac1734394b53b4002531d619c69195fce53b880`  
		Last Modified: Thu, 07 Apr 2022 22:25:28 GMT  
		Size: 27.6 MB (27567431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0962416aa49614e3fd3d50a91a0f47e80edc2c068c8eefbbf4c022fe80a421e6`  
		Last Modified: Thu, 07 Apr 2022 22:25:24 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e05404d71bfd40d3e7c7a785d85c9a0509d3ee10afb4988c70509113fd2cc8d`  
		Last Modified: Thu, 07 Apr 2022 22:25:24 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484b99a22ff9292d8539523a502634a0bbcebbba545ee57d04fc649d8a30620b`  
		Last Modified: Thu, 07 Apr 2022 22:25:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:ab73d05f2fc2e1087d7bc3c760318bf09bc901e5df2f3c0993eadc579442d7b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:01c09ce0790155fa4bbf1d2faaa9d9780ed5041adf38ce8092069deec2660cee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71516172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81fb6e814d96332092f65b8fcae115d7c983a6c716434f1d377050fb85c28350`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:38:53 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Wed, 11 May 2022 20:39:06 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 11 May 2022 20:39:06 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 11 May 2022 20:39:06 GMT
EXPOSE 8091
# Wed, 11 May 2022 20:39:06 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 20:39:06 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 11 May 2022 20:39:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:39:07 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565d52697dc7657483e66de35859480ec0bb9fdce45fd76e1512042633b2b15`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868f778be1cae17572176230edc857ed488332d56c180aa56233d5697d2fb2c7`  
		Last Modified: Wed, 11 May 2022 20:41:56 GMT  
		Size: 10.4 MB (10439543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339766b2592adf619a3826ed8de4434f5db126f249ddbaa2805854fe9b1c7606`  
		Last Modified: Wed, 11 May 2022 20:41:55 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cd45d658e4fa4920642338b4e0cc2bb6d2a153379cb4bf3c60c25195658af9`  
		Last Modified: Wed, 11 May 2022 20:41:55 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:742a51db8dfe569adb49a69071c44ddf0f373199e5b78d0a50e3839e63b8a5bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:559b89f7cb3304fe14660e80ca1af6001cde71e0c3f5b7ce787f326e5b4cbd1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14704251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a8cb4fbadc797b3409e60f86e0bebe475b9d724cd15f658d8211d794fe4b83`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:02:50 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 10:04:06 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Thu, 07 Apr 2022 22:23:26 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 07 Apr 2022 22:23:26 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 07 Apr 2022 22:23:27 GMT
EXPOSE 8091
# Thu, 07 Apr 2022 22:23:27 GMT
VOLUME [/var/lib/influxdb]
# Thu, 07 Apr 2022 22:23:27 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 07 Apr 2022 22:23:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:23:27 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a82c2bf0b07bc97e48386998fdb52307a711c8cde52325fb999e1b7a0f0073`  
		Last Modified: Tue, 05 Apr 2022 10:06:22 GMT  
		Size: 1.5 MB (1475485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f70b29b3caa461ee689124f3e52d1f96938ee16f711df91186f9de029f5b8d`  
		Last Modified: Thu, 07 Apr 2022 22:25:41 GMT  
		Size: 10.4 MB (10409651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db52da89842c67d69448b5f7a6c22170c52e7d6924782d73f71670cd9507143`  
		Last Modified: Thu, 07 Apr 2022 22:25:39 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc8508a3dc50232978c669e0a0e78a4d23b4a2b0310542757c506d69b7938d2`  
		Last Modified: Thu, 07 Apr 2022 22:25:39 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.7-data`

**does not exist** (yet?)

## `influxdb:1.9.7-data-alpine`

**does not exist** (yet?)

## `influxdb:1.9.7-meta`

**does not exist** (yet?)

## `influxdb:1.9.7-meta-alpine`

**does not exist** (yet?)

## `influxdb:2.0`

```console
$ docker pull influxdb@sha256:da7fea3b28b6a440ba54788b38eb9f1dae498050955e680e3ffbdb52b06bd32a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:8793b3a67a6fa2c6b12756016b94ff0a9d95ea4c8e938a9dd0f52f063a5e22fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.4 MB (172350547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:735092093014498618d6367ba78d6b566bf66086a81ba62e3551eb4289bba170`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:39:11 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 20:39:11 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 20:39:15 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 20:39:15 GMT
ENV INFLUXDB_VERSION=2.0.9
# Wed, 11 May 2022 20:39:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 11 May 2022 20:39:24 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 20:39:24 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 20:39:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 20:39:24 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Wed, 11 May 2022 20:39:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:39:24 GMT
CMD ["influxd"]
# Wed, 11 May 2022 20:39:24 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:39:24 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 20:39:25 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 20:39:25 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 20:39:25 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7502ee2d408fa6f349bdf986640e67d1424ad5f35061bd24f4f0453aec2cbb50`  
		Last Modified: Wed, 11 May 2022 20:42:10 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c05c9cd211b391c71fb38c29a6f3f27091d07df73f89a9e77fd5e0b9ffc1fbd`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 961.0 KB (960961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96753e3060b4178829ae1284df19e8548e710b178b200bec3ec22904ef6b153`  
		Last Modified: Wed, 11 May 2022 20:42:16 GMT  
		Size: 103.1 MB (103090637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b1783b3877260fc256e3b6565c5daaddb7794fcdc64a163b46a101ceeaccf8`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270a2a2fb432d0a9f91dc8cbb5cd33e4372bcf89ed549c3c6ccdb5c920094369`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b34554ba0498adcdacbfa464e987294a5283364b693dafb9b46480bf9ceec9`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 4.9 KB (4948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:aa77cddc6b4488e2bfbd37aa24d39759f3cb23033abc172606297ab9c311bed2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174145770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:325511f31df45a54f0c6d0030c20fbf5eae31fb25db715310e2b125b46e839d1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:48:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 19:48:33 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 19:48:37 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 19:48:37 GMT
ENV INFLUXDB_VERSION=2.0.9
# Wed, 11 May 2022 19:48:53 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 11 May 2022 19:48:54 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 19:48:55 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 19:48:57 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 19:48:58 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Wed, 11 May 2022 19:48:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:48:59 GMT
CMD ["influxd"]
# Wed, 11 May 2022 19:49:00 GMT
EXPOSE 8086
# Wed, 11 May 2022 19:49:01 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 19:49:02 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 19:49:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 19:49:04 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88155b239d4be6cbe8982344c645615907ceb1698ecd859485dc47854b1ae2fe`  
		Last Modified: Wed, 11 May 2022 19:51:42 GMT  
		Size: 1.7 KB (1661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c422d6301995ca5b81c45b24404c961c0b1ccc9bd31c9a54b82363a29844af`  
		Last Modified: Wed, 11 May 2022 19:51:40 GMT  
		Size: 896.3 KB (896335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57705bd4d82abbc8f0e5bdac3eabcd8dbaa7ec06ee9ae7f62811f74cb79c6d8c`  
		Last Modified: Wed, 11 May 2022 19:51:50 GMT  
		Size: 106.5 MB (106526969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb767ce4bc1c69af939271a91bfa0e7e84a196983c78967a6b6b6c11991ac905`  
		Last Modified: Wed, 11 May 2022 19:51:39 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853435fa3a0ec17ff0093e171015052a82191ec257be72a9660530ed11bc85f2`  
		Last Modified: Wed, 11 May 2022 19:51:39 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb9e39460ceffba9e32d32b3265a91aa2367717f8159cd6cf5668340deb0c0a`  
		Last Modified: Wed, 11 May 2022 19:51:39 GMT  
		Size: 4.9 KB (4945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0-alpine`

```console
$ docker pull influxdb@sha256:28b27ba51abbddb2113c728b9fb5e23261733a9bceb995402012e69aa34273d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:e0e9f4602a6cc0632ea1dbc8910759c86b61ece94f6d5894382d6f1b9bcc30e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116713298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac89ea59315d99dec3c08bb1723cf2fbf03c2e11b2705cbc281417dbafc9c37e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:04:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 10:04:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 10:04:29 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 10:04:32 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Apr 2022 10:04:32 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Apr 2022 10:04:44 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Apr 2022 10:04:45 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Apr 2022 10:04:45 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Apr 2022 10:04:45 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Apr 2022 10:04:45 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Tue, 05 Apr 2022 10:04:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 10:04:45 GMT
CMD ["influxd"]
# Tue, 05 Apr 2022 10:04:45 GMT
EXPOSE 8086
# Tue, 05 Apr 2022 10:04:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Apr 2022 10:04:46 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Apr 2022 10:04:46 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Apr 2022 10:04:46 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e824989658cee0fcd8b3e27d03a0b79d4ae37c3b765afaff6f49d076d0d9dc42`  
		Last Modified: Tue, 05 Apr 2022 10:08:40 GMT  
		Size: 9.8 MB (9836774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6fbe7d281a77910553db440ca9d0c4b709850e35385fc474a9b9b11e55db697`  
		Last Modified: Tue, 05 Apr 2022 10:08:38 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288cce5ed27daa2927f6bc96c87e2581197832a7210cf5813f6d6cfea28afb7e`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 960.6 KB (960617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bae8b0ec17a5d9dbf1eb7e1e3953baef4edaf26b616fcbc218d817636d79d8`  
		Last Modified: Tue, 05 Apr 2022 10:08:45 GMT  
		Size: 103.1 MB (103090641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed8f2b193010cbe745a05d4a2907ef5592bcfc3fcf2f8dc3effc77b3db59171`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485640ccb69c912529e7b70604b5ab52e45aaf7fc93bbca67c021628d1f9d141`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6553ced84695f9c93dba30575941508f22f23786270f7612e99ebd6045d0ff5c`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 4.9 KB (4942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:3047f61d3f0deb8b68f3bb32f77ad1da4dc3f935344d6b4978e2b32978569b5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119819824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6df860f31be0a1452ff106725cb2865b8792e1cbca0eac815cee16c231129b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:11:26 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:11:29 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 04:11:30 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 04:11:31 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 04:11:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Apr 2022 04:11:35 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Apr 2022 04:11:48 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Apr 2022 04:11:48 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Apr 2022 04:11:49 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Apr 2022 04:11:51 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Apr 2022 04:11:52 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Tue, 05 Apr 2022 04:11:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:11:53 GMT
CMD ["influxd"]
# Tue, 05 Apr 2022 04:11:54 GMT
EXPOSE 8086
# Tue, 05 Apr 2022 04:11:55 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Apr 2022 04:11:56 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Apr 2022 04:11:57 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Apr 2022 04:11:58 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a37e642510b42e25dbe3082e57f33cdcdb65bad4e9468cd5c76fdb5015c7a`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc96d3454b87ca3f120022077fc7d0ff9477f1b5d1c99519902ae6eed0d7b90`  
		Last Modified: Tue, 05 Apr 2022 04:13:16 GMT  
		Size: 9.7 MB (9672606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af6c62b5230b53a6e53da9a15c422cfb18b955afc941e7b68331dd84392405c`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281a900a68fae805f39a9a8461f2ef4778a30b18c30f3bc6b2b85e0e02a107e4`  
		Last Modified: Tue, 05 Apr 2022 04:13:13 GMT  
		Size: 896.1 KB (896074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b07cab3429e5cb05ce350093f453086d575ea3fa8b8409fca4cabf4772f1b7`  
		Last Modified: Tue, 05 Apr 2022 04:13:23 GMT  
		Size: 106.5 MB (106526974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb98004947e4307dd97bd5347a40979529a3856593981fdf5be5939eddf45abe`  
		Last Modified: Tue, 05 Apr 2022 04:13:12 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a58f13a13141d9b8be4fdfd19c9bc68286c28872b5e103b27a68bf9af7b4ce`  
		Last Modified: Tue, 05 Apr 2022 04:13:12 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f057be72e1bceb8361f6e113dba8d132297ec659a68596020245db9a7db3d89`  
		Last Modified: Tue, 05 Apr 2022 04:13:13 GMT  
		Size: 4.9 KB (4948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.9`

```console
$ docker pull influxdb@sha256:da7fea3b28b6a440ba54788b38eb9f1dae498050955e680e3ffbdb52b06bd32a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9` - linux; amd64

```console
$ docker pull influxdb@sha256:8793b3a67a6fa2c6b12756016b94ff0a9d95ea4c8e938a9dd0f52f063a5e22fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.4 MB (172350547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:735092093014498618d6367ba78d6b566bf66086a81ba62e3551eb4289bba170`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:39:11 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 20:39:11 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 20:39:15 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 20:39:15 GMT
ENV INFLUXDB_VERSION=2.0.9
# Wed, 11 May 2022 20:39:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 11 May 2022 20:39:24 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 20:39:24 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 20:39:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 20:39:24 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Wed, 11 May 2022 20:39:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:39:24 GMT
CMD ["influxd"]
# Wed, 11 May 2022 20:39:24 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:39:24 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 20:39:25 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 20:39:25 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 20:39:25 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7502ee2d408fa6f349bdf986640e67d1424ad5f35061bd24f4f0453aec2cbb50`  
		Last Modified: Wed, 11 May 2022 20:42:10 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c05c9cd211b391c71fb38c29a6f3f27091d07df73f89a9e77fd5e0b9ffc1fbd`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 961.0 KB (960961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96753e3060b4178829ae1284df19e8548e710b178b200bec3ec22904ef6b153`  
		Last Modified: Wed, 11 May 2022 20:42:16 GMT  
		Size: 103.1 MB (103090637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b1783b3877260fc256e3b6565c5daaddb7794fcdc64a163b46a101ceeaccf8`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270a2a2fb432d0a9f91dc8cbb5cd33e4372bcf89ed549c3c6ccdb5c920094369`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b34554ba0498adcdacbfa464e987294a5283364b693dafb9b46480bf9ceec9`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 4.9 KB (4948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:aa77cddc6b4488e2bfbd37aa24d39759f3cb23033abc172606297ab9c311bed2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174145770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:325511f31df45a54f0c6d0030c20fbf5eae31fb25db715310e2b125b46e839d1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:48:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 19:48:33 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 19:48:37 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 19:48:37 GMT
ENV INFLUXDB_VERSION=2.0.9
# Wed, 11 May 2022 19:48:53 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 11 May 2022 19:48:54 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 19:48:55 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 19:48:57 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 19:48:58 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Wed, 11 May 2022 19:48:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:48:59 GMT
CMD ["influxd"]
# Wed, 11 May 2022 19:49:00 GMT
EXPOSE 8086
# Wed, 11 May 2022 19:49:01 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 19:49:02 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 19:49:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 19:49:04 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88155b239d4be6cbe8982344c645615907ceb1698ecd859485dc47854b1ae2fe`  
		Last Modified: Wed, 11 May 2022 19:51:42 GMT  
		Size: 1.7 KB (1661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c422d6301995ca5b81c45b24404c961c0b1ccc9bd31c9a54b82363a29844af`  
		Last Modified: Wed, 11 May 2022 19:51:40 GMT  
		Size: 896.3 KB (896335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57705bd4d82abbc8f0e5bdac3eabcd8dbaa7ec06ee9ae7f62811f74cb79c6d8c`  
		Last Modified: Wed, 11 May 2022 19:51:50 GMT  
		Size: 106.5 MB (106526969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb767ce4bc1c69af939271a91bfa0e7e84a196983c78967a6b6b6c11991ac905`  
		Last Modified: Wed, 11 May 2022 19:51:39 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853435fa3a0ec17ff0093e171015052a82191ec257be72a9660530ed11bc85f2`  
		Last Modified: Wed, 11 May 2022 19:51:39 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb9e39460ceffba9e32d32b3265a91aa2367717f8159cd6cf5668340deb0c0a`  
		Last Modified: Wed, 11 May 2022 19:51:39 GMT  
		Size: 4.9 KB (4945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.9-alpine`

```console
$ docker pull influxdb@sha256:28b27ba51abbddb2113c728b9fb5e23261733a9bceb995402012e69aa34273d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:e0e9f4602a6cc0632ea1dbc8910759c86b61ece94f6d5894382d6f1b9bcc30e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116713298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac89ea59315d99dec3c08bb1723cf2fbf03c2e11b2705cbc281417dbafc9c37e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:04:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 10:04:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 10:04:29 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 10:04:32 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Apr 2022 10:04:32 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Apr 2022 10:04:44 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Apr 2022 10:04:45 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Apr 2022 10:04:45 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Apr 2022 10:04:45 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Apr 2022 10:04:45 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Tue, 05 Apr 2022 10:04:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 10:04:45 GMT
CMD ["influxd"]
# Tue, 05 Apr 2022 10:04:45 GMT
EXPOSE 8086
# Tue, 05 Apr 2022 10:04:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Apr 2022 10:04:46 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Apr 2022 10:04:46 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Apr 2022 10:04:46 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e824989658cee0fcd8b3e27d03a0b79d4ae37c3b765afaff6f49d076d0d9dc42`  
		Last Modified: Tue, 05 Apr 2022 10:08:40 GMT  
		Size: 9.8 MB (9836774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6fbe7d281a77910553db440ca9d0c4b709850e35385fc474a9b9b11e55db697`  
		Last Modified: Tue, 05 Apr 2022 10:08:38 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288cce5ed27daa2927f6bc96c87e2581197832a7210cf5813f6d6cfea28afb7e`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 960.6 KB (960617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bae8b0ec17a5d9dbf1eb7e1e3953baef4edaf26b616fcbc218d817636d79d8`  
		Last Modified: Tue, 05 Apr 2022 10:08:45 GMT  
		Size: 103.1 MB (103090641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed8f2b193010cbe745a05d4a2907ef5592bcfc3fcf2f8dc3effc77b3db59171`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485640ccb69c912529e7b70604b5ab52e45aaf7fc93bbca67c021628d1f9d141`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6553ced84695f9c93dba30575941508f22f23786270f7612e99ebd6045d0ff5c`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 4.9 KB (4942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:3047f61d3f0deb8b68f3bb32f77ad1da4dc3f935344d6b4978e2b32978569b5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119819824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6df860f31be0a1452ff106725cb2865b8792e1cbca0eac815cee16c231129b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:11:26 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:11:29 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 04:11:30 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 04:11:31 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 04:11:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Apr 2022 04:11:35 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Apr 2022 04:11:48 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Apr 2022 04:11:48 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Apr 2022 04:11:49 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Apr 2022 04:11:51 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Apr 2022 04:11:52 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Tue, 05 Apr 2022 04:11:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:11:53 GMT
CMD ["influxd"]
# Tue, 05 Apr 2022 04:11:54 GMT
EXPOSE 8086
# Tue, 05 Apr 2022 04:11:55 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Apr 2022 04:11:56 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Apr 2022 04:11:57 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Apr 2022 04:11:58 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a37e642510b42e25dbe3082e57f33cdcdb65bad4e9468cd5c76fdb5015c7a`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc96d3454b87ca3f120022077fc7d0ff9477f1b5d1c99519902ae6eed0d7b90`  
		Last Modified: Tue, 05 Apr 2022 04:13:16 GMT  
		Size: 9.7 MB (9672606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af6c62b5230b53a6e53da9a15c422cfb18b955afc941e7b68331dd84392405c`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281a900a68fae805f39a9a8461f2ef4778a30b18c30f3bc6b2b85e0e02a107e4`  
		Last Modified: Tue, 05 Apr 2022 04:13:13 GMT  
		Size: 896.1 KB (896074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b07cab3429e5cb05ce350093f453086d575ea3fa8b8409fca4cabf4772f1b7`  
		Last Modified: Tue, 05 Apr 2022 04:13:23 GMT  
		Size: 106.5 MB (106526974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb98004947e4307dd97bd5347a40979529a3856593981fdf5be5939eddf45abe`  
		Last Modified: Tue, 05 Apr 2022 04:13:12 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a58f13a13141d9b8be4fdfd19c9bc68286c28872b5e103b27a68bf9af7b4ce`  
		Last Modified: Tue, 05 Apr 2022 04:13:12 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f057be72e1bceb8361f6e113dba8d132297ec659a68596020245db9a7db3d89`  
		Last Modified: Tue, 05 Apr 2022 04:13:13 GMT  
		Size: 4.9 KB (4948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1`

```console
$ docker pull influxdb@sha256:8192656c7f5df9a0644c6007b032b72f97bbe28fe58559e0e30113c477f3aefc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1` - linux; amd64

```console
$ docker pull influxdb@sha256:377d26871bf51a03582b24e243b52fd931462cdd576852648674a50ae3455172
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182909267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e8ddbfb7e30b1909b8c3784a925423126ac735c92c5387e6749d7960e48b4a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:39:11 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 20:39:11 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 20:39:15 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 20:39:29 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 11 May 2022 20:39:36 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 11 May 2022 20:39:37 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 11 May 2022 20:39:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 11 May 2022 20:39:41 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 20:39:41 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 20:39:41 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 20:39:41 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 11 May 2022 20:39:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:39:41 GMT
CMD ["influxd"]
# Wed, 11 May 2022 20:39:41 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:39:41 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 20:39:42 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 20:39:42 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 20:39:42 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7502ee2d408fa6f349bdf986640e67d1424ad5f35061bd24f4f0453aec2cbb50`  
		Last Modified: Wed, 11 May 2022 20:42:10 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c05c9cd211b391c71fb38c29a6f3f27091d07df73f89a9e77fd5e0b9ffc1fbd`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 961.0 KB (960961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a3e79edc6f5192b65075550c13765347b4ed373663d44d100f3edf6ef834b8`  
		Last Modified: Wed, 11 May 2022 20:42:35 GMT  
		Size: 108.3 MB (108324801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb6f47384e82cca5f96e28d6f1770bf65cb4bd3452cff344c3cec27cfe25175`  
		Last Modified: Wed, 11 May 2022 20:42:27 GMT  
		Size: 5.3 MB (5324489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243b4da7ca1e3b8cfb5190b99496643529c5ffae74ee2da971f1333c8ca04593`  
		Last Modified: Wed, 11 May 2022 20:42:26 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b2ff72f92970bc9d77e6e1dfcfa3d401c48d4246d10f3607c59896236230e8`  
		Last Modified: Wed, 11 May 2022 20:42:26 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2dd7f36fd22c17c0ef4ac658a362fc3641321a67195cb7c0617a0039ea592b`  
		Last Modified: Wed, 11 May 2022 20:42:26 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f218e6d81b708b0a948a357dcaa9b3d4e29058e70a493141666a8d611d2de839
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183417201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7730c343d91a100e9d5df9c0543da9686af73c168fae482ef6595f5043cea48b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:48:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 19:48:33 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 19:48:37 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 19:49:14 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 11 May 2022 19:49:27 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 11 May 2022 19:49:27 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 11 May 2022 19:49:32 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 11 May 2022 19:49:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 19:49:33 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 19:49:35 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 19:49:36 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 11 May 2022 19:49:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:49:37 GMT
CMD ["influxd"]
# Wed, 11 May 2022 19:49:38 GMT
EXPOSE 8086
# Wed, 11 May 2022 19:49:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 19:49:40 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 19:49:41 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 19:49:42 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88155b239d4be6cbe8982344c645615907ceb1698ecd859485dc47854b1ae2fe`  
		Last Modified: Wed, 11 May 2022 19:51:42 GMT  
		Size: 1.7 KB (1661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c422d6301995ca5b81c45b24404c961c0b1ccc9bd31c9a54b82363a29844af`  
		Last Modified: Wed, 11 May 2022 19:51:40 GMT  
		Size: 896.3 KB (896335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2a1bcba3cfa97c56f5f700056af14656c43fd841cf9be0b7ead1f591118c1a`  
		Last Modified: Wed, 11 May 2022 19:52:12 GMT  
		Size: 110.9 MB (110891607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae396e9af317087d3a5cae295dc8c8bbfe766bf3628f5a40863c245b241292f1`  
		Last Modified: Wed, 11 May 2022 19:52:03 GMT  
		Size: 4.9 MB (4906725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b285326acf4028690dca04e4e8490ad5e8452aac280f824d5551b94b84d4da5a`  
		Last Modified: Wed, 11 May 2022 19:52:03 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2defffd0191c125fc18fc7be8cfae6336abffb264a121b218aece0498c6a87ed`  
		Last Modified: Wed, 11 May 2022 19:52:02 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b7f2d0a4597531970a90b7cac96ca52afae8031d035c0f1700352cf4162f`  
		Last Modified: Wed, 11 May 2022 19:52:03 GMT  
		Size: 5.0 KB (5012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1-alpine`

```console
$ docker pull influxdb@sha256:e291151cb07898a6bda5e4089054062f680e8da3f5640739055b53eef1c32616
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b079b754eac2179d0fb6cbd917b17dabaa61ec4b84d9043a0145aa7c843abf73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127272053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b625457991728963436e2e73df9b29da7f25ac3ee39381d20a3250aedbf21bad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:04:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 10:04:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 10:04:29 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 10:04:32 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Apr 2022 10:05:20 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 05 Apr 2022 10:05:31 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 05 Apr 2022 10:05:32 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 05 Apr 2022 10:05:34 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 05 Apr 2022 10:05:35 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Apr 2022 10:05:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Apr 2022 10:05:35 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Apr 2022 10:05:35 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Tue, 05 Apr 2022 10:05:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 10:05:35 GMT
CMD ["influxd"]
# Tue, 05 Apr 2022 10:05:35 GMT
EXPOSE 8086
# Tue, 05 Apr 2022 10:05:36 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Apr 2022 10:05:36 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Apr 2022 10:05:36 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Apr 2022 10:05:36 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e824989658cee0fcd8b3e27d03a0b79d4ae37c3b765afaff6f49d076d0d9dc42`  
		Last Modified: Tue, 05 Apr 2022 10:08:40 GMT  
		Size: 9.8 MB (9836774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6fbe7d281a77910553db440ca9d0c4b709850e35385fc474a9b9b11e55db697`  
		Last Modified: Tue, 05 Apr 2022 10:08:38 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288cce5ed27daa2927f6bc96c87e2581197832a7210cf5813f6d6cfea28afb7e`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 960.6 KB (960617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa20fe4d2144c6d8b09c669080f4145864de9ae356d813f67bddf10ed780428`  
		Last Modified: Tue, 05 Apr 2022 10:09:05 GMT  
		Size: 108.3 MB (108324842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e25e004a13a0ffacc4e90bbdd9e5c7e28df4b9bad56bbc9ec937d480616870c`  
		Last Modified: Tue, 05 Apr 2022 10:08:58 GMT  
		Size: 5.3 MB (5324482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2ec7b1f550404a6e00cc084eefd5a5848dc8048e6d5574e3c7f394a32ca496`  
		Last Modified: Tue, 05 Apr 2022 10:08:57 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b331187d9cf6871ee12477b3eb2b2e80ae08e4ddad74fe84755de07e7ffa25ca`  
		Last Modified: Tue, 05 Apr 2022 10:08:57 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15f47f19904df14de1b0ee2d747e393e312a1486920fa4c780f4d00c752b740`  
		Last Modified: Tue, 05 Apr 2022 10:08:57 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4bdd7bd9a0fac859951bb481dcb08bcc509d5e6a837466175fe623918ede1419
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129091252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9771a96083d7ccceef184f3c0809a099c72f18747f4cba3e332285019ef65bd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:11:26 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:11:29 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 04:11:30 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 04:11:31 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 04:11:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Apr 2022 04:12:08 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 05 Apr 2022 04:12:17 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 05 Apr 2022 04:12:17 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 05 Apr 2022 04:12:21 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 05 Apr 2022 04:12:22 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Apr 2022 04:12:23 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Apr 2022 04:12:25 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Apr 2022 04:12:26 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Tue, 05 Apr 2022 04:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:12:27 GMT
CMD ["influxd"]
# Tue, 05 Apr 2022 04:12:28 GMT
EXPOSE 8086
# Tue, 05 Apr 2022 04:12:29 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Apr 2022 04:12:30 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Apr 2022 04:12:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Apr 2022 04:12:32 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a37e642510b42e25dbe3082e57f33cdcdb65bad4e9468cd5c76fdb5015c7a`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc96d3454b87ca3f120022077fc7d0ff9477f1b5d1c99519902ae6eed0d7b90`  
		Last Modified: Tue, 05 Apr 2022 04:13:16 GMT  
		Size: 9.7 MB (9672606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af6c62b5230b53a6e53da9a15c422cfb18b955afc941e7b68331dd84392405c`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281a900a68fae805f39a9a8461f2ef4778a30b18c30f3bc6b2b85e0e02a107e4`  
		Last Modified: Tue, 05 Apr 2022 04:13:13 GMT  
		Size: 896.1 KB (896074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1257d89608d6eb5bdb2b1dfd384f22aa999ecf1f5beb80cbdca7a7ea84462f`  
		Last Modified: Tue, 05 Apr 2022 04:13:45 GMT  
		Size: 110.9 MB (110891601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b43473396e5795083c86476af148fe3f0f258afd208843cc16b2a324fc8d3b`  
		Last Modified: Tue, 05 Apr 2022 04:13:37 GMT  
		Size: 4.9 MB (4906734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411147f402cae334bfe0485c46406abcaf0dba246f334c9fc098fdb2b7d98626`  
		Last Modified: Tue, 05 Apr 2022 04:13:36 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5c74a2e1dee8c1831544c3bf6c3368525e04eeecac99a6a3de888c847c79cb`  
		Last Modified: Tue, 05 Apr 2022 04:13:36 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5384858da93c08ecacc18d9c934002579ab9c0f55d7a42eddc6910abb09ceaa2`  
		Last Modified: Tue, 05 Apr 2022 04:13:36 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1.1`

```console
$ docker pull influxdb@sha256:8192656c7f5df9a0644c6007b032b72f97bbe28fe58559e0e30113c477f3aefc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1` - linux; amd64

```console
$ docker pull influxdb@sha256:377d26871bf51a03582b24e243b52fd931462cdd576852648674a50ae3455172
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182909267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e8ddbfb7e30b1909b8c3784a925423126ac735c92c5387e6749d7960e48b4a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:39:11 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 20:39:11 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 20:39:15 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 20:39:29 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 11 May 2022 20:39:36 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 11 May 2022 20:39:37 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 11 May 2022 20:39:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 11 May 2022 20:39:41 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 20:39:41 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 20:39:41 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 20:39:41 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 11 May 2022 20:39:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:39:41 GMT
CMD ["influxd"]
# Wed, 11 May 2022 20:39:41 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:39:41 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 20:39:42 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 20:39:42 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 20:39:42 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7502ee2d408fa6f349bdf986640e67d1424ad5f35061bd24f4f0453aec2cbb50`  
		Last Modified: Wed, 11 May 2022 20:42:10 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c05c9cd211b391c71fb38c29a6f3f27091d07df73f89a9e77fd5e0b9ffc1fbd`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 961.0 KB (960961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a3e79edc6f5192b65075550c13765347b4ed373663d44d100f3edf6ef834b8`  
		Last Modified: Wed, 11 May 2022 20:42:35 GMT  
		Size: 108.3 MB (108324801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb6f47384e82cca5f96e28d6f1770bf65cb4bd3452cff344c3cec27cfe25175`  
		Last Modified: Wed, 11 May 2022 20:42:27 GMT  
		Size: 5.3 MB (5324489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243b4da7ca1e3b8cfb5190b99496643529c5ffae74ee2da971f1333c8ca04593`  
		Last Modified: Wed, 11 May 2022 20:42:26 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b2ff72f92970bc9d77e6e1dfcfa3d401c48d4246d10f3607c59896236230e8`  
		Last Modified: Wed, 11 May 2022 20:42:26 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2dd7f36fd22c17c0ef4ac658a362fc3641321a67195cb7c0617a0039ea592b`  
		Last Modified: Wed, 11 May 2022 20:42:26 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f218e6d81b708b0a948a357dcaa9b3d4e29058e70a493141666a8d611d2de839
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183417201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7730c343d91a100e9d5df9c0543da9686af73c168fae482ef6595f5043cea48b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:48:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 19:48:33 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 19:48:37 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 19:49:14 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 11 May 2022 19:49:27 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 11 May 2022 19:49:27 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 11 May 2022 19:49:32 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 11 May 2022 19:49:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 19:49:33 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 19:49:35 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 19:49:36 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 11 May 2022 19:49:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:49:37 GMT
CMD ["influxd"]
# Wed, 11 May 2022 19:49:38 GMT
EXPOSE 8086
# Wed, 11 May 2022 19:49:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 19:49:40 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 19:49:41 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 19:49:42 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88155b239d4be6cbe8982344c645615907ceb1698ecd859485dc47854b1ae2fe`  
		Last Modified: Wed, 11 May 2022 19:51:42 GMT  
		Size: 1.7 KB (1661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c422d6301995ca5b81c45b24404c961c0b1ccc9bd31c9a54b82363a29844af`  
		Last Modified: Wed, 11 May 2022 19:51:40 GMT  
		Size: 896.3 KB (896335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2a1bcba3cfa97c56f5f700056af14656c43fd841cf9be0b7ead1f591118c1a`  
		Last Modified: Wed, 11 May 2022 19:52:12 GMT  
		Size: 110.9 MB (110891607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae396e9af317087d3a5cae295dc8c8bbfe766bf3628f5a40863c245b241292f1`  
		Last Modified: Wed, 11 May 2022 19:52:03 GMT  
		Size: 4.9 MB (4906725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b285326acf4028690dca04e4e8490ad5e8452aac280f824d5551b94b84d4da5a`  
		Last Modified: Wed, 11 May 2022 19:52:03 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2defffd0191c125fc18fc7be8cfae6336abffb264a121b218aece0498c6a87ed`  
		Last Modified: Wed, 11 May 2022 19:52:02 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da32b7f2d0a4597531970a90b7cac96ca52afae8031d035c0f1700352cf4162f`  
		Last Modified: Wed, 11 May 2022 19:52:03 GMT  
		Size: 5.0 KB (5012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1.1-alpine`

```console
$ docker pull influxdb@sha256:e291151cb07898a6bda5e4089054062f680e8da3f5640739055b53eef1c32616
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b079b754eac2179d0fb6cbd917b17dabaa61ec4b84d9043a0145aa7c843abf73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127272053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b625457991728963436e2e73df9b29da7f25ac3ee39381d20a3250aedbf21bad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:04:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 10:04:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 10:04:29 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 10:04:32 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Apr 2022 10:05:20 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 05 Apr 2022 10:05:31 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 05 Apr 2022 10:05:32 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 05 Apr 2022 10:05:34 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 05 Apr 2022 10:05:35 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Apr 2022 10:05:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Apr 2022 10:05:35 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Apr 2022 10:05:35 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Tue, 05 Apr 2022 10:05:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 10:05:35 GMT
CMD ["influxd"]
# Tue, 05 Apr 2022 10:05:35 GMT
EXPOSE 8086
# Tue, 05 Apr 2022 10:05:36 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Apr 2022 10:05:36 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Apr 2022 10:05:36 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Apr 2022 10:05:36 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e824989658cee0fcd8b3e27d03a0b79d4ae37c3b765afaff6f49d076d0d9dc42`  
		Last Modified: Tue, 05 Apr 2022 10:08:40 GMT  
		Size: 9.8 MB (9836774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6fbe7d281a77910553db440ca9d0c4b709850e35385fc474a9b9b11e55db697`  
		Last Modified: Tue, 05 Apr 2022 10:08:38 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288cce5ed27daa2927f6bc96c87e2581197832a7210cf5813f6d6cfea28afb7e`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 960.6 KB (960617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa20fe4d2144c6d8b09c669080f4145864de9ae356d813f67bddf10ed780428`  
		Last Modified: Tue, 05 Apr 2022 10:09:05 GMT  
		Size: 108.3 MB (108324842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e25e004a13a0ffacc4e90bbdd9e5c7e28df4b9bad56bbc9ec937d480616870c`  
		Last Modified: Tue, 05 Apr 2022 10:08:58 GMT  
		Size: 5.3 MB (5324482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2ec7b1f550404a6e00cc084eefd5a5848dc8048e6d5574e3c7f394a32ca496`  
		Last Modified: Tue, 05 Apr 2022 10:08:57 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b331187d9cf6871ee12477b3eb2b2e80ae08e4ddad74fe84755de07e7ffa25ca`  
		Last Modified: Tue, 05 Apr 2022 10:08:57 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15f47f19904df14de1b0ee2d747e393e312a1486920fa4c780f4d00c752b740`  
		Last Modified: Tue, 05 Apr 2022 10:08:57 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4bdd7bd9a0fac859951bb481dcb08bcc509d5e6a837466175fe623918ede1419
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129091252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9771a96083d7ccceef184f3c0809a099c72f18747f4cba3e332285019ef65bd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:11:26 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:11:29 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 04:11:30 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 04:11:31 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 04:11:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Apr 2022 04:12:08 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 05 Apr 2022 04:12:17 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 05 Apr 2022 04:12:17 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 05 Apr 2022 04:12:21 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 05 Apr 2022 04:12:22 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Apr 2022 04:12:23 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Apr 2022 04:12:25 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Apr 2022 04:12:26 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Tue, 05 Apr 2022 04:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 04:12:27 GMT
CMD ["influxd"]
# Tue, 05 Apr 2022 04:12:28 GMT
EXPOSE 8086
# Tue, 05 Apr 2022 04:12:29 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Apr 2022 04:12:30 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Apr 2022 04:12:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Apr 2022 04:12:32 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a37e642510b42e25dbe3082e57f33cdcdb65bad4e9468cd5c76fdb5015c7a`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc96d3454b87ca3f120022077fc7d0ff9477f1b5d1c99519902ae6eed0d7b90`  
		Last Modified: Tue, 05 Apr 2022 04:13:16 GMT  
		Size: 9.7 MB (9672606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af6c62b5230b53a6e53da9a15c422cfb18b955afc941e7b68331dd84392405c`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281a900a68fae805f39a9a8461f2ef4778a30b18c30f3bc6b2b85e0e02a107e4`  
		Last Modified: Tue, 05 Apr 2022 04:13:13 GMT  
		Size: 896.1 KB (896074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1257d89608d6eb5bdb2b1dfd384f22aa999ecf1f5beb80cbdca7a7ea84462f`  
		Last Modified: Tue, 05 Apr 2022 04:13:45 GMT  
		Size: 110.9 MB (110891601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b43473396e5795083c86476af148fe3f0f258afd208843cc16b2a324fc8d3b`  
		Last Modified: Tue, 05 Apr 2022 04:13:37 GMT  
		Size: 4.9 MB (4906734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411147f402cae334bfe0485c46406abcaf0dba246f334c9fc098fdb2b7d98626`  
		Last Modified: Tue, 05 Apr 2022 04:13:36 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5c74a2e1dee8c1831544c3bf6c3368525e04eeecac99a6a3de888c847c79cb`  
		Last Modified: Tue, 05 Apr 2022 04:13:36 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5384858da93c08ecacc18d9c934002579ab9c0f55d7a42eddc6910abb09ceaa2`  
		Last Modified: Tue, 05 Apr 2022 04:13:36 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.2`

```console
$ docker pull influxdb@sha256:30f713486962e10bd6a53132c911a22dd0ea853e9c8c1ee3d2ed6c9798db2630
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.2` - linux; amd64

```console
$ docker pull influxdb@sha256:5e01c523954fade7f1ed4960444fdef7b5f5a812a6f214c9fdb9af76279c6eac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.8 MB (181847377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd94853c72a693e29c839030e65647007f4d6425c95591afd57a918305ccb10d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:39:11 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 20:39:11 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 20:39:15 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 20:39:47 GMT
ENV INFLUXDB_VERSION=2.2.0
# Wed, 11 May 2022 20:39:55 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 11 May 2022 20:39:55 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 11 May 2022 20:39:59 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 11 May 2022 20:39:59 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 20:39:59 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 20:39:59 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 20:39:59 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 11 May 2022 20:40:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:40:00 GMT
CMD ["influxd"]
# Wed, 11 May 2022 20:40:00 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:40:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 20:40:00 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 20:40:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 20:40:00 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7502ee2d408fa6f349bdf986640e67d1424ad5f35061bd24f4f0453aec2cbb50`  
		Last Modified: Wed, 11 May 2022 20:42:10 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c05c9cd211b391c71fb38c29a6f3f27091d07df73f89a9e77fd5e0b9ffc1fbd`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 961.0 KB (960961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08e617d243b846b1ac37f608fd195168497d32f8ecfa52ae383612181dfee08`  
		Last Modified: Wed, 11 May 2022 20:42:54 GMT  
		Size: 107.2 MB (107220548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710c31994f623e9e0514928f2d9ecbb690e6a6c91c61eb823756eddb40340dd1`  
		Last Modified: Wed, 11 May 2022 20:42:47 GMT  
		Size: 5.4 MB (5366854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7570547b5a75f38bd8c852c64a84e80a7f58608073dfa28b66578c77cb2bb58`  
		Last Modified: Wed, 11 May 2022 20:42:46 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be227de5be940f2a9982bdf69fa008f0734c6366a90223225fd82b90c1af0a`  
		Last Modified: Wed, 11 May 2022 20:42:46 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdae3cd3e170f28072f588bd3af2306df08b15621dc682ef98c3dad4598b4`  
		Last Modified: Wed, 11 May 2022 20:42:46 GMT  
		Size: 5.0 KB (5013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.2` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:395dcf8826b83f4290ce2dd5574379619dfd661a5baa0c05dba37d2af2650423
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.4 MB (182449384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2837550813ebce80ff49242f3a87487213974dc3af2659aabbeb1a9994a40011`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:48:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 19:48:33 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 19:48:37 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 19:49:54 GMT
ENV INFLUXDB_VERSION=2.2.0
# Wed, 11 May 2022 19:50:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 11 May 2022 19:50:11 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 11 May 2022 19:50:25 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 11 May 2022 19:50:26 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 19:50:27 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 19:50:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 19:50:30 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 11 May 2022 19:50:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:50:31 GMT
CMD ["influxd"]
# Wed, 11 May 2022 19:50:32 GMT
EXPOSE 8086
# Wed, 11 May 2022 19:50:33 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 19:50:34 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 19:50:35 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 19:50:36 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88155b239d4be6cbe8982344c645615907ceb1698ecd859485dc47854b1ae2fe`  
		Last Modified: Wed, 11 May 2022 19:51:42 GMT  
		Size: 1.7 KB (1661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c422d6301995ca5b81c45b24404c961c0b1ccc9bd31c9a54b82363a29844af`  
		Last Modified: Wed, 11 May 2022 19:51:40 GMT  
		Size: 896.3 KB (896335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e321e30cf1a2a95a6259bfcfc41a3e8be7f54261e381777f1891c06430607c2`  
		Last Modified: Wed, 11 May 2022 19:52:35 GMT  
		Size: 109.9 MB (109877888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f051e75770e880c5702a2c88333dd6d8193c0428229ed8f83121a5f845a7084`  
		Last Modified: Wed, 11 May 2022 19:52:26 GMT  
		Size: 5.0 MB (4952624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e58f19231e2ff7828cd469a4f6c932dcadaa4400975d3e4dee7fc05563466c1`  
		Last Modified: Wed, 11 May 2022 19:52:25 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89312617d3ec55a9566523ef5b44e51431414952e1baf536243edd5246debafb`  
		Last Modified: Wed, 11 May 2022 19:52:25 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33639c3ff5f33654d14405f44bbdad9a03f4225b36091e230d7d051828bf738`  
		Last Modified: Wed, 11 May 2022 19:52:25 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.2-alpine`

```console
$ docker pull influxdb@sha256:e54e532b67a466296fd229046de57ea364ec3fc311024fb6cf04ef8b3f826724
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.2-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:944d3703e0d229c834124702b52cb9a38ba70148cbe9a91047549a6f1d4100c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126210124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f915cf00224d1e1471d7f995be37339638c7a1f48ff534622ba6de7979fa918`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:04:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 10:04:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 10:04:29 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 10:04:32 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Apr 2022 22:23:52 GMT
ENV INFLUXDB_VERSION=2.2.0
# Thu, 07 Apr 2022 22:23:59 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 07 Apr 2022 22:23:59 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 07 Apr 2022 22:24:02 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 07 Apr 2022 22:24:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Apr 2022 22:24:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Apr 2022 22:24:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Apr 2022 22:24:03 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 07 Apr 2022 22:24:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:24:03 GMT
CMD ["influxd"]
# Thu, 07 Apr 2022 22:24:03 GMT
EXPOSE 8086
# Thu, 07 Apr 2022 22:24:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Apr 2022 22:24:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Apr 2022 22:24:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Apr 2022 22:24:03 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e824989658cee0fcd8b3e27d03a0b79d4ae37c3b765afaff6f49d076d0d9dc42`  
		Last Modified: Tue, 05 Apr 2022 10:08:40 GMT  
		Size: 9.8 MB (9836774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6fbe7d281a77910553db440ca9d0c4b709850e35385fc474a9b9b11e55db697`  
		Last Modified: Tue, 05 Apr 2022 10:08:38 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288cce5ed27daa2927f6bc96c87e2581197832a7210cf5813f6d6cfea28afb7e`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 960.6 KB (960617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda4cec68da03e4a2c0505bf914835d468d2381a18d7f5523dff04a4104548f0`  
		Last Modified: Thu, 07 Apr 2022 22:26:22 GMT  
		Size: 107.2 MB (107220530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1803721aa5af5cf4595b4f6d1ec77b85528f1d017159ee2795fbc7be1754dfd`  
		Last Modified: Thu, 07 Apr 2022 22:26:16 GMT  
		Size: 5.4 MB (5366860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698fbf636ae0f2c376b436111ab290b41ba6a62006984cba8613f717c197999a`  
		Last Modified: Thu, 07 Apr 2022 22:26:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d763963a1494238194f51588c6093ef14a5d5035d0b15370b6f8064484d6ab`  
		Last Modified: Thu, 07 Apr 2022 22:26:15 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab47c4b7f6fac482d97780e3e699c1976910bcda6881cd8ec4d264377e326bc5`  
		Last Modified: Thu, 07 Apr 2022 22:26:15 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4e04338689d6ae55cb2e51f9574dff5db9ecdabfefc979f32c19dd8109a36245
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128123536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d2948df1c4115ccad9b6da3e19299c8f6b1b80370b2aae23233b7e424d3713`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:11:26 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:11:29 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 04:11:30 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 04:11:31 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 04:11:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Apr 2022 22:41:04 GMT
ENV INFLUXDB_VERSION=2.2.0
# Thu, 07 Apr 2022 22:41:14 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 07 Apr 2022 22:41:15 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 07 Apr 2022 22:41:19 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 07 Apr 2022 22:41:20 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Apr 2022 22:41:21 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Apr 2022 22:41:23 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Apr 2022 22:41:24 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 07 Apr 2022 22:41:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:41:25 GMT
CMD ["influxd"]
# Thu, 07 Apr 2022 22:41:26 GMT
EXPOSE 8086
# Thu, 07 Apr 2022 22:41:27 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Apr 2022 22:41:28 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Apr 2022 22:41:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Apr 2022 22:41:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a37e642510b42e25dbe3082e57f33cdcdb65bad4e9468cd5c76fdb5015c7a`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc96d3454b87ca3f120022077fc7d0ff9477f1b5d1c99519902ae6eed0d7b90`  
		Last Modified: Tue, 05 Apr 2022 04:13:16 GMT  
		Size: 9.7 MB (9672606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af6c62b5230b53a6e53da9a15c422cfb18b955afc941e7b68331dd84392405c`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281a900a68fae805f39a9a8461f2ef4778a30b18c30f3bc6b2b85e0e02a107e4`  
		Last Modified: Tue, 05 Apr 2022 04:13:13 GMT  
		Size: 896.1 KB (896074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5fa0ea408fd6ffd1ee82e3ea8008fc3465cafabaeae75f18d2cf348351c1e4`  
		Last Modified: Thu, 07 Apr 2022 22:42:47 GMT  
		Size: 109.9 MB (109877972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960db3c3158879adcdf59bc12c3c38c1af5913bd9a84977150e7d8aeb95c801a`  
		Last Modified: Thu, 07 Apr 2022 22:42:40 GMT  
		Size: 5.0 MB (4952646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df20c8d48e4fd0c3e42141cc86af9e54a4216943054d882550dd9a77be5c77dd`  
		Last Modified: Thu, 07 Apr 2022 22:42:39 GMT  
		Size: 207.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd86c97dd0108cc33d98391fe4637c43e2ff7ad8dcb9f7663237e312c2fddb8`  
		Last Modified: Thu, 07 Apr 2022 22:42:38 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf6e9a8ef77f045422b81ae5a910ea9b4886105ed0d01777f0aead72441f00f`  
		Last Modified: Thu, 07 Apr 2022 22:42:38 GMT  
		Size: 5.0 KB (5018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.2.0`

```console
$ docker pull influxdb@sha256:30f713486962e10bd6a53132c911a22dd0ea853e9c8c1ee3d2ed6c9798db2630
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:5e01c523954fade7f1ed4960444fdef7b5f5a812a6f214c9fdb9af76279c6eac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.8 MB (181847377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd94853c72a693e29c839030e65647007f4d6425c95591afd57a918305ccb10d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:39:11 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 20:39:11 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 20:39:15 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 20:39:47 GMT
ENV INFLUXDB_VERSION=2.2.0
# Wed, 11 May 2022 20:39:55 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 11 May 2022 20:39:55 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 11 May 2022 20:39:59 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 11 May 2022 20:39:59 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 20:39:59 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 20:39:59 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 20:39:59 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 11 May 2022 20:40:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:40:00 GMT
CMD ["influxd"]
# Wed, 11 May 2022 20:40:00 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:40:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 20:40:00 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 20:40:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 20:40:00 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7502ee2d408fa6f349bdf986640e67d1424ad5f35061bd24f4f0453aec2cbb50`  
		Last Modified: Wed, 11 May 2022 20:42:10 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c05c9cd211b391c71fb38c29a6f3f27091d07df73f89a9e77fd5e0b9ffc1fbd`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 961.0 KB (960961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08e617d243b846b1ac37f608fd195168497d32f8ecfa52ae383612181dfee08`  
		Last Modified: Wed, 11 May 2022 20:42:54 GMT  
		Size: 107.2 MB (107220548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710c31994f623e9e0514928f2d9ecbb690e6a6c91c61eb823756eddb40340dd1`  
		Last Modified: Wed, 11 May 2022 20:42:47 GMT  
		Size: 5.4 MB (5366854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7570547b5a75f38bd8c852c64a84e80a7f58608073dfa28b66578c77cb2bb58`  
		Last Modified: Wed, 11 May 2022 20:42:46 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be227de5be940f2a9982bdf69fa008f0734c6366a90223225fd82b90c1af0a`  
		Last Modified: Wed, 11 May 2022 20:42:46 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdae3cd3e170f28072f588bd3af2306df08b15621dc682ef98c3dad4598b4`  
		Last Modified: Wed, 11 May 2022 20:42:46 GMT  
		Size: 5.0 KB (5013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:395dcf8826b83f4290ce2dd5574379619dfd661a5baa0c05dba37d2af2650423
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.4 MB (182449384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2837550813ebce80ff49242f3a87487213974dc3af2659aabbeb1a9994a40011`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:48:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 19:48:33 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 19:48:37 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 19:49:54 GMT
ENV INFLUXDB_VERSION=2.2.0
# Wed, 11 May 2022 19:50:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 11 May 2022 19:50:11 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 11 May 2022 19:50:25 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 11 May 2022 19:50:26 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 19:50:27 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 19:50:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 19:50:30 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 11 May 2022 19:50:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:50:31 GMT
CMD ["influxd"]
# Wed, 11 May 2022 19:50:32 GMT
EXPOSE 8086
# Wed, 11 May 2022 19:50:33 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 19:50:34 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 19:50:35 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 19:50:36 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88155b239d4be6cbe8982344c645615907ceb1698ecd859485dc47854b1ae2fe`  
		Last Modified: Wed, 11 May 2022 19:51:42 GMT  
		Size: 1.7 KB (1661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c422d6301995ca5b81c45b24404c961c0b1ccc9bd31c9a54b82363a29844af`  
		Last Modified: Wed, 11 May 2022 19:51:40 GMT  
		Size: 896.3 KB (896335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e321e30cf1a2a95a6259bfcfc41a3e8be7f54261e381777f1891c06430607c2`  
		Last Modified: Wed, 11 May 2022 19:52:35 GMT  
		Size: 109.9 MB (109877888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f051e75770e880c5702a2c88333dd6d8193c0428229ed8f83121a5f845a7084`  
		Last Modified: Wed, 11 May 2022 19:52:26 GMT  
		Size: 5.0 MB (4952624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e58f19231e2ff7828cd469a4f6c932dcadaa4400975d3e4dee7fc05563466c1`  
		Last Modified: Wed, 11 May 2022 19:52:25 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89312617d3ec55a9566523ef5b44e51431414952e1baf536243edd5246debafb`  
		Last Modified: Wed, 11 May 2022 19:52:25 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33639c3ff5f33654d14405f44bbdad9a03f4225b36091e230d7d051828bf738`  
		Last Modified: Wed, 11 May 2022 19:52:25 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.2.0-alpine`

```console
$ docker pull influxdb@sha256:e54e532b67a466296fd229046de57ea364ec3fc311024fb6cf04ef8b3f826724
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.2.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:944d3703e0d229c834124702b52cb9a38ba70148cbe9a91047549a6f1d4100c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126210124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f915cf00224d1e1471d7f995be37339638c7a1f48ff534622ba6de7979fa918`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:04:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 10:04:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 10:04:29 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 10:04:32 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Apr 2022 22:23:52 GMT
ENV INFLUXDB_VERSION=2.2.0
# Thu, 07 Apr 2022 22:23:59 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 07 Apr 2022 22:23:59 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 07 Apr 2022 22:24:02 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 07 Apr 2022 22:24:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Apr 2022 22:24:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Apr 2022 22:24:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Apr 2022 22:24:03 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 07 Apr 2022 22:24:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:24:03 GMT
CMD ["influxd"]
# Thu, 07 Apr 2022 22:24:03 GMT
EXPOSE 8086
# Thu, 07 Apr 2022 22:24:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Apr 2022 22:24:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Apr 2022 22:24:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Apr 2022 22:24:03 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e824989658cee0fcd8b3e27d03a0b79d4ae37c3b765afaff6f49d076d0d9dc42`  
		Last Modified: Tue, 05 Apr 2022 10:08:40 GMT  
		Size: 9.8 MB (9836774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6fbe7d281a77910553db440ca9d0c4b709850e35385fc474a9b9b11e55db697`  
		Last Modified: Tue, 05 Apr 2022 10:08:38 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288cce5ed27daa2927f6bc96c87e2581197832a7210cf5813f6d6cfea28afb7e`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 960.6 KB (960617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda4cec68da03e4a2c0505bf914835d468d2381a18d7f5523dff04a4104548f0`  
		Last Modified: Thu, 07 Apr 2022 22:26:22 GMT  
		Size: 107.2 MB (107220530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1803721aa5af5cf4595b4f6d1ec77b85528f1d017159ee2795fbc7be1754dfd`  
		Last Modified: Thu, 07 Apr 2022 22:26:16 GMT  
		Size: 5.4 MB (5366860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698fbf636ae0f2c376b436111ab290b41ba6a62006984cba8613f717c197999a`  
		Last Modified: Thu, 07 Apr 2022 22:26:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d763963a1494238194f51588c6093ef14a5d5035d0b15370b6f8064484d6ab`  
		Last Modified: Thu, 07 Apr 2022 22:26:15 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab47c4b7f6fac482d97780e3e699c1976910bcda6881cd8ec4d264377e326bc5`  
		Last Modified: Thu, 07 Apr 2022 22:26:15 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4e04338689d6ae55cb2e51f9574dff5db9ecdabfefc979f32c19dd8109a36245
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128123536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d2948df1c4115ccad9b6da3e19299c8f6b1b80370b2aae23233b7e424d3713`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:11:26 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:11:29 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 04:11:30 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 04:11:31 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 04:11:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Apr 2022 22:41:04 GMT
ENV INFLUXDB_VERSION=2.2.0
# Thu, 07 Apr 2022 22:41:14 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 07 Apr 2022 22:41:15 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 07 Apr 2022 22:41:19 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 07 Apr 2022 22:41:20 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Apr 2022 22:41:21 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Apr 2022 22:41:23 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Apr 2022 22:41:24 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 07 Apr 2022 22:41:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:41:25 GMT
CMD ["influxd"]
# Thu, 07 Apr 2022 22:41:26 GMT
EXPOSE 8086
# Thu, 07 Apr 2022 22:41:27 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Apr 2022 22:41:28 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Apr 2022 22:41:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Apr 2022 22:41:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a37e642510b42e25dbe3082e57f33cdcdb65bad4e9468cd5c76fdb5015c7a`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc96d3454b87ca3f120022077fc7d0ff9477f1b5d1c99519902ae6eed0d7b90`  
		Last Modified: Tue, 05 Apr 2022 04:13:16 GMT  
		Size: 9.7 MB (9672606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af6c62b5230b53a6e53da9a15c422cfb18b955afc941e7b68331dd84392405c`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281a900a68fae805f39a9a8461f2ef4778a30b18c30f3bc6b2b85e0e02a107e4`  
		Last Modified: Tue, 05 Apr 2022 04:13:13 GMT  
		Size: 896.1 KB (896074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5fa0ea408fd6ffd1ee82e3ea8008fc3465cafabaeae75f18d2cf348351c1e4`  
		Last Modified: Thu, 07 Apr 2022 22:42:47 GMT  
		Size: 109.9 MB (109877972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960db3c3158879adcdf59bc12c3c38c1af5913bd9a84977150e7d8aeb95c801a`  
		Last Modified: Thu, 07 Apr 2022 22:42:40 GMT  
		Size: 5.0 MB (4952646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df20c8d48e4fd0c3e42141cc86af9e54a4216943054d882550dd9a77be5c77dd`  
		Last Modified: Thu, 07 Apr 2022 22:42:39 GMT  
		Size: 207.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd86c97dd0108cc33d98391fe4637c43e2ff7ad8dcb9f7663237e312c2fddb8`  
		Last Modified: Thu, 07 Apr 2022 22:42:38 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf6e9a8ef77f045422b81ae5a910ea9b4886105ed0d01777f0aead72441f00f`  
		Last Modified: Thu, 07 Apr 2022 22:42:38 GMT  
		Size: 5.0 KB (5018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:e54e532b67a466296fd229046de57ea364ec3fc311024fb6cf04ef8b3f826724
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:944d3703e0d229c834124702b52cb9a38ba70148cbe9a91047549a6f1d4100c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126210124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f915cf00224d1e1471d7f995be37339638c7a1f48ff534622ba6de7979fa918`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:04:28 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 10:04:29 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 10:04:29 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 10:04:32 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Apr 2022 22:23:52 GMT
ENV INFLUXDB_VERSION=2.2.0
# Thu, 07 Apr 2022 22:23:59 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 07 Apr 2022 22:23:59 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 07 Apr 2022 22:24:02 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 07 Apr 2022 22:24:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Apr 2022 22:24:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Apr 2022 22:24:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Apr 2022 22:24:03 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 07 Apr 2022 22:24:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:24:03 GMT
CMD ["influxd"]
# Thu, 07 Apr 2022 22:24:03 GMT
EXPOSE 8086
# Thu, 07 Apr 2022 22:24:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Apr 2022 22:24:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Apr 2022 22:24:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Apr 2022 22:24:03 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e824989658cee0fcd8b3e27d03a0b79d4ae37c3b765afaff6f49d076d0d9dc42`  
		Last Modified: Tue, 05 Apr 2022 10:08:40 GMT  
		Size: 9.8 MB (9836774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6fbe7d281a77910553db440ca9d0c4b709850e35385fc474a9b9b11e55db697`  
		Last Modified: Tue, 05 Apr 2022 10:08:38 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288cce5ed27daa2927f6bc96c87e2581197832a7210cf5813f6d6cfea28afb7e`  
		Last Modified: Tue, 05 Apr 2022 10:08:36 GMT  
		Size: 960.6 KB (960617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda4cec68da03e4a2c0505bf914835d468d2381a18d7f5523dff04a4104548f0`  
		Last Modified: Thu, 07 Apr 2022 22:26:22 GMT  
		Size: 107.2 MB (107220530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1803721aa5af5cf4595b4f6d1ec77b85528f1d017159ee2795fbc7be1754dfd`  
		Last Modified: Thu, 07 Apr 2022 22:26:16 GMT  
		Size: 5.4 MB (5366860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698fbf636ae0f2c376b436111ab290b41ba6a62006984cba8613f717c197999a`  
		Last Modified: Thu, 07 Apr 2022 22:26:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d763963a1494238194f51588c6093ef14a5d5035d0b15370b6f8064484d6ab`  
		Last Modified: Thu, 07 Apr 2022 22:26:15 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab47c4b7f6fac482d97780e3e699c1976910bcda6881cd8ec4d264377e326bc5`  
		Last Modified: Thu, 07 Apr 2022 22:26:15 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4e04338689d6ae55cb2e51f9574dff5db9ecdabfefc979f32c19dd8109a36245
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128123536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d2948df1c4115ccad9b6da3e19299c8f6b1b80370b2aae23233b7e424d3713`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:11:26 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:11:29 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 05 Apr 2022 04:11:30 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 05 Apr 2022 04:11:31 GMT
ENV GOSU_VER=1.12
# Tue, 05 Apr 2022 04:11:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Apr 2022 22:41:04 GMT
ENV INFLUXDB_VERSION=2.2.0
# Thu, 07 Apr 2022 22:41:14 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 07 Apr 2022 22:41:15 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 07 Apr 2022 22:41:19 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 07 Apr 2022 22:41:20 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 07 Apr 2022 22:41:21 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 07 Apr 2022 22:41:23 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 07 Apr 2022 22:41:24 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 07 Apr 2022 22:41:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:41:25 GMT
CMD ["influxd"]
# Thu, 07 Apr 2022 22:41:26 GMT
EXPOSE 8086
# Thu, 07 Apr 2022 22:41:27 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 07 Apr 2022 22:41:28 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 07 Apr 2022 22:41:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 07 Apr 2022 22:41:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964a37e642510b42e25dbe3082e57f33cdcdb65bad4e9468cd5c76fdb5015c7a`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc96d3454b87ca3f120022077fc7d0ff9477f1b5d1c99519902ae6eed0d7b90`  
		Last Modified: Tue, 05 Apr 2022 04:13:16 GMT  
		Size: 9.7 MB (9672606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af6c62b5230b53a6e53da9a15c422cfb18b955afc941e7b68331dd84392405c`  
		Last Modified: Tue, 05 Apr 2022 04:13:15 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281a900a68fae805f39a9a8461f2ef4778a30b18c30f3bc6b2b85e0e02a107e4`  
		Last Modified: Tue, 05 Apr 2022 04:13:13 GMT  
		Size: 896.1 KB (896074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5fa0ea408fd6ffd1ee82e3ea8008fc3465cafabaeae75f18d2cf348351c1e4`  
		Last Modified: Thu, 07 Apr 2022 22:42:47 GMT  
		Size: 109.9 MB (109877972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960db3c3158879adcdf59bc12c3c38c1af5913bd9a84977150e7d8aeb95c801a`  
		Last Modified: Thu, 07 Apr 2022 22:42:40 GMT  
		Size: 5.0 MB (4952646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df20c8d48e4fd0c3e42141cc86af9e54a4216943054d882550dd9a77be5c77dd`  
		Last Modified: Thu, 07 Apr 2022 22:42:39 GMT  
		Size: 207.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd86c97dd0108cc33d98391fe4637c43e2ff7ad8dcb9f7663237e312c2fddb8`  
		Last Modified: Thu, 07 Apr 2022 22:42:38 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf6e9a8ef77f045422b81ae5a910ea9b4886105ed0d01777f0aead72441f00f`  
		Last Modified: Thu, 07 Apr 2022 22:42:38 GMT  
		Size: 5.0 KB (5018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:5b0b5c4d626c6486c1bd33a598500229e30086e622103392e582c08f5af2c961
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:b1490b4e0037c9ec65d02818851e0229ccaad0c3c1d0300418e4142a731258d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117786946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d87cf020fc2a813256c8a935cc37c72fdc75869a998b4a87cf875891e2032044`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:38:33 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 11 May 2022 20:38:39 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 11 May 2022 20:38:40 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 11 May 2022 20:38:40 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:38:40 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 20:38:40 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 11 May 2022 20:38:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 11 May 2022 20:38:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:38:40 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565d52697dc7657483e66de35859480ec0bb9fdce45fd76e1512042633b2b15`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3623f788a4d6e2cd10a137d1b81983e5a858e33ad4bf4cad01f47d90b8084200`  
		Last Modified: Wed, 11 May 2022 20:41:10 GMT  
		Size: 56.7 MB (56709115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242df9a8b2f790b9a34d5f6b7a55989913b076aa27425f3709b3ebaab620ffbc`  
		Last Modified: Wed, 11 May 2022 20:41:02 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b27dbc8850d0b6695b7b1d943292c56a290cf4786773c0e32e8639d16e4bd7`  
		Last Modified: Wed, 11 May 2022 20:41:02 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433d58cd840d19993e454795631954fac3097458b2b862700b9954bd383b1e4a`  
		Last Modified: Wed, 11 May 2022 20:41:02 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:5b6f51f9283101e2260d04e4ec6e97e6ac6b42906de0330d245556207485ff9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ffe5860e830f75f1ecc06f6d9ef5131783a4009bf8c178a202b221b7090991d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60799475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c51bbfae48c946a370eace3f872988f7daf93c3ee3586f383c6165ed132c4760`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:02:50 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 10:03:43 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 07 Apr 2022 22:22:53 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 07 Apr 2022 22:22:54 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 07 Apr 2022 22:22:54 GMT
EXPOSE 8086
# Thu, 07 Apr 2022 22:22:54 GMT
VOLUME [/var/lib/influxdb]
# Thu, 07 Apr 2022 22:22:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 07 Apr 2022 22:22:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 07 Apr 2022 22:22:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:22:54 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a82c2bf0b07bc97e48386998fdb52307a711c8cde52325fb999e1b7a0f0073`  
		Last Modified: Tue, 05 Apr 2022 10:06:22 GMT  
		Size: 1.5 MB (1475485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d253e65fc0c40504c5ab7ed8891c7535ce694e62e9b315612518257a49a27e`  
		Last Modified: Thu, 07 Apr 2022 22:24:53 GMT  
		Size: 56.5 MB (56503671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c14b9a988386b736ef6a259676adf189b9aee692453b5a41173a23bd2aed93e`  
		Last Modified: Thu, 07 Apr 2022 22:24:46 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1e32c4578db25e99bb2f5fbd9bae12550160681dd612559a2fdb24774b6636`  
		Last Modified: Thu, 07 Apr 2022 22:24:46 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3641a605f831a5d23969cb82df4b923d91d0377459df0169f7c92d5a15449a9`  
		Last Modified: Thu, 07 Apr 2022 22:24:46 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:30f713486962e10bd6a53132c911a22dd0ea853e9c8c1ee3d2ed6c9798db2630
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:5e01c523954fade7f1ed4960444fdef7b5f5a812a6f214c9fdb9af76279c6eac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.8 MB (181847377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd94853c72a693e29c839030e65647007f4d6425c95591afd57a918305ccb10d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:39:11 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 20:39:11 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 20:39:15 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 20:39:47 GMT
ENV INFLUXDB_VERSION=2.2.0
# Wed, 11 May 2022 20:39:55 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 11 May 2022 20:39:55 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 11 May 2022 20:39:59 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 11 May 2022 20:39:59 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 20:39:59 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 20:39:59 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 20:39:59 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 11 May 2022 20:40:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:40:00 GMT
CMD ["influxd"]
# Wed, 11 May 2022 20:40:00 GMT
EXPOSE 8086
# Wed, 11 May 2022 20:40:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 20:40:00 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 20:40:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 20:40:00 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7502ee2d408fa6f349bdf986640e67d1424ad5f35061bd24f4f0453aec2cbb50`  
		Last Modified: Wed, 11 May 2022 20:42:10 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c05c9cd211b391c71fb38c29a6f3f27091d07df73f89a9e77fd5e0b9ffc1fbd`  
		Last Modified: Wed, 11 May 2022 20:42:07 GMT  
		Size: 961.0 KB (960961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08e617d243b846b1ac37f608fd195168497d32f8ecfa52ae383612181dfee08`  
		Last Modified: Wed, 11 May 2022 20:42:54 GMT  
		Size: 107.2 MB (107220548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710c31994f623e9e0514928f2d9ecbb690e6a6c91c61eb823756eddb40340dd1`  
		Last Modified: Wed, 11 May 2022 20:42:47 GMT  
		Size: 5.4 MB (5366854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7570547b5a75f38bd8c852c64a84e80a7f58608073dfa28b66578c77cb2bb58`  
		Last Modified: Wed, 11 May 2022 20:42:46 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be227de5be940f2a9982bdf69fa008f0734c6366a90223225fd82b90c1af0a`  
		Last Modified: Wed, 11 May 2022 20:42:46 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28cdae3cd3e170f28072f588bd3af2306df08b15621dc682ef98c3dad4598b4`  
		Last Modified: Wed, 11 May 2022 20:42:46 GMT  
		Size: 5.0 KB (5013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:395dcf8826b83f4290ce2dd5574379619dfd661a5baa0c05dba37d2af2650423
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.4 MB (182449384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2837550813ebce80ff49242f3a87487213974dc3af2659aabbeb1a9994a40011`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:48:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 11 May 2022 19:48:33 GMT
ENV GOSU_VER=1.12
# Wed, 11 May 2022 19:48:37 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 11 May 2022 19:49:54 GMT
ENV INFLUXDB_VERSION=2.2.0
# Wed, 11 May 2022 19:50:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 11 May 2022 19:50:11 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 11 May 2022 19:50:25 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 11 May 2022 19:50:26 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 11 May 2022 19:50:27 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 11 May 2022 19:50:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 11 May 2022 19:50:30 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 11 May 2022 19:50:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:50:31 GMT
CMD ["influxd"]
# Wed, 11 May 2022 19:50:32 GMT
EXPOSE 8086
# Wed, 11 May 2022 19:50:33 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 11 May 2022 19:50:34 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 11 May 2022 19:50:35 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 11 May 2022 19:50:36 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88155b239d4be6cbe8982344c645615907ceb1698ecd859485dc47854b1ae2fe`  
		Last Modified: Wed, 11 May 2022 19:51:42 GMT  
		Size: 1.7 KB (1661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c422d6301995ca5b81c45b24404c961c0b1ccc9bd31c9a54b82363a29844af`  
		Last Modified: Wed, 11 May 2022 19:51:40 GMT  
		Size: 896.3 KB (896335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e321e30cf1a2a95a6259bfcfc41a3e8be7f54261e381777f1891c06430607c2`  
		Last Modified: Wed, 11 May 2022 19:52:35 GMT  
		Size: 109.9 MB (109877888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f051e75770e880c5702a2c88333dd6d8193c0428229ed8f83121a5f845a7084`  
		Last Modified: Wed, 11 May 2022 19:52:26 GMT  
		Size: 5.0 MB (4952624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e58f19231e2ff7828cd469a4f6c932dcadaa4400975d3e4dee7fc05563466c1`  
		Last Modified: Wed, 11 May 2022 19:52:25 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89312617d3ec55a9566523ef5b44e51431414952e1baf536243edd5246debafb`  
		Last Modified: Wed, 11 May 2022 19:52:25 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33639c3ff5f33654d14405f44bbdad9a03f4225b36091e230d7d051828bf738`  
		Last Modified: Wed, 11 May 2022 19:52:25 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:52cf241438911f68b82ca627dfb338fc09a90a0712e43a48bde0f923674c8d04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ced01456b4cd44c84a41de62ef164e2cdf38dd0ee474bbf67827aae43c764b0e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84493544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:470881da7fcdba67ecb9b682507e53aeb5518826856bb316132641238a2ef278`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:38:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:38:33 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 11 May 2022 20:38:48 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 11 May 2022 20:38:49 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 11 May 2022 20:38:49 GMT
EXPOSE 8091
# Wed, 11 May 2022 20:38:49 GMT
VOLUME [/var/lib/influxdb]
# Wed, 11 May 2022 20:38:49 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 11 May 2022 20:38:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:38:49 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5565d52697dc7657483e66de35859480ec0bb9fdce45fd76e1512042633b2b15`  
		Last Modified: Wed, 11 May 2022 20:40:44 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c80c146b168e3ced16a4c687940031768c8750b3c972237b2b742b0e09410f1`  
		Last Modified: Wed, 11 May 2022 20:41:26 GMT  
		Size: 23.4 MB (23416916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c721d0e8c99466248351dc4cc8f1dd68923ab2ac35bb71198d63b20edfa1c203`  
		Last Modified: Wed, 11 May 2022 20:41:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdbcc734429c05067742043f9ff495038a02f7be5ad26dfa0f2ca63de9b559d6`  
		Last Modified: Wed, 11 May 2022 20:41:23 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:008db7d140fce00d44cb0f11b4e04a8d5c151222c18e20f1a6e3c40432c1b6c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:06b3c6c7fdaaae61c386be3b2db8debdb79dc029c86b28fb2ddd57b7a813cca9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27587601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c59c3a9d5137ca189bf5be3e9b530b46a594f7e9911d79fb7ce49a68802cbdd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 10:02:50 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 10:03:43 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 07 Apr 2022 22:23:04 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 07 Apr 2022 22:23:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 07 Apr 2022 22:23:04 GMT
EXPOSE 8091
# Thu, 07 Apr 2022 22:23:04 GMT
VOLUME [/var/lib/influxdb]
# Thu, 07 Apr 2022 22:23:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 07 Apr 2022 22:23:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Apr 2022 22:23:05 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cc030286fba3c1f3131d94752cdc227e840c98131bf4fa7ae057a8e624e0cc`  
		Last Modified: Tue, 05 Apr 2022 04:27:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a82c2bf0b07bc97e48386998fdb52307a711c8cde52325fb999e1b7a0f0073`  
		Last Modified: Tue, 05 Apr 2022 10:06:22 GMT  
		Size: 1.5 MB (1475485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef0611ecd34d60d54d119ad0d5b217bf9bb505143a9a76d79a71588306f6962`  
		Last Modified: Thu, 07 Apr 2022 22:25:10 GMT  
		Size: 23.3 MB (23292997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03800bc1786c31a63f2ce29355aa6c75587b563883515d7db2faec592fe0bcc5`  
		Last Modified: Thu, 07 Apr 2022 22:25:07 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56614b1a615f4516c69895cb7e68ac004819d3dd52ffe4766c55c5686847eff`  
		Last Modified: Thu, 07 Apr 2022 22:25:07 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
