<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `influxdb`

-	[`influxdb:1.7`](#influxdb17)
-	[`influxdb:1.7-alpine`](#influxdb17-alpine)
-	[`influxdb:1.7-data`](#influxdb17-data)
-	[`influxdb:1.7-data-alpine`](#influxdb17-data-alpine)
-	[`influxdb:1.7-meta`](#influxdb17-meta)
-	[`influxdb:1.7-meta-alpine`](#influxdb17-meta-alpine)
-	[`influxdb:1.7.11`](#influxdb1711)
-	[`influxdb:1.7.11-alpine`](#influxdb1711-alpine)
-	[`influxdb:1.7.11-data`](#influxdb1711-data)
-	[`influxdb:1.7.11-data-alpine`](#influxdb1711-data-alpine)
-	[`influxdb:1.7.11-meta`](#influxdb1711-meta)
-	[`influxdb:1.7.11-meta-alpine`](#influxdb1711-meta-alpine)
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
-	[`influxdb:1.9.5-data`](#influxdb195-data)
-	[`influxdb:1.9.5-data-alpine`](#influxdb195-data-alpine)
-	[`influxdb:1.9.5-meta`](#influxdb195-meta)
-	[`influxdb:1.9.5-meta-alpine`](#influxdb195-meta-alpine)
-	[`influxdb:2.0`](#influxdb20)
-	[`influxdb:2.0-alpine`](#influxdb20-alpine)
-	[`influxdb:2.0.9`](#influxdb209)
-	[`influxdb:2.0.9-alpine`](#influxdb209-alpine)
-	[`influxdb:2.1`](#influxdb21)
-	[`influxdb:2.1-alpine`](#influxdb21-alpine)
-	[`influxdb:2.1.1`](#influxdb211)
-	[`influxdb:2.1.1-alpine`](#influxdb211-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.7`

```console
$ docker pull influxdb@sha256:2f31929cd48d6f39d12a31ee3ae99ebb27cee74c472b5b0b299c1776f31440c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7` - linux; amd64

```console
$ docker pull influxdb@sha256:86f1cfcdbeb83d429e0500a28fcff348b2e4740960ba78f1d321790cb6d1e3b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122313880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f011f70cae60f0d335def46540efe2ff6d1e1330c3933cbbb9b2f85680dc2fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:43:30 GMT
ENV INFLUXDB_VERSION=1.7.11
# Thu, 18 Nov 2021 09:43:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 18 Nov 2021 09:43:39 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 18 Nov 2021 09:43:39 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:43:39 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:43:39 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:43:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 18 Nov 2021 09:43:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:43:40 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417dfa61d29cf6fef46e761c963ada353795d6c57bce1bf6d340e6a70f97a5fe`  
		Last Modified: Thu, 18 Nov 2021 09:47:44 GMT  
		Size: 61.3 MB (61285092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa30700867447cc2e95857c55e4f25527e67fd1a63c61b99ac68b29bf7c5ebaa`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed35aa167fe9bb6251995b7928b2d8f36d38565495c2669ad9a219c98de651de`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af723c50ac3e9275d6d9b32a7013ba297de967db5033d08ef3159db34bd1a783`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:64940016027dcbc31b63c7e65ff23bacb6622daefa8c8fd7bb5b4099069a429e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113470068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e574e68819786c0e2b842a7756a9c1771f020fe54f2ba95d8f807bf64fd5d919`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Oct 2021 01:34:07 GMT
ADD file:eb5955ccd54a486767e85aeb1c03ffc6d8667b5476d0cf17b892ca407f1c8853 in / 
# Tue, 12 Oct 2021 01:34:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:48:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 Oct 2021 01:54:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 14 Oct 2021 01:54:02 GMT
ENV INFLUXDB_VERSION=1.7.11
# Thu, 14 Oct 2021 01:54:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 14 Oct 2021 01:54:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 14 Oct 2021 01:54:18 GMT
EXPOSE 8086
# Thu, 14 Oct 2021 01:54:18 GMT
VOLUME [/var/lib/influxdb]
# Thu, 14 Oct 2021 01:54:19 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 14 Oct 2021 01:54:19 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 14 Oct 2021 01:54:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 Oct 2021 01:54:20 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8e9db3616ec4491d75e6c28254ff2376f24900797e7c4cc464f36a0c502b111f`  
		Last Modified: Tue, 12 Oct 2021 01:51:20 GMT  
		Size: 42.1 MB (42119423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdf02e61fe0ab1563ba0431b63fade0e2dc7930d82d8c1a7ec6ee395072fdb3`  
		Last Modified: Tue, 12 Oct 2021 19:06:50 GMT  
		Size: 10.0 MB (9955968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a752ebf54d1b82943abce28e108346c5d28e94fdb8f419cfffea0b639341ce6`  
		Last Modified: Tue, 12 Oct 2021 19:06:46 GMT  
		Size: 3.9 MB (3921159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4731e07c15270f8d8ed739a4fc8c851d1f91985b1576d76f75e70b7763abdac9`  
		Last Modified: Thu, 14 Oct 2021 01:55:20 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bde838c92828dae84b5c20231973b3112a9e727d23f825ece87917c576fe6a8`  
		Last Modified: Thu, 14 Oct 2021 01:55:49 GMT  
		Size: 57.5 MB (57468948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebcff4a5dff8fce7e94d185dbb105e71561cfc37771429467e5dde722dfa510`  
		Last Modified: Thu, 14 Oct 2021 01:55:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4605b82330330bca3e7e136c3e4810d8f7cc6b8cdded66fdb1381c78c2835f35`  
		Last Modified: Thu, 14 Oct 2021 01:55:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19db3289b711eae836e9e528c5b35e7b73fc2f6640c7540b443e0cc6cab4cb9e`  
		Last Modified: Thu, 14 Oct 2021 01:55:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ed1764b34890c69f04a97222448184c0b2b0f36b906c17a66cce146b91e15ef2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114474156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e787a03959ed9bef472a7dedb598eb2ecee9b847035f083b2eb6db6506acfdf0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:38:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 17 Nov 2021 21:38:25 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 17 Nov 2021 21:38:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 17 Nov 2021 21:38:33 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 17 Nov 2021 21:38:33 GMT
EXPOSE 8086
# Wed, 17 Nov 2021 21:38:34 GMT
VOLUME [/var/lib/influxdb]
# Wed, 17 Nov 2021 21:38:36 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 17 Nov 2021 21:38:37 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 17 Nov 2021 21:38:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:38:38 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4456190c44d660cfa31233877be2b4ea47d82d18f269b8ebe72a965fcc7afc07`  
		Last Modified: Wed, 17 Nov 2021 21:40:59 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ea6427b0191a48951ff568d965bbc320b0f92ca8c138aa92b5bbcb542d995d`  
		Last Modified: Wed, 17 Nov 2021 21:41:07 GMT  
		Size: 57.2 MB (57204456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcca94f2817861fc87bd021272c35e45423cc0a287de1a5ae7585e603bea7e09`  
		Last Modified: Wed, 17 Nov 2021 21:40:59 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2ba35f3daf2a03d815518da6472f4476f4bba7962ccec7527a1cb85aeca71f`  
		Last Modified: Wed, 17 Nov 2021 21:40:59 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d228f9a077123ab993e9400ba3dbf6371078b767ff83c58c7ec17b23f53d086`  
		Last Modified: Wed, 17 Nov 2021 21:41:00 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-alpine`

```console
$ docker pull influxdb@sha256:e317cda9b1e08d21da87b8d5afdd74eba95fec8d1f135f58762d81ca45556ad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:effbf6236fb520350d780b5ee9112ee9fe9f87c5ff0474ad673a89f68175ec0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65345841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb60e4036838f81174a2d72f91b72ff211c227745c91dccafe33422068b644b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:28:06 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 13 Nov 2021 02:28:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:28:25 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 13 Nov 2021 02:28:25 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:28:25 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:28:25 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:28:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 13 Nov 2021 02:28:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:28:26 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfffaf8f454f59287b0327da99c9906cbacb21a87e393b24b97b67c80dc30ce`  
		Last Modified: Sat, 13 Nov 2021 02:33:12 GMT  
		Size: 61.0 MB (61034776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cb60baf3d3ad74477921edb24992877ed08995b91015c3d4fd93bc56b56a0c`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3197b954addeba2412b4c3005fd50c004005408d68e7cebf16191e23c0687850`  
		Last Modified: Sat, 13 Nov 2021 02:33:00 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50134c777014240923f56c3467039ad675b8685292a0e6a86fe42b3cbee26f07`  
		Last Modified: Sat, 13 Nov 2021 02:33:00 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data`

```console
$ docker pull influxdb@sha256:78ae885269b03fed5ad95a1c73824e2b7a370075f129dc6a9714a3fe18fd2abc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:08a6b84584fa14e2d248f12e31657edc49f07b6eb7f060fc51e612b89090ea4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148977822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb1e79f68ae4d35ea78f775b466cb8afaf462373b02eeefb2151476e30291c5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:43:44 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Thu, 18 Nov 2021 09:43:55 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:43:55 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 18 Nov 2021 09:43:56 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:43:56 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:43:56 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:43:56 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 18 Nov 2021 09:43:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:43:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850601fa924d33b07660c65ad9cc1d03b19ddf4b4560ecd3d88e922b4d2ac0c8`  
		Last Modified: Thu, 18 Nov 2021 09:48:10 GMT  
		Size: 87.9 MB (87948976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3676a11b217fd8958ec970daa2d667d00202c4d3a25652828c8555796eca6ff3`  
		Last Modified: Thu, 18 Nov 2021 09:47:55 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f66f90821b371e1b58d6b8eaa3af62c7ad0487997a2a9839e187d7abbd1564`  
		Last Modified: Thu, 18 Nov 2021 09:47:55 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c302b84094bb9be9252a9f5d268aad7f17b0aa869dda2c4faa703a70da19a816`  
		Last Modified: Thu, 18 Nov 2021 09:47:55 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data-alpine`

```console
$ docker pull influxdb@sha256:1b4fd66fab0b26a8df4e8ca0abc56247f1abaa6adcba4bd135b8678d2f0e86b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:3c00c93c9cf37da3e441a3745247d1a68476fb9ff4803611b1005ed8ec46db48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (91952685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c710a81bc9b80e81201349203ff478724791b8e4ad002e7e29d0cf7a7ee414b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:28:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 13 Nov 2021 02:28:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:28:45 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 13 Nov 2021 02:28:45 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:28:45 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:28:46 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:28:46 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 13 Nov 2021 02:28:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:28:46 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29af3629856a93dc620b39ed981fe9e7af8ba6796a05294a39b784b91965296`  
		Last Modified: Sat, 13 Nov 2021 02:33:40 GMT  
		Size: 87.6 MB (87641566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfda715994a13370b43264dec79ac083d497a0c41e78821572b5faa9f3d4b1ee`  
		Last Modified: Sat, 13 Nov 2021 02:33:24 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef59d77919202e7124e5f6265ab984593090101a3549b322db9791f49235ded`  
		Last Modified: Sat, 13 Nov 2021 02:33:25 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ee66cbb45cc950855eb41647456e1e310e64dd3e7eb81e29de63d85ff57c20`  
		Last Modified: Sat, 13 Nov 2021 02:33:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta`

```console
$ docker pull influxdb@sha256:b6b1d486137445175dfad459a88c4787091bc1020168f8ac70de78a571f09d5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ef5f5ac5677f26f239da87d5af0e9e8d237685ad10fc702791fe20091b2a658b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84161182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6077c3ceed2549ed3c2df31ac64d7e0cc3e5206c088b37e7e3ee110f351e2772`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:43:44 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Thu, 18 Nov 2021 09:44:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:44:12 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 18 Nov 2021 09:44:12 GMT
EXPOSE 8091
# Thu, 18 Nov 2021 09:44:13 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:44:13 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:44:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:44:14 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d656debd17ce00900d5165d9a33a3d077eaa58479ff9d2093fef95acc6a1104`  
		Last Modified: Thu, 18 Nov 2021 09:48:26 GMT  
		Size: 23.1 MB (23133539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8582efba42a4e711c853171a877f51d7f9da1a650cdf0046a848f62921aec68c`  
		Last Modified: Thu, 18 Nov 2021 09:48:22 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca8c9cc080cc7f5721ef9173b4fd6a483b49f4851eb9b7ae1113e0142bba216`  
		Last Modified: Thu, 18 Nov 2021 09:48:22 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta-alpine`

```console
$ docker pull influxdb@sha256:f904989c983a04e891fab168c587e0a0f926aae9f0a1c4b8bf8630a492525e19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:2efe5f09c3b1c0f3b41149361feebc9cabf8c060c9674e0b3f994121536521d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27313616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61b61c4702d1d2eb470885bb87ad48bc33c61193abf8064d5a88847891a27143`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:28:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 13 Nov 2021 02:29:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:29:00 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 13 Nov 2021 02:29:00 GMT
EXPOSE 8091
# Sat, 13 Nov 2021 02:29:00 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:29:01 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:29:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:29:01 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699dd83fea323c67dfe7c1d26c95c96b19adbdf0c16bc3b78ae67088a40132c0`  
		Last Modified: Sat, 13 Nov 2021 02:33:56 GMT  
		Size: 23.0 MB (23003697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3f8a6a9d4901e889b052b314d7ea86fb7b53a6791e63981bdc913c1c45506f`  
		Last Modified: Sat, 13 Nov 2021 02:33:52 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500b05540667dbf4a178b293bbbc7b47a914e6977e79098eb1d28286ec76bce8`  
		Last Modified: Sat, 13 Nov 2021 02:33:52 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11`

```console
$ docker pull influxdb@sha256:2f31929cd48d6f39d12a31ee3ae99ebb27cee74c472b5b0b299c1776f31440c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7.11` - linux; amd64

```console
$ docker pull influxdb@sha256:86f1cfcdbeb83d429e0500a28fcff348b2e4740960ba78f1d321790cb6d1e3b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122313880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f011f70cae60f0d335def46540efe2ff6d1e1330c3933cbbb9b2f85680dc2fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:43:30 GMT
ENV INFLUXDB_VERSION=1.7.11
# Thu, 18 Nov 2021 09:43:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 18 Nov 2021 09:43:39 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 18 Nov 2021 09:43:39 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:43:39 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:43:39 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:43:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 18 Nov 2021 09:43:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:43:40 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417dfa61d29cf6fef46e761c963ada353795d6c57bce1bf6d340e6a70f97a5fe`  
		Last Modified: Thu, 18 Nov 2021 09:47:44 GMT  
		Size: 61.3 MB (61285092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa30700867447cc2e95857c55e4f25527e67fd1a63c61b99ac68b29bf7c5ebaa`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed35aa167fe9bb6251995b7928b2d8f36d38565495c2669ad9a219c98de651de`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af723c50ac3e9275d6d9b32a7013ba297de967db5033d08ef3159db34bd1a783`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:64940016027dcbc31b63c7e65ff23bacb6622daefa8c8fd7bb5b4099069a429e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113470068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e574e68819786c0e2b842a7756a9c1771f020fe54f2ba95d8f807bf64fd5d919`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Oct 2021 01:34:07 GMT
ADD file:eb5955ccd54a486767e85aeb1c03ffc6d8667b5476d0cf17b892ca407f1c8853 in / 
# Tue, 12 Oct 2021 01:34:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:48:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 Oct 2021 01:54:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 14 Oct 2021 01:54:02 GMT
ENV INFLUXDB_VERSION=1.7.11
# Thu, 14 Oct 2021 01:54:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 14 Oct 2021 01:54:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 14 Oct 2021 01:54:18 GMT
EXPOSE 8086
# Thu, 14 Oct 2021 01:54:18 GMT
VOLUME [/var/lib/influxdb]
# Thu, 14 Oct 2021 01:54:19 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 14 Oct 2021 01:54:19 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 14 Oct 2021 01:54:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 Oct 2021 01:54:20 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8e9db3616ec4491d75e6c28254ff2376f24900797e7c4cc464f36a0c502b111f`  
		Last Modified: Tue, 12 Oct 2021 01:51:20 GMT  
		Size: 42.1 MB (42119423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdf02e61fe0ab1563ba0431b63fade0e2dc7930d82d8c1a7ec6ee395072fdb3`  
		Last Modified: Tue, 12 Oct 2021 19:06:50 GMT  
		Size: 10.0 MB (9955968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a752ebf54d1b82943abce28e108346c5d28e94fdb8f419cfffea0b639341ce6`  
		Last Modified: Tue, 12 Oct 2021 19:06:46 GMT  
		Size: 3.9 MB (3921159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4731e07c15270f8d8ed739a4fc8c851d1f91985b1576d76f75e70b7763abdac9`  
		Last Modified: Thu, 14 Oct 2021 01:55:20 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bde838c92828dae84b5c20231973b3112a9e727d23f825ece87917c576fe6a8`  
		Last Modified: Thu, 14 Oct 2021 01:55:49 GMT  
		Size: 57.5 MB (57468948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebcff4a5dff8fce7e94d185dbb105e71561cfc37771429467e5dde722dfa510`  
		Last Modified: Thu, 14 Oct 2021 01:55:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4605b82330330bca3e7e136c3e4810d8f7cc6b8cdded66fdb1381c78c2835f35`  
		Last Modified: Thu, 14 Oct 2021 01:55:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19db3289b711eae836e9e528c5b35e7b73fc2f6640c7540b443e0cc6cab4cb9e`  
		Last Modified: Thu, 14 Oct 2021 01:55:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ed1764b34890c69f04a97222448184c0b2b0f36b906c17a66cce146b91e15ef2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114474156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e787a03959ed9bef472a7dedb598eb2ecee9b847035f083b2eb6db6506acfdf0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:38:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 17 Nov 2021 21:38:25 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 17 Nov 2021 21:38:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 17 Nov 2021 21:38:33 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 17 Nov 2021 21:38:33 GMT
EXPOSE 8086
# Wed, 17 Nov 2021 21:38:34 GMT
VOLUME [/var/lib/influxdb]
# Wed, 17 Nov 2021 21:38:36 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 17 Nov 2021 21:38:37 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 17 Nov 2021 21:38:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:38:38 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4456190c44d660cfa31233877be2b4ea47d82d18f269b8ebe72a965fcc7afc07`  
		Last Modified: Wed, 17 Nov 2021 21:40:59 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ea6427b0191a48951ff568d965bbc320b0f92ca8c138aa92b5bbcb542d995d`  
		Last Modified: Wed, 17 Nov 2021 21:41:07 GMT  
		Size: 57.2 MB (57204456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcca94f2817861fc87bd021272c35e45423cc0a287de1a5ae7585e603bea7e09`  
		Last Modified: Wed, 17 Nov 2021 21:40:59 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2ba35f3daf2a03d815518da6472f4476f4bba7962ccec7527a1cb85aeca71f`  
		Last Modified: Wed, 17 Nov 2021 21:40:59 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d228f9a077123ab993e9400ba3dbf6371078b767ff83c58c7ec17b23f53d086`  
		Last Modified: Wed, 17 Nov 2021 21:41:00 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-alpine`

```console
$ docker pull influxdb@sha256:e317cda9b1e08d21da87b8d5afdd74eba95fec8d1f135f58762d81ca45556ad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:effbf6236fb520350d780b5ee9112ee9fe9f87c5ff0474ad673a89f68175ec0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65345841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb60e4036838f81174a2d72f91b72ff211c227745c91dccafe33422068b644b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:28:06 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 13 Nov 2021 02:28:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:28:25 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 13 Nov 2021 02:28:25 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:28:25 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:28:25 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:28:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 13 Nov 2021 02:28:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:28:26 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfffaf8f454f59287b0327da99c9906cbacb21a87e393b24b97b67c80dc30ce`  
		Last Modified: Sat, 13 Nov 2021 02:33:12 GMT  
		Size: 61.0 MB (61034776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cb60baf3d3ad74477921edb24992877ed08995b91015c3d4fd93bc56b56a0c`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3197b954addeba2412b4c3005fd50c004005408d68e7cebf16191e23c0687850`  
		Last Modified: Sat, 13 Nov 2021 02:33:00 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50134c777014240923f56c3467039ad675b8685292a0e6a86fe42b3cbee26f07`  
		Last Modified: Sat, 13 Nov 2021 02:33:00 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data`

```console
$ docker pull influxdb@sha256:78ae885269b03fed5ad95a1c73824e2b7a370075f129dc6a9714a3fe18fd2abc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:08a6b84584fa14e2d248f12e31657edc49f07b6eb7f060fc51e612b89090ea4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148977822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb1e79f68ae4d35ea78f775b466cb8afaf462373b02eeefb2151476e30291c5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:43:44 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Thu, 18 Nov 2021 09:43:55 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:43:55 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 18 Nov 2021 09:43:56 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:43:56 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:43:56 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:43:56 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 18 Nov 2021 09:43:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:43:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850601fa924d33b07660c65ad9cc1d03b19ddf4b4560ecd3d88e922b4d2ac0c8`  
		Last Modified: Thu, 18 Nov 2021 09:48:10 GMT  
		Size: 87.9 MB (87948976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3676a11b217fd8958ec970daa2d667d00202c4d3a25652828c8555796eca6ff3`  
		Last Modified: Thu, 18 Nov 2021 09:47:55 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f66f90821b371e1b58d6b8eaa3af62c7ad0487997a2a9839e187d7abbd1564`  
		Last Modified: Thu, 18 Nov 2021 09:47:55 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c302b84094bb9be9252a9f5d268aad7f17b0aa869dda2c4faa703a70da19a816`  
		Last Modified: Thu, 18 Nov 2021 09:47:55 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data-alpine`

```console
$ docker pull influxdb@sha256:1b4fd66fab0b26a8df4e8ca0abc56247f1abaa6adcba4bd135b8678d2f0e86b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:3c00c93c9cf37da3e441a3745247d1a68476fb9ff4803611b1005ed8ec46db48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (91952685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c710a81bc9b80e81201349203ff478724791b8e4ad002e7e29d0cf7a7ee414b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:28:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 13 Nov 2021 02:28:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:28:45 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 13 Nov 2021 02:28:45 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:28:45 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:28:46 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:28:46 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 13 Nov 2021 02:28:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:28:46 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29af3629856a93dc620b39ed981fe9e7af8ba6796a05294a39b784b91965296`  
		Last Modified: Sat, 13 Nov 2021 02:33:40 GMT  
		Size: 87.6 MB (87641566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfda715994a13370b43264dec79ac083d497a0c41e78821572b5faa9f3d4b1ee`  
		Last Modified: Sat, 13 Nov 2021 02:33:24 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef59d77919202e7124e5f6265ab984593090101a3549b322db9791f49235ded`  
		Last Modified: Sat, 13 Nov 2021 02:33:25 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ee66cbb45cc950855eb41647456e1e310e64dd3e7eb81e29de63d85ff57c20`  
		Last Modified: Sat, 13 Nov 2021 02:33:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta`

```console
$ docker pull influxdb@sha256:b6b1d486137445175dfad459a88c4787091bc1020168f8ac70de78a571f09d5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ef5f5ac5677f26f239da87d5af0e9e8d237685ad10fc702791fe20091b2a658b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84161182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6077c3ceed2549ed3c2df31ac64d7e0cc3e5206c088b37e7e3ee110f351e2772`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:43:44 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Thu, 18 Nov 2021 09:44:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:44:12 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 18 Nov 2021 09:44:12 GMT
EXPOSE 8091
# Thu, 18 Nov 2021 09:44:13 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:44:13 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:44:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:44:14 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d656debd17ce00900d5165d9a33a3d077eaa58479ff9d2093fef95acc6a1104`  
		Last Modified: Thu, 18 Nov 2021 09:48:26 GMT  
		Size: 23.1 MB (23133539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8582efba42a4e711c853171a877f51d7f9da1a650cdf0046a848f62921aec68c`  
		Last Modified: Thu, 18 Nov 2021 09:48:22 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca8c9cc080cc7f5721ef9173b4fd6a483b49f4851eb9b7ae1113e0142bba216`  
		Last Modified: Thu, 18 Nov 2021 09:48:22 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta-alpine`

```console
$ docker pull influxdb@sha256:f904989c983a04e891fab168c587e0a0f926aae9f0a1c4b8bf8630a492525e19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:2efe5f09c3b1c0f3b41149361feebc9cabf8c060c9674e0b3f994121536521d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27313616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61b61c4702d1d2eb470885bb87ad48bc33c61193abf8064d5a88847891a27143`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:28:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 13 Nov 2021 02:29:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:29:00 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 13 Nov 2021 02:29:00 GMT
EXPOSE 8091
# Sat, 13 Nov 2021 02:29:00 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:29:01 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:29:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:29:01 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699dd83fea323c67dfe7c1d26c95c96b19adbdf0c16bc3b78ae67088a40132c0`  
		Last Modified: Sat, 13 Nov 2021 02:33:56 GMT  
		Size: 23.0 MB (23003697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3f8a6a9d4901e889b052b314d7ea86fb7b53a6791e63981bdc913c1c45506f`  
		Last Modified: Sat, 13 Nov 2021 02:33:52 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500b05540667dbf4a178b293bbbc7b47a914e6977e79098eb1d28286ec76bce8`  
		Last Modified: Sat, 13 Nov 2021 02:33:52 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:45b597c60fe7b9591b8266981f0397096897e1b6e6c5df0054d25ad4172346e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:3c2f68b28b0bade3f8cb048e7f5c44bba75254c75b40b240dd1fc6c015096d5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115918268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5033d7324bc70cc2a7d53b89eabf4c1486494132b0cf20e767d0484458c17987`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:44:21 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 18 Nov 2021 09:44:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 18 Nov 2021 09:44:31 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 18 Nov 2021 09:44:31 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:44:31 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:44:32 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:44:32 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 18 Nov 2021 09:44:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:44:33 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2446380873b15b2b83b2745d97c665f0c1bdd04a1ba3a5c81ab427304166d561`  
		Last Modified: Thu, 18 Nov 2021 09:48:47 GMT  
		Size: 54.9 MB (54889479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf66fbadca0e946c863eda48e9dd4d0798cca99c361d6d1d211aa21fdfdcdd5`  
		Last Modified: Thu, 18 Nov 2021 09:48:37 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e86150139f8e5fb4afc5993fceb183d70299bd4917b6e4330ecdf7bd227c8f4`  
		Last Modified: Thu, 18 Nov 2021 09:48:37 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced933f74640d2d5b04eb06536cd6b4aeff061b7890693d6cd169b2ac53f2d9`  
		Last Modified: Thu, 18 Nov 2021 09:48:38 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:ddd8595eeb547ba17f170d763f0ede7864e22f0dd6c49238e5fb8c5481d675fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107617952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af897d893e658952166e15972e349734cc599650bd831546d3ef5f4241cb574`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Oct 2021 01:34:07 GMT
ADD file:eb5955ccd54a486767e85aeb1c03ffc6d8667b5476d0cf17b892ca407f1c8853 in / 
# Tue, 12 Oct 2021 01:34:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:48:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 Oct 2021 01:54:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 14 Oct 2021 01:54:32 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 14 Oct 2021 01:54:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 14 Oct 2021 01:54:46 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 14 Oct 2021 01:54:46 GMT
EXPOSE 8086
# Thu, 14 Oct 2021 01:54:46 GMT
VOLUME [/var/lib/influxdb]
# Thu, 14 Oct 2021 01:54:47 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 14 Oct 2021 01:54:48 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 14 Oct 2021 01:54:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 Oct 2021 01:54:48 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8e9db3616ec4491d75e6c28254ff2376f24900797e7c4cc464f36a0c502b111f`  
		Last Modified: Tue, 12 Oct 2021 01:51:20 GMT  
		Size: 42.1 MB (42119423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdf02e61fe0ab1563ba0431b63fade0e2dc7930d82d8c1a7ec6ee395072fdb3`  
		Last Modified: Tue, 12 Oct 2021 19:06:50 GMT  
		Size: 10.0 MB (9955968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a752ebf54d1b82943abce28e108346c5d28e94fdb8f419cfffea0b639341ce6`  
		Last Modified: Tue, 12 Oct 2021 19:06:46 GMT  
		Size: 3.9 MB (3921159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4731e07c15270f8d8ed739a4fc8c851d1f91985b1576d76f75e70b7763abdac9`  
		Last Modified: Thu, 14 Oct 2021 01:55:20 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1438e9866f20b05abbfb253c3cc59e1e13249b4773168c88ce6116b01d2b5ad`  
		Last Modified: Thu, 14 Oct 2021 01:56:29 GMT  
		Size: 51.6 MB (51616832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf39696ce8915323772d48a8d126b6903ab844a4e37c5706ed0f2ee707beee7`  
		Last Modified: Thu, 14 Oct 2021 01:56:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f539a50ce536eb1ea54014c31d4ec687d718389aa5581bd0b3af3d747516865`  
		Last Modified: Thu, 14 Oct 2021 01:56:01 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b023617978d13cb35b872cc29b3d7794f68a18f94d3caf41ab44dd5a919e497`  
		Last Modified: Thu, 14 Oct 2021 01:56:01 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b0b8108307446b29afdeac1b6ee9a755f7d13acf8cb8186a31c05cd71a2e1dc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108503378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5861559aedf0a49c59a3878827808bf3f758dc61c3b13d756bba9034893d893`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:38:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 17 Nov 2021 21:38:43 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 17 Nov 2021 21:38:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 17 Nov 2021 21:38:51 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 17 Nov 2021 21:38:51 GMT
EXPOSE 8086
# Wed, 17 Nov 2021 21:38:52 GMT
VOLUME [/var/lib/influxdb]
# Wed, 17 Nov 2021 21:38:54 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 17 Nov 2021 21:38:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 17 Nov 2021 21:38:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:38:56 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4456190c44d660cfa31233877be2b4ea47d82d18f269b8ebe72a965fcc7afc07`  
		Last Modified: Wed, 17 Nov 2021 21:40:59 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b345e5a874d846cf91fcbe307c58b82ab6ab62160f892820901f1ea8f8a92b`  
		Last Modified: Wed, 17 Nov 2021 21:41:32 GMT  
		Size: 51.2 MB (51233679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5697c2dd8f6c5955def0d924b5dd7ae8291fe5492e975dfe77b1ba5e1687deb`  
		Last Modified: Wed, 17 Nov 2021 21:41:25 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76182d3cf5c43f0df884323055c5f32e87915bd614211fb16a67faa482446cfa`  
		Last Modified: Wed, 17 Nov 2021 21:41:25 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7bde5de9347757cacd5e0c209c0bfb54fc174ee3124702f41ea482c4506e07`  
		Last Modified: Wed, 17 Nov 2021 21:41:25 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:4516e1ecf804f7272f3edf5bb5b924d3d3f746fb6c90613bc1857bb18f734a61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:77fdae83f757dd6ecc99759e462bef9320a6802324214e7464556ae7b8aaebdd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58971021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625d9d53793fbc06ef709cbb3654518139c959ba2fc02625062abe4289bd6471`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:29:06 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sat, 13 Nov 2021 02:29:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:29:19 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 13 Nov 2021 02:29:19 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:29:20 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:29:20 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:29:20 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 13 Nov 2021 02:29:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:29:21 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e69ac12e16dde6e93c022174a44efe4a5c3d3a497fd700b84bbbdf585621dc`  
		Last Modified: Sat, 13 Nov 2021 02:34:17 GMT  
		Size: 54.7 MB (54659958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559b358e805eb9db9724dac339e8ff41eb8f1b48efd5b7c3a275cb4be8b52ca`  
		Last Modified: Sat, 13 Nov 2021 02:34:08 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8597986d65b426ea904e2f32db5d04d15521ca679606c618d853e68ad1dbf1b`  
		Last Modified: Sat, 13 Nov 2021 02:34:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4e81cd3437ffc2903a84e9b3af9754282e039da023ee1f3334754311d813c3`  
		Last Modified: Sat, 13 Nov 2021 02:34:07 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:00cdba39140b5f3fe364dc6260d27bd61310bd1383c0639f6297f693c5c0ec11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:ec210def90412bcfd6586f056bf15cfba9a6ae2d83f329f3095914d7202fbada
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117737381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244874bc2bf861b02626382c1d1bd042fd26991a17b503bef6e57853764f3cf1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:44:42 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 18 Nov 2021 09:44:52 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:44:53 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 18 Nov 2021 09:44:53 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:44:53 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:44:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:44:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 18 Nov 2021 09:44:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:44:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08525dea5b6b885656a753a6deef7a71e230e77dafc7f831bd2a4c9f21df5da5`  
		Last Modified: Thu, 18 Nov 2021 09:49:07 GMT  
		Size: 56.7 MB (56708533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57d90367afa71b328b7c1e192c38ec3bc28ec42bfab9b9f002cd21e6f4b455e`  
		Last Modified: Thu, 18 Nov 2021 09:48:58 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e37b0832a2c9fc55d7d0e4b680f6da9e95a0aad7fe83ea36bdb03fb68b0aab`  
		Last Modified: Thu, 18 Nov 2021 09:48:58 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf287206df98f216591a3ae20f6a591c9970835eab55160656bb711f72094f5c`  
		Last Modified: Thu, 18 Nov 2021 09:48:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:9edb5e97912c1a30144b9674f7d24f957a6ee186dad14461da00075d7b3796cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f6c46290f9cfbd9b2fbe6e9f47ab18fe7314c5bd6758ed3c7fde006478ba2a47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60814908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9083f2c434fe802e0c24ff0518282b9c8956c0cb1156626ed29c0cacff0fd794`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:29:25 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 13 Nov 2021 02:29:38 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:29:39 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 13 Nov 2021 02:29:39 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:29:39 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:29:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:29:39 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 13 Nov 2021 02:29:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:29:40 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b1c62ddbddb14ed511aedfa47a61da93b52f2ebc434d573e6cccdeab360012`  
		Last Modified: Sat, 13 Nov 2021 02:34:40 GMT  
		Size: 56.5 MB (56503786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182dd80d9b0c7757cdea730b9d8438eddf10b2837f1bc4f9555e24a2e16c9f1f`  
		Last Modified: Sat, 13 Nov 2021 02:34:30 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad150614e74207f44ffbcda2bdd6d075d072e5d7e40c18aea4d02bf92012d3`  
		Last Modified: Sat, 13 Nov 2021 02:34:31 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebec01cb49874553e60a3087e07f6ea3be09a5253235bbc016d200b165f0740`  
		Last Modified: Sat, 13 Nov 2021 02:34:30 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:31500f40ed7a50fdb52e8a0990aea86bd8c0f50814d644754a9f57c35fca7ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:64534669863b8e1414ac4aa65a41d124604e61f8b9ce42b31e297cb2a8d15987
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84443975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6befdf4bac0b404e5ad4274eafa07f36729725f56bef2f3ae11f41259f0cc59d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:44:42 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 18 Nov 2021 09:45:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:45:05 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 18 Nov 2021 09:45:05 GMT
EXPOSE 8091
# Thu, 18 Nov 2021 09:45:05 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:45:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:45:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:45:06 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64521abd18cf018ab9316be9ab482c503cb3c6b8adeb380319d51c18556be12e`  
		Last Modified: Thu, 18 Nov 2021 09:49:24 GMT  
		Size: 23.4 MB (23416332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82be31c0c04837996a2f891230ea306a73ed63264076a52cff01efbae7234c49`  
		Last Modified: Thu, 18 Nov 2021 09:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6ebc4c9a6547fd06dd99b1c765524dfdd7a939834caad7a1fac1b01c95d3bd`  
		Last Modified: Thu, 18 Nov 2021 09:49:20 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:4cba27899d3f6324276746cc3d13e113171e58f0cd57b6f778f223d9e5fe1173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:fe5ecca89fb203a0a446abc95062c96221545125968f4f313c50cd821f5a4e7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27602958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:072b66b0c223ce772c78f84a6586e8080a5fb145cf5f1d00eefd6f23846e45cc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:29:25 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 13 Nov 2021 02:29:53 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:29:53 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 13 Nov 2021 02:29:54 GMT
EXPOSE 8091
# Sat, 13 Nov 2021 02:29:54 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:29:54 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:29:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:29:55 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7f836dc8033be4020b77d60ac1d010d51d58ce819fd31c8c903dd7bf1d9bed`  
		Last Modified: Sat, 13 Nov 2021 02:35:00 GMT  
		Size: 23.3 MB (23293039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352cd5d07590068a89a6415f0d3923109129dddfdae2762d95cf37b800faed14`  
		Last Modified: Sat, 13 Nov 2021 02:34:56 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a164a9ffc5db6c4dbad8265ed41221745f6094e8223216f516ecfb034794045`  
		Last Modified: Sat, 13 Nov 2021 02:34:56 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10`

```console
$ docker pull influxdb@sha256:45b597c60fe7b9591b8266981f0397096897e1b6e6c5df0054d25ad4172346e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:3c2f68b28b0bade3f8cb048e7f5c44bba75254c75b40b240dd1fc6c015096d5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115918268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5033d7324bc70cc2a7d53b89eabf4c1486494132b0cf20e767d0484458c17987`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:44:21 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 18 Nov 2021 09:44:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 18 Nov 2021 09:44:31 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 18 Nov 2021 09:44:31 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:44:31 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:44:32 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:44:32 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 18 Nov 2021 09:44:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:44:33 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2446380873b15b2b83b2745d97c665f0c1bdd04a1ba3a5c81ab427304166d561`  
		Last Modified: Thu, 18 Nov 2021 09:48:47 GMT  
		Size: 54.9 MB (54889479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf66fbadca0e946c863eda48e9dd4d0798cca99c361d6d1d211aa21fdfdcdd5`  
		Last Modified: Thu, 18 Nov 2021 09:48:37 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e86150139f8e5fb4afc5993fceb183d70299bd4917b6e4330ecdf7bd227c8f4`  
		Last Modified: Thu, 18 Nov 2021 09:48:37 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced933f74640d2d5b04eb06536cd6b4aeff061b7890693d6cd169b2ac53f2d9`  
		Last Modified: Thu, 18 Nov 2021 09:48:38 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:ddd8595eeb547ba17f170d763f0ede7864e22f0dd6c49238e5fb8c5481d675fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107617952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af897d893e658952166e15972e349734cc599650bd831546d3ef5f4241cb574`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Oct 2021 01:34:07 GMT
ADD file:eb5955ccd54a486767e85aeb1c03ffc6d8667b5476d0cf17b892ca407f1c8853 in / 
# Tue, 12 Oct 2021 01:34:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:48:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 Oct 2021 01:54:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 14 Oct 2021 01:54:32 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 14 Oct 2021 01:54:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 14 Oct 2021 01:54:46 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 14 Oct 2021 01:54:46 GMT
EXPOSE 8086
# Thu, 14 Oct 2021 01:54:46 GMT
VOLUME [/var/lib/influxdb]
# Thu, 14 Oct 2021 01:54:47 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 14 Oct 2021 01:54:48 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 14 Oct 2021 01:54:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 Oct 2021 01:54:48 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8e9db3616ec4491d75e6c28254ff2376f24900797e7c4cc464f36a0c502b111f`  
		Last Modified: Tue, 12 Oct 2021 01:51:20 GMT  
		Size: 42.1 MB (42119423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdf02e61fe0ab1563ba0431b63fade0e2dc7930d82d8c1a7ec6ee395072fdb3`  
		Last Modified: Tue, 12 Oct 2021 19:06:50 GMT  
		Size: 10.0 MB (9955968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a752ebf54d1b82943abce28e108346c5d28e94fdb8f419cfffea0b639341ce6`  
		Last Modified: Tue, 12 Oct 2021 19:06:46 GMT  
		Size: 3.9 MB (3921159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4731e07c15270f8d8ed739a4fc8c851d1f91985b1576d76f75e70b7763abdac9`  
		Last Modified: Thu, 14 Oct 2021 01:55:20 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1438e9866f20b05abbfb253c3cc59e1e13249b4773168c88ce6116b01d2b5ad`  
		Last Modified: Thu, 14 Oct 2021 01:56:29 GMT  
		Size: 51.6 MB (51616832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf39696ce8915323772d48a8d126b6903ab844a4e37c5706ed0f2ee707beee7`  
		Last Modified: Thu, 14 Oct 2021 01:56:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f539a50ce536eb1ea54014c31d4ec687d718389aa5581bd0b3af3d747516865`  
		Last Modified: Thu, 14 Oct 2021 01:56:01 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b023617978d13cb35b872cc29b3d7794f68a18f94d3caf41ab44dd5a919e497`  
		Last Modified: Thu, 14 Oct 2021 01:56:01 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b0b8108307446b29afdeac1b6ee9a755f7d13acf8cb8186a31c05cd71a2e1dc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108503378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5861559aedf0a49c59a3878827808bf3f758dc61c3b13d756bba9034893d893`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:38:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 17 Nov 2021 21:38:43 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 17 Nov 2021 21:38:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 17 Nov 2021 21:38:51 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 17 Nov 2021 21:38:51 GMT
EXPOSE 8086
# Wed, 17 Nov 2021 21:38:52 GMT
VOLUME [/var/lib/influxdb]
# Wed, 17 Nov 2021 21:38:54 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 17 Nov 2021 21:38:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 17 Nov 2021 21:38:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:38:56 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4456190c44d660cfa31233877be2b4ea47d82d18f269b8ebe72a965fcc7afc07`  
		Last Modified: Wed, 17 Nov 2021 21:40:59 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b345e5a874d846cf91fcbe307c58b82ab6ab62160f892820901f1ea8f8a92b`  
		Last Modified: Wed, 17 Nov 2021 21:41:32 GMT  
		Size: 51.2 MB (51233679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5697c2dd8f6c5955def0d924b5dd7ae8291fe5492e975dfe77b1ba5e1687deb`  
		Last Modified: Wed, 17 Nov 2021 21:41:25 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76182d3cf5c43f0df884323055c5f32e87915bd614211fb16a67faa482446cfa`  
		Last Modified: Wed, 17 Nov 2021 21:41:25 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7bde5de9347757cacd5e0c209c0bfb54fc174ee3124702f41ea482c4506e07`  
		Last Modified: Wed, 17 Nov 2021 21:41:25 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-alpine`

```console
$ docker pull influxdb@sha256:4516e1ecf804f7272f3edf5bb5b924d3d3f746fb6c90613bc1857bb18f734a61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:77fdae83f757dd6ecc99759e462bef9320a6802324214e7464556ae7b8aaebdd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58971021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625d9d53793fbc06ef709cbb3654518139c959ba2fc02625062abe4289bd6471`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:29:06 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sat, 13 Nov 2021 02:29:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:29:19 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 13 Nov 2021 02:29:19 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:29:20 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:29:20 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:29:20 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 13 Nov 2021 02:29:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:29:21 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e69ac12e16dde6e93c022174a44efe4a5c3d3a497fd700b84bbbdf585621dc`  
		Last Modified: Sat, 13 Nov 2021 02:34:17 GMT  
		Size: 54.7 MB (54659958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559b358e805eb9db9724dac339e8ff41eb8f1b48efd5b7c3a275cb4be8b52ca`  
		Last Modified: Sat, 13 Nov 2021 02:34:08 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8597986d65b426ea904e2f32db5d04d15521ca679606c618d853e68ad1dbf1b`  
		Last Modified: Sat, 13 Nov 2021 02:34:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4e81cd3437ffc2903a84e9b3af9754282e039da023ee1f3334754311d813c3`  
		Last Modified: Sat, 13 Nov 2021 02:34:07 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data`

```console
$ docker pull influxdb@sha256:00cdba39140b5f3fe364dc6260d27bd61310bd1383c0639f6297f693c5c0ec11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:ec210def90412bcfd6586f056bf15cfba9a6ae2d83f329f3095914d7202fbada
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117737381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244874bc2bf861b02626382c1d1bd042fd26991a17b503bef6e57853764f3cf1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:44:42 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 18 Nov 2021 09:44:52 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:44:53 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 18 Nov 2021 09:44:53 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:44:53 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:44:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:44:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 18 Nov 2021 09:44:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:44:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08525dea5b6b885656a753a6deef7a71e230e77dafc7f831bd2a4c9f21df5da5`  
		Last Modified: Thu, 18 Nov 2021 09:49:07 GMT  
		Size: 56.7 MB (56708533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57d90367afa71b328b7c1e192c38ec3bc28ec42bfab9b9f002cd21e6f4b455e`  
		Last Modified: Thu, 18 Nov 2021 09:48:58 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e37b0832a2c9fc55d7d0e4b680f6da9e95a0aad7fe83ea36bdb03fb68b0aab`  
		Last Modified: Thu, 18 Nov 2021 09:48:58 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf287206df98f216591a3ae20f6a591c9970835eab55160656bb711f72094f5c`  
		Last Modified: Thu, 18 Nov 2021 09:48:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data-alpine`

```console
$ docker pull influxdb@sha256:9edb5e97912c1a30144b9674f7d24f957a6ee186dad14461da00075d7b3796cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f6c46290f9cfbd9b2fbe6e9f47ab18fe7314c5bd6758ed3c7fde006478ba2a47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60814908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9083f2c434fe802e0c24ff0518282b9c8956c0cb1156626ed29c0cacff0fd794`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:29:25 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 13 Nov 2021 02:29:38 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:29:39 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 13 Nov 2021 02:29:39 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:29:39 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:29:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:29:39 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 13 Nov 2021 02:29:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:29:40 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b1c62ddbddb14ed511aedfa47a61da93b52f2ebc434d573e6cccdeab360012`  
		Last Modified: Sat, 13 Nov 2021 02:34:40 GMT  
		Size: 56.5 MB (56503786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182dd80d9b0c7757cdea730b9d8438eddf10b2837f1bc4f9555e24a2e16c9f1f`  
		Last Modified: Sat, 13 Nov 2021 02:34:30 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad150614e74207f44ffbcda2bdd6d075d072e5d7e40c18aea4d02bf92012d3`  
		Last Modified: Sat, 13 Nov 2021 02:34:31 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebec01cb49874553e60a3087e07f6ea3be09a5253235bbc016d200b165f0740`  
		Last Modified: Sat, 13 Nov 2021 02:34:30 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta`

```console
$ docker pull influxdb@sha256:31500f40ed7a50fdb52e8a0990aea86bd8c0f50814d644754a9f57c35fca7ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:64534669863b8e1414ac4aa65a41d124604e61f8b9ce42b31e297cb2a8d15987
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84443975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6befdf4bac0b404e5ad4274eafa07f36729725f56bef2f3ae11f41259f0cc59d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:44:42 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 18 Nov 2021 09:45:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:45:05 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 18 Nov 2021 09:45:05 GMT
EXPOSE 8091
# Thu, 18 Nov 2021 09:45:05 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:45:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:45:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:45:06 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64521abd18cf018ab9316be9ab482c503cb3c6b8adeb380319d51c18556be12e`  
		Last Modified: Thu, 18 Nov 2021 09:49:24 GMT  
		Size: 23.4 MB (23416332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82be31c0c04837996a2f891230ea306a73ed63264076a52cff01efbae7234c49`  
		Last Modified: Thu, 18 Nov 2021 09:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6ebc4c9a6547fd06dd99b1c765524dfdd7a939834caad7a1fac1b01c95d3bd`  
		Last Modified: Thu, 18 Nov 2021 09:49:20 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta-alpine`

```console
$ docker pull influxdb@sha256:4cba27899d3f6324276746cc3d13e113171e58f0cd57b6f778f223d9e5fe1173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:fe5ecca89fb203a0a446abc95062c96221545125968f4f313c50cd821f5a4e7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27602958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:072b66b0c223ce772c78f84a6586e8080a5fb145cf5f1d00eefd6f23846e45cc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:29:25 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 13 Nov 2021 02:29:53 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:29:53 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 13 Nov 2021 02:29:54 GMT
EXPOSE 8091
# Sat, 13 Nov 2021 02:29:54 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:29:54 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:29:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:29:55 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7f836dc8033be4020b77d60ac1d010d51d58ce819fd31c8c903dd7bf1d9bed`  
		Last Modified: Sat, 13 Nov 2021 02:35:00 GMT  
		Size: 23.3 MB (23293039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352cd5d07590068a89a6415f0d3923109129dddfdae2762d95cf37b800faed14`  
		Last Modified: Sat, 13 Nov 2021 02:34:56 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a164a9ffc5db6c4dbad8265ed41221745f6094e8223216f516ecfb034794045`  
		Last Modified: Sat, 13 Nov 2021 02:34:56 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data`

```console
$ docker pull influxdb@sha256:90c55fa369ae76454312b0c38dc52edc762bc6ffdadd4f1ef10899843ab9389f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:beb02394358cfda2c6fbb5653296faad979b73f9daf90d5e702e094c8897c478
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115568449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547fcd33d6ffcb009e0bbe548c7ccdc82786d56c59b405ffcfb056305d323673`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:45:11 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Thu, 18 Nov 2021 09:45:20 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:45:21 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 18 Nov 2021 09:45:21 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:45:21 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:45:22 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:45:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 18 Nov 2021 09:45:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:45:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620e33b2f370792dca8de045249890815d1188d411d6c6355b9ff599f6c46bb8`  
		Last Modified: Thu, 18 Nov 2021 09:49:45 GMT  
		Size: 54.5 MB (54539599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9353324283ffb8fb34bd0ec49632f4d1bae5295ce4fa35fa942dc9d47b5174`  
		Last Modified: Thu, 18 Nov 2021 09:49:37 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff29b84122f4475b00498c5a7b453f6d923c79a8cd78be3a09d8da92d930105`  
		Last Modified: Thu, 18 Nov 2021 09:49:37 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9538845663658c5526cc9808f18f5c4086df8b73b213c183c5b3e97cbea19c9`  
		Last Modified: Thu, 18 Nov 2021 09:49:37 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:7c281639d7ba649c9877941e1c74c0d931edf4082f495938b7aaa8d53d651b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:0e74c2f0b9df807eb348767dbf87d47adbca743ae8bc002353cc4396ea599a92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58817673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85dd900d3af852053e9b17d61564cc7c698166036ee8ae6ca162e6e9f3ec0ec2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:30:00 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Sat, 13 Nov 2021 02:30:13 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:30:13 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 13 Nov 2021 02:30:14 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:30:14 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:30:14 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:30:15 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 13 Nov 2021 02:30:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:30:15 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84aba9f220f8744b015ce88ca35a1e04843fe60c2657b434a1dfaf54f118c4`  
		Last Modified: Sat, 13 Nov 2021 02:35:22 GMT  
		Size: 54.5 MB (54506551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1357868332733c609de87a805decd44dc6d8edeb7dd98497a56b1e7740e2b61f`  
		Last Modified: Sat, 13 Nov 2021 02:35:14 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ddf39e4ecb850043fc546c23a2687948939ded4587b1a9b56643432da42a390`  
		Last Modified: Sat, 13 Nov 2021 02:35:14 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb481d684ab7ff475cf1c366e382e5a8c11e4666b080434ed26d5c79939d305`  
		Last Modified: Sat, 13 Nov 2021 02:35:14 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:17fe91c0dcef029ba7702aa1e1269a9bb069417d7783459ecb6b3eeaba4898e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:cb3fe08deb72085e2c787e9159819ba972f2c63b79027ab2a50d707bd32470e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86087822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb877c2c048c09fdf187a8ed30949f1139abcfe622f2aa65b8b1ba4fc490555a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:45:11 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Thu, 18 Nov 2021 09:45:33 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:45:34 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 18 Nov 2021 09:45:34 GMT
EXPOSE 8091
# Thu, 18 Nov 2021 09:45:34 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:45:35 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:45:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:45:35 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29a1712b43a9013c0b8fef164a21984143d0e5ce4affcd681f86647c4b30ed0`  
		Last Modified: Thu, 18 Nov 2021 09:49:59 GMT  
		Size: 25.1 MB (25060179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6861e5e850f3f5e080da67169b35c57f741ec446458341e1a29afa97a19863`  
		Last Modified: Thu, 18 Nov 2021 09:49:55 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5291a49427fe344d0e76cb73204b1b793f7db6bd2c34553d8e3824025859f6a1`  
		Last Modified: Thu, 18 Nov 2021 09:49:55 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:c8a9af74d6ccd1d57c1309c74adb63c9a399b3746c1dd2b8227058def29381dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:bd0f57c607378082df031f088d6da80dee45aae659ec97933e1b372e1cacb3c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29339037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a18ce9967ce12ae94a093f44bf25552b547b4b2ded05f7230e769f2d1f7d32`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:30:00 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Sat, 13 Nov 2021 02:30:31 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     (rm -rf /root/.gnupg || true) &&     rm -rf *.tar.gz* /usr/src &&     apk del .build-deps
# Sat, 13 Nov 2021 02:30:32 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 13 Nov 2021 02:30:32 GMT
EXPOSE 8091
# Sat, 13 Nov 2021 02:30:32 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:30:33 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:30:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:30:34 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d06be92c9ce93ca405b7851f2fbfdaf3adfcd6d241090941068b97f0e1d6cf`  
		Last Modified: Sat, 13 Nov 2021 02:35:36 GMT  
		Size: 25.0 MB (25029115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7eacd05661ddb9fba8f5a9ce5a977ea7fef7f122f6d3af97f869fb17d2dd64`  
		Last Modified: Sat, 13 Nov 2021 02:35:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1aa15383fe9afad4d0648d0ef4ebd57bf83eedb8926bfc476ad5083f37221d`  
		Last Modified: Sat, 13 Nov 2021 02:35:32 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.5-data`

```console
$ docker pull influxdb@sha256:90c55fa369ae76454312b0c38dc52edc762bc6ffdadd4f1ef10899843ab9389f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.5-data` - linux; amd64

```console
$ docker pull influxdb@sha256:beb02394358cfda2c6fbb5653296faad979b73f9daf90d5e702e094c8897c478
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115568449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547fcd33d6ffcb009e0bbe548c7ccdc82786d56c59b405ffcfb056305d323673`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:45:11 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Thu, 18 Nov 2021 09:45:20 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:45:21 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 18 Nov 2021 09:45:21 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:45:21 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:45:22 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:45:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 18 Nov 2021 09:45:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:45:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620e33b2f370792dca8de045249890815d1188d411d6c6355b9ff599f6c46bb8`  
		Last Modified: Thu, 18 Nov 2021 09:49:45 GMT  
		Size: 54.5 MB (54539599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9353324283ffb8fb34bd0ec49632f4d1bae5295ce4fa35fa942dc9d47b5174`  
		Last Modified: Thu, 18 Nov 2021 09:49:37 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff29b84122f4475b00498c5a7b453f6d923c79a8cd78be3a09d8da92d930105`  
		Last Modified: Thu, 18 Nov 2021 09:49:37 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9538845663658c5526cc9808f18f5c4086df8b73b213c183c5b3e97cbea19c9`  
		Last Modified: Thu, 18 Nov 2021 09:49:37 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.5-data-alpine`

```console
$ docker pull influxdb@sha256:7c281639d7ba649c9877941e1c74c0d931edf4082f495938b7aaa8d53d651b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.5-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:0e74c2f0b9df807eb348767dbf87d47adbca743ae8bc002353cc4396ea599a92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58817673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85dd900d3af852053e9b17d61564cc7c698166036ee8ae6ca162e6e9f3ec0ec2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:30:00 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Sat, 13 Nov 2021 02:30:13 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:30:13 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 13 Nov 2021 02:30:14 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:30:14 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:30:14 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:30:15 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 13 Nov 2021 02:30:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:30:15 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84aba9f220f8744b015ce88ca35a1e04843fe60c2657b434a1dfaf54f118c4`  
		Last Modified: Sat, 13 Nov 2021 02:35:22 GMT  
		Size: 54.5 MB (54506551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1357868332733c609de87a805decd44dc6d8edeb7dd98497a56b1e7740e2b61f`  
		Last Modified: Sat, 13 Nov 2021 02:35:14 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ddf39e4ecb850043fc546c23a2687948939ded4587b1a9b56643432da42a390`  
		Last Modified: Sat, 13 Nov 2021 02:35:14 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb481d684ab7ff475cf1c366e382e5a8c11e4666b080434ed26d5c79939d305`  
		Last Modified: Sat, 13 Nov 2021 02:35:14 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.5-meta`

```console
$ docker pull influxdb@sha256:17fe91c0dcef029ba7702aa1e1269a9bb069417d7783459ecb6b3eeaba4898e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.5-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:cb3fe08deb72085e2c787e9159819ba972f2c63b79027ab2a50d707bd32470e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86087822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb877c2c048c09fdf187a8ed30949f1139abcfe622f2aa65b8b1ba4fc490555a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:45:11 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Thu, 18 Nov 2021 09:45:33 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:45:34 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 18 Nov 2021 09:45:34 GMT
EXPOSE 8091
# Thu, 18 Nov 2021 09:45:34 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:45:35 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:45:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:45:35 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29a1712b43a9013c0b8fef164a21984143d0e5ce4affcd681f86647c4b30ed0`  
		Last Modified: Thu, 18 Nov 2021 09:49:59 GMT  
		Size: 25.1 MB (25060179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6861e5e850f3f5e080da67169b35c57f741ec446458341e1a29afa97a19863`  
		Last Modified: Thu, 18 Nov 2021 09:49:55 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5291a49427fe344d0e76cb73204b1b793f7db6bd2c34553d8e3824025859f6a1`  
		Last Modified: Thu, 18 Nov 2021 09:49:55 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.5-meta-alpine`

```console
$ docker pull influxdb@sha256:c8a9af74d6ccd1d57c1309c74adb63c9a399b3746c1dd2b8227058def29381dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.5-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:bd0f57c607378082df031f088d6da80dee45aae659ec97933e1b372e1cacb3c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29339037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a18ce9967ce12ae94a093f44bf25552b547b4b2ded05f7230e769f2d1f7d32`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:30:00 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Sat, 13 Nov 2021 02:30:31 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     (rm -rf /root/.gnupg || true) &&     rm -rf *.tar.gz* /usr/src &&     apk del .build-deps
# Sat, 13 Nov 2021 02:30:32 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 13 Nov 2021 02:30:32 GMT
EXPOSE 8091
# Sat, 13 Nov 2021 02:30:32 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:30:33 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:30:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:30:34 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d06be92c9ce93ca405b7851f2fbfdaf3adfcd6d241090941068b97f0e1d6cf`  
		Last Modified: Sat, 13 Nov 2021 02:35:36 GMT  
		Size: 25.0 MB (25029115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7eacd05661ddb9fba8f5a9ce5a977ea7fef7f122f6d3af97f869fb17d2dd64`  
		Last Modified: Sat, 13 Nov 2021 02:35:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1aa15383fe9afad4d0648d0ef4ebd57bf83eedb8926bfc476ad5083f37221d`  
		Last Modified: Sat, 13 Nov 2021 02:35:32 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0`

```console
$ docker pull influxdb@sha256:98711bca212e28f694af6e5cb9b37f404da57f8e67f129b3684c0caae3fc7221
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:780855e33ef1d68064038a4bbea6c48a18029dc6c5657813203481560a8b4a32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172326365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75105b457f6c8079acccba7bdec23a37fb96f58dba827e81f3faeee5996d4cb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:45:40 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 18 Nov 2021 09:45:40 GMT
ENV GOSU_VER=1.12
# Thu, 18 Nov 2021 09:45:44 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Thu, 18 Nov 2021 09:45:45 GMT
ENV INFLUXDB_VERSION=2.0.9
# Thu, 18 Nov 2021 09:45:57 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Thu, 18 Nov 2021 09:45:58 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 18 Nov 2021 09:45:58 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 18 Nov 2021 09:45:58 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 18 Nov 2021 09:45:59 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:45:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:45:59 GMT
CMD ["influxd"]
# Thu, 18 Nov 2021 09:45:59 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:45:59 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 18 Nov 2021 09:46:00 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 18 Nov 2021 09:46:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 18 Nov 2021 09:46:00 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a603b07c93043ffbd790761bf1cf232dd2763ec10c3ef84ce381390713c99`  
		Last Modified: Thu, 18 Nov 2021 09:50:12 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80de06b69dbd583c55db5aebf57682c087c624d343e0410552603f35686a40`  
		Last Modified: Thu, 18 Nov 2021 09:50:10 GMT  
		Size: 961.0 KB (960988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e055ac4566bf0d5f58a0fb69c50d905c5144cba4c0c10161fddc19169bc17`  
		Last Modified: Thu, 18 Nov 2021 09:50:24 GMT  
		Size: 103.1 MB (103090643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbe4a05062a10d6b8871fa09d08933c96c58a0ee7fadfe6596b7597d42b90a2`  
		Last Modified: Thu, 18 Nov 2021 09:50:10 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e6932eea0b1fbb2bb89278e58b829eccad31ac268ae5e3183235b9abfe3101`  
		Last Modified: Thu, 18 Nov 2021 09:50:09 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bdccaaa2c773c9e62397112e429724062302f8bdabd5f7a2958b2c88c7f0d3`  
		Last Modified: Thu, 18 Nov 2021 09:50:09 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c86dd9b0df51a5f254d2c64f4f7ca2690c3c13e5328d04ee5b739e9a55e93ec3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174115074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38484974e6131a99d5dd9da5141e0e433a99a8a5fff26e0d8388c3425ec967b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:39:03 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 17 Nov 2021 21:39:04 GMT
ENV GOSU_VER=1.12
# Wed, 17 Nov 2021 21:39:08 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 17 Nov 2021 21:39:09 GMT
ENV INFLUXDB_VERSION=2.0.9
# Wed, 17 Nov 2021 21:39:21 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 17 Nov 2021 21:39:22 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 17 Nov 2021 21:39:22 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 17 Nov 2021 21:39:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 17 Nov 2021 21:39:25 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Wed, 17 Nov 2021 21:39:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:39:26 GMT
CMD ["influxd"]
# Wed, 17 Nov 2021 21:39:27 GMT
EXPOSE 8086
# Wed, 17 Nov 2021 21:39:28 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 17 Nov 2021 21:39:29 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 17 Nov 2021 21:39:30 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 17 Nov 2021 21:39:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90efb0d865d89e679077061bdca34c60306bacab5579d93a951cd8c31441ec`  
		Last Modified: Wed, 17 Nov 2021 21:41:46 GMT  
		Size: 1.7 KB (1659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f283e1015297042ffd1e94f9753b4ef6b9ce33339509b31d96c13eb7dcd03f82`  
		Last Modified: Wed, 17 Nov 2021 21:41:44 GMT  
		Size: 896.4 KB (896361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125a0be757488435dcb7e8fe4f32fc742f15b88e1195c176b23c777f63fd48b6`  
		Last Modified: Wed, 17 Nov 2021 21:41:54 GMT  
		Size: 106.5 MB (106526998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795b77a162b6c429502489a9df15d408b24f69221988ea65d447e6f19ec55240`  
		Last Modified: Wed, 17 Nov 2021 21:41:43 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c21e7ebb0abc8e0427899838a37511a4664900fcd8c92b19135027f490e3e8`  
		Last Modified: Wed, 17 Nov 2021 21:41:43 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58462a5fca496eedf527ccf2a00be1f8680644e3510e62fc7568121d54d436fe`  
		Last Modified: Wed, 17 Nov 2021 21:41:43 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0-alpine`

```console
$ docker pull influxdb@sha256:e83d95eb40544b7ae8102fdb7a69971558df789b1f16351ebe78c9aaa4ea95ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ee0ddf966e5331ad03a1a93ffe245af88de291d96fb93271601c670dbaa6f0bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116735114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:179c4b26e4345c3d75e7bf4484fe690844b39af3cdfc01cd0004633d2a912e77`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:30:45 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 13 Nov 2021 02:30:47 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 13 Nov 2021 02:30:48 GMT
ENV GOSU_VER=1.12
# Sat, 13 Nov 2021 02:30:53 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 02:30:53 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sat, 13 Nov 2021 02:31:07 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 13 Nov 2021 02:31:09 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 13 Nov 2021 02:31:09 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 13 Nov 2021 02:31:10 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 13 Nov 2021 02:31:10 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:31:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:31:11 GMT
CMD ["influxd"]
# Sat, 13 Nov 2021 02:31:12 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:31:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 13 Nov 2021 02:31:12 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 13 Nov 2021 02:31:13 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 13 Nov 2021 02:31:13 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb48a4c6ea759da391d76004114a5ee8ee41f81dfae508ddfd4c9a2d36f84c`  
		Last Modified: Sat, 13 Nov 2021 02:35:51 GMT  
		Size: 9.9 MB (9854595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f25e434782a05647d6530f2a12eec8118d5df67373eb45fb04033377d5d1b`  
		Last Modified: Sat, 13 Nov 2021 02:35:49 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58f08bf46f1b06d391462bc99b273bb53267c678b30135522996f0390e7865c`  
		Last Modified: Sat, 13 Nov 2021 02:35:47 GMT  
		Size: 960.6 KB (960615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7227a33d189485c965626da2f3d2025b9edcad120ba95257accac0d46854f`  
		Last Modified: Sat, 13 Nov 2021 02:35:57 GMT  
		Size: 103.1 MB (103090643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455cdc26dca33ecd27e7260181b04aaefe22c919dca894d724fac50a8140b791`  
		Last Modified: Sat, 13 Nov 2021 02:35:46 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f181a50317c57003600b0be0ad95ebad740142f4a0d80628c3a5c68a596399c1`  
		Last Modified: Sat, 13 Nov 2021 02:35:46 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd101ccd030d53a25f18914fef800e3132d4bd1dffcc75d3d957c21a70e77c7`  
		Last Modified: Sat, 13 Nov 2021 02:35:47 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:35fc24acbab06fe4bd94b3e498d5f732f5487d44f91ff8fad3cf03929dca4811
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119835591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d95a75ebd8c699740949ae6649559beb134fc0c1c3b51e2ed76e342db476ea1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:23:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:23:11 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 13 Nov 2021 06:23:12 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 13 Nov 2021 06:23:13 GMT
ENV GOSU_VER=1.12
# Sat, 13 Nov 2021 06:23:16 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 06:23:17 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sat, 13 Nov 2021 06:23:31 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 13 Nov 2021 06:23:31 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 13 Nov 2021 06:23:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 13 Nov 2021 06:23:34 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 13 Nov 2021 06:23:35 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Sat, 13 Nov 2021 06:23:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:23:36 GMT
CMD ["influxd"]
# Sat, 13 Nov 2021 06:23:37 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 06:23:38 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 13 Nov 2021 06:23:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 13 Nov 2021 06:23:40 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 13 Nov 2021 06:23:41 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd8bff15f28e0e2cd2ccb61904ad49022b3252c074dd64a3e7ab49c41ef2e24`  
		Last Modified: Sat, 13 Nov 2021 06:25:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01db43e1eccfeabd1a2a22c07f6303840d1566375fe8cd4ecaa1e15c363f258`  
		Last Modified: Sat, 13 Nov 2021 06:25:07 GMT  
		Size: 9.7 MB (9688653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f189869e04c42c9f2488fc1516e1a567f55da7bff406758600ddbf20835eea7`  
		Last Modified: Sat, 13 Nov 2021 06:25:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e6fbb9a1a27e8801496b32b26fdd9e3a960d9b63124df203e308b391c80c98`  
		Last Modified: Sat, 13 Nov 2021 06:25:03 GMT  
		Size: 896.1 KB (896076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cef4f41ce59bda87dd4ee533fa65e474375f5a7c5c32408a8d2d5f8581d3405`  
		Last Modified: Sat, 13 Nov 2021 06:25:13 GMT  
		Size: 106.5 MB (106527003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786083987e27642b453bb2b90b23e6f147bbd4ae0d9283b43cd292dea347131b`  
		Last Modified: Sat, 13 Nov 2021 06:25:03 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96360dd8c4d2e081b0f545efea0e987c5aeec0e8311ba6d1b7fcf77f2abcb24b`  
		Last Modified: Sat, 13 Nov 2021 06:25:03 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c459dd404b88c0959a29656d40909eb63d263cbbe9e2c1526eff1dbfd97d3970`  
		Last Modified: Sat, 13 Nov 2021 06:25:03 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.9`

```console
$ docker pull influxdb@sha256:98711bca212e28f694af6e5cb9b37f404da57f8e67f129b3684c0caae3fc7221
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9` - linux; amd64

```console
$ docker pull influxdb@sha256:780855e33ef1d68064038a4bbea6c48a18029dc6c5657813203481560a8b4a32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172326365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75105b457f6c8079acccba7bdec23a37fb96f58dba827e81f3faeee5996d4cb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:45:40 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 18 Nov 2021 09:45:40 GMT
ENV GOSU_VER=1.12
# Thu, 18 Nov 2021 09:45:44 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Thu, 18 Nov 2021 09:45:45 GMT
ENV INFLUXDB_VERSION=2.0.9
# Thu, 18 Nov 2021 09:45:57 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Thu, 18 Nov 2021 09:45:58 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 18 Nov 2021 09:45:58 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 18 Nov 2021 09:45:58 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 18 Nov 2021 09:45:59 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:45:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:45:59 GMT
CMD ["influxd"]
# Thu, 18 Nov 2021 09:45:59 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:45:59 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 18 Nov 2021 09:46:00 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 18 Nov 2021 09:46:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 18 Nov 2021 09:46:00 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a603b07c93043ffbd790761bf1cf232dd2763ec10c3ef84ce381390713c99`  
		Last Modified: Thu, 18 Nov 2021 09:50:12 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80de06b69dbd583c55db5aebf57682c087c624d343e0410552603f35686a40`  
		Last Modified: Thu, 18 Nov 2021 09:50:10 GMT  
		Size: 961.0 KB (960988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e055ac4566bf0d5f58a0fb69c50d905c5144cba4c0c10161fddc19169bc17`  
		Last Modified: Thu, 18 Nov 2021 09:50:24 GMT  
		Size: 103.1 MB (103090643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbe4a05062a10d6b8871fa09d08933c96c58a0ee7fadfe6596b7597d42b90a2`  
		Last Modified: Thu, 18 Nov 2021 09:50:10 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e6932eea0b1fbb2bb89278e58b829eccad31ac268ae5e3183235b9abfe3101`  
		Last Modified: Thu, 18 Nov 2021 09:50:09 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bdccaaa2c773c9e62397112e429724062302f8bdabd5f7a2958b2c88c7f0d3`  
		Last Modified: Thu, 18 Nov 2021 09:50:09 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:c86dd9b0df51a5f254d2c64f4f7ca2690c3c13e5328d04ee5b739e9a55e93ec3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174115074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38484974e6131a99d5dd9da5141e0e433a99a8a5fff26e0d8388c3425ec967b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:39:03 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 17 Nov 2021 21:39:04 GMT
ENV GOSU_VER=1.12
# Wed, 17 Nov 2021 21:39:08 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 17 Nov 2021 21:39:09 GMT
ENV INFLUXDB_VERSION=2.0.9
# Wed, 17 Nov 2021 21:39:21 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 17 Nov 2021 21:39:22 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 17 Nov 2021 21:39:22 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 17 Nov 2021 21:39:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 17 Nov 2021 21:39:25 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Wed, 17 Nov 2021 21:39:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:39:26 GMT
CMD ["influxd"]
# Wed, 17 Nov 2021 21:39:27 GMT
EXPOSE 8086
# Wed, 17 Nov 2021 21:39:28 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 17 Nov 2021 21:39:29 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 17 Nov 2021 21:39:30 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 17 Nov 2021 21:39:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90efb0d865d89e679077061bdca34c60306bacab5579d93a951cd8c31441ec`  
		Last Modified: Wed, 17 Nov 2021 21:41:46 GMT  
		Size: 1.7 KB (1659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f283e1015297042ffd1e94f9753b4ef6b9ce33339509b31d96c13eb7dcd03f82`  
		Last Modified: Wed, 17 Nov 2021 21:41:44 GMT  
		Size: 896.4 KB (896361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125a0be757488435dcb7e8fe4f32fc742f15b88e1195c176b23c777f63fd48b6`  
		Last Modified: Wed, 17 Nov 2021 21:41:54 GMT  
		Size: 106.5 MB (106526998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795b77a162b6c429502489a9df15d408b24f69221988ea65d447e6f19ec55240`  
		Last Modified: Wed, 17 Nov 2021 21:41:43 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c21e7ebb0abc8e0427899838a37511a4664900fcd8c92b19135027f490e3e8`  
		Last Modified: Wed, 17 Nov 2021 21:41:43 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58462a5fca496eedf527ccf2a00be1f8680644e3510e62fc7568121d54d436fe`  
		Last Modified: Wed, 17 Nov 2021 21:41:43 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.9-alpine`

```console
$ docker pull influxdb@sha256:e83d95eb40544b7ae8102fdb7a69971558df789b1f16351ebe78c9aaa4ea95ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ee0ddf966e5331ad03a1a93ffe245af88de291d96fb93271601c670dbaa6f0bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116735114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:179c4b26e4345c3d75e7bf4484fe690844b39af3cdfc01cd0004633d2a912e77`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:30:45 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 13 Nov 2021 02:30:47 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 13 Nov 2021 02:30:48 GMT
ENV GOSU_VER=1.12
# Sat, 13 Nov 2021 02:30:53 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 02:30:53 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sat, 13 Nov 2021 02:31:07 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 13 Nov 2021 02:31:09 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 13 Nov 2021 02:31:09 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 13 Nov 2021 02:31:10 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 13 Nov 2021 02:31:10 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:31:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:31:11 GMT
CMD ["influxd"]
# Sat, 13 Nov 2021 02:31:12 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:31:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 13 Nov 2021 02:31:12 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 13 Nov 2021 02:31:13 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 13 Nov 2021 02:31:13 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb48a4c6ea759da391d76004114a5ee8ee41f81dfae508ddfd4c9a2d36f84c`  
		Last Modified: Sat, 13 Nov 2021 02:35:51 GMT  
		Size: 9.9 MB (9854595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f25e434782a05647d6530f2a12eec8118d5df67373eb45fb04033377d5d1b`  
		Last Modified: Sat, 13 Nov 2021 02:35:49 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58f08bf46f1b06d391462bc99b273bb53267c678b30135522996f0390e7865c`  
		Last Modified: Sat, 13 Nov 2021 02:35:47 GMT  
		Size: 960.6 KB (960615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc7227a33d189485c965626da2f3d2025b9edcad120ba95257accac0d46854f`  
		Last Modified: Sat, 13 Nov 2021 02:35:57 GMT  
		Size: 103.1 MB (103090643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455cdc26dca33ecd27e7260181b04aaefe22c919dca894d724fac50a8140b791`  
		Last Modified: Sat, 13 Nov 2021 02:35:46 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f181a50317c57003600b0be0ad95ebad740142f4a0d80628c3a5c68a596399c1`  
		Last Modified: Sat, 13 Nov 2021 02:35:46 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd101ccd030d53a25f18914fef800e3132d4bd1dffcc75d3d957c21a70e77c7`  
		Last Modified: Sat, 13 Nov 2021 02:35:47 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:35fc24acbab06fe4bd94b3e498d5f732f5487d44f91ff8fad3cf03929dca4811
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119835591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d95a75ebd8c699740949ae6649559beb134fc0c1c3b51e2ed76e342db476ea1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:23:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:23:11 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 13 Nov 2021 06:23:12 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 13 Nov 2021 06:23:13 GMT
ENV GOSU_VER=1.12
# Sat, 13 Nov 2021 06:23:16 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 06:23:17 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sat, 13 Nov 2021 06:23:31 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 13 Nov 2021 06:23:31 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 13 Nov 2021 06:23:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 13 Nov 2021 06:23:34 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 13 Nov 2021 06:23:35 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Sat, 13 Nov 2021 06:23:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:23:36 GMT
CMD ["influxd"]
# Sat, 13 Nov 2021 06:23:37 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 06:23:38 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 13 Nov 2021 06:23:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 13 Nov 2021 06:23:40 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 13 Nov 2021 06:23:41 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd8bff15f28e0e2cd2ccb61904ad49022b3252c074dd64a3e7ab49c41ef2e24`  
		Last Modified: Sat, 13 Nov 2021 06:25:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01db43e1eccfeabd1a2a22c07f6303840d1566375fe8cd4ecaa1e15c363f258`  
		Last Modified: Sat, 13 Nov 2021 06:25:07 GMT  
		Size: 9.7 MB (9688653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f189869e04c42c9f2488fc1516e1a567f55da7bff406758600ddbf20835eea7`  
		Last Modified: Sat, 13 Nov 2021 06:25:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e6fbb9a1a27e8801496b32b26fdd9e3a960d9b63124df203e308b391c80c98`  
		Last Modified: Sat, 13 Nov 2021 06:25:03 GMT  
		Size: 896.1 KB (896076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cef4f41ce59bda87dd4ee533fa65e474375f5a7c5c32408a8d2d5f8581d3405`  
		Last Modified: Sat, 13 Nov 2021 06:25:13 GMT  
		Size: 106.5 MB (106527003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786083987e27642b453bb2b90b23e6f147bbd4ae0d9283b43cd292dea347131b`  
		Last Modified: Sat, 13 Nov 2021 06:25:03 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96360dd8c4d2e081b0f545efea0e987c5aeec0e8311ba6d1b7fcf77f2abcb24b`  
		Last Modified: Sat, 13 Nov 2021 06:25:03 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c459dd404b88c0959a29656d40909eb63d263cbbe9e2c1526eff1dbfd97d3970`  
		Last Modified: Sat, 13 Nov 2021 06:25:03 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1`

```console
$ docker pull influxdb@sha256:f2543c9cc70fd75298a52647d828047ff5fbcd28f19be8a70bf9fb1429b5b6f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1` - linux; amd64

```console
$ docker pull influxdb@sha256:7fd69f4a2c16efc0d5c2863ce2d74d9479dfc458ade2132379b94c28a04913c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182885029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfb4d421b2f653f5e58125af722b2677eb5c4f0fc2a125ef654b8ebd91550f34`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:45:40 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 18 Nov 2021 09:45:40 GMT
ENV GOSU_VER=1.12
# Thu, 18 Nov 2021 09:45:44 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Thu, 18 Nov 2021 09:46:04 GMT
ENV INFLUXDB_VERSION=2.1.1
# Thu, 18 Nov 2021 09:46:12 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 18 Nov 2021 09:46:13 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Thu, 18 Nov 2021 09:46:17 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 18 Nov 2021 09:46:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 18 Nov 2021 09:46:19 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 18 Nov 2021 09:46:19 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 18 Nov 2021 09:46:19 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:46:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:46:20 GMT
CMD ["influxd"]
# Thu, 18 Nov 2021 09:46:20 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 18 Nov 2021 09:46:21 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a603b07c93043ffbd790761bf1cf232dd2763ec10c3ef84ce381390713c99`  
		Last Modified: Thu, 18 Nov 2021 09:50:12 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80de06b69dbd583c55db5aebf57682c087c624d343e0410552603f35686a40`  
		Last Modified: Thu, 18 Nov 2021 09:50:10 GMT  
		Size: 961.0 KB (960988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf4fe7d34889b9b417a1448e1fee0a421bef2c9533916a1f513e8fdfd7baf99`  
		Last Modified: Thu, 18 Nov 2021 09:50:44 GMT  
		Size: 108.3 MB (108324825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8efd2d9a5def9f50aa609b47f8a39012190fb713c9ea285b497c24d014155`  
		Last Modified: Thu, 18 Nov 2021 09:50:36 GMT  
		Size: 5.3 MB (5324484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0d1b444bc9f9096339ec15ce0e4456f4823121b9214b2710b46c82e9147c8d`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f05877070f022483807a8ff887e1619260f8008f79b31053d9d3761acc7174`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c522e98cfb3d02a730692d7aef75148fd190b0192ed98300bed425c66842a9fd`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 4.3 KB (4321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b50ab5a02481210516a7b440d910051c76f1b3fea61255bf554657f7368bb60d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183386413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905455e4cd353ee4e93fd7658b084034e0ad5661373b055973befbc41ae696c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:39:03 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 17 Nov 2021 21:39:04 GMT
ENV GOSU_VER=1.12
# Wed, 17 Nov 2021 21:39:08 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 17 Nov 2021 21:39:43 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 17 Nov 2021 21:40:02 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 17 Nov 2021 21:40:02 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 17 Nov 2021 21:40:07 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 17 Nov 2021 21:40:07 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 17 Nov 2021 21:40:08 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 17 Nov 2021 21:40:10 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 17 Nov 2021 21:40:11 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Wed, 17 Nov 2021 21:40:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:40:12 GMT
CMD ["influxd"]
# Wed, 17 Nov 2021 21:40:13 GMT
EXPOSE 8086
# Wed, 17 Nov 2021 21:40:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 17 Nov 2021 21:40:15 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 17 Nov 2021 21:40:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 17 Nov 2021 21:40:17 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90efb0d865d89e679077061bdca34c60306bacab5579d93a951cd8c31441ec`  
		Last Modified: Wed, 17 Nov 2021 21:41:46 GMT  
		Size: 1.7 KB (1659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f283e1015297042ffd1e94f9753b4ef6b9ce33339509b31d96c13eb7dcd03f82`  
		Last Modified: Wed, 17 Nov 2021 21:41:44 GMT  
		Size: 896.4 KB (896361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d89c50dbb1d05a49120a4b621b6b382d2b29d6304c7f10b0eee084dab7d8dac`  
		Last Modified: Wed, 17 Nov 2021 21:42:16 GMT  
		Size: 110.9 MB (110891616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e6709d1f966cd8da3d817ff591df547559a47204cff841140f0c4f205c829f`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 4.9 MB (4906724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31859363882c3135133fce1a0f41006d7cb4c7ee4a669ea650ba2c541af3b7d5`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec1462a4ae6c9e136f82cbc586a32ea5c2b7089fa2ae02d94cdb2380b2369f`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e7de37831dc0c6521d41919d1fff71b50a3dfe399e29199fcb1e812dad17cb`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1-alpine`

```console
$ docker pull influxdb@sha256:a5b34976d4cb3dbc627bfe3d6c08b752ec81586c5c98ac167d84f891c9c7db9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:05af8b4364b19365b722025c16867e0143af044cefd0376566398e91f32c59dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127293784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae8a2276202e4e4296fa44cdedc2ae794d791793d92a4071645957a7dfc4729f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:30:45 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 13 Nov 2021 02:30:47 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 13 Nov 2021 02:30:48 GMT
ENV GOSU_VER=1.12
# Sat, 13 Nov 2021 02:30:53 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 02:31:26 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 13 Nov 2021 02:31:40 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 13 Nov 2021 02:31:41 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 13 Nov 2021 02:31:46 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 13 Nov 2021 02:31:48 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 13 Nov 2021 02:31:48 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 13 Nov 2021 02:31:48 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 13 Nov 2021 02:31:49 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:31:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:31:49 GMT
CMD ["influxd"]
# Sat, 13 Nov 2021 02:31:50 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:31:50 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 13 Nov 2021 02:31:50 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 13 Nov 2021 02:31:51 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 13 Nov 2021 02:31:51 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb48a4c6ea759da391d76004114a5ee8ee41f81dfae508ddfd4c9a2d36f84c`  
		Last Modified: Sat, 13 Nov 2021 02:35:51 GMT  
		Size: 9.9 MB (9854595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f25e434782a05647d6530f2a12eec8118d5df67373eb45fb04033377d5d1b`  
		Last Modified: Sat, 13 Nov 2021 02:35:49 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58f08bf46f1b06d391462bc99b273bb53267c678b30135522996f0390e7865c`  
		Last Modified: Sat, 13 Nov 2021 02:35:47 GMT  
		Size: 960.6 KB (960615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4932f7c0bf2c64c409cdbf559c862abe12f1e35739f607b1f01ef5fbf4d48c8d`  
		Last Modified: Sat, 13 Nov 2021 02:36:17 GMT  
		Size: 108.3 MB (108324832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ee722c391549402cc89928a8fda99f7df93809fb12bf4467b58d5496b1f786`  
		Last Modified: Sat, 13 Nov 2021 02:36:09 GMT  
		Size: 5.3 MB (5324481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8a207dcf3db635875ef8e64ef5d5741fd25973b15c13f17cbaf1f0a3a7d806`  
		Last Modified: Sat, 13 Nov 2021 02:36:08 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18a95327fc1267591ada3258741d12ab945661277db68acaf2704e816863239`  
		Last Modified: Sat, 13 Nov 2021 02:36:08 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63622aee97d1be163f7d1c35b7b6ea3036e969fd4f80e25652cd82d3f79fbceb`  
		Last Modified: Sat, 13 Nov 2021 02:36:08 GMT  
		Size: 4.3 KB (4321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:076c5bb03d8b0640abae6f59d2c56355bb9dc0935fe8c6d21e7d8ad8022f52a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129106956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09910eb8d6e16e8faaab059b68da3d19d0a39cfb325b3bf3adce323801f9fd29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:23:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:23:11 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 13 Nov 2021 06:23:12 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 13 Nov 2021 06:23:13 GMT
ENV GOSU_VER=1.12
# Sat, 13 Nov 2021 06:23:16 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 06:23:55 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 13 Nov 2021 06:24:09 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 13 Nov 2021 06:24:09 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 13 Nov 2021 06:24:13 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 13 Nov 2021 06:24:13 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 13 Nov 2021 06:24:14 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 13 Nov 2021 06:24:16 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 13 Nov 2021 06:24:17 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Sat, 13 Nov 2021 06:24:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:24:18 GMT
CMD ["influxd"]
# Sat, 13 Nov 2021 06:24:19 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 06:24:20 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 13 Nov 2021 06:24:21 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 13 Nov 2021 06:24:22 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 13 Nov 2021 06:24:23 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd8bff15f28e0e2cd2ccb61904ad49022b3252c074dd64a3e7ab49c41ef2e24`  
		Last Modified: Sat, 13 Nov 2021 06:25:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01db43e1eccfeabd1a2a22c07f6303840d1566375fe8cd4ecaa1e15c363f258`  
		Last Modified: Sat, 13 Nov 2021 06:25:07 GMT  
		Size: 9.7 MB (9688653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f189869e04c42c9f2488fc1516e1a567f55da7bff406758600ddbf20835eea7`  
		Last Modified: Sat, 13 Nov 2021 06:25:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e6fbb9a1a27e8801496b32b26fdd9e3a960d9b63124df203e308b391c80c98`  
		Last Modified: Sat, 13 Nov 2021 06:25:03 GMT  
		Size: 896.1 KB (896076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6319331c4cdc62912255f11aae12b1f673f490925bd7da960bb0db5a3ff56a`  
		Last Modified: Sat, 13 Nov 2021 06:25:38 GMT  
		Size: 110.9 MB (110891633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fa72b56e723e675c86ffbf0376877a29f50264c62edab7bd5fa8cb67164979`  
		Last Modified: Sat, 13 Nov 2021 06:25:28 GMT  
		Size: 4.9 MB (4906732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292a3ef1ac3d3eabe42f00620e64da5a236679203f7b9fa2e480fe5d7ecbf5f5`  
		Last Modified: Sat, 13 Nov 2021 06:25:27 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c3c7e6457c3663e71f45fbb7e68be6916d5c99f0e8b960c8d032f7d63e3a93`  
		Last Modified: Sat, 13 Nov 2021 06:25:27 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9585f8dd6f4a8d4debec0c866b84de6a327b0600d39b001d7c8a5448f981ab7`  
		Last Modified: Sat, 13 Nov 2021 06:25:27 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1.1`

```console
$ docker pull influxdb@sha256:f2543c9cc70fd75298a52647d828047ff5fbcd28f19be8a70bf9fb1429b5b6f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1` - linux; amd64

```console
$ docker pull influxdb@sha256:7fd69f4a2c16efc0d5c2863ce2d74d9479dfc458ade2132379b94c28a04913c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182885029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfb4d421b2f653f5e58125af722b2677eb5c4f0fc2a125ef654b8ebd91550f34`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:45:40 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 18 Nov 2021 09:45:40 GMT
ENV GOSU_VER=1.12
# Thu, 18 Nov 2021 09:45:44 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Thu, 18 Nov 2021 09:46:04 GMT
ENV INFLUXDB_VERSION=2.1.1
# Thu, 18 Nov 2021 09:46:12 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 18 Nov 2021 09:46:13 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Thu, 18 Nov 2021 09:46:17 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 18 Nov 2021 09:46:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 18 Nov 2021 09:46:19 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 18 Nov 2021 09:46:19 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 18 Nov 2021 09:46:19 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:46:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:46:20 GMT
CMD ["influxd"]
# Thu, 18 Nov 2021 09:46:20 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 18 Nov 2021 09:46:21 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a603b07c93043ffbd790761bf1cf232dd2763ec10c3ef84ce381390713c99`  
		Last Modified: Thu, 18 Nov 2021 09:50:12 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80de06b69dbd583c55db5aebf57682c087c624d343e0410552603f35686a40`  
		Last Modified: Thu, 18 Nov 2021 09:50:10 GMT  
		Size: 961.0 KB (960988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf4fe7d34889b9b417a1448e1fee0a421bef2c9533916a1f513e8fdfd7baf99`  
		Last Modified: Thu, 18 Nov 2021 09:50:44 GMT  
		Size: 108.3 MB (108324825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8efd2d9a5def9f50aa609b47f8a39012190fb713c9ea285b497c24d014155`  
		Last Modified: Thu, 18 Nov 2021 09:50:36 GMT  
		Size: 5.3 MB (5324484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0d1b444bc9f9096339ec15ce0e4456f4823121b9214b2710b46c82e9147c8d`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f05877070f022483807a8ff887e1619260f8008f79b31053d9d3761acc7174`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c522e98cfb3d02a730692d7aef75148fd190b0192ed98300bed425c66842a9fd`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 4.3 KB (4321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b50ab5a02481210516a7b440d910051c76f1b3fea61255bf554657f7368bb60d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183386413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905455e4cd353ee4e93fd7658b084034e0ad5661373b055973befbc41ae696c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:39:03 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 17 Nov 2021 21:39:04 GMT
ENV GOSU_VER=1.12
# Wed, 17 Nov 2021 21:39:08 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 17 Nov 2021 21:39:43 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 17 Nov 2021 21:40:02 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 17 Nov 2021 21:40:02 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 17 Nov 2021 21:40:07 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 17 Nov 2021 21:40:07 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 17 Nov 2021 21:40:08 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 17 Nov 2021 21:40:10 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 17 Nov 2021 21:40:11 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Wed, 17 Nov 2021 21:40:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:40:12 GMT
CMD ["influxd"]
# Wed, 17 Nov 2021 21:40:13 GMT
EXPOSE 8086
# Wed, 17 Nov 2021 21:40:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 17 Nov 2021 21:40:15 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 17 Nov 2021 21:40:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 17 Nov 2021 21:40:17 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90efb0d865d89e679077061bdca34c60306bacab5579d93a951cd8c31441ec`  
		Last Modified: Wed, 17 Nov 2021 21:41:46 GMT  
		Size: 1.7 KB (1659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f283e1015297042ffd1e94f9753b4ef6b9ce33339509b31d96c13eb7dcd03f82`  
		Last Modified: Wed, 17 Nov 2021 21:41:44 GMT  
		Size: 896.4 KB (896361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d89c50dbb1d05a49120a4b621b6b382d2b29d6304c7f10b0eee084dab7d8dac`  
		Last Modified: Wed, 17 Nov 2021 21:42:16 GMT  
		Size: 110.9 MB (110891616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e6709d1f966cd8da3d817ff591df547559a47204cff841140f0c4f205c829f`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 4.9 MB (4906724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31859363882c3135133fce1a0f41006d7cb4c7ee4a669ea650ba2c541af3b7d5`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec1462a4ae6c9e136f82cbc586a32ea5c2b7089fa2ae02d94cdb2380b2369f`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e7de37831dc0c6521d41919d1fff71b50a3dfe399e29199fcb1e812dad17cb`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1.1-alpine`

```console
$ docker pull influxdb@sha256:a5b34976d4cb3dbc627bfe3d6c08b752ec81586c5c98ac167d84f891c9c7db9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:05af8b4364b19365b722025c16867e0143af044cefd0376566398e91f32c59dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127293784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae8a2276202e4e4296fa44cdedc2ae794d791793d92a4071645957a7dfc4729f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:30:45 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 13 Nov 2021 02:30:47 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 13 Nov 2021 02:30:48 GMT
ENV GOSU_VER=1.12
# Sat, 13 Nov 2021 02:30:53 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 02:31:26 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 13 Nov 2021 02:31:40 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 13 Nov 2021 02:31:41 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 13 Nov 2021 02:31:46 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 13 Nov 2021 02:31:48 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 13 Nov 2021 02:31:48 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 13 Nov 2021 02:31:48 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 13 Nov 2021 02:31:49 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:31:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:31:49 GMT
CMD ["influxd"]
# Sat, 13 Nov 2021 02:31:50 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:31:50 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 13 Nov 2021 02:31:50 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 13 Nov 2021 02:31:51 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 13 Nov 2021 02:31:51 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb48a4c6ea759da391d76004114a5ee8ee41f81dfae508ddfd4c9a2d36f84c`  
		Last Modified: Sat, 13 Nov 2021 02:35:51 GMT  
		Size: 9.9 MB (9854595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f25e434782a05647d6530f2a12eec8118d5df67373eb45fb04033377d5d1b`  
		Last Modified: Sat, 13 Nov 2021 02:35:49 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58f08bf46f1b06d391462bc99b273bb53267c678b30135522996f0390e7865c`  
		Last Modified: Sat, 13 Nov 2021 02:35:47 GMT  
		Size: 960.6 KB (960615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4932f7c0bf2c64c409cdbf559c862abe12f1e35739f607b1f01ef5fbf4d48c8d`  
		Last Modified: Sat, 13 Nov 2021 02:36:17 GMT  
		Size: 108.3 MB (108324832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ee722c391549402cc89928a8fda99f7df93809fb12bf4467b58d5496b1f786`  
		Last Modified: Sat, 13 Nov 2021 02:36:09 GMT  
		Size: 5.3 MB (5324481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8a207dcf3db635875ef8e64ef5d5741fd25973b15c13f17cbaf1f0a3a7d806`  
		Last Modified: Sat, 13 Nov 2021 02:36:08 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18a95327fc1267591ada3258741d12ab945661277db68acaf2704e816863239`  
		Last Modified: Sat, 13 Nov 2021 02:36:08 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63622aee97d1be163f7d1c35b7b6ea3036e969fd4f80e25652cd82d3f79fbceb`  
		Last Modified: Sat, 13 Nov 2021 02:36:08 GMT  
		Size: 4.3 KB (4321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:076c5bb03d8b0640abae6f59d2c56355bb9dc0935fe8c6d21e7d8ad8022f52a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129106956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09910eb8d6e16e8faaab059b68da3d19d0a39cfb325b3bf3adce323801f9fd29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:23:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:23:11 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 13 Nov 2021 06:23:12 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 13 Nov 2021 06:23:13 GMT
ENV GOSU_VER=1.12
# Sat, 13 Nov 2021 06:23:16 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 06:23:55 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 13 Nov 2021 06:24:09 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 13 Nov 2021 06:24:09 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 13 Nov 2021 06:24:13 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 13 Nov 2021 06:24:13 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 13 Nov 2021 06:24:14 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 13 Nov 2021 06:24:16 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 13 Nov 2021 06:24:17 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Sat, 13 Nov 2021 06:24:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:24:18 GMT
CMD ["influxd"]
# Sat, 13 Nov 2021 06:24:19 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 06:24:20 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 13 Nov 2021 06:24:21 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 13 Nov 2021 06:24:22 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 13 Nov 2021 06:24:23 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd8bff15f28e0e2cd2ccb61904ad49022b3252c074dd64a3e7ab49c41ef2e24`  
		Last Modified: Sat, 13 Nov 2021 06:25:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01db43e1eccfeabd1a2a22c07f6303840d1566375fe8cd4ecaa1e15c363f258`  
		Last Modified: Sat, 13 Nov 2021 06:25:07 GMT  
		Size: 9.7 MB (9688653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f189869e04c42c9f2488fc1516e1a567f55da7bff406758600ddbf20835eea7`  
		Last Modified: Sat, 13 Nov 2021 06:25:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e6fbb9a1a27e8801496b32b26fdd9e3a960d9b63124df203e308b391c80c98`  
		Last Modified: Sat, 13 Nov 2021 06:25:03 GMT  
		Size: 896.1 KB (896076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6319331c4cdc62912255f11aae12b1f673f490925bd7da960bb0db5a3ff56a`  
		Last Modified: Sat, 13 Nov 2021 06:25:38 GMT  
		Size: 110.9 MB (110891633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fa72b56e723e675c86ffbf0376877a29f50264c62edab7bd5fa8cb67164979`  
		Last Modified: Sat, 13 Nov 2021 06:25:28 GMT  
		Size: 4.9 MB (4906732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292a3ef1ac3d3eabe42f00620e64da5a236679203f7b9fa2e480fe5d7ecbf5f5`  
		Last Modified: Sat, 13 Nov 2021 06:25:27 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c3c7e6457c3663e71f45fbb7e68be6916d5c99f0e8b960c8d032f7d63e3a93`  
		Last Modified: Sat, 13 Nov 2021 06:25:27 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9585f8dd6f4a8d4debec0c866b84de6a327b0600d39b001d7c8a5448f981ab7`  
		Last Modified: Sat, 13 Nov 2021 06:25:27 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:a5b34976d4cb3dbc627bfe3d6c08b752ec81586c5c98ac167d84f891c9c7db9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:05af8b4364b19365b722025c16867e0143af044cefd0376566398e91f32c59dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127293784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae8a2276202e4e4296fa44cdedc2ae794d791793d92a4071645957a7dfc4729f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:30:45 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 13 Nov 2021 02:30:47 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 13 Nov 2021 02:30:48 GMT
ENV GOSU_VER=1.12
# Sat, 13 Nov 2021 02:30:53 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 02:31:26 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 13 Nov 2021 02:31:40 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 13 Nov 2021 02:31:41 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 13 Nov 2021 02:31:46 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 13 Nov 2021 02:31:48 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 13 Nov 2021 02:31:48 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 13 Nov 2021 02:31:48 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 13 Nov 2021 02:31:49 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:31:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:31:49 GMT
CMD ["influxd"]
# Sat, 13 Nov 2021 02:31:50 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:31:50 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 13 Nov 2021 02:31:50 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 13 Nov 2021 02:31:51 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 13 Nov 2021 02:31:51 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb48a4c6ea759da391d76004114a5ee8ee41f81dfae508ddfd4c9a2d36f84c`  
		Last Modified: Sat, 13 Nov 2021 02:35:51 GMT  
		Size: 9.9 MB (9854595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f25e434782a05647d6530f2a12eec8118d5df67373eb45fb04033377d5d1b`  
		Last Modified: Sat, 13 Nov 2021 02:35:49 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58f08bf46f1b06d391462bc99b273bb53267c678b30135522996f0390e7865c`  
		Last Modified: Sat, 13 Nov 2021 02:35:47 GMT  
		Size: 960.6 KB (960615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4932f7c0bf2c64c409cdbf559c862abe12f1e35739f607b1f01ef5fbf4d48c8d`  
		Last Modified: Sat, 13 Nov 2021 02:36:17 GMT  
		Size: 108.3 MB (108324832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ee722c391549402cc89928a8fda99f7df93809fb12bf4467b58d5496b1f786`  
		Last Modified: Sat, 13 Nov 2021 02:36:09 GMT  
		Size: 5.3 MB (5324481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8a207dcf3db635875ef8e64ef5d5741fd25973b15c13f17cbaf1f0a3a7d806`  
		Last Modified: Sat, 13 Nov 2021 02:36:08 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18a95327fc1267591ada3258741d12ab945661277db68acaf2704e816863239`  
		Last Modified: Sat, 13 Nov 2021 02:36:08 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63622aee97d1be163f7d1c35b7b6ea3036e969fd4f80e25652cd82d3f79fbceb`  
		Last Modified: Sat, 13 Nov 2021 02:36:08 GMT  
		Size: 4.3 KB (4321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:076c5bb03d8b0640abae6f59d2c56355bb9dc0935fe8c6d21e7d8ad8022f52a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129106956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09910eb8d6e16e8faaab059b68da3d19d0a39cfb325b3bf3adce323801f9fd29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:23:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:23:11 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 13 Nov 2021 06:23:12 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 13 Nov 2021 06:23:13 GMT
ENV GOSU_VER=1.12
# Sat, 13 Nov 2021 06:23:16 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 13 Nov 2021 06:23:55 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 13 Nov 2021 06:24:09 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 13 Nov 2021 06:24:09 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 13 Nov 2021 06:24:13 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 13 Nov 2021 06:24:13 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 13 Nov 2021 06:24:14 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 13 Nov 2021 06:24:16 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 13 Nov 2021 06:24:17 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Sat, 13 Nov 2021 06:24:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:24:18 GMT
CMD ["influxd"]
# Sat, 13 Nov 2021 06:24:19 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 06:24:20 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 13 Nov 2021 06:24:21 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 13 Nov 2021 06:24:22 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 13 Nov 2021 06:24:23 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd8bff15f28e0e2cd2ccb61904ad49022b3252c074dd64a3e7ab49c41ef2e24`  
		Last Modified: Sat, 13 Nov 2021 06:25:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01db43e1eccfeabd1a2a22c07f6303840d1566375fe8cd4ecaa1e15c363f258`  
		Last Modified: Sat, 13 Nov 2021 06:25:07 GMT  
		Size: 9.7 MB (9688653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f189869e04c42c9f2488fc1516e1a567f55da7bff406758600ddbf20835eea7`  
		Last Modified: Sat, 13 Nov 2021 06:25:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e6fbb9a1a27e8801496b32b26fdd9e3a960d9b63124df203e308b391c80c98`  
		Last Modified: Sat, 13 Nov 2021 06:25:03 GMT  
		Size: 896.1 KB (896076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6319331c4cdc62912255f11aae12b1f673f490925bd7da960bb0db5a3ff56a`  
		Last Modified: Sat, 13 Nov 2021 06:25:38 GMT  
		Size: 110.9 MB (110891633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fa72b56e723e675c86ffbf0376877a29f50264c62edab7bd5fa8cb67164979`  
		Last Modified: Sat, 13 Nov 2021 06:25:28 GMT  
		Size: 4.9 MB (4906732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292a3ef1ac3d3eabe42f00620e64da5a236679203f7b9fa2e480fe5d7ecbf5f5`  
		Last Modified: Sat, 13 Nov 2021 06:25:27 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c3c7e6457c3663e71f45fbb7e68be6916d5c99f0e8b960c8d032f7d63e3a93`  
		Last Modified: Sat, 13 Nov 2021 06:25:27 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9585f8dd6f4a8d4debec0c866b84de6a327b0600d39b001d7c8a5448f981ab7`  
		Last Modified: Sat, 13 Nov 2021 06:25:27 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:00cdba39140b5f3fe364dc6260d27bd61310bd1383c0639f6297f693c5c0ec11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:ec210def90412bcfd6586f056bf15cfba9a6ae2d83f329f3095914d7202fbada
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117737381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244874bc2bf861b02626382c1d1bd042fd26991a17b503bef6e57853764f3cf1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:44:42 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 18 Nov 2021 09:44:52 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:44:53 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 18 Nov 2021 09:44:53 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:44:53 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:44:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:44:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 18 Nov 2021 09:44:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:44:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08525dea5b6b885656a753a6deef7a71e230e77dafc7f831bd2a4c9f21df5da5`  
		Last Modified: Thu, 18 Nov 2021 09:49:07 GMT  
		Size: 56.7 MB (56708533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57d90367afa71b328b7c1e192c38ec3bc28ec42bfab9b9f002cd21e6f4b455e`  
		Last Modified: Thu, 18 Nov 2021 09:48:58 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e37b0832a2c9fc55d7d0e4b680f6da9e95a0aad7fe83ea36bdb03fb68b0aab`  
		Last Modified: Thu, 18 Nov 2021 09:48:58 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf287206df98f216591a3ae20f6a591c9970835eab55160656bb711f72094f5c`  
		Last Modified: Thu, 18 Nov 2021 09:48:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:9edb5e97912c1a30144b9674f7d24f957a6ee186dad14461da00075d7b3796cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f6c46290f9cfbd9b2fbe6e9f47ab18fe7314c5bd6758ed3c7fde006478ba2a47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60814908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9083f2c434fe802e0c24ff0518282b9c8956c0cb1156626ed29c0cacff0fd794`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:29:25 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 13 Nov 2021 02:29:38 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:29:39 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 13 Nov 2021 02:29:39 GMT
EXPOSE 8086
# Sat, 13 Nov 2021 02:29:39 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:29:39 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:29:39 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 13 Nov 2021 02:29:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:29:40 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b1c62ddbddb14ed511aedfa47a61da93b52f2ebc434d573e6cccdeab360012`  
		Last Modified: Sat, 13 Nov 2021 02:34:40 GMT  
		Size: 56.5 MB (56503786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182dd80d9b0c7757cdea730b9d8438eddf10b2837f1bc4f9555e24a2e16c9f1f`  
		Last Modified: Sat, 13 Nov 2021 02:34:30 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad150614e74207f44ffbcda2bdd6d075d072e5d7e40c18aea4d02bf92012d3`  
		Last Modified: Sat, 13 Nov 2021 02:34:31 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebec01cb49874553e60a3087e07f6ea3be09a5253235bbc016d200b165f0740`  
		Last Modified: Sat, 13 Nov 2021 02:34:30 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:f2543c9cc70fd75298a52647d828047ff5fbcd28f19be8a70bf9fb1429b5b6f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:7fd69f4a2c16efc0d5c2863ce2d74d9479dfc458ade2132379b94c28a04913c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182885029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfb4d421b2f653f5e58125af722b2677eb5c4f0fc2a125ef654b8ebd91550f34`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:45:40 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 18 Nov 2021 09:45:40 GMT
ENV GOSU_VER=1.12
# Thu, 18 Nov 2021 09:45:44 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Thu, 18 Nov 2021 09:46:04 GMT
ENV INFLUXDB_VERSION=2.1.1
# Thu, 18 Nov 2021 09:46:12 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 18 Nov 2021 09:46:13 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Thu, 18 Nov 2021 09:46:17 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 18 Nov 2021 09:46:18 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 18 Nov 2021 09:46:19 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 18 Nov 2021 09:46:19 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 18 Nov 2021 09:46:19 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:46:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:46:20 GMT
CMD ["influxd"]
# Thu, 18 Nov 2021 09:46:20 GMT
EXPOSE 8086
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 18 Nov 2021 09:46:20 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 18 Nov 2021 09:46:21 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a603b07c93043ffbd790761bf1cf232dd2763ec10c3ef84ce381390713c99`  
		Last Modified: Thu, 18 Nov 2021 09:50:12 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80de06b69dbd583c55db5aebf57682c087c624d343e0410552603f35686a40`  
		Last Modified: Thu, 18 Nov 2021 09:50:10 GMT  
		Size: 961.0 KB (960988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf4fe7d34889b9b417a1448e1fee0a421bef2c9533916a1f513e8fdfd7baf99`  
		Last Modified: Thu, 18 Nov 2021 09:50:44 GMT  
		Size: 108.3 MB (108324825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e8efd2d9a5def9f50aa609b47f8a39012190fb713c9ea285b497c24d014155`  
		Last Modified: Thu, 18 Nov 2021 09:50:36 GMT  
		Size: 5.3 MB (5324484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0d1b444bc9f9096339ec15ce0e4456f4823121b9214b2710b46c82e9147c8d`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f05877070f022483807a8ff887e1619260f8008f79b31053d9d3761acc7174`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c522e98cfb3d02a730692d7aef75148fd190b0192ed98300bed425c66842a9fd`  
		Last Modified: Thu, 18 Nov 2021 09:50:35 GMT  
		Size: 4.3 KB (4321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b50ab5a02481210516a7b440d910051c76f1b3fea61255bf554657f7368bb60d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183386413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905455e4cd353ee4e93fd7658b084034e0ad5661373b055973befbc41ae696c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:39:03 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 17 Nov 2021 21:39:04 GMT
ENV GOSU_VER=1.12
# Wed, 17 Nov 2021 21:39:08 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 17 Nov 2021 21:39:43 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 17 Nov 2021 21:40:02 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 17 Nov 2021 21:40:02 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 17 Nov 2021 21:40:07 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 17 Nov 2021 21:40:07 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 17 Nov 2021 21:40:08 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 17 Nov 2021 21:40:10 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 17 Nov 2021 21:40:11 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Wed, 17 Nov 2021 21:40:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:40:12 GMT
CMD ["influxd"]
# Wed, 17 Nov 2021 21:40:13 GMT
EXPOSE 8086
# Wed, 17 Nov 2021 21:40:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 17 Nov 2021 21:40:15 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 17 Nov 2021 21:40:16 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 17 Nov 2021 21:40:17 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90efb0d865d89e679077061bdca34c60306bacab5579d93a951cd8c31441ec`  
		Last Modified: Wed, 17 Nov 2021 21:41:46 GMT  
		Size: 1.7 KB (1659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f283e1015297042ffd1e94f9753b4ef6b9ce33339509b31d96c13eb7dcd03f82`  
		Last Modified: Wed, 17 Nov 2021 21:41:44 GMT  
		Size: 896.4 KB (896361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d89c50dbb1d05a49120a4b621b6b382d2b29d6304c7f10b0eee084dab7d8dac`  
		Last Modified: Wed, 17 Nov 2021 21:42:16 GMT  
		Size: 110.9 MB (110891616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e6709d1f966cd8da3d817ff591df547559a47204cff841140f0c4f205c829f`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 4.9 MB (4906724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31859363882c3135133fce1a0f41006d7cb4c7ee4a669ea650ba2c541af3b7d5`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec1462a4ae6c9e136f82cbc586a32ea5c2b7089fa2ae02d94cdb2380b2369f`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e7de37831dc0c6521d41919d1fff71b50a3dfe399e29199fcb1e812dad17cb`  
		Last Modified: Wed, 17 Nov 2021 21:42:07 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:31500f40ed7a50fdb52e8a0990aea86bd8c0f50814d644754a9f57c35fca7ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:64534669863b8e1414ac4aa65a41d124604e61f8b9ce42b31e297cb2a8d15987
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84443975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6befdf4bac0b404e5ad4274eafa07f36729725f56bef2f3ae11f41259f0cc59d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:43:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:44:42 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 18 Nov 2021 09:45:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 18 Nov 2021 09:45:05 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 18 Nov 2021 09:45:05 GMT
EXPOSE 8091
# Thu, 18 Nov 2021 09:45:05 GMT
VOLUME [/var/lib/influxdb]
# Thu, 18 Nov 2021 09:45:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 18 Nov 2021 09:45:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:45:06 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf57bf976327f4c85d929d1bce1afaf77b4072db460def8408c791295ee8802`  
		Last Modified: Thu, 18 Nov 2021 09:47:32 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64521abd18cf018ab9316be9ab482c503cb3c6b8adeb380319d51c18556be12e`  
		Last Modified: Thu, 18 Nov 2021 09:49:24 GMT  
		Size: 23.4 MB (23416332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82be31c0c04837996a2f891230ea306a73ed63264076a52cff01efbae7234c49`  
		Last Modified: Thu, 18 Nov 2021 09:49:20 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6ebc4c9a6547fd06dd99b1c765524dfdd7a939834caad7a1fac1b01c95d3bd`  
		Last Modified: Thu, 18 Nov 2021 09:49:20 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:4cba27899d3f6324276746cc3d13e113171e58f0cd57b6f778f223d9e5fe1173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:fe5ecca89fb203a0a446abc95062c96221545125968f4f313c50cd821f5a4e7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27602958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:072b66b0c223ce772c78f84a6586e8080a5fb145cf5f1d00eefd6f23846e45cc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 13 Nov 2021 02:28:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 02:29:25 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 13 Nov 2021 02:29:53 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 02:29:53 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 13 Nov 2021 02:29:54 GMT
EXPOSE 8091
# Sat, 13 Nov 2021 02:29:54 GMT
VOLUME [/var/lib/influxdb]
# Sat, 13 Nov 2021 02:29:54 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 13 Nov 2021 02:29:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 02:29:55 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2760002f3a8065fa54c3ac5a0e9ba89494a20c2fe01e85f1e7da19ea5940713`  
		Last Modified: Sat, 13 Nov 2021 02:33:01 GMT  
		Size: 1.5 MB (1486187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7f836dc8033be4020b77d60ac1d010d51d58ce819fd31c8c903dd7bf1d9bed`  
		Last Modified: Sat, 13 Nov 2021 02:35:00 GMT  
		Size: 23.3 MB (23293039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352cd5d07590068a89a6415f0d3923109129dddfdae2762d95cf37b800faed14`  
		Last Modified: Sat, 13 Nov 2021 02:34:56 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a164a9ffc5db6c4dbad8265ed41221745f6094e8223216f516ecfb034794045`  
		Last Modified: Sat, 13 Nov 2021 02:34:56 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
