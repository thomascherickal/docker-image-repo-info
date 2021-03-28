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
-	[`influxdb:1.8.3-data`](#influxdb183-data)
-	[`influxdb:1.8.3-data-alpine`](#influxdb183-data-alpine)
-	[`influxdb:1.8.3-meta`](#influxdb183-meta)
-	[`influxdb:1.8.3-meta-alpine`](#influxdb183-meta-alpine)
-	[`influxdb:1.8.4`](#influxdb184)
-	[`influxdb:1.8.4-alpine`](#influxdb184-alpine)
-	[`influxdb:2.0`](#influxdb20)
-	[`influxdb:2.0-alpine`](#influxdb20-alpine)
-	[`influxdb:2.0.4`](#influxdb204)
-	[`influxdb:2.0.4-alpine`](#influxdb204-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.7`

```console
$ docker pull influxdb@sha256:b43bdb37b4b594119b079497c2b420dfc70ede3218b2f3bbc94c57a05b6a719f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7` - linux; amd64

```console
$ docker pull influxdb@sha256:15547a870842715579e9fe703de4f8b300ab795a628a7aa2092a51e4f2038132
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122298186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8124fa2256c1515dfeb8c4b95ae998b62e6865d7f77a29c5d7547b9241c9844b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:41:35 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 27 Mar 2021 19:41:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 19:41:40 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 19:41:40 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:41:40 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:41:41 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:41:41 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 19:41:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:41:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08826ed24505040d3aea5f8ceb402e11b039029c6699e8d96f27b98942b70f93`  
		Last Modified: Sat, 27 Mar 2021 19:43:50 GMT  
		Size: 61.3 MB (61285144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f6a56d2b5a1b6cc16b11c9a334a81ebc3de86cb6b3aa12c9816924f163e9fc`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762a67aa4e3cefa92495d49e3b661e23e68705490a950972b7478c2612ae5c2`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40e5cfa323d8bc1b31049df33aa833745c7e026b5db51e6518817daa1ebb8ea`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:0e2c7f2c709855afa149d2b6b88f89a5db25f7c8ba6e976e93248bae8ae52d1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113454424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72fb2d7cd322ffe5d0701d0ec03ce4707b0f06b25713a4ba86389526a3bea4d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:16 GMT
ADD file:9ca2a8d5e2b8ba00bb66699e4970399555c20e8f9a4b8afa0b01076b90f0d8e3 in / 
# Fri, 26 Mar 2021 11:22:19 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:31:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 08:56:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 08:56:06 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 27 Mar 2021 08:56:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 08:56:20 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 08:56:21 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 08:56:22 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 08:56:25 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 08:56:25 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 08:56:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 08:56:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:011348b3c4acf7cfad3a8899e3a5f135377a30045eb428e4d759ef7e138740b1`  
		Last Modified: Fri, 26 Mar 2021 11:31:14 GMT  
		Size: 42.1 MB (42119842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cf4418db1e976b0b84122d61cab9eb3bf7616e363a557275308ca2ccc72365`  
		Last Modified: Fri, 26 Mar 2021 13:55:29 GMT  
		Size: 9.9 MB (9939755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe21b354ae04ba513e56799a77ae6f0f57339ee9fec76a66d4e7aaffda99e4`  
		Last Modified: Fri, 26 Mar 2021 13:55:25 GMT  
		Size: 3.9 MB (3921260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a76b27d874885bc2ffc45dfc20cbcd50677bc00b7fc307440a91f88affda671`  
		Last Modified: Sat, 27 Mar 2021 08:57:11 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8875b71e7cac0dfff7fde8778bffcc1bf63deddca0815b8fcc94f6abf3214891`  
		Last Modified: Sat, 27 Mar 2021 08:57:27 GMT  
		Size: 57.5 MB (57468995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5172259d8ae8727f9c4f3d73254e8195d59ebc3729695d759568078a87bda37`  
		Last Modified: Sat, 27 Mar 2021 08:57:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fb58ba62ee75c327b9a2aa6d8d0f4626af5d34ad7693e7f14c65ca847ff78`  
		Last Modified: Sat, 27 Mar 2021 08:57:11 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8d072857b70dee500cbac3e1b73f9a90f9db5d07ab27bda0880e2eb78f9161`  
		Last Modified: Sat, 27 Mar 2021 08:57:11 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:15c88d4f743afbf770f38fb64f59011585691b5668c496dc3d20de8bc4380568
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114683122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a1c3535650017ba24d38309dfc0b207f51e2e66f1686ab2553fbe50e4cbabd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:44:15 GMT
ADD file:cf753fedc426819aa5f93f4ad934479efd8fbf024b408627239b77ddc5223108 in / 
# Fri, 26 Mar 2021 15:44:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:20:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 23:44:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 23:44:25 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 27 Mar 2021 23:44:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 23:44:34 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 23:44:35 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 23:44:35 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 23:44:36 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 23:44:37 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 23:44:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 23:44:39 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1a0736e738921f2c70c8ce48d5ba8b042279c41c41f32a1af43a6cbd299f6d89`  
		Last Modified: Fri, 26 Mar 2021 15:50:55 GMT  
		Size: 43.2 MB (43176405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c963a30dbe4f7f47cba7603121834cb6b6f206d9c25e8a96df41cfd42eab3e`  
		Last Modified: Sat, 27 Mar 2021 04:30:49 GMT  
		Size: 10.2 MB (10201048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97078da83c94ce9db743f96c02e8deaf24987dd4e94aced6c6b5ceb860b8f8ac`  
		Last Modified: Sat, 27 Mar 2021 04:30:47 GMT  
		Size: 4.1 MB (4096666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82837508a33b535f062fbf9f6c7a0129e152fc9b8853870b116ff0de071e6ae`  
		Last Modified: Sat, 27 Mar 2021 23:45:51 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d6fbdd4e063dbf788ecd306489c85f749c6592edbc795d77255d6aa38ca63a`  
		Last Modified: Sat, 27 Mar 2021 23:46:04 GMT  
		Size: 57.2 MB (57204433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2396ea814b582387259b3ec93edcc63d3020bd6f374713f7da750cb941d6ece3`  
		Last Modified: Sat, 27 Mar 2021 23:45:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60252646a495325faea2f0bbf9a300d8de00cc27fd3cc4c14300db0c0ae61bef`  
		Last Modified: Sat, 27 Mar 2021 23:45:51 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07adc3651ecdbfe605beb6586e3c706189036aa5f5c3bf3c7d1dc4f0b5774b4a`  
		Last Modified: Sat, 27 Mar 2021 23:45:51 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-alpine`

```console
$ docker pull influxdb@sha256:0c821cac18c561b4ef40823579492e33e97480333ed967ae0db70e92781f55e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:6ee68b47fdc312baf3fd1dea5d42a41189b2dbafb8e8a0ff7aaeba4c23db74f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65267236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:902a3104dbf4a45aeaf5caf3a01c01c39487390b4eb5db438395129136f0f7c3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:11:21 GMT
ENV INFLUXDB_VERSION=1.7.11
# Fri, 26 Mar 2021 03:11:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:11:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 26 Mar 2021 03:11:30 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:11:31 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:11:31 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:11:32 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 26 Mar 2021 03:11:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:11:32 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbf93b2c7043570c0cb0379868b7dfc53ef6d2d6da8522224db0387ba87bb19`  
		Last Modified: Fri, 26 Mar 2021 03:14:26 GMT  
		Size: 61.0 MB (61034805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f2efb5e94af6d94d305bcd16c7527b5dbb281c2dd96fde0a42365201be2a09`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dc54d2ed7b68f802e67c35f879906d7915af1a41b51e3f2e58e9fc44c76f69`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbf514a81e76c5a92d20c976b346c95668f5552427c5f712b508dfb5254c755`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data`

```console
$ docker pull influxdb@sha256:0f0ab9bbcf436b5fa8196108cf0231b0493d00681c766e43a8ca96cc77d06513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:0afe19d32b073a6702214d5fabd06aaf82541368f9cc4c76139fab52440f0302
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148962130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca111bc075057efa04d035ca0358e456e461bb87a9fdec9d03fdf5ee2165b807`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:41:48 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 27 Mar 2021 19:41:56 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 27 Mar 2021 19:41:56 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 19:41:56 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:41:57 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:41:57 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:41:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 19:41:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:41:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723291eef586dd53f4dd2ffbb3e9425dcf5b3ee34032b6237a8e626a4e1382d1`  
		Last Modified: Sat, 27 Mar 2021 19:44:13 GMT  
		Size: 87.9 MB (87949029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b85cdb0b91bc66a97e206db2973ce35c2ea7e07b3f95b1b859fe08d90645e4e`  
		Last Modified: Sat, 27 Mar 2021 19:44:01 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd8fd74b169093e60acc9ccacad2aed14ee5afb965b6ea351d4b895ce75eded`  
		Last Modified: Sat, 27 Mar 2021 19:44:01 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b923f3a348287a8f5218d37cb6a42b552c382437bfc84ab7126cd86eb0f146cb`  
		Last Modified: Sat, 27 Mar 2021 19:44:01 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data-alpine`

```console
$ docker pull influxdb@sha256:761bc091ddc6444f7e4171d0f7130389bcea7d7e5155cfaa2708c5ae61a94b40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:c4b793b3abcf6705cca7fb4df80b225b47cb44d6f9eafedfb1c81bba9c743ac4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91871361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad5039bd299d5c989f4f742a64921d621518542e42d82d3a69103c6daba0f576`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:11:40 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Fri, 26 Mar 2021 03:11:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:11:53 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 26 Mar 2021 03:11:53 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:11:53 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:11:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:11:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 26 Mar 2021 03:11:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:11:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647100a26b95798661136a92cd612904d49359f99c306be82751034015041fcf`  
		Last Modified: Fri, 26 Mar 2021 03:14:53 GMT  
		Size: 87.6 MB (87638875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427f07360a9756b0355199578277ad635ffb017da23c14e2b8fb7a47f0da1ebd`  
		Last Modified: Fri, 26 Mar 2021 03:14:37 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c637997daad003eadd9eda042740a3dae88bd90809f72b58aa5d30e303ed8c6e`  
		Last Modified: Fri, 26 Mar 2021 03:14:37 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22d2876c852d3421f496130fe0848508a61e381fb0c6221cf00aa08357b4ab6`  
		Last Modified: Fri, 26 Mar 2021 03:14:37 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta`

```console
$ docker pull influxdb@sha256:970a55b6293d63a448f8d2072ea72f8b6c035a315b5a1465f40b31b67cc49135
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:9ccb0532d49b8c909fc579fbc152d6763716a39bdcd9a98716dcbeeaf3aa5846
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.1 MB (84145507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d199a6483424e74a8020f6819b0539655e7c3aebcc61f6f830fe7393c8e98130`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:41:48 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 27 Mar 2021 19:42:07 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 27 Mar 2021 19:42:08 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 27 Mar 2021 19:42:08 GMT
EXPOSE 8091
# Sat, 27 Mar 2021 19:42:08 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:42:08 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:42:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:42:08 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bd69bd822d3eb5788392dcb79846861d9fbb6dee74dbbe1605650f56d53031`  
		Last Modified: Sat, 27 Mar 2021 19:44:33 GMT  
		Size: 23.1 MB (23133614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a6204338e1dbbd1bb5b78eb644c75c85af1fdb763ea77f12f3326a527b838f`  
		Last Modified: Sat, 27 Mar 2021 19:44:25 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f639eff73a27ff66cb3aa922efbff6b98a48069c707e64df067c677119d9c8b1`  
		Last Modified: Sat, 27 Mar 2021 19:44:25 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta-alpine`

```console
$ docker pull influxdb@sha256:35c3a562e4b1c72b0bed3094085a5b33f767f10f019f7d8c8adeadb3e7ae4960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:41dbb90897ac10c905fd36760d9692cbcb6888708b6a18e04dd68c986a66135d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27234280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7f40d34a67464419b440a7d2a19192bfed162df61fbebe3b48f75862dd612b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:11:40 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Fri, 26 Mar 2021 03:12:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:12:09 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 26 Mar 2021 03:12:10 GMT
EXPOSE 8091
# Fri, 26 Mar 2021 03:12:10 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:12:11 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:12:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:12:12 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ceb01385ab0bf1712a886c12133faefe6232f6d47f0743dbd80a4ecec66602`  
		Last Modified: Fri, 26 Mar 2021 03:15:12 GMT  
		Size: 23.0 MB (23002998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c0303c4b3b61339a9da23c86ed7deb8ca668bd5afcda8cb9477c62ba1d3941`  
		Last Modified: Fri, 26 Mar 2021 03:15:07 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f342bf5da7b882ba09eb63b078550422d42f1c8fd27c4f394cfd441ef9cf8e48`  
		Last Modified: Fri, 26 Mar 2021 03:15:06 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11`

```console
$ docker pull influxdb@sha256:b43bdb37b4b594119b079497c2b420dfc70ede3218b2f3bbc94c57a05b6a719f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7.11` - linux; amd64

```console
$ docker pull influxdb@sha256:15547a870842715579e9fe703de4f8b300ab795a628a7aa2092a51e4f2038132
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122298186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8124fa2256c1515dfeb8c4b95ae998b62e6865d7f77a29c5d7547b9241c9844b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:41:35 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 27 Mar 2021 19:41:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 19:41:40 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 19:41:40 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:41:40 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:41:41 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:41:41 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 19:41:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:41:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08826ed24505040d3aea5f8ceb402e11b039029c6699e8d96f27b98942b70f93`  
		Last Modified: Sat, 27 Mar 2021 19:43:50 GMT  
		Size: 61.3 MB (61285144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f6a56d2b5a1b6cc16b11c9a334a81ebc3de86cb6b3aa12c9816924f163e9fc`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762a67aa4e3cefa92495d49e3b661e23e68705490a950972b7478c2612ae5c2`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40e5cfa323d8bc1b31049df33aa833745c7e026b5db51e6518817daa1ebb8ea`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:0e2c7f2c709855afa149d2b6b88f89a5db25f7c8ba6e976e93248bae8ae52d1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113454424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72fb2d7cd322ffe5d0701d0ec03ce4707b0f06b25713a4ba86389526a3bea4d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:16 GMT
ADD file:9ca2a8d5e2b8ba00bb66699e4970399555c20e8f9a4b8afa0b01076b90f0d8e3 in / 
# Fri, 26 Mar 2021 11:22:19 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:31:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 08:56:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 08:56:06 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 27 Mar 2021 08:56:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 08:56:20 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 08:56:21 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 08:56:22 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 08:56:25 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 08:56:25 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 08:56:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 08:56:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:011348b3c4acf7cfad3a8899e3a5f135377a30045eb428e4d759ef7e138740b1`  
		Last Modified: Fri, 26 Mar 2021 11:31:14 GMT  
		Size: 42.1 MB (42119842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cf4418db1e976b0b84122d61cab9eb3bf7616e363a557275308ca2ccc72365`  
		Last Modified: Fri, 26 Mar 2021 13:55:29 GMT  
		Size: 9.9 MB (9939755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe21b354ae04ba513e56799a77ae6f0f57339ee9fec76a66d4e7aaffda99e4`  
		Last Modified: Fri, 26 Mar 2021 13:55:25 GMT  
		Size: 3.9 MB (3921260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a76b27d874885bc2ffc45dfc20cbcd50677bc00b7fc307440a91f88affda671`  
		Last Modified: Sat, 27 Mar 2021 08:57:11 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8875b71e7cac0dfff7fde8778bffcc1bf63deddca0815b8fcc94f6abf3214891`  
		Last Modified: Sat, 27 Mar 2021 08:57:27 GMT  
		Size: 57.5 MB (57468995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5172259d8ae8727f9c4f3d73254e8195d59ebc3729695d759568078a87bda37`  
		Last Modified: Sat, 27 Mar 2021 08:57:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fb58ba62ee75c327b9a2aa6d8d0f4626af5d34ad7693e7f14c65ca847ff78`  
		Last Modified: Sat, 27 Mar 2021 08:57:11 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8d072857b70dee500cbac3e1b73f9a90f9db5d07ab27bda0880e2eb78f9161`  
		Last Modified: Sat, 27 Mar 2021 08:57:11 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:15c88d4f743afbf770f38fb64f59011585691b5668c496dc3d20de8bc4380568
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114683122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a1c3535650017ba24d38309dfc0b207f51e2e66f1686ab2553fbe50e4cbabd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:44:15 GMT
ADD file:cf753fedc426819aa5f93f4ad934479efd8fbf024b408627239b77ddc5223108 in / 
# Fri, 26 Mar 2021 15:44:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:20:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 23:44:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 23:44:25 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 27 Mar 2021 23:44:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 23:44:34 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 23:44:35 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 23:44:35 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 23:44:36 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 23:44:37 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 23:44:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 23:44:39 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1a0736e738921f2c70c8ce48d5ba8b042279c41c41f32a1af43a6cbd299f6d89`  
		Last Modified: Fri, 26 Mar 2021 15:50:55 GMT  
		Size: 43.2 MB (43176405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c963a30dbe4f7f47cba7603121834cb6b6f206d9c25e8a96df41cfd42eab3e`  
		Last Modified: Sat, 27 Mar 2021 04:30:49 GMT  
		Size: 10.2 MB (10201048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97078da83c94ce9db743f96c02e8deaf24987dd4e94aced6c6b5ceb860b8f8ac`  
		Last Modified: Sat, 27 Mar 2021 04:30:47 GMT  
		Size: 4.1 MB (4096666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82837508a33b535f062fbf9f6c7a0129e152fc9b8853870b116ff0de071e6ae`  
		Last Modified: Sat, 27 Mar 2021 23:45:51 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d6fbdd4e063dbf788ecd306489c85f749c6592edbc795d77255d6aa38ca63a`  
		Last Modified: Sat, 27 Mar 2021 23:46:04 GMT  
		Size: 57.2 MB (57204433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2396ea814b582387259b3ec93edcc63d3020bd6f374713f7da750cb941d6ece3`  
		Last Modified: Sat, 27 Mar 2021 23:45:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60252646a495325faea2f0bbf9a300d8de00cc27fd3cc4c14300db0c0ae61bef`  
		Last Modified: Sat, 27 Mar 2021 23:45:51 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07adc3651ecdbfe605beb6586e3c706189036aa5f5c3bf3c7d1dc4f0b5774b4a`  
		Last Modified: Sat, 27 Mar 2021 23:45:51 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-alpine`

```console
$ docker pull influxdb@sha256:0c821cac18c561b4ef40823579492e33e97480333ed967ae0db70e92781f55e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:6ee68b47fdc312baf3fd1dea5d42a41189b2dbafb8e8a0ff7aaeba4c23db74f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65267236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:902a3104dbf4a45aeaf5caf3a01c01c39487390b4eb5db438395129136f0f7c3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:11:21 GMT
ENV INFLUXDB_VERSION=1.7.11
# Fri, 26 Mar 2021 03:11:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:11:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 26 Mar 2021 03:11:30 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:11:31 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:11:31 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:11:32 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 26 Mar 2021 03:11:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:11:32 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbf93b2c7043570c0cb0379868b7dfc53ef6d2d6da8522224db0387ba87bb19`  
		Last Modified: Fri, 26 Mar 2021 03:14:26 GMT  
		Size: 61.0 MB (61034805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f2efb5e94af6d94d305bcd16c7527b5dbb281c2dd96fde0a42365201be2a09`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dc54d2ed7b68f802e67c35f879906d7915af1a41b51e3f2e58e9fc44c76f69`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbf514a81e76c5a92d20c976b346c95668f5552427c5f712b508dfb5254c755`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data`

```console
$ docker pull influxdb@sha256:0f0ab9bbcf436b5fa8196108cf0231b0493d00681c766e43a8ca96cc77d06513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:0afe19d32b073a6702214d5fabd06aaf82541368f9cc4c76139fab52440f0302
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148962130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca111bc075057efa04d035ca0358e456e461bb87a9fdec9d03fdf5ee2165b807`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:41:48 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 27 Mar 2021 19:41:56 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 27 Mar 2021 19:41:56 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 19:41:56 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:41:57 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:41:57 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:41:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 19:41:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:41:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723291eef586dd53f4dd2ffbb3e9425dcf5b3ee34032b6237a8e626a4e1382d1`  
		Last Modified: Sat, 27 Mar 2021 19:44:13 GMT  
		Size: 87.9 MB (87949029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b85cdb0b91bc66a97e206db2973ce35c2ea7e07b3f95b1b859fe08d90645e4e`  
		Last Modified: Sat, 27 Mar 2021 19:44:01 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd8fd74b169093e60acc9ccacad2aed14ee5afb965b6ea351d4b895ce75eded`  
		Last Modified: Sat, 27 Mar 2021 19:44:01 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b923f3a348287a8f5218d37cb6a42b552c382437bfc84ab7126cd86eb0f146cb`  
		Last Modified: Sat, 27 Mar 2021 19:44:01 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data-alpine`

```console
$ docker pull influxdb@sha256:761bc091ddc6444f7e4171d0f7130389bcea7d7e5155cfaa2708c5ae61a94b40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:c4b793b3abcf6705cca7fb4df80b225b47cb44d6f9eafedfb1c81bba9c743ac4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91871361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad5039bd299d5c989f4f742a64921d621518542e42d82d3a69103c6daba0f576`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:11:40 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Fri, 26 Mar 2021 03:11:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:11:53 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 26 Mar 2021 03:11:53 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:11:53 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:11:54 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:11:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 26 Mar 2021 03:11:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:11:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647100a26b95798661136a92cd612904d49359f99c306be82751034015041fcf`  
		Last Modified: Fri, 26 Mar 2021 03:14:53 GMT  
		Size: 87.6 MB (87638875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427f07360a9756b0355199578277ad635ffb017da23c14e2b8fb7a47f0da1ebd`  
		Last Modified: Fri, 26 Mar 2021 03:14:37 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c637997daad003eadd9eda042740a3dae88bd90809f72b58aa5d30e303ed8c6e`  
		Last Modified: Fri, 26 Mar 2021 03:14:37 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22d2876c852d3421f496130fe0848508a61e381fb0c6221cf00aa08357b4ab6`  
		Last Modified: Fri, 26 Mar 2021 03:14:37 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta`

```console
$ docker pull influxdb@sha256:970a55b6293d63a448f8d2072ea72f8b6c035a315b5a1465f40b31b67cc49135
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:9ccb0532d49b8c909fc579fbc152d6763716a39bdcd9a98716dcbeeaf3aa5846
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.1 MB (84145507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d199a6483424e74a8020f6819b0539655e7c3aebcc61f6f830fe7393c8e98130`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:41:48 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 27 Mar 2021 19:42:07 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 27 Mar 2021 19:42:08 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 27 Mar 2021 19:42:08 GMT
EXPOSE 8091
# Sat, 27 Mar 2021 19:42:08 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:42:08 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:42:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:42:08 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bd69bd822d3eb5788392dcb79846861d9fbb6dee74dbbe1605650f56d53031`  
		Last Modified: Sat, 27 Mar 2021 19:44:33 GMT  
		Size: 23.1 MB (23133614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a6204338e1dbbd1bb5b78eb644c75c85af1fdb763ea77f12f3326a527b838f`  
		Last Modified: Sat, 27 Mar 2021 19:44:25 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f639eff73a27ff66cb3aa922efbff6b98a48069c707e64df067c677119d9c8b1`  
		Last Modified: Sat, 27 Mar 2021 19:44:25 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta-alpine`

```console
$ docker pull influxdb@sha256:35c3a562e4b1c72b0bed3094085a5b33f767f10f019f7d8c8adeadb3e7ae4960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:41dbb90897ac10c905fd36760d9692cbcb6888708b6a18e04dd68c986a66135d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27234280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7f40d34a67464419b440a7d2a19192bfed162df61fbebe3b48f75862dd612b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:11:40 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Fri, 26 Mar 2021 03:12:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:12:09 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 26 Mar 2021 03:12:10 GMT
EXPOSE 8091
# Fri, 26 Mar 2021 03:12:10 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:12:11 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:12:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:12:12 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ceb01385ab0bf1712a886c12133faefe6232f6d47f0743dbd80a4ecec66602`  
		Last Modified: Fri, 26 Mar 2021 03:15:12 GMT  
		Size: 23.0 MB (23002998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c0303c4b3b61339a9da23c86ed7deb8ca668bd5afcda8cb9477c62ba1d3941`  
		Last Modified: Fri, 26 Mar 2021 03:15:07 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f342bf5da7b882ba09eb63b078550422d42f1c8fd27c4f394cfd441ef9cf8e48`  
		Last Modified: Fri, 26 Mar 2021 03:15:06 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:0006cb3fbf80c4e26edbcf2a8e7589268b4d5444771f2d8f5d28949020bd6b6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:f4f942eb3ea83b2421ad015adbcdb6ae6e4b745f01a172f1d364acef198c7917
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125979793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bcbb4510bb6e1d9f81f11af066a55f794e7360386b72e16a2d9ddd4c3a3789f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:42:15 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 27 Mar 2021 19:42:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 19:42:19 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 19:42:19 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:42:20 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:42:20 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:42:20 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 19:42:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:42:20 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1351cfa2d8f288aadef6cdae0d057bea8d770bf9b345ea3d33054c241b77454`  
		Last Modified: Sat, 27 Mar 2021 19:44:53 GMT  
		Size: 65.0 MB (64966751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef9510052e6afd7139ae7f52bf0e24fc3a3ccfc21395cd756b28c68f9de0ec2`  
		Last Modified: Sat, 27 Mar 2021 19:44:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0b65c8d322d339dd253fc231a1ece8278e52fec28f8b4715839290deff9182`  
		Last Modified: Sat, 27 Mar 2021 19:44:44 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5e2695363a2a491bb33730fbdca330ac1a32a61f7bc81bf11923b26ba60bf`  
		Last Modified: Sat, 27 Mar 2021 19:44:44 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:b2a633080728ee73ab6d35f487a9324156d2ef3d09f801109d4a50fa5d92fae4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117045421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632c0976c1e0c0b1a26228df6c0b0b2b4ca41f77fa8c25887e70a3eae6a5ddc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:16 GMT
ADD file:9ca2a8d5e2b8ba00bb66699e4970399555c20e8f9a4b8afa0b01076b90f0d8e3 in / 
# Fri, 26 Mar 2021 11:22:19 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:31:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 08:56:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 08:56:37 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 27 Mar 2021 08:56:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 08:56:48 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 08:56:49 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 08:56:50 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 08:56:52 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 08:56:53 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 08:56:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 08:56:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:011348b3c4acf7cfad3a8899e3a5f135377a30045eb428e4d759ef7e138740b1`  
		Last Modified: Fri, 26 Mar 2021 11:31:14 GMT  
		Size: 42.1 MB (42119842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cf4418db1e976b0b84122d61cab9eb3bf7616e363a557275308ca2ccc72365`  
		Last Modified: Fri, 26 Mar 2021 13:55:29 GMT  
		Size: 9.9 MB (9939755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe21b354ae04ba513e56799a77ae6f0f57339ee9fec76a66d4e7aaffda99e4`  
		Last Modified: Fri, 26 Mar 2021 13:55:25 GMT  
		Size: 3.9 MB (3921260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a76b27d874885bc2ffc45dfc20cbcd50677bc00b7fc307440a91f88affda671`  
		Last Modified: Sat, 27 Mar 2021 08:57:11 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b22d14638c820ff4ee51aa643ae39bebee4c48098048a6291431ed116a3b03`  
		Last Modified: Sat, 27 Mar 2021 08:57:50 GMT  
		Size: 61.1 MB (61059991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca08119190393db9a6bad1cc9f9572bfd2e77b781722b6a9f72ad0a9e9d57d8`  
		Last Modified: Sat, 27 Mar 2021 08:57:35 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8249437d7dd03dcc3c2204efc7402c5a058587f6445aee53324afbcf6b04b3`  
		Last Modified: Sat, 27 Mar 2021 08:57:35 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a7cbf1b2d7a9034316b9daa1952c07a648a6a3f0524203efdd79f12312018a`  
		Last Modified: Sat, 27 Mar 2021 08:57:35 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:98434363d0960bd74559af56115ce8d64f23218af598d54e17a03feaf01f2c29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.1 MB (118107889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c18863041b1ea1f4d40e6ce09726617bab6b8c8fc7bbcad6442fe70b630bfad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:44:15 GMT
ADD file:cf753fedc426819aa5f93f4ad934479efd8fbf024b408627239b77ddc5223108 in / 
# Fri, 26 Mar 2021 15:44:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:20:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 23:44:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 23:44:45 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 27 Mar 2021 23:44:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 23:44:55 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 23:44:55 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 23:44:56 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 23:44:57 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 23:44:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 23:44:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 23:44:59 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1a0736e738921f2c70c8ce48d5ba8b042279c41c41f32a1af43a6cbd299f6d89`  
		Last Modified: Fri, 26 Mar 2021 15:50:55 GMT  
		Size: 43.2 MB (43176405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c963a30dbe4f7f47cba7603121834cb6b6f206d9c25e8a96df41cfd42eab3e`  
		Last Modified: Sat, 27 Mar 2021 04:30:49 GMT  
		Size: 10.2 MB (10201048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97078da83c94ce9db743f96c02e8deaf24987dd4e94aced6c6b5ceb860b8f8ac`  
		Last Modified: Sat, 27 Mar 2021 04:30:47 GMT  
		Size: 4.1 MB (4096666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82837508a33b535f062fbf9f6c7a0129e152fc9b8853870b116ff0de071e6ae`  
		Last Modified: Sat, 27 Mar 2021 23:45:51 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2deb2335efb63fed6fbf03238fe64f9aae832ce783a300b84c6172c500421a`  
		Last Modified: Sat, 27 Mar 2021 23:46:25 GMT  
		Size: 60.6 MB (60629200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89a16aa81b804076695cfaafa32e82b3be4c2019789cc3494e40bcd40f04a9b`  
		Last Modified: Sat, 27 Mar 2021 23:46:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5bb6d3cf6aa43e364aedeb7eebea9454719c081f6c6066d891dd10d3c9ace6`  
		Last Modified: Sat, 27 Mar 2021 23:46:11 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f28a37e32b1c6d6455ed2f15ee6f155175fe15c0dfb7328e6da920ad46d40d`  
		Last Modified: Sat, 27 Mar 2021 23:46:12 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:e83e54460cdf862b646753c189d9412dd07b574188f92e2a69b5a31a0ae1811f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:51438137c77e3d9815094b3353312a0554de632ae1e11e181686ea297a4a090f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68939083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7148c7a887b389d22015abf7bfa4a8442eb1cc275e7aef6f2745d29f2c96b61`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:12:21 GMT
ENV INFLUXDB_VERSION=1.8.4
# Fri, 26 Mar 2021 03:12:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:12:32 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 26 Mar 2021 03:12:32 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:12:33 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:12:33 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:12:33 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 26 Mar 2021 03:12:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:12:34 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e49c4772ca21c6efb0b4ff0db2c0d6b1a36d30cd7aa1f8eb4b30e4dd107e7bd`  
		Last Modified: Fri, 26 Mar 2021 03:15:36 GMT  
		Size: 64.7 MB (64706652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362cd378e24eef36e481aa3dd7959a8f9a1ed43c6f547933911e4f197dcf9cd8`  
		Last Modified: Fri, 26 Mar 2021 03:15:25 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49b9b787bf5c540d9209736e478228899e5c59ab4910a13975b0d809e8e61df`  
		Last Modified: Fri, 26 Mar 2021 03:15:27 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781c55e5b6a229e6b2301e3c3c178917ed1a2afa9c930f3ff635fce76f8accd9`  
		Last Modified: Fri, 26 Mar 2021 03:15:27 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:49df54670928c2b6bf4f5e6f876a5d64c1da4d50e17876d35c085129ba4748ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:c3a0449009aa160b6064006604e18f3d2302efbe058c513148f1f4eb9d3b7e82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126809506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d8c4ed955ac913c5664059f1bd548e886723c5904e4bb4d10d206c853df2c1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:42:27 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 27 Mar 2021 19:42:33 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 27 Mar 2021 19:42:34 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 19:42:34 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:42:34 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:42:34 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:42:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 19:42:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:42:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2eb14e13429979e0834c04294d2acc452529f55ee033f3a342c78e9e932989`  
		Last Modified: Sat, 27 Mar 2021 19:45:13 GMT  
		Size: 65.8 MB (65796406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756ce47003b15c0ba3abc8c713409f23cf46f17813ac98d9f305962cb1f26bdd`  
		Last Modified: Sat, 27 Mar 2021 19:45:05 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd6c14a1740aad3a96771b407f95e651e5f8807806743bddaab40f3e12956a1`  
		Last Modified: Sat, 27 Mar 2021 19:45:04 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a9e4ff0aa80fea19687371a113b46d2d4b85e2a3fbb34241bafd1594be5a8e`  
		Last Modified: Sat, 27 Mar 2021 19:45:04 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:346bbcd11b148f2f16a2d57983651d041bc4e76b7be37a229761cb98be9ea1a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:66d7e13c7398cb7b7b24ab11e93b8fc6df9810ce3caf5454f48af573ec4f8e44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69773212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dcc8ef82e51b0b1ca496f666455d47ffa16db0e4724182b9181a5a3a7085450`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:12:43 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 26 Mar 2021 03:12:54 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:12:55 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 26 Mar 2021 03:12:55 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:12:56 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:12:56 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:12:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 26 Mar 2021 03:12:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:12:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f93414593c5ed20572ce823821624c75d9c5b5cce7c386fe9445ff53fdcffd`  
		Last Modified: Fri, 26 Mar 2021 03:16:08 GMT  
		Size: 65.5 MB (65540725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7c5e0669089ff1561d42a79ad8d07770a2dba46aa881d978db4f8f6d4d4122`  
		Last Modified: Fri, 26 Mar 2021 03:15:50 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf828604c316ad2013675a8600f3a995e439fea0d8b58ce7f7dc4829645059e`  
		Last Modified: Fri, 26 Mar 2021 03:15:50 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e0af7932850ca1be3799cfc676e181d8fba9118492598f7971c4702217c0e0`  
		Last Modified: Fri, 26 Mar 2021 03:15:50 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:816f00e011ce1f123d2e79f77348b0fb7d89f29cf5089abeafd8738ff8291e6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ceedd9bb063cdb578ea9fe0b01e36bdbf04089c24f3fce51a7fea9d0a88e265c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83878159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a487cd34d550cc77f9217861618de8d698339758318d82eab265cfced3add71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:42:27 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 27 Mar 2021 19:42:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 27 Mar 2021 19:42:45 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 27 Mar 2021 19:42:45 GMT
EXPOSE 8091
# Sat, 27 Mar 2021 19:42:45 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:42:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:42:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:42:46 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf46fcf44385964742efc7341a1f94dab172bfd2c0bac74da4351c0a3074d1b`  
		Last Modified: Sat, 27 Mar 2021 19:45:37 GMT  
		Size: 22.9 MB (22866264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151881c42bede65ec63b01bd46e79e8ae0741dadbef07302b65f8c7c8af5d1f2`  
		Last Modified: Sat, 27 Mar 2021 19:45:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa39e1af5349913b80fa2dd7819056fd0d450677a3486570ecbe685bbe39ed6`  
		Last Modified: Sat, 27 Mar 2021 19:45:34 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:025343db4f4725ad6fca8cefab25de95f35f2ee1f7edfcb3df2912266946cfee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b3d7c436989265bf677e7b4b8cc2917b39cf23db010d5b21f509d5819bf8c659
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26966664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3552651a28dd4ac2d063768f7ac74647bb09599913a3b1a764b3b5195e0d222`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:12:43 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 26 Mar 2021 03:13:09 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:13:09 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 26 Mar 2021 03:13:09 GMT
EXPOSE 8091
# Fri, 26 Mar 2021 03:13:09 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:13:09 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:13:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:13:10 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679043eb8b78af43a53255aaa9ed0573069cf4a7fe0244b00c22bb689168e8c`  
		Last Modified: Fri, 26 Mar 2021 03:16:32 GMT  
		Size: 22.7 MB (22735384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f24fb9849144e6672b70615e2c9a10ce060177818a687eda336bfb685811f9`  
		Last Modified: Fri, 26 Mar 2021 03:16:28 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a37293518b1401d50def8f45962801ec2568ccb4148145240934a9c0c21b2`  
		Last Modified: Fri, 26 Mar 2021 03:16:29 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-data`

```console
$ docker pull influxdb@sha256:49df54670928c2b6bf4f5e6f876a5d64c1da4d50e17876d35c085129ba4748ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-data` - linux; amd64

```console
$ docker pull influxdb@sha256:c3a0449009aa160b6064006604e18f3d2302efbe058c513148f1f4eb9d3b7e82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126809506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d8c4ed955ac913c5664059f1bd548e886723c5904e4bb4d10d206c853df2c1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:42:27 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 27 Mar 2021 19:42:33 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 27 Mar 2021 19:42:34 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 19:42:34 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:42:34 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:42:34 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:42:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 19:42:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:42:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2eb14e13429979e0834c04294d2acc452529f55ee033f3a342c78e9e932989`  
		Last Modified: Sat, 27 Mar 2021 19:45:13 GMT  
		Size: 65.8 MB (65796406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756ce47003b15c0ba3abc8c713409f23cf46f17813ac98d9f305962cb1f26bdd`  
		Last Modified: Sat, 27 Mar 2021 19:45:05 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd6c14a1740aad3a96771b407f95e651e5f8807806743bddaab40f3e12956a1`  
		Last Modified: Sat, 27 Mar 2021 19:45:04 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a9e4ff0aa80fea19687371a113b46d2d4b85e2a3fbb34241bafd1594be5a8e`  
		Last Modified: Sat, 27 Mar 2021 19:45:04 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-data-alpine`

```console
$ docker pull influxdb@sha256:346bbcd11b148f2f16a2d57983651d041bc4e76b7be37a229761cb98be9ea1a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:66d7e13c7398cb7b7b24ab11e93b8fc6df9810ce3caf5454f48af573ec4f8e44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69773212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dcc8ef82e51b0b1ca496f666455d47ffa16db0e4724182b9181a5a3a7085450`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:12:43 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 26 Mar 2021 03:12:54 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:12:55 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 26 Mar 2021 03:12:55 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:12:56 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:12:56 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:12:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 26 Mar 2021 03:12:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:12:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f93414593c5ed20572ce823821624c75d9c5b5cce7c386fe9445ff53fdcffd`  
		Last Modified: Fri, 26 Mar 2021 03:16:08 GMT  
		Size: 65.5 MB (65540725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7c5e0669089ff1561d42a79ad8d07770a2dba46aa881d978db4f8f6d4d4122`  
		Last Modified: Fri, 26 Mar 2021 03:15:50 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf828604c316ad2013675a8600f3a995e439fea0d8b58ce7f7dc4829645059e`  
		Last Modified: Fri, 26 Mar 2021 03:15:50 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e0af7932850ca1be3799cfc676e181d8fba9118492598f7971c4702217c0e0`  
		Last Modified: Fri, 26 Mar 2021 03:15:50 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-meta`

```console
$ docker pull influxdb@sha256:816f00e011ce1f123d2e79f77348b0fb7d89f29cf5089abeafd8738ff8291e6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ceedd9bb063cdb578ea9fe0b01e36bdbf04089c24f3fce51a7fea9d0a88e265c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83878159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a487cd34d550cc77f9217861618de8d698339758318d82eab265cfced3add71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:42:27 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 27 Mar 2021 19:42:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 27 Mar 2021 19:42:45 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 27 Mar 2021 19:42:45 GMT
EXPOSE 8091
# Sat, 27 Mar 2021 19:42:45 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:42:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:42:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:42:46 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf46fcf44385964742efc7341a1f94dab172bfd2c0bac74da4351c0a3074d1b`  
		Last Modified: Sat, 27 Mar 2021 19:45:37 GMT  
		Size: 22.9 MB (22866264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151881c42bede65ec63b01bd46e79e8ae0741dadbef07302b65f8c7c8af5d1f2`  
		Last Modified: Sat, 27 Mar 2021 19:45:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa39e1af5349913b80fa2dd7819056fd0d450677a3486570ecbe685bbe39ed6`  
		Last Modified: Sat, 27 Mar 2021 19:45:34 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-meta-alpine`

```console
$ docker pull influxdb@sha256:025343db4f4725ad6fca8cefab25de95f35f2ee1f7edfcb3df2912266946cfee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b3d7c436989265bf677e7b4b8cc2917b39cf23db010d5b21f509d5819bf8c659
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26966664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3552651a28dd4ac2d063768f7ac74647bb09599913a3b1a764b3b5195e0d222`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:12:43 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 26 Mar 2021 03:13:09 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:13:09 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 26 Mar 2021 03:13:09 GMT
EXPOSE 8091
# Fri, 26 Mar 2021 03:13:09 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:13:09 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:13:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:13:10 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679043eb8b78af43a53255aaa9ed0573069cf4a7fe0244b00c22bb689168e8c`  
		Last Modified: Fri, 26 Mar 2021 03:16:32 GMT  
		Size: 22.7 MB (22735384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f24fb9849144e6672b70615e2c9a10ce060177818a687eda336bfb685811f9`  
		Last Modified: Fri, 26 Mar 2021 03:16:28 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a37293518b1401d50def8f45962801ec2568ccb4148145240934a9c0c21b2`  
		Last Modified: Fri, 26 Mar 2021 03:16:29 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.4`

```console
$ docker pull influxdb@sha256:0006cb3fbf80c4e26edbcf2a8e7589268b4d5444771f2d8f5d28949020bd6b6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.4` - linux; amd64

```console
$ docker pull influxdb@sha256:f4f942eb3ea83b2421ad015adbcdb6ae6e4b745f01a172f1d364acef198c7917
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125979793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bcbb4510bb6e1d9f81f11af066a55f794e7360386b72e16a2d9ddd4c3a3789f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:42:15 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 27 Mar 2021 19:42:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 19:42:19 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 19:42:19 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:42:20 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:42:20 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:42:20 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 19:42:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:42:20 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1351cfa2d8f288aadef6cdae0d057bea8d770bf9b345ea3d33054c241b77454`  
		Last Modified: Sat, 27 Mar 2021 19:44:53 GMT  
		Size: 65.0 MB (64966751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef9510052e6afd7139ae7f52bf0e24fc3a3ccfc21395cd756b28c68f9de0ec2`  
		Last Modified: Sat, 27 Mar 2021 19:44:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0b65c8d322d339dd253fc231a1ece8278e52fec28f8b4715839290deff9182`  
		Last Modified: Sat, 27 Mar 2021 19:44:44 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5e2695363a2a491bb33730fbdca330ac1a32a61f7bc81bf11923b26ba60bf`  
		Last Modified: Sat, 27 Mar 2021 19:44:44 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.4` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:b2a633080728ee73ab6d35f487a9324156d2ef3d09f801109d4a50fa5d92fae4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117045421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632c0976c1e0c0b1a26228df6c0b0b2b4ca41f77fa8c25887e70a3eae6a5ddc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:16 GMT
ADD file:9ca2a8d5e2b8ba00bb66699e4970399555c20e8f9a4b8afa0b01076b90f0d8e3 in / 
# Fri, 26 Mar 2021 11:22:19 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:31:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 08:56:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 08:56:37 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 27 Mar 2021 08:56:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 08:56:48 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 08:56:49 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 08:56:50 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 08:56:52 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 08:56:53 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 08:56:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 08:56:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:011348b3c4acf7cfad3a8899e3a5f135377a30045eb428e4d759ef7e138740b1`  
		Last Modified: Fri, 26 Mar 2021 11:31:14 GMT  
		Size: 42.1 MB (42119842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cf4418db1e976b0b84122d61cab9eb3bf7616e363a557275308ca2ccc72365`  
		Last Modified: Fri, 26 Mar 2021 13:55:29 GMT  
		Size: 9.9 MB (9939755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe21b354ae04ba513e56799a77ae6f0f57339ee9fec76a66d4e7aaffda99e4`  
		Last Modified: Fri, 26 Mar 2021 13:55:25 GMT  
		Size: 3.9 MB (3921260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a76b27d874885bc2ffc45dfc20cbcd50677bc00b7fc307440a91f88affda671`  
		Last Modified: Sat, 27 Mar 2021 08:57:11 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b22d14638c820ff4ee51aa643ae39bebee4c48098048a6291431ed116a3b03`  
		Last Modified: Sat, 27 Mar 2021 08:57:50 GMT  
		Size: 61.1 MB (61059991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca08119190393db9a6bad1cc9f9572bfd2e77b781722b6a9f72ad0a9e9d57d8`  
		Last Modified: Sat, 27 Mar 2021 08:57:35 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8249437d7dd03dcc3c2204efc7402c5a058587f6445aee53324afbcf6b04b3`  
		Last Modified: Sat, 27 Mar 2021 08:57:35 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a7cbf1b2d7a9034316b9daa1952c07a648a6a3f0524203efdd79f12312018a`  
		Last Modified: Sat, 27 Mar 2021 08:57:35 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.4` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:98434363d0960bd74559af56115ce8d64f23218af598d54e17a03feaf01f2c29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.1 MB (118107889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c18863041b1ea1f4d40e6ce09726617bab6b8c8fc7bbcad6442fe70b630bfad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:44:15 GMT
ADD file:cf753fedc426819aa5f93f4ad934479efd8fbf024b408627239b77ddc5223108 in / 
# Fri, 26 Mar 2021 15:44:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:20:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:21:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 23:44:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 23:44:45 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 27 Mar 2021 23:44:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 27 Mar 2021 23:44:55 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 23:44:55 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 23:44:56 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 23:44:57 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 27 Mar 2021 23:44:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 23:44:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 23:44:59 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1a0736e738921f2c70c8ce48d5ba8b042279c41c41f32a1af43a6cbd299f6d89`  
		Last Modified: Fri, 26 Mar 2021 15:50:55 GMT  
		Size: 43.2 MB (43176405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c963a30dbe4f7f47cba7603121834cb6b6f206d9c25e8a96df41cfd42eab3e`  
		Last Modified: Sat, 27 Mar 2021 04:30:49 GMT  
		Size: 10.2 MB (10201048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97078da83c94ce9db743f96c02e8deaf24987dd4e94aced6c6b5ceb860b8f8ac`  
		Last Modified: Sat, 27 Mar 2021 04:30:47 GMT  
		Size: 4.1 MB (4096666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82837508a33b535f062fbf9f6c7a0129e152fc9b8853870b116ff0de071e6ae`  
		Last Modified: Sat, 27 Mar 2021 23:45:51 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2deb2335efb63fed6fbf03238fe64f9aae832ce783a300b84c6172c500421a`  
		Last Modified: Sat, 27 Mar 2021 23:46:25 GMT  
		Size: 60.6 MB (60629200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89a16aa81b804076695cfaafa32e82b3be4c2019789cc3494e40bcd40f04a9b`  
		Last Modified: Sat, 27 Mar 2021 23:46:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5bb6d3cf6aa43e364aedeb7eebea9454719c081f6c6066d891dd10d3c9ace6`  
		Last Modified: Sat, 27 Mar 2021 23:46:11 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f28a37e32b1c6d6455ed2f15ee6f155175fe15c0dfb7328e6da920ad46d40d`  
		Last Modified: Sat, 27 Mar 2021 23:46:12 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.4-alpine`

```console
$ docker pull influxdb@sha256:e83e54460cdf862b646753c189d9412dd07b574188f92e2a69b5a31a0ae1811f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.4-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:51438137c77e3d9815094b3353312a0554de632ae1e11e181686ea297a4a090f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68939083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7148c7a887b389d22015abf7bfa4a8442eb1cc275e7aef6f2745d29f2c96b61`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:12:21 GMT
ENV INFLUXDB_VERSION=1.8.4
# Fri, 26 Mar 2021 03:12:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:12:32 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 26 Mar 2021 03:12:32 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:12:33 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:12:33 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:12:33 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 26 Mar 2021 03:12:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:12:34 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e49c4772ca21c6efb0b4ff0db2c0d6b1a36d30cd7aa1f8eb4b30e4dd107e7bd`  
		Last Modified: Fri, 26 Mar 2021 03:15:36 GMT  
		Size: 64.7 MB (64706652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362cd378e24eef36e481aa3dd7959a8f9a1ed43c6f547933911e4f197dcf9cd8`  
		Last Modified: Fri, 26 Mar 2021 03:15:25 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49b9b787bf5c540d9209736e478228899e5c59ab4910a13975b0d809e8e61df`  
		Last Modified: Fri, 26 Mar 2021 03:15:27 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781c55e5b6a229e6b2301e3c3c178917ed1a2afa9c930f3ff635fce76f8accd9`  
		Last Modified: Fri, 26 Mar 2021 03:15:27 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0`

```console
$ docker pull influxdb@sha256:98e0e481b47c9086f449eeb794d0c3d864ee484e57b11295d0f10d057798efc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:7f4c7691433d5455780d74ea1061a984e47169698f084ec5043bbaf3efd0bed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116198833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe204f506d07ab41501c5828535a7d1fc4cc7ce31d3d680535eb1bb6a2c57f57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:41 GMT
ADD file:89234bb2f86c7eb890235a48904d1c9898a8d287a525c4fe5698d4a04cdd8f12 in / 
# Fri, 26 Mar 2021 15:20:42 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:53:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:53:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:42:52 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 27 Mar 2021 19:42:52 GMT
ENV GOSU_VER=1.12
# Sat, 27 Mar 2021 19:42:56 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 27 Mar 2021 19:42:56 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 27 Mar 2021 19:43:01 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 27 Mar 2021 19:43:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 27 Mar 2021 19:43:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 27 Mar 2021 19:43:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 27 Mar 2021 19:43:03 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 27 Mar 2021 19:43:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:43:03 GMT
CMD ["influxd"]
# Sat, 27 Mar 2021 19:43:03 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:43:04 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 27 Mar 2021 19:43:04 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:8bf9c589d5f9475f1fcc050e02308d6b4eeb86eab7752ef948a13693e81a6aaa`  
		Last Modified: Fri, 26 Mar 2021 15:27:11 GMT  
		Size: 50.4 MB (50400278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c70e46d8b5f0e1d77797b7a0565b7a316bd8c7c024f5cca82592128af142dac`  
		Last Modified: Sat, 27 Mar 2021 06:03:41 GMT  
		Size: 7.8 MB (7832558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea848ad42f0d1676b3a0ce709208ba3fa154cd53370c50e7cf8e580c63d96ae0`  
		Last Modified: Sat, 27 Mar 2021 06:03:41 GMT  
		Size: 10.0 MB (9997159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4128f8ffcfe88fa178747d01d5c846d89ead7ab1fc142393b6922ee67c738860`  
		Last Modified: Sat, 27 Mar 2021 19:45:54 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a15f27e7d4a43ee07d7ef9507feba5477654eb08434617c542301fe42e91f4`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 961.0 KB (960997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722b33d1fcf2c7c8983b6501e8b48c0c2a7e57c20af4299cc4b46ef49bb45240`  
		Last Modified: Sat, 27 Mar 2021 19:45:59 GMT  
		Size: 47.0 MB (47001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef92080dd590e5240fac0b0e4b40816a7e6b065f510820ed3573334f7db839dc`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a2b28bbb868bf65a3302e43612bdf81c8bcb24f1739c4c4118467d5e3b4745`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632b97ef2f701d5f8845a445f42726970effa736f526b95ed3b8505afd1e86ea`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 3.9 KB (3924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:510cda6d33e5d1b0dc0acc65f360bde18a6c87e5be3054ab6a92e9b3bdf6dc5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112181670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeded243649f4e8c2c71421273a8f59d6786c759926cf9b6bd8d141f183d9ded`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:27 GMT
ADD file:536306ac674764a6a921b71adcbb4440797b916a0583b9270cd1565d62642e4d in / 
# Fri, 26 Mar 2021 15:41:30 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:14:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 23:45:08 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 27 Mar 2021 23:45:09 GMT
ENV GOSU_VER=1.12
# Sat, 27 Mar 2021 23:45:14 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 27 Mar 2021 23:45:15 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 27 Mar 2021 23:45:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 27 Mar 2021 23:45:25 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 27 Mar 2021 23:45:26 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 27 Mar 2021 23:45:26 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 27 Mar 2021 23:45:27 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 27 Mar 2021 23:45:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 23:45:29 GMT
CMD ["influxd"]
# Sat, 27 Mar 2021 23:45:29 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 23:45:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 27 Mar 2021 23:45:31 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:383261dafcc4f63ecae5f2d661d1ef8d0a5e1c9f4b1f12285115baca7d101d5a`  
		Last Modified: Fri, 26 Mar 2021 15:48:21 GMT  
		Size: 49.2 MB (49196215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a8073d5d993eeeb13d2b5798a56220bed01add2f8e543d1a68cf5bdeb13b3a`  
		Last Modified: Sat, 27 Mar 2021 04:28:03 GMT  
		Size: 7.7 MB (7694449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e04ac5d1463667a0a3b2db65c9975df4dda175b8d5442808d4b141537d5531`  
		Last Modified: Sat, 27 Mar 2021 04:28:03 GMT  
		Size: 10.0 MB (9984376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6055553a6c354d4736d36059e317aaf6c573521ce1a6f381252d2418a5b22cc5`  
		Last Modified: Sat, 27 Mar 2021 23:46:33 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491bbbdd45059f5769d2bb0bdb837ba80cac2724f6e6965922ed4158c9cba265`  
		Last Modified: Sat, 27 Mar 2021 23:46:32 GMT  
		Size: 896.4 KB (896377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665c874e986f062b2080ad17ceecb5870089fc85c6dd9e508dfc13be08d8ce3a`  
		Last Modified: Sat, 27 Mar 2021 23:46:42 GMT  
		Size: 44.4 MB (44403983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87dac5cb3dad1c12cfc0defda563435433ac0c36a68beed10027b91647fd0ce`  
		Last Modified: Sat, 27 Mar 2021 23:46:31 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697255ec667025f6221eb0d566cf9686b98aceb00f4d74b95c9edfb49acbae88`  
		Last Modified: Sat, 27 Mar 2021 23:46:31 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd163f394f9a890244bb2aee5ba3eae7c4be3a8d883726e42ba5b73784fba60`  
		Last Modified: Sat, 27 Mar 2021 23:46:31 GMT  
		Size: 3.9 KB (3923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0-alpine`

```console
$ docker pull influxdb@sha256:788884e8414acbfbeb0d0f8f578e9c0aac740ddcd24d701c4b78ddfcfae8dff4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b3dfad1350afce2d5a41727554f086bd78c8e1ffe7276e8cb366c05e69bf0ded
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60480731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a7a4bce161d9f95a9549ac2f9070c8010956d327b1802c547e55b32f7226192`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 03:13:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:13:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Fri, 26 Mar 2021 03:13:20 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 26 Mar 2021 03:13:21 GMT
ENV GOSU_VER=1.12
# Fri, 26 Mar 2021 03:13:24 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 03:13:24 GMT
ENV INFLUXDB_VERSION=2.0.4
# Fri, 26 Mar 2021 03:13:30 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Fri, 26 Mar 2021 03:13:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 26 Mar 2021 03:13:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 26 Mar 2021 03:13:32 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 26 Mar 2021 03:13:33 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Fri, 26 Mar 2021 03:13:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:13:33 GMT
CMD ["influxd"]
# Fri, 26 Mar 2021 03:13:33 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:13:34 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 26 Mar 2021 03:13:34 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa281e10be7a89f184e97022e75c8c01c0ad3f620eae5fb72cbf6a602bf049`  
		Last Modified: Fri, 26 Mar 2021 03:16:51 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074119a82c783c5a05e5506af7d3f59e1290c61670f5dc70618546217be37b2f`  
		Last Modified: Fri, 26 Mar 2021 03:16:54 GMT  
		Size: 9.7 MB (9701006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c522dd4d682875e489a658dc5560f25c5c40d8bc56bd678068a638bc13671e`  
		Last Modified: Fri, 26 Mar 2021 03:16:52 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba83209f362ad7a28474ea87f439ef1054e73fcb27a1a4d6145e4e43e2ea2bef`  
		Last Modified: Fri, 26 Mar 2021 03:16:49 GMT  
		Size: 960.6 KB (960613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d7789c0190c16b3c5980c8b8022a1206bdf2a42ad0a7c2ce0fbbbc4e9b0594`  
		Last Modified: Fri, 26 Mar 2021 03:16:59 GMT  
		Size: 47.0 MB (47001561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce3f5555653045056dde56d8f9d02878ee41650427102a9f25137904c740846`  
		Last Modified: Fri, 26 Mar 2021 03:16:49 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d6a79194a3e08c3ec8d3634b97cfe5d325538407e73d36aa893a9247dac88a`  
		Last Modified: Fri, 26 Mar 2021 03:16:48 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffed1b38d1928f16a58cb543b059eef16c78ab1fa8b624f96e6d340e519eb378`  
		Last Modified: Fri, 26 Mar 2021 03:16:48 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:7928311c9723a1f254433212d7ca2cfb220d7e721e46fdd26dd29f9aab5cdc04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57559543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456e1e2b23d556b5706a62ccfa1c10b4be02feb03ff083b277ad0090d3eb23f0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:23:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 01:23:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Fri, 26 Mar 2021 01:23:09 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 26 Mar 2021 01:23:10 GMT
ENV GOSU_VER=1.12
# Fri, 26 Mar 2021 01:23:15 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 01:23:16 GMT
ENV INFLUXDB_VERSION=2.0.4
# Fri, 26 Mar 2021 01:23:28 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Fri, 26 Mar 2021 01:23:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 26 Mar 2021 01:23:33 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 26 Mar 2021 01:23:34 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 26 Mar 2021 01:23:35 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Fri, 26 Mar 2021 01:23:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 01:23:37 GMT
CMD ["influxd"]
# Fri, 26 Mar 2021 01:23:38 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 01:23:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 26 Mar 2021 01:23:41 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c66d69085d55364acf545d06662277eb28e02a15db508ac63bfd310936ea3f`  
		Last Modified: Fri, 26 Mar 2021 01:24:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95ce2d86e2205748adfcceeb2cdcadbc4249252c7cc922a0a8127bdf794252`  
		Last Modified: Fri, 26 Mar 2021 01:24:13 GMT  
		Size: 9.5 MB (9541704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a5e616b579edbd75019eca934256e78a0e406eca03c11f2739bbbb539edc17`  
		Last Modified: Fri, 26 Mar 2021 01:24:10 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d177e27b48bc295428d040dc34524b55ea25ee2002b8904d97fbd65852cc8df`  
		Last Modified: Fri, 26 Mar 2021 01:24:08 GMT  
		Size: 896.1 KB (896105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f76c521cf1774059c5681e83c614efefa8da20f51e0e5c103a525aaacbd399`  
		Last Modified: Fri, 26 Mar 2021 01:24:19 GMT  
		Size: 44.4 MB (44403961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726a41b76f732152b387beec268a2db057684743fd4153a6584cd57841792f6f`  
		Last Modified: Fri, 26 Mar 2021 01:24:08 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459db7f28e6a9b7b3b411e1dfb427cfff89b73317ebfeaa96f1f9d57f3090979`  
		Last Modified: Fri, 26 Mar 2021 01:24:08 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf97a3b4eadc65f76552446f69698daa18702dac2333106d10665d2f77f4d4`  
		Last Modified: Fri, 26 Mar 2021 01:24:07 GMT  
		Size: 3.9 KB (3925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.4`

```console
$ docker pull influxdb@sha256:98e0e481b47c9086f449eeb794d0c3d864ee484e57b11295d0f10d057798efc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.4` - linux; amd64

```console
$ docker pull influxdb@sha256:7f4c7691433d5455780d74ea1061a984e47169698f084ec5043bbaf3efd0bed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116198833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe204f506d07ab41501c5828535a7d1fc4cc7ce31d3d680535eb1bb6a2c57f57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:41 GMT
ADD file:89234bb2f86c7eb890235a48904d1c9898a8d287a525c4fe5698d4a04cdd8f12 in / 
# Fri, 26 Mar 2021 15:20:42 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:53:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:53:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:42:52 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 27 Mar 2021 19:42:52 GMT
ENV GOSU_VER=1.12
# Sat, 27 Mar 2021 19:42:56 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 27 Mar 2021 19:42:56 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 27 Mar 2021 19:43:01 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 27 Mar 2021 19:43:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 27 Mar 2021 19:43:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 27 Mar 2021 19:43:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 27 Mar 2021 19:43:03 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 27 Mar 2021 19:43:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:43:03 GMT
CMD ["influxd"]
# Sat, 27 Mar 2021 19:43:03 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:43:04 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 27 Mar 2021 19:43:04 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:8bf9c589d5f9475f1fcc050e02308d6b4eeb86eab7752ef948a13693e81a6aaa`  
		Last Modified: Fri, 26 Mar 2021 15:27:11 GMT  
		Size: 50.4 MB (50400278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c70e46d8b5f0e1d77797b7a0565b7a316bd8c7c024f5cca82592128af142dac`  
		Last Modified: Sat, 27 Mar 2021 06:03:41 GMT  
		Size: 7.8 MB (7832558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea848ad42f0d1676b3a0ce709208ba3fa154cd53370c50e7cf8e580c63d96ae0`  
		Last Modified: Sat, 27 Mar 2021 06:03:41 GMT  
		Size: 10.0 MB (9997159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4128f8ffcfe88fa178747d01d5c846d89ead7ab1fc142393b6922ee67c738860`  
		Last Modified: Sat, 27 Mar 2021 19:45:54 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a15f27e7d4a43ee07d7ef9507feba5477654eb08434617c542301fe42e91f4`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 961.0 KB (960997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722b33d1fcf2c7c8983b6501e8b48c0c2a7e57c20af4299cc4b46ef49bb45240`  
		Last Modified: Sat, 27 Mar 2021 19:45:59 GMT  
		Size: 47.0 MB (47001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef92080dd590e5240fac0b0e4b40816a7e6b065f510820ed3573334f7db839dc`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a2b28bbb868bf65a3302e43612bdf81c8bcb24f1739c4c4118467d5e3b4745`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632b97ef2f701d5f8845a445f42726970effa736f526b95ed3b8505afd1e86ea`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 3.9 KB (3924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.4` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:510cda6d33e5d1b0dc0acc65f360bde18a6c87e5be3054ab6a92e9b3bdf6dc5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112181670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeded243649f4e8c2c71421273a8f59d6786c759926cf9b6bd8d141f183d9ded`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:27 GMT
ADD file:536306ac674764a6a921b71adcbb4440797b916a0583b9270cd1565d62642e4d in / 
# Fri, 26 Mar 2021 15:41:30 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:14:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 23:45:08 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 27 Mar 2021 23:45:09 GMT
ENV GOSU_VER=1.12
# Sat, 27 Mar 2021 23:45:14 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 27 Mar 2021 23:45:15 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 27 Mar 2021 23:45:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 27 Mar 2021 23:45:25 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 27 Mar 2021 23:45:26 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 27 Mar 2021 23:45:26 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 27 Mar 2021 23:45:27 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 27 Mar 2021 23:45:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 23:45:29 GMT
CMD ["influxd"]
# Sat, 27 Mar 2021 23:45:29 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 23:45:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 27 Mar 2021 23:45:31 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:383261dafcc4f63ecae5f2d661d1ef8d0a5e1c9f4b1f12285115baca7d101d5a`  
		Last Modified: Fri, 26 Mar 2021 15:48:21 GMT  
		Size: 49.2 MB (49196215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a8073d5d993eeeb13d2b5798a56220bed01add2f8e543d1a68cf5bdeb13b3a`  
		Last Modified: Sat, 27 Mar 2021 04:28:03 GMT  
		Size: 7.7 MB (7694449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e04ac5d1463667a0a3b2db65c9975df4dda175b8d5442808d4b141537d5531`  
		Last Modified: Sat, 27 Mar 2021 04:28:03 GMT  
		Size: 10.0 MB (9984376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6055553a6c354d4736d36059e317aaf6c573521ce1a6f381252d2418a5b22cc5`  
		Last Modified: Sat, 27 Mar 2021 23:46:33 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491bbbdd45059f5769d2bb0bdb837ba80cac2724f6e6965922ed4158c9cba265`  
		Last Modified: Sat, 27 Mar 2021 23:46:32 GMT  
		Size: 896.4 KB (896377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665c874e986f062b2080ad17ceecb5870089fc85c6dd9e508dfc13be08d8ce3a`  
		Last Modified: Sat, 27 Mar 2021 23:46:42 GMT  
		Size: 44.4 MB (44403983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87dac5cb3dad1c12cfc0defda563435433ac0c36a68beed10027b91647fd0ce`  
		Last Modified: Sat, 27 Mar 2021 23:46:31 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697255ec667025f6221eb0d566cf9686b98aceb00f4d74b95c9edfb49acbae88`  
		Last Modified: Sat, 27 Mar 2021 23:46:31 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd163f394f9a890244bb2aee5ba3eae7c4be3a8d883726e42ba5b73784fba60`  
		Last Modified: Sat, 27 Mar 2021 23:46:31 GMT  
		Size: 3.9 KB (3923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.4-alpine`

```console
$ docker pull influxdb@sha256:788884e8414acbfbeb0d0f8f578e9c0aac740ddcd24d701c4b78ddfcfae8dff4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.4-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b3dfad1350afce2d5a41727554f086bd78c8e1ffe7276e8cb366c05e69bf0ded
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60480731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a7a4bce161d9f95a9549ac2f9070c8010956d327b1802c547e55b32f7226192`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 03:13:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:13:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Fri, 26 Mar 2021 03:13:20 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 26 Mar 2021 03:13:21 GMT
ENV GOSU_VER=1.12
# Fri, 26 Mar 2021 03:13:24 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 03:13:24 GMT
ENV INFLUXDB_VERSION=2.0.4
# Fri, 26 Mar 2021 03:13:30 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Fri, 26 Mar 2021 03:13:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 26 Mar 2021 03:13:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 26 Mar 2021 03:13:32 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 26 Mar 2021 03:13:33 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Fri, 26 Mar 2021 03:13:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:13:33 GMT
CMD ["influxd"]
# Fri, 26 Mar 2021 03:13:33 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:13:34 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 26 Mar 2021 03:13:34 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa281e10be7a89f184e97022e75c8c01c0ad3f620eae5fb72cbf6a602bf049`  
		Last Modified: Fri, 26 Mar 2021 03:16:51 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074119a82c783c5a05e5506af7d3f59e1290c61670f5dc70618546217be37b2f`  
		Last Modified: Fri, 26 Mar 2021 03:16:54 GMT  
		Size: 9.7 MB (9701006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c522dd4d682875e489a658dc5560f25c5c40d8bc56bd678068a638bc13671e`  
		Last Modified: Fri, 26 Mar 2021 03:16:52 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba83209f362ad7a28474ea87f439ef1054e73fcb27a1a4d6145e4e43e2ea2bef`  
		Last Modified: Fri, 26 Mar 2021 03:16:49 GMT  
		Size: 960.6 KB (960613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d7789c0190c16b3c5980c8b8022a1206bdf2a42ad0a7c2ce0fbbbc4e9b0594`  
		Last Modified: Fri, 26 Mar 2021 03:16:59 GMT  
		Size: 47.0 MB (47001561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce3f5555653045056dde56d8f9d02878ee41650427102a9f25137904c740846`  
		Last Modified: Fri, 26 Mar 2021 03:16:49 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d6a79194a3e08c3ec8d3634b97cfe5d325538407e73d36aa893a9247dac88a`  
		Last Modified: Fri, 26 Mar 2021 03:16:48 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffed1b38d1928f16a58cb543b059eef16c78ab1fa8b624f96e6d340e519eb378`  
		Last Modified: Fri, 26 Mar 2021 03:16:48 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.4-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:7928311c9723a1f254433212d7ca2cfb220d7e721e46fdd26dd29f9aab5cdc04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57559543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456e1e2b23d556b5706a62ccfa1c10b4be02feb03ff083b277ad0090d3eb23f0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:23:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 01:23:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Fri, 26 Mar 2021 01:23:09 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 26 Mar 2021 01:23:10 GMT
ENV GOSU_VER=1.12
# Fri, 26 Mar 2021 01:23:15 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 01:23:16 GMT
ENV INFLUXDB_VERSION=2.0.4
# Fri, 26 Mar 2021 01:23:28 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Fri, 26 Mar 2021 01:23:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 26 Mar 2021 01:23:33 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 26 Mar 2021 01:23:34 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 26 Mar 2021 01:23:35 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Fri, 26 Mar 2021 01:23:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 01:23:37 GMT
CMD ["influxd"]
# Fri, 26 Mar 2021 01:23:38 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 01:23:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 26 Mar 2021 01:23:41 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c66d69085d55364acf545d06662277eb28e02a15db508ac63bfd310936ea3f`  
		Last Modified: Fri, 26 Mar 2021 01:24:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95ce2d86e2205748adfcceeb2cdcadbc4249252c7cc922a0a8127bdf794252`  
		Last Modified: Fri, 26 Mar 2021 01:24:13 GMT  
		Size: 9.5 MB (9541704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a5e616b579edbd75019eca934256e78a0e406eca03c11f2739bbbb539edc17`  
		Last Modified: Fri, 26 Mar 2021 01:24:10 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d177e27b48bc295428d040dc34524b55ea25ee2002b8904d97fbd65852cc8df`  
		Last Modified: Fri, 26 Mar 2021 01:24:08 GMT  
		Size: 896.1 KB (896105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f76c521cf1774059c5681e83c614efefa8da20f51e0e5c103a525aaacbd399`  
		Last Modified: Fri, 26 Mar 2021 01:24:19 GMT  
		Size: 44.4 MB (44403961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726a41b76f732152b387beec268a2db057684743fd4153a6584cd57841792f6f`  
		Last Modified: Fri, 26 Mar 2021 01:24:08 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459db7f28e6a9b7b3b411e1dfb427cfff89b73317ebfeaa96f1f9d57f3090979`  
		Last Modified: Fri, 26 Mar 2021 01:24:08 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf97a3b4eadc65f76552446f69698daa18702dac2333106d10665d2f77f4d4`  
		Last Modified: Fri, 26 Mar 2021 01:24:07 GMT  
		Size: 3.9 KB (3925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:788884e8414acbfbeb0d0f8f578e9c0aac740ddcd24d701c4b78ddfcfae8dff4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b3dfad1350afce2d5a41727554f086bd78c8e1ffe7276e8cb366c05e69bf0ded
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60480731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a7a4bce161d9f95a9549ac2f9070c8010956d327b1802c547e55b32f7226192`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 03:13:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:13:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Fri, 26 Mar 2021 03:13:20 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 26 Mar 2021 03:13:21 GMT
ENV GOSU_VER=1.12
# Fri, 26 Mar 2021 03:13:24 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 03:13:24 GMT
ENV INFLUXDB_VERSION=2.0.4
# Fri, 26 Mar 2021 03:13:30 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Fri, 26 Mar 2021 03:13:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 26 Mar 2021 03:13:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 26 Mar 2021 03:13:32 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 26 Mar 2021 03:13:33 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Fri, 26 Mar 2021 03:13:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:13:33 GMT
CMD ["influxd"]
# Fri, 26 Mar 2021 03:13:33 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:13:34 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 26 Mar 2021 03:13:34 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa281e10be7a89f184e97022e75c8c01c0ad3f620eae5fb72cbf6a602bf049`  
		Last Modified: Fri, 26 Mar 2021 03:16:51 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074119a82c783c5a05e5506af7d3f59e1290c61670f5dc70618546217be37b2f`  
		Last Modified: Fri, 26 Mar 2021 03:16:54 GMT  
		Size: 9.7 MB (9701006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c522dd4d682875e489a658dc5560f25c5c40d8bc56bd678068a638bc13671e`  
		Last Modified: Fri, 26 Mar 2021 03:16:52 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba83209f362ad7a28474ea87f439ef1054e73fcb27a1a4d6145e4e43e2ea2bef`  
		Last Modified: Fri, 26 Mar 2021 03:16:49 GMT  
		Size: 960.6 KB (960613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d7789c0190c16b3c5980c8b8022a1206bdf2a42ad0a7c2ce0fbbbc4e9b0594`  
		Last Modified: Fri, 26 Mar 2021 03:16:59 GMT  
		Size: 47.0 MB (47001561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce3f5555653045056dde56d8f9d02878ee41650427102a9f25137904c740846`  
		Last Modified: Fri, 26 Mar 2021 03:16:49 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d6a79194a3e08c3ec8d3634b97cfe5d325538407e73d36aa893a9247dac88a`  
		Last Modified: Fri, 26 Mar 2021 03:16:48 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffed1b38d1928f16a58cb543b059eef16c78ab1fa8b624f96e6d340e519eb378`  
		Last Modified: Fri, 26 Mar 2021 03:16:48 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:7928311c9723a1f254433212d7ca2cfb220d7e721e46fdd26dd29f9aab5cdc04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57559543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456e1e2b23d556b5706a62ccfa1c10b4be02feb03ff083b277ad0090d3eb23f0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:23:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 01:23:06 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Fri, 26 Mar 2021 01:23:09 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 26 Mar 2021 01:23:10 GMT
ENV GOSU_VER=1.12
# Fri, 26 Mar 2021 01:23:15 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 01:23:16 GMT
ENV INFLUXDB_VERSION=2.0.4
# Fri, 26 Mar 2021 01:23:28 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Fri, 26 Mar 2021 01:23:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 26 Mar 2021 01:23:33 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 26 Mar 2021 01:23:34 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 26 Mar 2021 01:23:35 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Fri, 26 Mar 2021 01:23:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 01:23:37 GMT
CMD ["influxd"]
# Fri, 26 Mar 2021 01:23:38 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 01:23:39 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 26 Mar 2021 01:23:41 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c66d69085d55364acf545d06662277eb28e02a15db508ac63bfd310936ea3f`  
		Last Modified: Fri, 26 Mar 2021 01:24:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a95ce2d86e2205748adfcceeb2cdcadbc4249252c7cc922a0a8127bdf794252`  
		Last Modified: Fri, 26 Mar 2021 01:24:13 GMT  
		Size: 9.5 MB (9541704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a5e616b579edbd75019eca934256e78a0e406eca03c11f2739bbbb539edc17`  
		Last Modified: Fri, 26 Mar 2021 01:24:10 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d177e27b48bc295428d040dc34524b55ea25ee2002b8904d97fbd65852cc8df`  
		Last Modified: Fri, 26 Mar 2021 01:24:08 GMT  
		Size: 896.1 KB (896105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f76c521cf1774059c5681e83c614efefa8da20f51e0e5c103a525aaacbd399`  
		Last Modified: Fri, 26 Mar 2021 01:24:19 GMT  
		Size: 44.4 MB (44403961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726a41b76f732152b387beec268a2db057684743fd4153a6584cd57841792f6f`  
		Last Modified: Fri, 26 Mar 2021 01:24:08 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459db7f28e6a9b7b3b411e1dfb427cfff89b73317ebfeaa96f1f9d57f3090979`  
		Last Modified: Fri, 26 Mar 2021 01:24:08 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf97a3b4eadc65f76552446f69698daa18702dac2333106d10665d2f77f4d4`  
		Last Modified: Fri, 26 Mar 2021 01:24:07 GMT  
		Size: 3.9 KB (3925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:49df54670928c2b6bf4f5e6f876a5d64c1da4d50e17876d35c085129ba4748ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:c3a0449009aa160b6064006604e18f3d2302efbe058c513148f1f4eb9d3b7e82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126809506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d8c4ed955ac913c5664059f1bd548e886723c5904e4bb4d10d206c853df2c1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:42:27 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 27 Mar 2021 19:42:33 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 27 Mar 2021 19:42:34 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 27 Mar 2021 19:42:34 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:42:34 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:42:34 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:42:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 27 Mar 2021 19:42:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:42:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2eb14e13429979e0834c04294d2acc452529f55ee033f3a342c78e9e932989`  
		Last Modified: Sat, 27 Mar 2021 19:45:13 GMT  
		Size: 65.8 MB (65796406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756ce47003b15c0ba3abc8c713409f23cf46f17813ac98d9f305962cb1f26bdd`  
		Last Modified: Sat, 27 Mar 2021 19:45:05 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd6c14a1740aad3a96771b407f95e651e5f8807806743bddaab40f3e12956a1`  
		Last Modified: Sat, 27 Mar 2021 19:45:04 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a9e4ff0aa80fea19687371a113b46d2d4b85e2a3fbb34241bafd1594be5a8e`  
		Last Modified: Sat, 27 Mar 2021 19:45:04 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:346bbcd11b148f2f16a2d57983651d041bc4e76b7be37a229761cb98be9ea1a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:66d7e13c7398cb7b7b24ab11e93b8fc6df9810ce3caf5454f48af573ec4f8e44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69773212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dcc8ef82e51b0b1ca496f666455d47ffa16db0e4724182b9181a5a3a7085450`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:12:43 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 26 Mar 2021 03:12:54 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:12:55 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 26 Mar 2021 03:12:55 GMT
EXPOSE 8086
# Fri, 26 Mar 2021 03:12:56 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:12:56 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:12:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 26 Mar 2021 03:12:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:12:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f93414593c5ed20572ce823821624c75d9c5b5cce7c386fe9445ff53fdcffd`  
		Last Modified: Fri, 26 Mar 2021 03:16:08 GMT  
		Size: 65.5 MB (65540725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7c5e0669089ff1561d42a79ad8d07770a2dba46aa881d978db4f8f6d4d4122`  
		Last Modified: Fri, 26 Mar 2021 03:15:50 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf828604c316ad2013675a8600f3a995e439fea0d8b58ce7f7dc4829645059e`  
		Last Modified: Fri, 26 Mar 2021 03:15:50 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e0af7932850ca1be3799cfc676e181d8fba9118492598f7971c4702217c0e0`  
		Last Modified: Fri, 26 Mar 2021 03:15:50 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:98e0e481b47c9086f449eeb794d0c3d864ee484e57b11295d0f10d057798efc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:7f4c7691433d5455780d74ea1061a984e47169698f084ec5043bbaf3efd0bed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116198833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe204f506d07ab41501c5828535a7d1fc4cc7ce31d3d680535eb1bb6a2c57f57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:41 GMT
ADD file:89234bb2f86c7eb890235a48904d1c9898a8d287a525c4fe5698d4a04cdd8f12 in / 
# Fri, 26 Mar 2021 15:20:42 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:53:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:53:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:42:52 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 27 Mar 2021 19:42:52 GMT
ENV GOSU_VER=1.12
# Sat, 27 Mar 2021 19:42:56 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 27 Mar 2021 19:42:56 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 27 Mar 2021 19:43:01 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 27 Mar 2021 19:43:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 27 Mar 2021 19:43:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 27 Mar 2021 19:43:03 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 27 Mar 2021 19:43:03 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 27 Mar 2021 19:43:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:43:03 GMT
CMD ["influxd"]
# Sat, 27 Mar 2021 19:43:03 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 19:43:04 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 27 Mar 2021 19:43:04 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:8bf9c589d5f9475f1fcc050e02308d6b4eeb86eab7752ef948a13693e81a6aaa`  
		Last Modified: Fri, 26 Mar 2021 15:27:11 GMT  
		Size: 50.4 MB (50400278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c70e46d8b5f0e1d77797b7a0565b7a316bd8c7c024f5cca82592128af142dac`  
		Last Modified: Sat, 27 Mar 2021 06:03:41 GMT  
		Size: 7.8 MB (7832558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea848ad42f0d1676b3a0ce709208ba3fa154cd53370c50e7cf8e580c63d96ae0`  
		Last Modified: Sat, 27 Mar 2021 06:03:41 GMT  
		Size: 10.0 MB (9997159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4128f8ffcfe88fa178747d01d5c846d89ead7ab1fc142393b6922ee67c738860`  
		Last Modified: Sat, 27 Mar 2021 19:45:54 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a15f27e7d4a43ee07d7ef9507feba5477654eb08434617c542301fe42e91f4`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 961.0 KB (960997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722b33d1fcf2c7c8983b6501e8b48c0c2a7e57c20af4299cc4b46ef49bb45240`  
		Last Modified: Sat, 27 Mar 2021 19:45:59 GMT  
		Size: 47.0 MB (47001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef92080dd590e5240fac0b0e4b40816a7e6b065f510820ed3573334f7db839dc`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a2b28bbb868bf65a3302e43612bdf81c8bcb24f1739c4c4118467d5e3b4745`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632b97ef2f701d5f8845a445f42726970effa736f526b95ed3b8505afd1e86ea`  
		Last Modified: Sat, 27 Mar 2021 19:45:52 GMT  
		Size: 3.9 KB (3924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:510cda6d33e5d1b0dc0acc65f360bde18a6c87e5be3054ab6a92e9b3bdf6dc5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112181670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeded243649f4e8c2c71421273a8f59d6786c759926cf9b6bd8d141f183d9ded`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:27 GMT
ADD file:536306ac674764a6a921b71adcbb4440797b916a0583b9270cd1565d62642e4d in / 
# Fri, 26 Mar 2021 15:41:30 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:14:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:14:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 23:45:08 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 27 Mar 2021 23:45:09 GMT
ENV GOSU_VER=1.12
# Sat, 27 Mar 2021 23:45:14 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 27 Mar 2021 23:45:15 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 27 Mar 2021 23:45:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 27 Mar 2021 23:45:25 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 27 Mar 2021 23:45:26 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 27 Mar 2021 23:45:26 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 27 Mar 2021 23:45:27 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 27 Mar 2021 23:45:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 23:45:29 GMT
CMD ["influxd"]
# Sat, 27 Mar 2021 23:45:29 GMT
EXPOSE 8086
# Sat, 27 Mar 2021 23:45:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 27 Mar 2021 23:45:31 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:383261dafcc4f63ecae5f2d661d1ef8d0a5e1c9f4b1f12285115baca7d101d5a`  
		Last Modified: Fri, 26 Mar 2021 15:48:21 GMT  
		Size: 49.2 MB (49196215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a8073d5d993eeeb13d2b5798a56220bed01add2f8e543d1a68cf5bdeb13b3a`  
		Last Modified: Sat, 27 Mar 2021 04:28:03 GMT  
		Size: 7.7 MB (7694449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e04ac5d1463667a0a3b2db65c9975df4dda175b8d5442808d4b141537d5531`  
		Last Modified: Sat, 27 Mar 2021 04:28:03 GMT  
		Size: 10.0 MB (9984376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6055553a6c354d4736d36059e317aaf6c573521ce1a6f381252d2418a5b22cc5`  
		Last Modified: Sat, 27 Mar 2021 23:46:33 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491bbbdd45059f5769d2bb0bdb837ba80cac2724f6e6965922ed4158c9cba265`  
		Last Modified: Sat, 27 Mar 2021 23:46:32 GMT  
		Size: 896.4 KB (896377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665c874e986f062b2080ad17ceecb5870089fc85c6dd9e508dfc13be08d8ce3a`  
		Last Modified: Sat, 27 Mar 2021 23:46:42 GMT  
		Size: 44.4 MB (44403983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87dac5cb3dad1c12cfc0defda563435433ac0c36a68beed10027b91647fd0ce`  
		Last Modified: Sat, 27 Mar 2021 23:46:31 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697255ec667025f6221eb0d566cf9686b98aceb00f4d74b95c9edfb49acbae88`  
		Last Modified: Sat, 27 Mar 2021 23:46:31 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd163f394f9a890244bb2aee5ba3eae7c4be3a8d883726e42ba5b73784fba60`  
		Last Modified: Sat, 27 Mar 2021 23:46:31 GMT  
		Size: 3.9 KB (3923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:816f00e011ce1f123d2e79f77348b0fb7d89f29cf5089abeafd8738ff8291e6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:ceedd9bb063cdb578ea9fe0b01e36bdbf04089c24f3fce51a7fea9d0a88e265c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83878159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a487cd34d550cc77f9217861618de8d698339758318d82eab265cfced3add71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:57:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 27 Mar 2021 19:41:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 27 Mar 2021 19:42:27 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 27 Mar 2021 19:42:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 27 Mar 2021 19:42:45 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 27 Mar 2021 19:42:45 GMT
EXPOSE 8091
# Sat, 27 Mar 2021 19:42:45 GMT
VOLUME [/var/lib/influxdb]
# Sat, 27 Mar 2021 19:42:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 27 Mar 2021 19:42:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 27 Mar 2021 19:42:46 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df86b11a61e4b8cbb37a4a570baf51ae6bbc8cbf231f56401403e21dea70144d`  
		Last Modified: Sat, 27 Mar 2021 06:06:53 GMT  
		Size: 11.3 MB (11286512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006eb4a69e602dcb61f4680d7e4a0d4853902062ab1230263e33125ae86b2700`  
		Last Modified: Sat, 27 Mar 2021 06:06:52 GMT  
		Size: 4.3 MB (4342442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f334f04211966274923f6e3303f71d3a69f2ec38b58016931df839cae6f95`  
		Last Modified: Sat, 27 Mar 2021 19:43:41 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf46fcf44385964742efc7341a1f94dab172bfd2c0bac74da4351c0a3074d1b`  
		Last Modified: Sat, 27 Mar 2021 19:45:37 GMT  
		Size: 22.9 MB (22866264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151881c42bede65ec63b01bd46e79e8ae0741dadbef07302b65f8c7c8af5d1f2`  
		Last Modified: Sat, 27 Mar 2021 19:45:34 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa39e1af5349913b80fa2dd7819056fd0d450677a3486570ecbe685bbe39ed6`  
		Last Modified: Sat, 27 Mar 2021 19:45:34 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:025343db4f4725ad6fca8cefab25de95f35f2ee1f7edfcb3df2912266946cfee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b3d7c436989265bf677e7b4b8cc2917b39cf23db010d5b21f509d5819bf8c659
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26966664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3552651a28dd4ac2d063768f7ac74647bb09599913a3b1a764b3b5195e0d222`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:40:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 26 Mar 2021 03:11:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Fri, 26 Mar 2021 03:12:43 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Fri, 26 Mar 2021 03:13:09 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 26 Mar 2021 03:13:09 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 26 Mar 2021 03:13:09 GMT
EXPOSE 8091
# Fri, 26 Mar 2021 03:13:09 GMT
VOLUME [/var/lib/influxdb]
# Fri, 26 Mar 2021 03:13:09 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 26 Mar 2021 03:13:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 03:13:10 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496828ab4972e79f1f4703990b2ca8339bccc53b23b09661bad5a86079d7ce44`  
		Last Modified: Fri, 26 Mar 2021 02:42:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64ab2af75b4248049e701efe5cd1fa66875886437eeec230f54a5ccf79d51cb`  
		Last Modified: Fri, 26 Mar 2021 03:14:17 GMT  
		Size: 1.4 MB (1430773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679043eb8b78af43a53255aaa9ed0573069cf4a7fe0244b00c22bb689168e8c`  
		Last Modified: Fri, 26 Mar 2021 03:16:32 GMT  
		Size: 22.7 MB (22735384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f24fb9849144e6672b70615e2c9a10ce060177818a687eda336bfb685811f9`  
		Last Modified: Fri, 26 Mar 2021 03:16:28 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a37293518b1401d50def8f45962801ec2568ccb4148145240934a9c0c21b2`  
		Last Modified: Fri, 26 Mar 2021 03:16:29 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
