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
$ docker pull influxdb@sha256:3e23e74d436f89fb134bbfef4b6188225f9a0199d841973bf5d4cc3526e638ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:e7642e7fd25dc094df012b88e12cac06626b7d28777fcf289b3109d88f3ed3b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115970390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eb0b30646db6f78a74c75860998a847b63e5e98bee7d1301a52fe099878316c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:13:58 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sun, 29 May 2022 01:14:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sun, 29 May 2022 01:14:02 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sun, 29 May 2022 01:14:02 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:14:02 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:03 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:03 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 29 May 2022 01:14:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:03 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c017d03cc583a80f6e10340b2c65d5d24b4e559a43d30551587ea69fb28b6`  
		Last Modified: Sun, 29 May 2022 01:16:30 GMT  
		Size: 54.9 MB (54890107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3ce16e7902af5b08e7d704301ae5fbad72ae55718ded09d0bbaba54891362f`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c56feafaeb5f8b64d65128378cc442bac4709023412187205d9727f751fd67f`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09aac5087631bd26e60d0b3be0664c2f829a94c68ba1d5eeca91013d2ad7bf2`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
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
$ docker pull influxdb@sha256:bf4c43b86a1a35083f22cb851f028db5e80be578307dd88614be5c37693556dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108544662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb0422acbed500ce1984b9131af8d841f02e605a5db6406b2762a45eb060a87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 00:42:45 GMT
ADD file:93d675ee0bc32a88dc4d6c0872276c4678dc31f0b6eb8b936cb823f191bc07f0 in / 
# Sat, 28 May 2022 00:42:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:10:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:11:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 02:28:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 02:28:35 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sun, 29 May 2022 02:28:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sun, 29 May 2022 02:28:42 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sun, 29 May 2022 02:28:42 GMT
EXPOSE 8086
# Sun, 29 May 2022 02:28:43 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 02:28:45 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sun, 29 May 2022 02:28:46 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 29 May 2022 02:28:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 02:28:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:de7fc2a3b80bcd193de687188fc9051c8be6c61ec81fec3aeae61c079f71e69e`  
		Last Modified: Sat, 28 May 2022 00:51:21 GMT  
		Size: 43.2 MB (43212871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee73573552502f742607ea1dcdefcee9aeafa4ad8d5deca24b48a262f4ba108`  
		Last Modified: Sat, 28 May 2022 11:20:36 GMT  
		Size: 10.2 MB (10218522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05d3983d65175e68348dcb2cd43933f2af4d2d8c1bf36c9d5f237394c9fa53b`  
		Last Modified: Sat, 28 May 2022 11:20:35 GMT  
		Size: 3.9 MB (3874461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234a6005350a3b5cbd08a230d099eb3910ad109cab3c9cd4a971cf4f08beedba`  
		Last Modified: Sun, 29 May 2022 02:31:35 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a3f6c8bd6855a100f1e541a14430c3e0f705c253c040aba12a9cb3fc0ae5cf`  
		Last Modified: Sun, 29 May 2022 02:31:42 GMT  
		Size: 51.2 MB (51234265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a52fa0e0508020ebc9c98803ca3625db95665053a1e9eafac5567edb37b6cc2`  
		Last Modified: Sun, 29 May 2022 02:31:35 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23345dfd5f1bf05d0c47268ca17e8725728ca712fce13940821f81d3c381754c`  
		Last Modified: Sun, 29 May 2022 02:31:35 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c05baf513d87daba400875c6c4b35bd169b5a8e22f6e165fb62310a934df31`  
		Last Modified: Sun, 29 May 2022 02:31:35 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:80d1447e23194ac263dc324d567eaca3cd7d8c743286466eb403a193be76806d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:f057b9826c94f3cbffeae1559f46aa7d57e11d4313d620ebb2b8f3c03de49aba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117789479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e07f37814d7711a17b11ae3b7b0c2494ddd56c77a1f31560ec99d38cf733e6d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:14:07 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sun, 29 May 2022 01:14:12 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sun, 29 May 2022 01:14:13 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sun, 29 May 2022 01:14:13 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:14:13 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:13 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:13 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 29 May 2022 01:14:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:13 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd97197a056b127568e26d51e8dc0b1726ec9dac509b9c2e7de161521dffe9f`  
		Last Modified: Sun, 29 May 2022 01:16:47 GMT  
		Size: 56.7 MB (56709134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c0d2f38f0f0cd00842c355b2780895a8dff3d698baf794162c142ae4301837`  
		Last Modified: Sun, 29 May 2022 01:16:40 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b4717d882bf2ca3662fbd88b6cb429c8cfc1002675288fd52c7dad654bfb49`  
		Last Modified: Sun, 29 May 2022 01:16:40 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db994e43254a59c721f524e5585b89f7b7efd529dc94349c11eadd14216f4fcd`  
		Last Modified: Sun, 29 May 2022 01:16:40 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:8d5402e304325edfcfe660e5321fcb966321984116fbaf1d7e4087a6a813dcbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:6fb1429a96ad2bcc86b596dc4f45b7a181217051455baafb8050e0be81531136
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84496090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7274da2aaef773679225007f1a42b5b7b34b2e3465543334a2ab49705e3491ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:14:07 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sun, 29 May 2022 01:14:21 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sun, 29 May 2022 01:14:21 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sun, 29 May 2022 01:14:21 GMT
EXPOSE 8091
# Sun, 29 May 2022 01:14:22 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:22 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:22 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d08dfd21984cd88d13eaeeef51a60a6f7b6cf6a7675932bf9801f77743b1c84`  
		Last Modified: Sun, 29 May 2022 01:17:04 GMT  
		Size: 23.4 MB (23416952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076936713b4ccd154076ca92824f3308d44b1d52dac385010c1e2e4cb7736409`  
		Last Modified: Sun, 29 May 2022 01:17:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90904d4629e11d99c4e980cecd4a397427acd53acec6df81a641928ca4ddc85`  
		Last Modified: Sun, 29 May 2022 01:17:01 GMT  
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
$ docker pull influxdb@sha256:3e23e74d436f89fb134bbfef4b6188225f9a0199d841973bf5d4cc3526e638ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:e7642e7fd25dc094df012b88e12cac06626b7d28777fcf289b3109d88f3ed3b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115970390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eb0b30646db6f78a74c75860998a847b63e5e98bee7d1301a52fe099878316c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:13:58 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sun, 29 May 2022 01:14:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sun, 29 May 2022 01:14:02 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sun, 29 May 2022 01:14:02 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:14:02 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:03 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:03 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 29 May 2022 01:14:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:03 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c017d03cc583a80f6e10340b2c65d5d24b4e559a43d30551587ea69fb28b6`  
		Last Modified: Sun, 29 May 2022 01:16:30 GMT  
		Size: 54.9 MB (54890107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3ce16e7902af5b08e7d704301ae5fbad72ae55718ded09d0bbaba54891362f`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c56feafaeb5f8b64d65128378cc442bac4709023412187205d9727f751fd67f`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09aac5087631bd26e60d0b3be0664c2f829a94c68ba1d5eeca91013d2ad7bf2`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
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
$ docker pull influxdb@sha256:bf4c43b86a1a35083f22cb851f028db5e80be578307dd88614be5c37693556dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108544662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb0422acbed500ce1984b9131af8d841f02e605a5db6406b2762a45eb060a87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 00:42:45 GMT
ADD file:93d675ee0bc32a88dc4d6c0872276c4678dc31f0b6eb8b936cb823f191bc07f0 in / 
# Sat, 28 May 2022 00:42:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:10:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:11:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 02:28:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 02:28:35 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sun, 29 May 2022 02:28:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sun, 29 May 2022 02:28:42 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sun, 29 May 2022 02:28:42 GMT
EXPOSE 8086
# Sun, 29 May 2022 02:28:43 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 02:28:45 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sun, 29 May 2022 02:28:46 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 29 May 2022 02:28:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 02:28:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:de7fc2a3b80bcd193de687188fc9051c8be6c61ec81fec3aeae61c079f71e69e`  
		Last Modified: Sat, 28 May 2022 00:51:21 GMT  
		Size: 43.2 MB (43212871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee73573552502f742607ea1dcdefcee9aeafa4ad8d5deca24b48a262f4ba108`  
		Last Modified: Sat, 28 May 2022 11:20:36 GMT  
		Size: 10.2 MB (10218522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05d3983d65175e68348dcb2cd43933f2af4d2d8c1bf36c9d5f237394c9fa53b`  
		Last Modified: Sat, 28 May 2022 11:20:35 GMT  
		Size: 3.9 MB (3874461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234a6005350a3b5cbd08a230d099eb3910ad109cab3c9cd4a971cf4f08beedba`  
		Last Modified: Sun, 29 May 2022 02:31:35 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a3f6c8bd6855a100f1e541a14430c3e0f705c253c040aba12a9cb3fc0ae5cf`  
		Last Modified: Sun, 29 May 2022 02:31:42 GMT  
		Size: 51.2 MB (51234265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a52fa0e0508020ebc9c98803ca3625db95665053a1e9eafac5567edb37b6cc2`  
		Last Modified: Sun, 29 May 2022 02:31:35 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23345dfd5f1bf05d0c47268ca17e8725728ca712fce13940821f81d3c381754c`  
		Last Modified: Sun, 29 May 2022 02:31:35 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c05baf513d87daba400875c6c4b35bd169b5a8e22f6e165fb62310a934df31`  
		Last Modified: Sun, 29 May 2022 02:31:35 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:80d1447e23194ac263dc324d567eaca3cd7d8c743286466eb403a193be76806d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:f057b9826c94f3cbffeae1559f46aa7d57e11d4313d620ebb2b8f3c03de49aba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117789479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e07f37814d7711a17b11ae3b7b0c2494ddd56c77a1f31560ec99d38cf733e6d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:14:07 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sun, 29 May 2022 01:14:12 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sun, 29 May 2022 01:14:13 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sun, 29 May 2022 01:14:13 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:14:13 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:13 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:13 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 29 May 2022 01:14:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:13 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd97197a056b127568e26d51e8dc0b1726ec9dac509b9c2e7de161521dffe9f`  
		Last Modified: Sun, 29 May 2022 01:16:47 GMT  
		Size: 56.7 MB (56709134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c0d2f38f0f0cd00842c355b2780895a8dff3d698baf794162c142ae4301837`  
		Last Modified: Sun, 29 May 2022 01:16:40 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b4717d882bf2ca3662fbd88b6cb429c8cfc1002675288fd52c7dad654bfb49`  
		Last Modified: Sun, 29 May 2022 01:16:40 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db994e43254a59c721f524e5585b89f7b7efd529dc94349c11eadd14216f4fcd`  
		Last Modified: Sun, 29 May 2022 01:16:40 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:8d5402e304325edfcfe660e5321fcb966321984116fbaf1d7e4087a6a813dcbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:6fb1429a96ad2bcc86b596dc4f45b7a181217051455baafb8050e0be81531136
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84496090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7274da2aaef773679225007f1a42b5b7b34b2e3465543334a2ab49705e3491ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:14:07 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sun, 29 May 2022 01:14:21 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sun, 29 May 2022 01:14:21 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sun, 29 May 2022 01:14:21 GMT
EXPOSE 8091
# Sun, 29 May 2022 01:14:22 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:22 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:22 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d08dfd21984cd88d13eaeeef51a60a6f7b6cf6a7675932bf9801f77743b1c84`  
		Last Modified: Sun, 29 May 2022 01:17:04 GMT  
		Size: 23.4 MB (23416952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076936713b4ccd154076ca92824f3308d44b1d52dac385010c1e2e4cb7736409`  
		Last Modified: Sun, 29 May 2022 01:17:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90904d4629e11d99c4e980cecd4a397427acd53acec6df81a641928ca4ddc85`  
		Last Modified: Sun, 29 May 2022 01:17:01 GMT  
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
$ docker pull influxdb@sha256:1550e722d294f447e80e6aa7e8a108bf7e440d295599ce8506194a1f5a559a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:e7d4908cf166f4791e91623df7af568de9857e2edb063f79a5c8a6db2b44c2b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90704635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9408124d60bd08f23ad42567877c649d093deb15a10b56e68bec97d89d8a85db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:14:26 GMT
ENV INFLUXDB_VERSION=1.9.7-c1.9.7
# Sun, 29 May 2022 01:14:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sun, 29 May 2022 01:14:31 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sun, 29 May 2022 01:14:31 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:14:31 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:31 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:31 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 29 May 2022 01:14:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:31 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4d8c872dbcd4775f4e067e966c471e617f439af8c1a0da4cede1bdf7bc2481`  
		Last Modified: Sun, 29 May 2022 01:17:22 GMT  
		Size: 29.6 MB (29624291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249e847b5893e8d87fe75d0d7c5594aa6093a78fc2c6d6b2ea97be76ea35bdfb`  
		Last Modified: Sun, 29 May 2022 01:17:17 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e18d078bd59cf2722699d5cdf2d5d0a70d3bd0c3643d3f6d6a78d9e36fd677`  
		Last Modified: Sun, 29 May 2022 01:17:17 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665265d2ff5f97908b9f336c9543a82e7d96ff00c4a0dfebcf0693cc6ac7f3ff`  
		Last Modified: Sun, 29 May 2022 01:17:17 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:e1d9e54bd24a17d1a032944ba8cc23fdf84ba953762378c3510552cdf24fcc09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:6ee728ab13142ad52cebb66e48deacafb475724292d2cb95939c00ea0ff94348
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33883939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fff07ab0a9f4a120e5cf2b8b28873ac6d2dadcc8661981e2e21b83db87efb6`
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
# Fri, 13 May 2022 23:22:29 GMT
ENV INFLUXDB_VERSION=1.9.7-c1.9.7
# Fri, 13 May 2022 23:22:36 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 13 May 2022 23:22:36 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 13 May 2022 23:22:36 GMT
EXPOSE 8086
# Fri, 13 May 2022 23:22:36 GMT
VOLUME [/var/lib/influxdb]
# Fri, 13 May 2022 23:22:36 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 13 May 2022 23:22:36 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 13 May 2022 23:22:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 May 2022 23:22:37 GMT
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
	-	`sha256:8049c647458ac03fd6fc3ded991f8887dd00e66f1ac0a991a103c1fc95e200a2`  
		Last Modified: Fri, 13 May 2022 23:25:07 GMT  
		Size: 29.6 MB (29588132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa367debb769aca195f3c2fdf417b827766b1619b699d9e1731dac63a8f0ec`  
		Last Modified: Fri, 13 May 2022 23:25:02 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0bbaadebfc484c99a58191d4624a63639ab06a7587ab389acbd9f6ed75cfcb`  
		Last Modified: Fri, 13 May 2022 23:25:02 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e4e2ce745b712133979f576dd84263d017a95859721424406ce309239a8573`  
		Last Modified: Fri, 13 May 2022 23:25:02 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:b9ceb3efb7e8e47b5ffca7c34853d081514ef90e5bc2046d150a179c69269cf0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:b600514001d04352c3cad833acd56ab1e73b9437a186f4cd1c05858c93e8287b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72483404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba660fcc24bbddb9113a8d34f1192a269d44da91d50e9cde82d921177448521b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:14:26 GMT
ENV INFLUXDB_VERSION=1.9.7-c1.9.7
# Sun, 29 May 2022 01:14:38 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sun, 29 May 2022 01:14:38 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sun, 29 May 2022 01:14:38 GMT
EXPOSE 8091
# Sun, 29 May 2022 01:14:38 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:39 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:39 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048aaf9807b775deab6c3ebcf616ec94a83b23e90811c5ccbb001691ee0c2314`  
		Last Modified: Sun, 29 May 2022 01:17:34 GMT  
		Size: 11.4 MB (11404267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d93801f01feb302e094710ea8f8f5961df0f23ccfb88c3b563e60251b8bb0e9`  
		Last Modified: Sun, 29 May 2022 01:17:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72729640e2cb8b465ef7ed414fcfcce62e588cdfd378b4668e2fe795dcf256d2`  
		Last Modified: Sun, 29 May 2022 01:17:32 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:dc39332e9b6223d1e6bdeadd5f0320371bb1f62ca446f22a96a3a324442623e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4ee9e2ace9f40ba0f5741ecd257cc34a3e005b2c75cb652dae6da4d61e74c22a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15661343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3421824827bb411e72011ad67c76f54579337fc6bed34edeca3051a178a6513c`
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
# Fri, 13 May 2022 23:22:29 GMT
ENV INFLUXDB_VERSION=1.9.7-c1.9.7
# Fri, 13 May 2022 23:22:48 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 13 May 2022 23:22:49 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 13 May 2022 23:22:49 GMT
EXPOSE 8091
# Fri, 13 May 2022 23:22:49 GMT
VOLUME [/var/lib/influxdb]
# Fri, 13 May 2022 23:22:49 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 13 May 2022 23:22:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 May 2022 23:22:49 GMT
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
	-	`sha256:673915b6ac8889537ff4f3dfce036e70e2a124e4d248b538a34e9ed88de2a5b8`  
		Last Modified: Fri, 13 May 2022 23:25:29 GMT  
		Size: 11.4 MB (11366738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f6c0b53e10ee68139a29ff4f4a087a1d449b73adc7e032d30559d38fd3d377`  
		Last Modified: Fri, 13 May 2022 23:25:27 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55318cf751b9c9ed7c361dcfbba8e06f4defa772d3097909638d968e5ce2655d`  
		Last Modified: Fri, 13 May 2022 23:25:27 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.7-data`

```console
$ docker pull influxdb@sha256:1550e722d294f447e80e6aa7e8a108bf7e440d295599ce8506194a1f5a559a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:e7d4908cf166f4791e91623df7af568de9857e2edb063f79a5c8a6db2b44c2b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90704635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9408124d60bd08f23ad42567877c649d093deb15a10b56e68bec97d89d8a85db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:14:26 GMT
ENV INFLUXDB_VERSION=1.9.7-c1.9.7
# Sun, 29 May 2022 01:14:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sun, 29 May 2022 01:14:31 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sun, 29 May 2022 01:14:31 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:14:31 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:31 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:31 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 29 May 2022 01:14:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:31 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4d8c872dbcd4775f4e067e966c471e617f439af8c1a0da4cede1bdf7bc2481`  
		Last Modified: Sun, 29 May 2022 01:17:22 GMT  
		Size: 29.6 MB (29624291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249e847b5893e8d87fe75d0d7c5594aa6093a78fc2c6d6b2ea97be76ea35bdfb`  
		Last Modified: Sun, 29 May 2022 01:17:17 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e18d078bd59cf2722699d5cdf2d5d0a70d3bd0c3643d3f6d6a78d9e36fd677`  
		Last Modified: Sun, 29 May 2022 01:17:17 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665265d2ff5f97908b9f336c9543a82e7d96ff00c4a0dfebcf0693cc6ac7f3ff`  
		Last Modified: Sun, 29 May 2022 01:17:17 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.7-data-alpine`

```console
$ docker pull influxdb@sha256:e1d9e54bd24a17d1a032944ba8cc23fdf84ba953762378c3510552cdf24fcc09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.7-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:6ee728ab13142ad52cebb66e48deacafb475724292d2cb95939c00ea0ff94348
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33883939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fff07ab0a9f4a120e5cf2b8b28873ac6d2dadcc8661981e2e21b83db87efb6`
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
# Fri, 13 May 2022 23:22:29 GMT
ENV INFLUXDB_VERSION=1.9.7-c1.9.7
# Fri, 13 May 2022 23:22:36 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 13 May 2022 23:22:36 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 13 May 2022 23:22:36 GMT
EXPOSE 8086
# Fri, 13 May 2022 23:22:36 GMT
VOLUME [/var/lib/influxdb]
# Fri, 13 May 2022 23:22:36 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 13 May 2022 23:22:36 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 13 May 2022 23:22:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 May 2022 23:22:37 GMT
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
	-	`sha256:8049c647458ac03fd6fc3ded991f8887dd00e66f1ac0a991a103c1fc95e200a2`  
		Last Modified: Fri, 13 May 2022 23:25:07 GMT  
		Size: 29.6 MB (29588132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa367debb769aca195f3c2fdf417b827766b1619b699d9e1731dac63a8f0ec`  
		Last Modified: Fri, 13 May 2022 23:25:02 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0bbaadebfc484c99a58191d4624a63639ab06a7587ab389acbd9f6ed75cfcb`  
		Last Modified: Fri, 13 May 2022 23:25:02 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e4e2ce745b712133979f576dd84263d017a95859721424406ce309239a8573`  
		Last Modified: Fri, 13 May 2022 23:25:02 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.7-meta`

```console
$ docker pull influxdb@sha256:b9ceb3efb7e8e47b5ffca7c34853d081514ef90e5bc2046d150a179c69269cf0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:b600514001d04352c3cad833acd56ab1e73b9437a186f4cd1c05858c93e8287b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72483404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba660fcc24bbddb9113a8d34f1192a269d44da91d50e9cde82d921177448521b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:14:26 GMT
ENV INFLUXDB_VERSION=1.9.7-c1.9.7
# Sun, 29 May 2022 01:14:38 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sun, 29 May 2022 01:14:38 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sun, 29 May 2022 01:14:38 GMT
EXPOSE 8091
# Sun, 29 May 2022 01:14:38 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:39 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:39 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048aaf9807b775deab6c3ebcf616ec94a83b23e90811c5ccbb001691ee0c2314`  
		Last Modified: Sun, 29 May 2022 01:17:34 GMT  
		Size: 11.4 MB (11404267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d93801f01feb302e094710ea8f8f5961df0f23ccfb88c3b563e60251b8bb0e9`  
		Last Modified: Sun, 29 May 2022 01:17:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72729640e2cb8b465ef7ed414fcfcce62e588cdfd378b4668e2fe795dcf256d2`  
		Last Modified: Sun, 29 May 2022 01:17:32 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.7-meta-alpine`

```console
$ docker pull influxdb@sha256:dc39332e9b6223d1e6bdeadd5f0320371bb1f62ca446f22a96a3a324442623e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.7-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4ee9e2ace9f40ba0f5741ecd257cc34a3e005b2c75cb652dae6da4d61e74c22a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15661343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3421824827bb411e72011ad67c76f54579337fc6bed34edeca3051a178a6513c`
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
# Fri, 13 May 2022 23:22:29 GMT
ENV INFLUXDB_VERSION=1.9.7-c1.9.7
# Fri, 13 May 2022 23:22:48 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 13 May 2022 23:22:49 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 13 May 2022 23:22:49 GMT
EXPOSE 8091
# Fri, 13 May 2022 23:22:49 GMT
VOLUME [/var/lib/influxdb]
# Fri, 13 May 2022 23:22:49 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 13 May 2022 23:22:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 May 2022 23:22:49 GMT
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
	-	`sha256:673915b6ac8889537ff4f3dfce036e70e2a124e4d248b538a34e9ed88de2a5b8`  
		Last Modified: Fri, 13 May 2022 23:25:29 GMT  
		Size: 11.4 MB (11366738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f6c0b53e10ee68139a29ff4f4a087a1d449b73adc7e032d30559d38fd3d377`  
		Last Modified: Fri, 13 May 2022 23:25:27 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55318cf751b9c9ed7c361dcfbba8e06f4defa772d3097909638d968e5ce2655d`  
		Last Modified: Fri, 13 May 2022 23:25:27 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0`

```console
$ docker pull influxdb@sha256:6dd9d3894e92c31ba25c59736d00871b46b960e40e65658bd8bd62825a53f88c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:3340da0c65f7f4e1036b445a2228a2ddfbb06853c43d788f6da68c6ab71cf085
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.4 MB (172353198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e977ef79a26bbd4062b6e3e9d2a5e21ac040d59082b40e27bdb458529cd27fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:42:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:42:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:14:44 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 01:14:44 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 01:14:48 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sun, 29 May 2022 01:14:48 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sun, 29 May 2022 01:14:55 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sun, 29 May 2022 01:14:55 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 01:14:55 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 01:14:56 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 01:14:56 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Sun, 29 May 2022 01:14:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:56 GMT
CMD ["influxd"]
# Sun, 29 May 2022 01:14:56 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:14:56 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 01:14:56 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 01:14:56 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 01:14:56 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02d86f59850f3e13d394072350625a8526b912af24b3bfc0e50e9a8862a79d0`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 7.9 MB (7856653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b047e8f2e47bdf998a952572ae5e9d64edf8e29b716be0ee50a15e6d21cb2ce`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 10.0 MB (9997224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44b41d3b54f81ac9b15b79d938c2d2f7ce9387856470f56e2b1bf6f167afae`  
		Last Modified: Sun, 29 May 2022 01:17:46 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd83ba9d903f7240886fd6e55d2c427caf96f9d8aa9b6b27342971c24932181`  
		Last Modified: Sun, 29 May 2022 01:17:44 GMT  
		Size: 961.0 KB (960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2978b95b0d4a5fb1f44de458e0a7085e979508d8d0422a3b0d987b7f7e0ca39c`  
		Last Modified: Sun, 29 May 2022 01:17:53 GMT  
		Size: 103.1 MB (103090644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8202613e12d43c4dcf6e77e23043573463deb7cc3f48d8c3ac7799cf6369217`  
		Last Modified: Sun, 29 May 2022 01:17:44 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3416f8db9dcd0b2fe148adde9ac5b027610dae86b8a01704d4b1bccb6fd9b`  
		Last Modified: Sun, 29 May 2022 01:17:44 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6315db68403334cc095f757265cb5b581b356d0fdaf7bb4a0991b78e954b4559`  
		Last Modified: Sun, 29 May 2022 01:17:44 GMT  
		Size: 4.9 KB (4948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a8cee866dc257bf55a305711720a4def9f1dac8bd9fbaf9fdebd7598d2e756a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174146564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae09f9d93a57fb7c039ea6e78f275ccb325a21e975250e273985742b75e2c101`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:07:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 02:28:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 02:28:55 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 02:28:58 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sun, 29 May 2022 02:28:59 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sun, 29 May 2022 02:29:15 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sun, 29 May 2022 02:29:16 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 02:29:17 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 02:29:19 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 02:29:20 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Sun, 29 May 2022 02:29:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 02:29:21 GMT
CMD ["influxd"]
# Sun, 29 May 2022 02:29:22 GMT
EXPOSE 8086
# Sun, 29 May 2022 02:29:23 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 02:29:24 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 02:29:25 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 02:29:26 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5795076bf6e9bf96da71f2e31cbe91d3c49a17f211c5b0d33e032e095c5564a5`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 7.7 MB (7719823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eda3e266fa432ba8ae8ba25a5ad2fa4c5349ef2aa244612c89f990704c5b25`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 9.8 MB (9767307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0f5443af812585848f35a0c394a1510e548db84651500f20b69c8fd177c0e2`  
		Last Modified: Sun, 29 May 2022 02:31:56 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1f0ed20c1a53ee0dc8c120bc08109085a39df68ea03a3844b7ca1852bf608a`  
		Last Modified: Sun, 29 May 2022 02:31:54 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c83c667071c5934659f25b26e1a850164064fef708f2a6600d3d4767fbf0eb1`  
		Last Modified: Sun, 29 May 2022 02:32:04 GMT  
		Size: 106.5 MB (106526999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3bef01a75ab8266eebb18230f7c07a2ce197cbadef0032121dce4dad504efa`  
		Last Modified: Sun, 29 May 2022 02:31:53 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e764baaabdb3a574640cd09241e06d54f30bb96c5cd06e1c08a825babd989bce`  
		Last Modified: Sun, 29 May 2022 02:31:53 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13be48d53306fa683b601aa56be827b2aa32c048616b991fd801e82ae6e4fcd`  
		Last Modified: Sun, 29 May 2022 02:31:53 GMT  
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
$ docker pull influxdb@sha256:6dd9d3894e92c31ba25c59736d00871b46b960e40e65658bd8bd62825a53f88c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9` - linux; amd64

```console
$ docker pull influxdb@sha256:3340da0c65f7f4e1036b445a2228a2ddfbb06853c43d788f6da68c6ab71cf085
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.4 MB (172353198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e977ef79a26bbd4062b6e3e9d2a5e21ac040d59082b40e27bdb458529cd27fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:42:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:42:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:14:44 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 01:14:44 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 01:14:48 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sun, 29 May 2022 01:14:48 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sun, 29 May 2022 01:14:55 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sun, 29 May 2022 01:14:55 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 01:14:55 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 01:14:56 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 01:14:56 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Sun, 29 May 2022 01:14:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:56 GMT
CMD ["influxd"]
# Sun, 29 May 2022 01:14:56 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:14:56 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 01:14:56 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 01:14:56 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 01:14:56 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02d86f59850f3e13d394072350625a8526b912af24b3bfc0e50e9a8862a79d0`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 7.9 MB (7856653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b047e8f2e47bdf998a952572ae5e9d64edf8e29b716be0ee50a15e6d21cb2ce`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 10.0 MB (9997224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44b41d3b54f81ac9b15b79d938c2d2f7ce9387856470f56e2b1bf6f167afae`  
		Last Modified: Sun, 29 May 2022 01:17:46 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd83ba9d903f7240886fd6e55d2c427caf96f9d8aa9b6b27342971c24932181`  
		Last Modified: Sun, 29 May 2022 01:17:44 GMT  
		Size: 961.0 KB (960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2978b95b0d4a5fb1f44de458e0a7085e979508d8d0422a3b0d987b7f7e0ca39c`  
		Last Modified: Sun, 29 May 2022 01:17:53 GMT  
		Size: 103.1 MB (103090644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8202613e12d43c4dcf6e77e23043573463deb7cc3f48d8c3ac7799cf6369217`  
		Last Modified: Sun, 29 May 2022 01:17:44 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d3416f8db9dcd0b2fe148adde9ac5b027610dae86b8a01704d4b1bccb6fd9b`  
		Last Modified: Sun, 29 May 2022 01:17:44 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6315db68403334cc095f757265cb5b581b356d0fdaf7bb4a0991b78e954b4559`  
		Last Modified: Sun, 29 May 2022 01:17:44 GMT  
		Size: 4.9 KB (4948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a8cee866dc257bf55a305711720a4def9f1dac8bd9fbaf9fdebd7598d2e756a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174146564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae09f9d93a57fb7c039ea6e78f275ccb325a21e975250e273985742b75e2c101`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:07:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 02:28:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 02:28:55 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 02:28:58 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sun, 29 May 2022 02:28:59 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sun, 29 May 2022 02:29:15 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sun, 29 May 2022 02:29:16 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 02:29:17 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 02:29:19 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 02:29:20 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Sun, 29 May 2022 02:29:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 02:29:21 GMT
CMD ["influxd"]
# Sun, 29 May 2022 02:29:22 GMT
EXPOSE 8086
# Sun, 29 May 2022 02:29:23 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 02:29:24 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 02:29:25 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 02:29:26 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5795076bf6e9bf96da71f2e31cbe91d3c49a17f211c5b0d33e032e095c5564a5`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 7.7 MB (7719823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eda3e266fa432ba8ae8ba25a5ad2fa4c5349ef2aa244612c89f990704c5b25`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 9.8 MB (9767307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0f5443af812585848f35a0c394a1510e548db84651500f20b69c8fd177c0e2`  
		Last Modified: Sun, 29 May 2022 02:31:56 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1f0ed20c1a53ee0dc8c120bc08109085a39df68ea03a3844b7ca1852bf608a`  
		Last Modified: Sun, 29 May 2022 02:31:54 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c83c667071c5934659f25b26e1a850164064fef708f2a6600d3d4767fbf0eb1`  
		Last Modified: Sun, 29 May 2022 02:32:04 GMT  
		Size: 106.5 MB (106526999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3bef01a75ab8266eebb18230f7c07a2ce197cbadef0032121dce4dad504efa`  
		Last Modified: Sun, 29 May 2022 02:31:53 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e764baaabdb3a574640cd09241e06d54f30bb96c5cd06e1c08a825babd989bce`  
		Last Modified: Sun, 29 May 2022 02:31:53 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13be48d53306fa683b601aa56be827b2aa32c048616b991fd801e82ae6e4fcd`  
		Last Modified: Sun, 29 May 2022 02:31:53 GMT  
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
$ docker pull influxdb@sha256:f2770c39002fe1027c3fce8e41762853d51ca51c376ba04046dc7f1c913dbbad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1` - linux; amd64

```console
$ docker pull influxdb@sha256:649bf77e328a9ef497c0bf100fe4f6ad1bf5ee62e985bd4af08787a966548ac3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182911931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd02ed19e30304a60ff009bb0ceb0bcec39881d86b1380fab55bd724334c90ff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:42:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:42:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:14:44 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 01:14:44 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 01:15:04 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Sun, 29 May 2022 01:15:04 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sun, 29 May 2022 01:15:14 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sun, 29 May 2022 01:15:14 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sun, 29 May 2022 01:15:18 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sun, 29 May 2022 01:15:19 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 01:15:19 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 01:15:19 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 01:15:19 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sun, 29 May 2022 01:15:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:15:19 GMT
CMD ["influxd"]
# Sun, 29 May 2022 01:15:19 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:15:20 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 01:15:20 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 01:15:20 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 01:15:20 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02d86f59850f3e13d394072350625a8526b912af24b3bfc0e50e9a8862a79d0`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 7.9 MB (7856653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b047e8f2e47bdf998a952572ae5e9d64edf8e29b716be0ee50a15e6d21cb2ce`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 10.0 MB (9997224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44b41d3b54f81ac9b15b79d938c2d2f7ce9387856470f56e2b1bf6f167afae`  
		Last Modified: Sun, 29 May 2022 01:17:46 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defebe72e01b0060660d0152a33bcb207d754ff847155c4a9c35ffcfd809fe81`  
		Last Modified: Sun, 29 May 2022 01:18:06 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6a22f6313637df3a662b130df9b676c641fcffeee420a9355122e135dd86b`  
		Last Modified: Sun, 29 May 2022 01:18:11 GMT  
		Size: 108.3 MB (108324830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cb9d6503bb45cb8c98b94709ba955442016b327f130571f803563a49fa7ff9`  
		Last Modified: Sun, 29 May 2022 01:18:04 GMT  
		Size: 5.3 MB (5324488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6186c790d800358f9b2f092bc8e9f76293ea39f2afd73b1989ed3342387abe4a`  
		Last Modified: Sun, 29 May 2022 01:18:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171bcc724f204627040909d965bbe9ba1853fc24d1fd62a5274ffcb99398569a`  
		Last Modified: Sun, 29 May 2022 01:18:03 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6f370faad6406facbe1f4bd6f759783b517eaddf46f663016c99fc6c1a971c`  
		Last Modified: Sun, 29 May 2022 01:18:03 GMT  
		Size: 5.0 KB (5013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:be2633ade4dcfc5b9c463e7eccb5324e9cdac874bf3982db93cbd5cd58dd490f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183418008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f097f737bf20cffa6ea7ba95e44579195ebef06cd8a53a8299ad46f5260c8d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:07:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 02:28:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 02:28:55 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 02:29:38 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Sun, 29 May 2022 02:29:38 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sun, 29 May 2022 02:29:55 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sun, 29 May 2022 02:29:56 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sun, 29 May 2022 02:30:00 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sun, 29 May 2022 02:30:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 02:30:01 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 02:30:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 02:30:04 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sun, 29 May 2022 02:30:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 02:30:05 GMT
CMD ["influxd"]
# Sun, 29 May 2022 02:30:06 GMT
EXPOSE 8086
# Sun, 29 May 2022 02:30:07 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 02:30:08 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 02:30:09 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 02:30:10 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5795076bf6e9bf96da71f2e31cbe91d3c49a17f211c5b0d33e032e095c5564a5`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 7.7 MB (7719823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eda3e266fa432ba8ae8ba25a5ad2fa4c5349ef2aa244612c89f990704c5b25`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 9.8 MB (9767307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0f5443af812585848f35a0c394a1510e548db84651500f20b69c8fd177c0e2`  
		Last Modified: Sun, 29 May 2022 02:31:56 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74321fb0673e5200e61727207187742de353b576e99c069daa95938cbcc3c34`  
		Last Modified: Sun, 29 May 2022 02:32:19 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ff5c8727d66245fc8f1b942f3e38b9192440d023ffc22893bfa7a18dd1ff93`  
		Last Modified: Sun, 29 May 2022 02:32:26 GMT  
		Size: 110.9 MB (110891645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51679d7c35d3500995d74c22e447c4d6b718981b4c84102a1a557e2f480e67`  
		Last Modified: Sun, 29 May 2022 02:32:17 GMT  
		Size: 4.9 MB (4906728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867099d45360c2f3f7c57077c69779e1b7f26819a74ba816df4f09dd20a528fb`  
		Last Modified: Sun, 29 May 2022 02:32:17 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793f10209d5243f80d3ae22ba8c2e3698b31dcf54577a0b446803813e7c94135`  
		Last Modified: Sun, 29 May 2022 02:32:17 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f4cc8cad56f9798684c779a88fad21b5344d7f0afecd3932762b731ceb27b0`  
		Last Modified: Sun, 29 May 2022 02:32:17 GMT  
		Size: 5.0 KB (5013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1-alpine`

```console
$ docker pull influxdb@sha256:b0526384d0abb3ea2a98a8f4ee3fdb8e0fb8a3db3afbcc3d030963dcaecd62b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:76ff3abffce8813793a72cf43cae3e39947804ea5aca2c3eb51efc5971484c38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127272080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7c55292c93aa37a83cb792257e68898d826204c401ab8e3b291b79b501a2d97`
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
# Fri, 13 May 2022 23:23:18 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu --version;     gosu nobody true
# Fri, 13 May 2022 23:23:18 GMT
ENV INFLUXDB_VERSION=2.1.1
# Fri, 13 May 2022 23:23:25 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 13 May 2022 23:23:25 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Fri, 13 May 2022 23:23:28 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 13 May 2022 23:23:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 13 May 2022 23:23:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 13 May 2022 23:23:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 13 May 2022 23:23:29 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Fri, 13 May 2022 23:23:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 May 2022 23:23:29 GMT
CMD ["influxd"]
# Fri, 13 May 2022 23:23:29 GMT
EXPOSE 8086
# Fri, 13 May 2022 23:23:29 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 13 May 2022 23:23:29 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 13 May 2022 23:23:30 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 13 May 2022 23:23:30 GMT
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
	-	`sha256:c9e8df9da8d1c8426e1caad99cf5795de908d0c016597335d6ea348135fe0207`  
		Last Modified: Fri, 13 May 2022 23:26:02 GMT  
		Size: 960.6 KB (960628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cf4a1abffaa9098b3c38918f1b2b3945f2fe047fec65bcfc2d9b83aafafa78`  
		Last Modified: Fri, 13 May 2022 23:26:08 GMT  
		Size: 108.3 MB (108324839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4612c9f990cb7934b692da9ed47390228bc4342dd3903d82d98fd8fc2c72d`  
		Last Modified: Fri, 13 May 2022 23:26:00 GMT  
		Size: 5.3 MB (5324495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a145fdb30f8770792ca38c6afc0bb3fe473f4466cb7e70929837dea2cecc1b`  
		Last Modified: Fri, 13 May 2022 23:25:59 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5b0822f40524712329a68b9a34e4cf8dc0de6730a88eaf95a65071276729bd`  
		Last Modified: Fri, 13 May 2022 23:25:59 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb540f7cbe055ceb60a812ea9c4bc8372997e67c51316092cb5bd2ae2a8c5fd1`  
		Last Modified: Fri, 13 May 2022 23:25:59 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:dacc704ea2ebaa3419ce90a606a33f286ff2b22bc2eaccef3ecf13c2828f8102
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129091311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa76b7db555fffa3c54f90ecb35686a9d70ae4115ee37de86fd1d9c942dbae16`
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
# Sat, 14 May 2022 00:06:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu --version;     gosu nobody true
# Sat, 14 May 2022 00:06:35 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 14 May 2022 00:06:42 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 14 May 2022 00:06:42 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 14 May 2022 00:06:45 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 14 May 2022 00:06:46 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 14 May 2022 00:06:47 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 14 May 2022 00:06:49 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 14 May 2022 00:06:50 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Sat, 14 May 2022 00:06:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 14 May 2022 00:06:51 GMT
CMD ["influxd"]
# Sat, 14 May 2022 00:06:52 GMT
EXPOSE 8086
# Sat, 14 May 2022 00:06:53 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 14 May 2022 00:06:54 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 14 May 2022 00:06:55 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 14 May 2022 00:06:56 GMT
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
	-	`sha256:0afc3d7db6fd1402a0c98e944744dfab7b0b5f751f5d23a2f8e4dbec68fa03a8`  
		Last Modified: Sat, 14 May 2022 00:09:08 GMT  
		Size: 896.1 KB (896088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89baa370716329523aa39d2eb64ce1758f98c46ace4bb46bf649698fd575ae8`  
		Last Modified: Sat, 14 May 2022 00:09:15 GMT  
		Size: 110.9 MB (110891633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd29bd0526ec79f902391ae8f9660c6b06ddc3b237cf93602589ba602d1beb6`  
		Last Modified: Sat, 14 May 2022 00:09:06 GMT  
		Size: 4.9 MB (4906747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d55ea67abda746bfd79b4c959d6e45bd2c2ce8f09907f98c292e31a85a331`  
		Last Modified: Sat, 14 May 2022 00:09:05 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad8dfcdc35b737fb160cd497062ad130d5714287782447d997e00453a24dd7e`  
		Last Modified: Sat, 14 May 2022 00:09:05 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57389abfa9482e8ce782e9ffa475291510c2a626c2b2b5456372303f423f12d5`  
		Last Modified: Sat, 14 May 2022 00:09:05 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1.1`

```console
$ docker pull influxdb@sha256:f2770c39002fe1027c3fce8e41762853d51ca51c376ba04046dc7f1c913dbbad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1` - linux; amd64

```console
$ docker pull influxdb@sha256:649bf77e328a9ef497c0bf100fe4f6ad1bf5ee62e985bd4af08787a966548ac3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182911931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd02ed19e30304a60ff009bb0ceb0bcec39881d86b1380fab55bd724334c90ff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:42:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:42:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:14:44 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 01:14:44 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 01:15:04 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Sun, 29 May 2022 01:15:04 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sun, 29 May 2022 01:15:14 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sun, 29 May 2022 01:15:14 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sun, 29 May 2022 01:15:18 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sun, 29 May 2022 01:15:19 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 01:15:19 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 01:15:19 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 01:15:19 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sun, 29 May 2022 01:15:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:15:19 GMT
CMD ["influxd"]
# Sun, 29 May 2022 01:15:19 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:15:20 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 01:15:20 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 01:15:20 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 01:15:20 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02d86f59850f3e13d394072350625a8526b912af24b3bfc0e50e9a8862a79d0`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 7.9 MB (7856653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b047e8f2e47bdf998a952572ae5e9d64edf8e29b716be0ee50a15e6d21cb2ce`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 10.0 MB (9997224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44b41d3b54f81ac9b15b79d938c2d2f7ce9387856470f56e2b1bf6f167afae`  
		Last Modified: Sun, 29 May 2022 01:17:46 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defebe72e01b0060660d0152a33bcb207d754ff847155c4a9c35ffcfd809fe81`  
		Last Modified: Sun, 29 May 2022 01:18:06 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6a22f6313637df3a662b130df9b676c641fcffeee420a9355122e135dd86b`  
		Last Modified: Sun, 29 May 2022 01:18:11 GMT  
		Size: 108.3 MB (108324830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cb9d6503bb45cb8c98b94709ba955442016b327f130571f803563a49fa7ff9`  
		Last Modified: Sun, 29 May 2022 01:18:04 GMT  
		Size: 5.3 MB (5324488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6186c790d800358f9b2f092bc8e9f76293ea39f2afd73b1989ed3342387abe4a`  
		Last Modified: Sun, 29 May 2022 01:18:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171bcc724f204627040909d965bbe9ba1853fc24d1fd62a5274ffcb99398569a`  
		Last Modified: Sun, 29 May 2022 01:18:03 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6f370faad6406facbe1f4bd6f759783b517eaddf46f663016c99fc6c1a971c`  
		Last Modified: Sun, 29 May 2022 01:18:03 GMT  
		Size: 5.0 KB (5013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:be2633ade4dcfc5b9c463e7eccb5324e9cdac874bf3982db93cbd5cd58dd490f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183418008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f097f737bf20cffa6ea7ba95e44579195ebef06cd8a53a8299ad46f5260c8d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:07:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 02:28:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 02:28:55 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 02:29:38 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Sun, 29 May 2022 02:29:38 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sun, 29 May 2022 02:29:55 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sun, 29 May 2022 02:29:56 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sun, 29 May 2022 02:30:00 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sun, 29 May 2022 02:30:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 02:30:01 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 02:30:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 02:30:04 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sun, 29 May 2022 02:30:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 02:30:05 GMT
CMD ["influxd"]
# Sun, 29 May 2022 02:30:06 GMT
EXPOSE 8086
# Sun, 29 May 2022 02:30:07 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 02:30:08 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 02:30:09 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 02:30:10 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5795076bf6e9bf96da71f2e31cbe91d3c49a17f211c5b0d33e032e095c5564a5`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 7.7 MB (7719823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eda3e266fa432ba8ae8ba25a5ad2fa4c5349ef2aa244612c89f990704c5b25`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 9.8 MB (9767307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0f5443af812585848f35a0c394a1510e548db84651500f20b69c8fd177c0e2`  
		Last Modified: Sun, 29 May 2022 02:31:56 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74321fb0673e5200e61727207187742de353b576e99c069daa95938cbcc3c34`  
		Last Modified: Sun, 29 May 2022 02:32:19 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ff5c8727d66245fc8f1b942f3e38b9192440d023ffc22893bfa7a18dd1ff93`  
		Last Modified: Sun, 29 May 2022 02:32:26 GMT  
		Size: 110.9 MB (110891645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a51679d7c35d3500995d74c22e447c4d6b718981b4c84102a1a557e2f480e67`  
		Last Modified: Sun, 29 May 2022 02:32:17 GMT  
		Size: 4.9 MB (4906728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867099d45360c2f3f7c57077c69779e1b7f26819a74ba816df4f09dd20a528fb`  
		Last Modified: Sun, 29 May 2022 02:32:17 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793f10209d5243f80d3ae22ba8c2e3698b31dcf54577a0b446803813e7c94135`  
		Last Modified: Sun, 29 May 2022 02:32:17 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f4cc8cad56f9798684c779a88fad21b5344d7f0afecd3932762b731ceb27b0`  
		Last Modified: Sun, 29 May 2022 02:32:17 GMT  
		Size: 5.0 KB (5013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1.1-alpine`

```console
$ docker pull influxdb@sha256:b0526384d0abb3ea2a98a8f4ee3fdb8e0fb8a3db3afbcc3d030963dcaecd62b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:76ff3abffce8813793a72cf43cae3e39947804ea5aca2c3eb51efc5971484c38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127272080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7c55292c93aa37a83cb792257e68898d826204c401ab8e3b291b79b501a2d97`
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
# Fri, 13 May 2022 23:23:18 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu --version;     gosu nobody true
# Fri, 13 May 2022 23:23:18 GMT
ENV INFLUXDB_VERSION=2.1.1
# Fri, 13 May 2022 23:23:25 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 13 May 2022 23:23:25 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Fri, 13 May 2022 23:23:28 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 13 May 2022 23:23:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 13 May 2022 23:23:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 13 May 2022 23:23:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 13 May 2022 23:23:29 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Fri, 13 May 2022 23:23:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 May 2022 23:23:29 GMT
CMD ["influxd"]
# Fri, 13 May 2022 23:23:29 GMT
EXPOSE 8086
# Fri, 13 May 2022 23:23:29 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 13 May 2022 23:23:29 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 13 May 2022 23:23:30 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 13 May 2022 23:23:30 GMT
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
	-	`sha256:c9e8df9da8d1c8426e1caad99cf5795de908d0c016597335d6ea348135fe0207`  
		Last Modified: Fri, 13 May 2022 23:26:02 GMT  
		Size: 960.6 KB (960628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cf4a1abffaa9098b3c38918f1b2b3945f2fe047fec65bcfc2d9b83aafafa78`  
		Last Modified: Fri, 13 May 2022 23:26:08 GMT  
		Size: 108.3 MB (108324839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4612c9f990cb7934b692da9ed47390228bc4342dd3903d82d98fd8fc2c72d`  
		Last Modified: Fri, 13 May 2022 23:26:00 GMT  
		Size: 5.3 MB (5324495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a145fdb30f8770792ca38c6afc0bb3fe473f4466cb7e70929837dea2cecc1b`  
		Last Modified: Fri, 13 May 2022 23:25:59 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5b0822f40524712329a68b9a34e4cf8dc0de6730a88eaf95a65071276729bd`  
		Last Modified: Fri, 13 May 2022 23:25:59 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb540f7cbe055ceb60a812ea9c4bc8372997e67c51316092cb5bd2ae2a8c5fd1`  
		Last Modified: Fri, 13 May 2022 23:25:59 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:dacc704ea2ebaa3419ce90a606a33f286ff2b22bc2eaccef3ecf13c2828f8102
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129091311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa76b7db555fffa3c54f90ecb35686a9d70ae4115ee37de86fd1d9c942dbae16`
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
# Sat, 14 May 2022 00:06:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu --version;     gosu nobody true
# Sat, 14 May 2022 00:06:35 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 14 May 2022 00:06:42 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 14 May 2022 00:06:42 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 14 May 2022 00:06:45 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 14 May 2022 00:06:46 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 14 May 2022 00:06:47 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 14 May 2022 00:06:49 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 14 May 2022 00:06:50 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Sat, 14 May 2022 00:06:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 14 May 2022 00:06:51 GMT
CMD ["influxd"]
# Sat, 14 May 2022 00:06:52 GMT
EXPOSE 8086
# Sat, 14 May 2022 00:06:53 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 14 May 2022 00:06:54 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 14 May 2022 00:06:55 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 14 May 2022 00:06:56 GMT
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
	-	`sha256:0afc3d7db6fd1402a0c98e944744dfab7b0b5f751f5d23a2f8e4dbec68fa03a8`  
		Last Modified: Sat, 14 May 2022 00:09:08 GMT  
		Size: 896.1 KB (896088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89baa370716329523aa39d2eb64ce1758f98c46ace4bb46bf649698fd575ae8`  
		Last Modified: Sat, 14 May 2022 00:09:15 GMT  
		Size: 110.9 MB (110891633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd29bd0526ec79f902391ae8f9660c6b06ddc3b237cf93602589ba602d1beb6`  
		Last Modified: Sat, 14 May 2022 00:09:06 GMT  
		Size: 4.9 MB (4906747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d55ea67abda746bfd79b4c959d6e45bd2c2ce8f09907f98c292e31a85a331`  
		Last Modified: Sat, 14 May 2022 00:09:05 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad8dfcdc35b737fb160cd497062ad130d5714287782447d997e00453a24dd7e`  
		Last Modified: Sat, 14 May 2022 00:09:05 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57389abfa9482e8ce782e9ffa475291510c2a626c2b2b5456372303f423f12d5`  
		Last Modified: Sat, 14 May 2022 00:09:05 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.2`

```console
$ docker pull influxdb@sha256:6001e2ccabc8009dceae5de97019781ae10ae55868c1212b9426e89943550847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.2` - linux; amd64

```console
$ docker pull influxdb@sha256:3348f6b261ffd5c5ddee200a1a94b8848da96c68d19504b4c25931801894535c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.9 MB (181850005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b24dbcedefc1fa73c6a92cf682e27f060e2fc8f78511a2a76bfbf5417093888`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:42:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:42:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:14:44 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 01:14:44 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 01:15:04 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Sun, 29 May 2022 01:15:26 GMT
ENV INFLUXDB_VERSION=2.2.0
# Sun, 29 May 2022 01:15:37 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sun, 29 May 2022 01:15:37 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Sun, 29 May 2022 01:15:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sun, 29 May 2022 01:15:40 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 01:15:41 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 01:15:41 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 01:15:41 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sun, 29 May 2022 01:15:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:15:41 GMT
CMD ["influxd"]
# Sun, 29 May 2022 01:15:41 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:15:41 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 01:15:41 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 01:15:41 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 01:15:42 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02d86f59850f3e13d394072350625a8526b912af24b3bfc0e50e9a8862a79d0`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 7.9 MB (7856653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b047e8f2e47bdf998a952572ae5e9d64edf8e29b716be0ee50a15e6d21cb2ce`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 10.0 MB (9997224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44b41d3b54f81ac9b15b79d938c2d2f7ce9387856470f56e2b1bf6f167afae`  
		Last Modified: Sun, 29 May 2022 01:17:46 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defebe72e01b0060660d0152a33bcb207d754ff847155c4a9c35ffcfd809fe81`  
		Last Modified: Sun, 29 May 2022 01:18:06 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2d01e46b1fec6e451eeadf8e00735c4b6be6c449837da2f495a3153dd65140`  
		Last Modified: Sun, 29 May 2022 01:18:30 GMT  
		Size: 107.2 MB (107220548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a325b0038b0f2326faa051d52cae8bf4bf3c3350cc08fe15dda650de91f3d5e`  
		Last Modified: Sun, 29 May 2022 01:18:23 GMT  
		Size: 5.4 MB (5366842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19c51cfbec38bacf3c3c30565ebec25e0ed03719d3d47723522b8578fcf5745`  
		Last Modified: Sun, 29 May 2022 01:18:21 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3486ad84606fa9a4090b690401c84b6a75678ce3934506d272f6ac0459df452e`  
		Last Modified: Sun, 29 May 2022 01:18:21 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671d1fd30484ca27a5abaad71fcb3ffafbca409ea5f3a4a9851ceb7b628859a`  
		Last Modified: Sun, 29 May 2022 01:18:22 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.2` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:7580fcf2b3b85100d95ec77228afc65fcec01c31a77c0581d76897ebf7e7aecb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182450179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf0f548452395ddbb1b10f2f0193303da25caa4b93da3ce162f53f6a77c99b97`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:07:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 02:28:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 02:28:55 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 02:29:38 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Sun, 29 May 2022 02:30:24 GMT
ENV INFLUXDB_VERSION=2.2.0
# Sun, 29 May 2022 02:30:34 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sun, 29 May 2022 02:30:34 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Sun, 29 May 2022 02:30:43 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sun, 29 May 2022 02:30:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 02:30:44 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 02:30:46 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 02:30:47 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sun, 29 May 2022 02:30:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 02:30:48 GMT
CMD ["influxd"]
# Sun, 29 May 2022 02:30:49 GMT
EXPOSE 8086
# Sun, 29 May 2022 02:30:50 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 02:30:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 02:30:52 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 02:30:53 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5795076bf6e9bf96da71f2e31cbe91d3c49a17f211c5b0d33e032e095c5564a5`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 7.7 MB (7719823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eda3e266fa432ba8ae8ba25a5ad2fa4c5349ef2aa244612c89f990704c5b25`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 9.8 MB (9767307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0f5443af812585848f35a0c394a1510e548db84651500f20b69c8fd177c0e2`  
		Last Modified: Sun, 29 May 2022 02:31:56 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74321fb0673e5200e61727207187742de353b576e99c069daa95938cbcc3c34`  
		Last Modified: Sun, 29 May 2022 02:32:19 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6355637454b964dbfe575e8cd41511f8bfbe66731fb99be45690bfa099dcf1f6`  
		Last Modified: Sun, 29 May 2022 02:32:49 GMT  
		Size: 109.9 MB (109877910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe5962b941f6b217210533974260e8e909232929908250c1574696b92f3936f`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 5.0 MB (4952630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60111b462a9c3152cdc36c7e6e0da1d66f7e49c095a650298eb3a528587597c`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9045af35515f3059bb942ff8335d089d33c77b74b890184932dc869ffd9d97ae`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8688444f0cbf9b6677ac03fafa1216dcedf6d82ebe354e02a99b552a8d4cba`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.2-alpine`

```console
$ docker pull influxdb@sha256:8c4c759256fe60404ee2c7948c5fd41bb3516a0d0a03938ae88dbcca973aa20a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.2-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:773cd5c1c13206b041699ce85c15f102a47f2a873cd795e19bccc9a4fa611ad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126210156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0319a19d73f86be1c6fe8fa54a8f40a1c29774419c75fc5605927eba847d851c`
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
# Fri, 13 May 2022 23:23:18 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu --version;     gosu nobody true
# Fri, 13 May 2022 23:23:51 GMT
ENV INFLUXDB_VERSION=2.2.0
# Fri, 13 May 2022 23:23:58 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 13 May 2022 23:23:58 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Fri, 13 May 2022 23:24:01 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 13 May 2022 23:24:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 13 May 2022 23:24:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 13 May 2022 23:24:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 13 May 2022 23:24:02 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Fri, 13 May 2022 23:24:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 May 2022 23:24:02 GMT
CMD ["influxd"]
# Fri, 13 May 2022 23:24:02 GMT
EXPOSE 8086
# Fri, 13 May 2022 23:24:02 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 13 May 2022 23:24:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 13 May 2022 23:24:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 13 May 2022 23:24:03 GMT
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
	-	`sha256:c9e8df9da8d1c8426e1caad99cf5795de908d0c016597335d6ea348135fe0207`  
		Last Modified: Fri, 13 May 2022 23:26:02 GMT  
		Size: 960.6 KB (960628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59158600988bc4e3f133be53214acdddfb0614d41e5c5de9d5aaf992f1a2fa68`  
		Last Modified: Fri, 13 May 2022 23:26:48 GMT  
		Size: 107.2 MB (107220537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3015f45475dbe8293139cd81dc54ecde8cef0ea6171ca888ae91140cac4e6c`  
		Last Modified: Fri, 13 May 2022 23:26:41 GMT  
		Size: 5.4 MB (5366873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a719d14db8fff5fc5144bdef9f52a423b0e95c1beb67d1f2139bb7fb2a8bcd`  
		Last Modified: Fri, 13 May 2022 23:26:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd65e63e274dde9f185aeec4d298c0768b2fc26d6b49aca43b6c1010aea6a279`  
		Last Modified: Fri, 13 May 2022 23:26:40 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d3d9d888e71fa4ac0b23d44cf101f1ed568e7d1257e01598d928d086225033`  
		Last Modified: Fri, 13 May 2022 23:26:40 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:63d31763855a4dd9f0adb8d1cd39067ced574968dac67443958b2567a4b52083
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128123546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88b4c297a04b088fb506976dfa051844f3f9d9447b1091137156b0a2ea72098`
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
# Sat, 14 May 2022 00:06:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu --version;     gosu nobody true
# Sat, 14 May 2022 00:07:40 GMT
ENV INFLUXDB_VERSION=2.2.0
# Sat, 14 May 2022 00:07:49 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 14 May 2022 00:07:49 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Sat, 14 May 2022 00:07:52 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 14 May 2022 00:07:53 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 14 May 2022 00:07:54 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 14 May 2022 00:07:56 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 14 May 2022 00:07:57 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Sat, 14 May 2022 00:07:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 14 May 2022 00:07:58 GMT
CMD ["influxd"]
# Sat, 14 May 2022 00:07:59 GMT
EXPOSE 8086
# Sat, 14 May 2022 00:08:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 14 May 2022 00:08:01 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 14 May 2022 00:08:02 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 14 May 2022 00:08:03 GMT
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
	-	`sha256:0afc3d7db6fd1402a0c98e944744dfab7b0b5f751f5d23a2f8e4dbec68fa03a8`  
		Last Modified: Sat, 14 May 2022 00:09:08 GMT  
		Size: 896.1 KB (896088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308efbff13826540c88ce6d36eb2944813343286cc791ac8be604fb3dfb12780`  
		Last Modified: Sat, 14 May 2022 00:10:00 GMT  
		Size: 109.9 MB (109877960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45401ea99dc04a9b5d8bbb4a6b4f2e73c41393986dcd23ee5dd00acf1bd51251`  
		Last Modified: Sat, 14 May 2022 00:09:51 GMT  
		Size: 5.0 MB (4952652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e3ffe8a4ff9b9b439a6a8dad9de48f5ce3c2e11e9118d7233b45a2b0734971`  
		Last Modified: Sat, 14 May 2022 00:09:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b681591c87c3e0de6d3438e39881a98a10fe38f6f3369e01f6f0e89f511099`  
		Last Modified: Sat, 14 May 2022 00:09:50 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1803ca7cf48730bbafdbfc11bd10eab4c556f0fc3696c20594d731c4d9658f`  
		Last Modified: Sat, 14 May 2022 00:09:50 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.2.0`

```console
$ docker pull influxdb@sha256:6001e2ccabc8009dceae5de97019781ae10ae55868c1212b9426e89943550847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:3348f6b261ffd5c5ddee200a1a94b8848da96c68d19504b4c25931801894535c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.9 MB (181850005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b24dbcedefc1fa73c6a92cf682e27f060e2fc8f78511a2a76bfbf5417093888`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:42:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:42:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:14:44 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 01:14:44 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 01:15:04 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Sun, 29 May 2022 01:15:26 GMT
ENV INFLUXDB_VERSION=2.2.0
# Sun, 29 May 2022 01:15:37 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sun, 29 May 2022 01:15:37 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Sun, 29 May 2022 01:15:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sun, 29 May 2022 01:15:40 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 01:15:41 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 01:15:41 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 01:15:41 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sun, 29 May 2022 01:15:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:15:41 GMT
CMD ["influxd"]
# Sun, 29 May 2022 01:15:41 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:15:41 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 01:15:41 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 01:15:41 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 01:15:42 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02d86f59850f3e13d394072350625a8526b912af24b3bfc0e50e9a8862a79d0`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 7.9 MB (7856653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b047e8f2e47bdf998a952572ae5e9d64edf8e29b716be0ee50a15e6d21cb2ce`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 10.0 MB (9997224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44b41d3b54f81ac9b15b79d938c2d2f7ce9387856470f56e2b1bf6f167afae`  
		Last Modified: Sun, 29 May 2022 01:17:46 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defebe72e01b0060660d0152a33bcb207d754ff847155c4a9c35ffcfd809fe81`  
		Last Modified: Sun, 29 May 2022 01:18:06 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2d01e46b1fec6e451eeadf8e00735c4b6be6c449837da2f495a3153dd65140`  
		Last Modified: Sun, 29 May 2022 01:18:30 GMT  
		Size: 107.2 MB (107220548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a325b0038b0f2326faa051d52cae8bf4bf3c3350cc08fe15dda650de91f3d5e`  
		Last Modified: Sun, 29 May 2022 01:18:23 GMT  
		Size: 5.4 MB (5366842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19c51cfbec38bacf3c3c30565ebec25e0ed03719d3d47723522b8578fcf5745`  
		Last Modified: Sun, 29 May 2022 01:18:21 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3486ad84606fa9a4090b690401c84b6a75678ce3934506d272f6ac0459df452e`  
		Last Modified: Sun, 29 May 2022 01:18:21 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671d1fd30484ca27a5abaad71fcb3ffafbca409ea5f3a4a9851ceb7b628859a`  
		Last Modified: Sun, 29 May 2022 01:18:22 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:7580fcf2b3b85100d95ec77228afc65fcec01c31a77c0581d76897ebf7e7aecb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182450179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf0f548452395ddbb1b10f2f0193303da25caa4b93da3ce162f53f6a77c99b97`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:07:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 02:28:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 02:28:55 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 02:29:38 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Sun, 29 May 2022 02:30:24 GMT
ENV INFLUXDB_VERSION=2.2.0
# Sun, 29 May 2022 02:30:34 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sun, 29 May 2022 02:30:34 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Sun, 29 May 2022 02:30:43 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sun, 29 May 2022 02:30:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 02:30:44 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 02:30:46 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 02:30:47 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sun, 29 May 2022 02:30:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 02:30:48 GMT
CMD ["influxd"]
# Sun, 29 May 2022 02:30:49 GMT
EXPOSE 8086
# Sun, 29 May 2022 02:30:50 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 02:30:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 02:30:52 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 02:30:53 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5795076bf6e9bf96da71f2e31cbe91d3c49a17f211c5b0d33e032e095c5564a5`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 7.7 MB (7719823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eda3e266fa432ba8ae8ba25a5ad2fa4c5349ef2aa244612c89f990704c5b25`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 9.8 MB (9767307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0f5443af812585848f35a0c394a1510e548db84651500f20b69c8fd177c0e2`  
		Last Modified: Sun, 29 May 2022 02:31:56 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74321fb0673e5200e61727207187742de353b576e99c069daa95938cbcc3c34`  
		Last Modified: Sun, 29 May 2022 02:32:19 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6355637454b964dbfe575e8cd41511f8bfbe66731fb99be45690bfa099dcf1f6`  
		Last Modified: Sun, 29 May 2022 02:32:49 GMT  
		Size: 109.9 MB (109877910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe5962b941f6b217210533974260e8e909232929908250c1574696b92f3936f`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 5.0 MB (4952630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60111b462a9c3152cdc36c7e6e0da1d66f7e49c095a650298eb3a528587597c`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9045af35515f3059bb942ff8335d089d33c77b74b890184932dc869ffd9d97ae`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8688444f0cbf9b6677ac03fafa1216dcedf6d82ebe354e02a99b552a8d4cba`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.2.0-alpine`

```console
$ docker pull influxdb@sha256:8c4c759256fe60404ee2c7948c5fd41bb3516a0d0a03938ae88dbcca973aa20a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.2.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:773cd5c1c13206b041699ce85c15f102a47f2a873cd795e19bccc9a4fa611ad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126210156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0319a19d73f86be1c6fe8fa54a8f40a1c29774419c75fc5605927eba847d851c`
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
# Fri, 13 May 2022 23:23:18 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu --version;     gosu nobody true
# Fri, 13 May 2022 23:23:51 GMT
ENV INFLUXDB_VERSION=2.2.0
# Fri, 13 May 2022 23:23:58 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 13 May 2022 23:23:58 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Fri, 13 May 2022 23:24:01 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 13 May 2022 23:24:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 13 May 2022 23:24:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 13 May 2022 23:24:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 13 May 2022 23:24:02 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Fri, 13 May 2022 23:24:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 May 2022 23:24:02 GMT
CMD ["influxd"]
# Fri, 13 May 2022 23:24:02 GMT
EXPOSE 8086
# Fri, 13 May 2022 23:24:02 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 13 May 2022 23:24:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 13 May 2022 23:24:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 13 May 2022 23:24:03 GMT
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
	-	`sha256:c9e8df9da8d1c8426e1caad99cf5795de908d0c016597335d6ea348135fe0207`  
		Last Modified: Fri, 13 May 2022 23:26:02 GMT  
		Size: 960.6 KB (960628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59158600988bc4e3f133be53214acdddfb0614d41e5c5de9d5aaf992f1a2fa68`  
		Last Modified: Fri, 13 May 2022 23:26:48 GMT  
		Size: 107.2 MB (107220537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3015f45475dbe8293139cd81dc54ecde8cef0ea6171ca888ae91140cac4e6c`  
		Last Modified: Fri, 13 May 2022 23:26:41 GMT  
		Size: 5.4 MB (5366873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a719d14db8fff5fc5144bdef9f52a423b0e95c1beb67d1f2139bb7fb2a8bcd`  
		Last Modified: Fri, 13 May 2022 23:26:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd65e63e274dde9f185aeec4d298c0768b2fc26d6b49aca43b6c1010aea6a279`  
		Last Modified: Fri, 13 May 2022 23:26:40 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d3d9d888e71fa4ac0b23d44cf101f1ed568e7d1257e01598d928d086225033`  
		Last Modified: Fri, 13 May 2022 23:26:40 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:63d31763855a4dd9f0adb8d1cd39067ced574968dac67443958b2567a4b52083
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128123546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88b4c297a04b088fb506976dfa051844f3f9d9447b1091137156b0a2ea72098`
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
# Sat, 14 May 2022 00:06:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu --version;     gosu nobody true
# Sat, 14 May 2022 00:07:40 GMT
ENV INFLUXDB_VERSION=2.2.0
# Sat, 14 May 2022 00:07:49 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 14 May 2022 00:07:49 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Sat, 14 May 2022 00:07:52 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 14 May 2022 00:07:53 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 14 May 2022 00:07:54 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 14 May 2022 00:07:56 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 14 May 2022 00:07:57 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Sat, 14 May 2022 00:07:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 14 May 2022 00:07:58 GMT
CMD ["influxd"]
# Sat, 14 May 2022 00:07:59 GMT
EXPOSE 8086
# Sat, 14 May 2022 00:08:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 14 May 2022 00:08:01 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 14 May 2022 00:08:02 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 14 May 2022 00:08:03 GMT
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
	-	`sha256:0afc3d7db6fd1402a0c98e944744dfab7b0b5f751f5d23a2f8e4dbec68fa03a8`  
		Last Modified: Sat, 14 May 2022 00:09:08 GMT  
		Size: 896.1 KB (896088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308efbff13826540c88ce6d36eb2944813343286cc791ac8be604fb3dfb12780`  
		Last Modified: Sat, 14 May 2022 00:10:00 GMT  
		Size: 109.9 MB (109877960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45401ea99dc04a9b5d8bbb4a6b4f2e73c41393986dcd23ee5dd00acf1bd51251`  
		Last Modified: Sat, 14 May 2022 00:09:51 GMT  
		Size: 5.0 MB (4952652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e3ffe8a4ff9b9b439a6a8dad9de48f5ce3c2e11e9118d7233b45a2b0734971`  
		Last Modified: Sat, 14 May 2022 00:09:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b681591c87c3e0de6d3438e39881a98a10fe38f6f3369e01f6f0e89f511099`  
		Last Modified: Sat, 14 May 2022 00:09:50 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1803ca7cf48730bbafdbfc11bd10eab4c556f0fc3696c20594d731c4d9658f`  
		Last Modified: Sat, 14 May 2022 00:09:50 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:8c4c759256fe60404ee2c7948c5fd41bb3516a0d0a03938ae88dbcca973aa20a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:773cd5c1c13206b041699ce85c15f102a47f2a873cd795e19bccc9a4fa611ad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126210156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0319a19d73f86be1c6fe8fa54a8f40a1c29774419c75fc5605927eba847d851c`
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
# Fri, 13 May 2022 23:23:18 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu --version;     gosu nobody true
# Fri, 13 May 2022 23:23:51 GMT
ENV INFLUXDB_VERSION=2.2.0
# Fri, 13 May 2022 23:23:58 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 13 May 2022 23:23:58 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Fri, 13 May 2022 23:24:01 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 13 May 2022 23:24:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 13 May 2022 23:24:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 13 May 2022 23:24:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 13 May 2022 23:24:02 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Fri, 13 May 2022 23:24:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 May 2022 23:24:02 GMT
CMD ["influxd"]
# Fri, 13 May 2022 23:24:02 GMT
EXPOSE 8086
# Fri, 13 May 2022 23:24:02 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 13 May 2022 23:24:03 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 13 May 2022 23:24:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 13 May 2022 23:24:03 GMT
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
	-	`sha256:c9e8df9da8d1c8426e1caad99cf5795de908d0c016597335d6ea348135fe0207`  
		Last Modified: Fri, 13 May 2022 23:26:02 GMT  
		Size: 960.6 KB (960628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59158600988bc4e3f133be53214acdddfb0614d41e5c5de9d5aaf992f1a2fa68`  
		Last Modified: Fri, 13 May 2022 23:26:48 GMT  
		Size: 107.2 MB (107220537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3015f45475dbe8293139cd81dc54ecde8cef0ea6171ca888ae91140cac4e6c`  
		Last Modified: Fri, 13 May 2022 23:26:41 GMT  
		Size: 5.4 MB (5366873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a719d14db8fff5fc5144bdef9f52a423b0e95c1beb67d1f2139bb7fb2a8bcd`  
		Last Modified: Fri, 13 May 2022 23:26:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd65e63e274dde9f185aeec4d298c0768b2fc26d6b49aca43b6c1010aea6a279`  
		Last Modified: Fri, 13 May 2022 23:26:40 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d3d9d888e71fa4ac0b23d44cf101f1ed568e7d1257e01598d928d086225033`  
		Last Modified: Fri, 13 May 2022 23:26:40 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:63d31763855a4dd9f0adb8d1cd39067ced574968dac67443958b2567a4b52083
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128123546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88b4c297a04b088fb506976dfa051844f3f9d9447b1091137156b0a2ea72098`
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
# Sat, 14 May 2022 00:06:34 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     gpgconf --kill all;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu --version;     gosu nobody true
# Sat, 14 May 2022 00:07:40 GMT
ENV INFLUXDB_VERSION=2.2.0
# Sat, 14 May 2022 00:07:49 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 14 May 2022 00:07:49 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Sat, 14 May 2022 00:07:52 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 14 May 2022 00:07:53 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 14 May 2022 00:07:54 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 14 May 2022 00:07:56 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 14 May 2022 00:07:57 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Sat, 14 May 2022 00:07:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 14 May 2022 00:07:58 GMT
CMD ["influxd"]
# Sat, 14 May 2022 00:07:59 GMT
EXPOSE 8086
# Sat, 14 May 2022 00:08:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 14 May 2022 00:08:01 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 14 May 2022 00:08:02 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 14 May 2022 00:08:03 GMT
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
	-	`sha256:0afc3d7db6fd1402a0c98e944744dfab7b0b5f751f5d23a2f8e4dbec68fa03a8`  
		Last Modified: Sat, 14 May 2022 00:09:08 GMT  
		Size: 896.1 KB (896088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308efbff13826540c88ce6d36eb2944813343286cc791ac8be604fb3dfb12780`  
		Last Modified: Sat, 14 May 2022 00:10:00 GMT  
		Size: 109.9 MB (109877960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45401ea99dc04a9b5d8bbb4a6b4f2e73c41393986dcd23ee5dd00acf1bd51251`  
		Last Modified: Sat, 14 May 2022 00:09:51 GMT  
		Size: 5.0 MB (4952652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e3ffe8a4ff9b9b439a6a8dad9de48f5ce3c2e11e9118d7233b45a2b0734971`  
		Last Modified: Sat, 14 May 2022 00:09:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b681591c87c3e0de6d3438e39881a98a10fe38f6f3369e01f6f0e89f511099`  
		Last Modified: Sat, 14 May 2022 00:09:50 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1803ca7cf48730bbafdbfc11bd10eab4c556f0fc3696c20594d731c4d9658f`  
		Last Modified: Sat, 14 May 2022 00:09:50 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:80d1447e23194ac263dc324d567eaca3cd7d8c743286466eb403a193be76806d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:f057b9826c94f3cbffeae1559f46aa7d57e11d4313d620ebb2b8f3c03de49aba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117789479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e07f37814d7711a17b11ae3b7b0c2494ddd56c77a1f31560ec99d38cf733e6d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:14:07 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sun, 29 May 2022 01:14:12 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sun, 29 May 2022 01:14:13 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sun, 29 May 2022 01:14:13 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:14:13 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:13 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:13 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 29 May 2022 01:14:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:13 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd97197a056b127568e26d51e8dc0b1726ec9dac509b9c2e7de161521dffe9f`  
		Last Modified: Sun, 29 May 2022 01:16:47 GMT  
		Size: 56.7 MB (56709134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c0d2f38f0f0cd00842c355b2780895a8dff3d698baf794162c142ae4301837`  
		Last Modified: Sun, 29 May 2022 01:16:40 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b4717d882bf2ca3662fbd88b6cb429c8cfc1002675288fd52c7dad654bfb49`  
		Last Modified: Sun, 29 May 2022 01:16:40 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db994e43254a59c721f524e5585b89f7b7efd529dc94349c11eadd14216f4fcd`  
		Last Modified: Sun, 29 May 2022 01:16:40 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:6001e2ccabc8009dceae5de97019781ae10ae55868c1212b9426e89943550847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:3348f6b261ffd5c5ddee200a1a94b8848da96c68d19504b4c25931801894535c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.9 MB (181850005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b24dbcedefc1fa73c6a92cf682e27f060e2fc8f78511a2a76bfbf5417093888`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:42:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:42:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:14:44 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 01:14:44 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 01:15:04 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Sun, 29 May 2022 01:15:26 GMT
ENV INFLUXDB_VERSION=2.2.0
# Sun, 29 May 2022 01:15:37 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sun, 29 May 2022 01:15:37 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Sun, 29 May 2022 01:15:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sun, 29 May 2022 01:15:40 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 01:15:41 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 01:15:41 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 01:15:41 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sun, 29 May 2022 01:15:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:15:41 GMT
CMD ["influxd"]
# Sun, 29 May 2022 01:15:41 GMT
EXPOSE 8086
# Sun, 29 May 2022 01:15:41 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 01:15:41 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 01:15:41 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 01:15:42 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02d86f59850f3e13d394072350625a8526b912af24b3bfc0e50e9a8862a79d0`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 7.9 MB (7856653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b047e8f2e47bdf998a952572ae5e9d64edf8e29b716be0ee50a15e6d21cb2ce`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 10.0 MB (9997224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc44b41d3b54f81ac9b15b79d938c2d2f7ce9387856470f56e2b1bf6f167afae`  
		Last Modified: Sun, 29 May 2022 01:17:46 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defebe72e01b0060660d0152a33bcb207d754ff847155c4a9c35ffcfd809fe81`  
		Last Modified: Sun, 29 May 2022 01:18:06 GMT  
		Size: 961.0 KB (960960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2d01e46b1fec6e451eeadf8e00735c4b6be6c449837da2f495a3153dd65140`  
		Last Modified: Sun, 29 May 2022 01:18:30 GMT  
		Size: 107.2 MB (107220548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a325b0038b0f2326faa051d52cae8bf4bf3c3350cc08fe15dda650de91f3d5e`  
		Last Modified: Sun, 29 May 2022 01:18:23 GMT  
		Size: 5.4 MB (5366842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19c51cfbec38bacf3c3c30565ebec25e0ed03719d3d47723522b8578fcf5745`  
		Last Modified: Sun, 29 May 2022 01:18:21 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3486ad84606fa9a4090b690401c84b6a75678ce3934506d272f6ac0459df452e`  
		Last Modified: Sun, 29 May 2022 01:18:21 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0671d1fd30484ca27a5abaad71fcb3ffafbca409ea5f3a4a9851ceb7b628859a`  
		Last Modified: Sun, 29 May 2022 01:18:22 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:7580fcf2b3b85100d95ec77228afc65fcec01c31a77c0581d76897ebf7e7aecb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182450179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf0f548452395ddbb1b10f2f0193303da25caa4b93da3ce162f53f6a77c99b97`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 28 May 2022 00:40:49 GMT
ADD file:af879be34a7eccc177a3000eb8c45d5207bfbec108caf9be9d11c1a6620c376c in / 
# Sat, 28 May 2022 00:40:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:07:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 02:28:55 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sun, 29 May 2022 02:28:55 GMT
ENV GOSU_VER=1.12
# Sun, 29 May 2022 02:29:38 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Sun, 29 May 2022 02:30:24 GMT
ENV INFLUXDB_VERSION=2.2.0
# Sun, 29 May 2022 02:30:34 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sun, 29 May 2022 02:30:34 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Sun, 29 May 2022 02:30:43 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sun, 29 May 2022 02:30:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sun, 29 May 2022 02:30:44 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sun, 29 May 2022 02:30:46 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sun, 29 May 2022 02:30:47 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sun, 29 May 2022 02:30:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 02:30:48 GMT
CMD ["influxd"]
# Sun, 29 May 2022 02:30:49 GMT
EXPOSE 8086
# Sun, 29 May 2022 02:30:50 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sun, 29 May 2022 02:30:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Sun, 29 May 2022 02:30:52 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sun, 29 May 2022 02:30:53 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:fadbed17b01e84815ca3018d3dc42670c3add65c67e7cc74d6bc477ae8425934`  
		Last Modified: Sat, 28 May 2022 00:47:58 GMT  
		Size: 49.2 MB (49229054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5795076bf6e9bf96da71f2e31cbe91d3c49a17f211c5b0d33e032e095c5564a5`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 7.7 MB (7719823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eda3e266fa432ba8ae8ba25a5ad2fa4c5349ef2aa244612c89f990704c5b25`  
		Last Modified: Sat, 28 May 2022 11:18:22 GMT  
		Size: 9.8 MB (9767307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0f5443af812585848f35a0c394a1510e548db84651500f20b69c8fd177c0e2`  
		Last Modified: Sun, 29 May 2022 02:31:56 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74321fb0673e5200e61727207187742de353b576e99c069daa95938cbcc3c34`  
		Last Modified: Sun, 29 May 2022 02:32:19 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6355637454b964dbfe575e8cd41511f8bfbe66731fb99be45690bfa099dcf1f6`  
		Last Modified: Sun, 29 May 2022 02:32:49 GMT  
		Size: 109.9 MB (109877910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe5962b941f6b217210533974260e8e909232929908250c1574696b92f3936f`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 5.0 MB (4952630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60111b462a9c3152cdc36c7e6e0da1d66f7e49c095a650298eb3a528587597c`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9045af35515f3059bb942ff8335d089d33c77b74b890184932dc869ffd9d97ae`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8688444f0cbf9b6677ac03fafa1216dcedf6d82ebe354e02a99b552a8d4cba`  
		Last Modified: Sun, 29 May 2022 02:32:40 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:8d5402e304325edfcfe660e5321fcb966321984116fbaf1d7e4087a6a813dcbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:6fb1429a96ad2bcc86b596dc4f45b7a181217051455baafb8050e0be81531136
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84496090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7274da2aaef773679225007f1a42b5b7b34b2e3465543334a2ab49705e3491ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:13:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:14:07 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sun, 29 May 2022 01:14:21 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sun, 29 May 2022 01:14:21 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sun, 29 May 2022 01:14:21 GMT
EXPOSE 8091
# Sun, 29 May 2022 01:14:22 GMT
VOLUME [/var/lib/influxdb]
# Sun, 29 May 2022 01:14:22 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sun, 29 May 2022 01:14:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:14:22 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386debe6a9999be3c003f19bc8848d062480e60c05f846d134e34cc9c606e0a5`  
		Last Modified: Sun, 29 May 2022 01:16:22 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d08dfd21984cd88d13eaeeef51a60a6f7b6cf6a7675932bf9801f77743b1c84`  
		Last Modified: Sun, 29 May 2022 01:17:04 GMT  
		Size: 23.4 MB (23416952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076936713b4ccd154076ca92824f3308d44b1d52dac385010c1e2e4cb7736409`  
		Last Modified: Sun, 29 May 2022 01:17:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90904d4629e11d99c4e980cecd4a397427acd53acec6df81a641928ca4ddc85`  
		Last Modified: Sun, 29 May 2022 01:17:01 GMT  
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
