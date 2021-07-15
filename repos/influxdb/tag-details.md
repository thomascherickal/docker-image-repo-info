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
-	[`influxdb:1.8.6`](#influxdb186)
-	[`influxdb:1.8.6-alpine`](#influxdb186-alpine)
-	[`influxdb:1.8.6-data`](#influxdb186-data)
-	[`influxdb:1.8.6-data-alpine`](#influxdb186-data-alpine)
-	[`influxdb:1.8.6-meta`](#influxdb186-meta)
-	[`influxdb:1.8.6-meta-alpine`](#influxdb186-meta-alpine)
-	[`influxdb:1.9-data`](#influxdb19-data)
-	[`influxdb:1.9-data-alpine`](#influxdb19-data-alpine)
-	[`influxdb:1.9-meta`](#influxdb19-meta)
-	[`influxdb:1.9-meta-alpine`](#influxdb19-meta-alpine)
-	[`influxdb:1.9.2-data`](#influxdb192-data)
-	[`influxdb:1.9.2-data-alpine`](#influxdb192-data-alpine)
-	[`influxdb:1.9.2-meta`](#influxdb192-meta)
-	[`influxdb:1.9.2-meta-alpine`](#influxdb192-meta-alpine)
-	[`influxdb:2.0`](#influxdb20)
-	[`influxdb:2.0-alpine`](#influxdb20-alpine)
-	[`influxdb:2.0.7`](#influxdb207)
-	[`influxdb:2.0.7-alpine`](#influxdb207-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.7`

```console
$ docker pull influxdb@sha256:64dbc18f8621c8a969ce90b465a84ae68e8e263ebbdbbd0e4e3a0764d610684a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7` - linux; amd64

```console
$ docker pull influxdb@sha256:5d01da20690702731668e96b8b5b3956811c314374f6f56bd27283f33f9b693f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122306653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939ee543d5c4b59334a4e7188fc482de81c061207bc7fb26ba221e6a9b275305`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:45:59 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 29 Jun 2021 02:46:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 02:46:04 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:46:05 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:46:05 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:46:05 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:46:05 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:46:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:46:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236629b14503ffd64e15f15b980fac5a8167a06f4b37c940f4b8c7be5539632c`  
		Last Modified: Tue, 29 Jun 2021 02:50:35 GMT  
		Size: 61.3 MB (61285133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7c34bf439b10082563b29c9e89e5afdc9ad3f43111e18e4bd77f7cca8fe8e5`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e655b16643567529d787a396c4e398332ebcc8a32c3d8fe66abb6b8bc5dc3525`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2a4d55f7400a074a7e4f1f9fa67a7e130a42bc4e33a084966236209530c305`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:34187e3b77f56f8b15fddf2c62605c51924788a8cce58781cc2a0ffb54d2fd61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113465763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a74002f4e910bb04bbea4d7c094ae17db73db9e385b4527f4f4b1f36716a480d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:06 GMT
ADD file:8c289b4c3c40ee076e3b3563f38ccd72dee8b2ee3122170cf1bdd417ae9e03c0 in / 
# Wed, 23 Jun 2021 00:23:08 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:53:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 04:00:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 04:00:53 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 29 Jun 2021 04:01:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 04:01:07 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 04:01:08 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 04:01:08 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 04:01:09 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 04:01:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 04:01:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 04:01:10 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d2f34e8839b40d84b70d62e2c8a6909422dad9688919bf387ad4a092d38ab62f`  
		Last Modified: Wed, 23 Jun 2021 00:36:08 GMT  
		Size: 42.1 MB (42119988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327954c584e8a66a22440b9a731a29ecccc047aa5f3477d6191e1c7167a37503`  
		Last Modified: Wed, 23 Jun 2021 06:24:47 GMT  
		Size: 10.0 MB (9950929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7274a619e45e9e714e599f6ae62b529f504ec947a07a58908ad99c464907420`  
		Last Modified: Wed, 23 Jun 2021 06:24:44 GMT  
		Size: 3.9 MB (3921297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889e41b8ac9d00748aefaab9b3862dacd7137084b28ed2594b49a1cbd5159065`  
		Last Modified: Tue, 29 Jun 2021 04:02:08 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b027a60a111151752309b809e970fadc6b25c024675ebc6166175250f1e3fcf2`  
		Last Modified: Tue, 29 Jun 2021 04:02:39 GMT  
		Size: 57.5 MB (57468977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483ed4bdfb50b0022683b4d5a973c88ff093a97a84f7ccaf044313ab5f37e59`  
		Last Modified: Tue, 29 Jun 2021 04:02:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4433aad6b50e48c8aa2c523f6f0cc8d362f83deba660ef58a76838625dd2c92`  
		Last Modified: Tue, 29 Jun 2021 04:02:08 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc73a43ca1b1f8e2b0e3fb8e25db40aa4bb666850605f96158f85226dbd291a`  
		Last Modified: Tue, 29 Jun 2021 04:02:08 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:e9f83e327a1e43b6650e09d9e5c48bd779b3a863bc75bcfe187202f6dd6da51a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f0a0bd2e5cf4d62b48390c9792a0fe04c8aa4e1ed909d279e13f5360044e4a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:55 GMT
ADD file:02285d0bd3ea996a7ebbe069a83e508701cbaf14f53fdeaa123775acd7e0537f in / 
# Tue, 22 Jun 2021 23:50:56 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 04:01:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 04:01:27 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 29 Jun 2021 04:01:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 04:01:31 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 04:01:32 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 04:01:32 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 04:01:32 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 04:01:32 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 04:01:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 04:01:33 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0789e4a342a11c7c57a241829a41af53fbd194e6dede60c6d6f63d69e403b2cd`  
		Last Modified: Tue, 22 Jun 2021 23:57:52 GMT  
		Size: 43.2 MB (43177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd2ed69368e8a7d296f1c91060e897753bed4a79ab68ed47c544e1f4d6fadcd`  
		Last Modified: Wed, 23 Jun 2021 00:35:58 GMT  
		Size: 10.2 MB (10214577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c76e514669ff971481e0d19dc0581f90d72eab2d0e117a5761ae016e14f213`  
		Last Modified: Wed, 23 Jun 2021 00:35:57 GMT  
		Size: 4.1 MB (4096534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662bae9a83b25173fc68e4cb5047c90674a050340f21fde0342f410db310c17`  
		Last Modified: Tue, 29 Jun 2021 04:02:25 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a288cb2639c794b5f6489ec57512ac44c7492faa9202628dd652009705b3999b`  
		Last Modified: Tue, 29 Jun 2021 04:02:34 GMT  
		Size: 57.2 MB (57204334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae79ff486b9d2843c495e6fc59652ece6fdb1812b314c4ba76f42af0d8083a19`  
		Last Modified: Tue, 29 Jun 2021 04:02:25 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b8d93474d559c2ab7d39c774953eea7cb503339e7362c09c0bd89f9babb568`  
		Last Modified: Tue, 29 Jun 2021 04:02:25 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512a144257344d994b00b90c519692d24d15210c282ee68c2c7e7c30a0d34760`  
		Last Modified: Tue, 29 Jun 2021 04:02:25 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-alpine`

```console
$ docker pull influxdb@sha256:8bac42efda822b46efd622e24904910b38d754ecfcd64010c78edcd83b59dfc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ed05281ac54d7028366de26daf3ec72691fc911d2a31b9a4b9d2424f7d0c0152
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65268072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21019e48a3f4c20a7c22c79ce8b9d1121687d6335af7d8b4ac1ba0a6d5f0db79`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:19 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 29 Jun 2021 02:46:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:46:19 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:46:19 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:46:19 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:46:19 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:46:20 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:46:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:46:20 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfd9d500df8351ee2d1b6c9fba08ca61ddb69508dcc0e6c796026e50a6bf853`  
		Last Modified: Tue, 29 Jun 2021 02:50:55 GMT  
		Size: 61.0 MB (61034826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bae33322b4bd6968ac47b418c20526b05732b8f18a822e27808505197424c`  
		Last Modified: Tue, 29 Jun 2021 02:50:46 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef3fb1002ad583d847b4e1466f968786dec78abd83a2aa6b53dd742998adbca`  
		Last Modified: Tue, 29 Jun 2021 02:50:46 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171e56064c9b87e0ceee549f3255b11eb4d2a47a8e2e95240bccb15866d66ba9`  
		Last Modified: Tue, 29 Jun 2021 02:50:46 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data`

```console
$ docker pull influxdb@sha256:805150f4349b5f177e7cfd65bb3ab25bbac13cccd7fb7f790d92eac962bbd96a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:b7cb9af9311cb0d6300149135c32e72a3afafa1640a651827f559d4b2873f019
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148970616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b4feed13bec3152b25070d09dd0a20b16bad46fb6f106f1d31f58672f4584f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:46:24 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Tue, 29 Jun 2021 02:46:33 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:46:33 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:46:34 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:46:34 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:46:34 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:46:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:46:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:46:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a83adfa11ff6fce2f61e6cc24f8aa5b87c5622584b7013879cdb9c884180f6e`  
		Last Modified: Tue, 29 Jun 2021 02:51:18 GMT  
		Size: 87.9 MB (87949038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1f8fd427194be6f3d3fc28d3f635bf30c5b0ca8dda32b61a0abc0b1508cb06`  
		Last Modified: Tue, 29 Jun 2021 02:51:05 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a12b17a629649fac1a0cee21540c1c4b1bc48e23ca32f1adb37d758e49334a`  
		Last Modified: Tue, 29 Jun 2021 02:51:06 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5a99874ce97657b57612e39df6b5ce2c2f88f40ce6470be84a25e143defcd4`  
		Last Modified: Tue, 29 Jun 2021 02:51:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data-alpine`

```console
$ docker pull influxdb@sha256:656c0b783d69f899d250797d79d2d6972b37ea2339be8394bd3fc9eec38267e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:10c0f22b11d8ed5c617b9407ad583ae26238c90685cd200cf30897bf84b61f35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91872120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6763179ef9052b94e7a106652666400b8250da008f49e231e787259e1701aa29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Tue, 29 Jun 2021 02:46:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:46:48 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:46:48 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:46:49 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:46:49 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:46:49 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:46:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:46:50 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcffaeb4c3ddd9e885a4fceb5bf51ce701b0c94e3c026caa8cc4267480684790`  
		Last Modified: Tue, 29 Jun 2021 02:51:42 GMT  
		Size: 87.6 MB (87638817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae2edb0b905d82f68bbf13bc240d6529e6aabf2023d5d9758b476ede8796e8e`  
		Last Modified: Tue, 29 Jun 2021 02:51:29 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30f50d155be84aeebbaaa793b9c5deeb18a0d026a126130f25a5af8ab5b26be`  
		Last Modified: Tue, 29 Jun 2021 02:51:29 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6103ac0379d35c877bbd2b0dea8a54b5a0a589bae601db97c88d97ae110d2730`  
		Last Modified: Tue, 29 Jun 2021 02:51:29 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta`

```console
$ docker pull influxdb@sha256:d186c27511e8c04ed0e5e3aee01922c5c2e597b71100aad04bde7620410ad584
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:19cd43bbc247bb12de66db8833af1e30e9c1c995d8762ac7eb091f290bc3b13c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84153984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ddd20ec8cba4f9340ce6926a92f2320f8cd08489d15cd67f4fd8d000b8ba502`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:46:24 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Tue, 29 Jun 2021 02:46:55 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:46:56 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:46:56 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:46:56 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:46:56 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:46:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:46:57 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2523bbd4e0866324ab74cfad5f15669fd47c8e45f8e04953357b90dc65bee5d8`  
		Last Modified: Tue, 29 Jun 2021 02:51:56 GMT  
		Size: 23.1 MB (23133610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046c67faac6934076e06e6a44d92e63a771fdec7ea1fe78b8834b26b20f5f776`  
		Last Modified: Tue, 29 Jun 2021 02:51:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3faa3e213a6c049b7034db70903db3a4a3e59d63ecfa4197d52f3debb8a6c7`  
		Last Modified: Tue, 29 Jun 2021 02:51:53 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta-alpine`

```console
$ docker pull influxdb@sha256:4ba4d614939eebb65c47141be3e9d585f0dcc62f1ad54dd13e1a7fe33f548607
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:c00bf82b825775a152e566ab0efbcb90ae50bcbaec979c99e5d61b17ba37ca71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27235057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:072d6bd4992e7ce8b48ccbb7eceb94eaeae74fa98d2bac4bd0d65836e5ec094a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Tue, 29 Jun 2021 02:47:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:47:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:47:05 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:47:05 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:47:06 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcd198100cc930b2daf7cc185ac6a6ae000ac641b7ddabacdc0471d36792afe`  
		Last Modified: Tue, 29 Jun 2021 02:52:10 GMT  
		Size: 23.0 MB (23002960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12eccdc7211c5d880848652f6e47bdd0f9eda58797bbacfe795cc9a9f6c33eda`  
		Last Modified: Tue, 29 Jun 2021 02:52:06 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20eb9c3296fedeae155393dcc058b9865975d70f7bf5d231e7f07b535e2a0ff6`  
		Last Modified: Tue, 29 Jun 2021 02:52:06 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11`

```console
$ docker pull influxdb@sha256:64dbc18f8621c8a969ce90b465a84ae68e8e263ebbdbbd0e4e3a0764d610684a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7.11` - linux; amd64

```console
$ docker pull influxdb@sha256:5d01da20690702731668e96b8b5b3956811c314374f6f56bd27283f33f9b693f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122306653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939ee543d5c4b59334a4e7188fc482de81c061207bc7fb26ba221e6a9b275305`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:45:59 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 29 Jun 2021 02:46:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 02:46:04 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:46:05 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:46:05 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:46:05 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:46:05 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:46:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:46:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236629b14503ffd64e15f15b980fac5a8167a06f4b37c940f4b8c7be5539632c`  
		Last Modified: Tue, 29 Jun 2021 02:50:35 GMT  
		Size: 61.3 MB (61285133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7c34bf439b10082563b29c9e89e5afdc9ad3f43111e18e4bd77f7cca8fe8e5`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e655b16643567529d787a396c4e398332ebcc8a32c3d8fe66abb6b8bc5dc3525`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2a4d55f7400a074a7e4f1f9fa67a7e130a42bc4e33a084966236209530c305`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:34187e3b77f56f8b15fddf2c62605c51924788a8cce58781cc2a0ffb54d2fd61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113465763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a74002f4e910bb04bbea4d7c094ae17db73db9e385b4527f4f4b1f36716a480d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:06 GMT
ADD file:8c289b4c3c40ee076e3b3563f38ccd72dee8b2ee3122170cf1bdd417ae9e03c0 in / 
# Wed, 23 Jun 2021 00:23:08 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:53:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 04:00:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 04:00:53 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 29 Jun 2021 04:01:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 04:01:07 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 04:01:08 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 04:01:08 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 04:01:09 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 04:01:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 04:01:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 04:01:10 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d2f34e8839b40d84b70d62e2c8a6909422dad9688919bf387ad4a092d38ab62f`  
		Last Modified: Wed, 23 Jun 2021 00:36:08 GMT  
		Size: 42.1 MB (42119988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327954c584e8a66a22440b9a731a29ecccc047aa5f3477d6191e1c7167a37503`  
		Last Modified: Wed, 23 Jun 2021 06:24:47 GMT  
		Size: 10.0 MB (9950929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7274a619e45e9e714e599f6ae62b529f504ec947a07a58908ad99c464907420`  
		Last Modified: Wed, 23 Jun 2021 06:24:44 GMT  
		Size: 3.9 MB (3921297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889e41b8ac9d00748aefaab9b3862dacd7137084b28ed2594b49a1cbd5159065`  
		Last Modified: Tue, 29 Jun 2021 04:02:08 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b027a60a111151752309b809e970fadc6b25c024675ebc6166175250f1e3fcf2`  
		Last Modified: Tue, 29 Jun 2021 04:02:39 GMT  
		Size: 57.5 MB (57468977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483ed4bdfb50b0022683b4d5a973c88ff093a97a84f7ccaf044313ab5f37e59`  
		Last Modified: Tue, 29 Jun 2021 04:02:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4433aad6b50e48c8aa2c523f6f0cc8d362f83deba660ef58a76838625dd2c92`  
		Last Modified: Tue, 29 Jun 2021 04:02:08 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc73a43ca1b1f8e2b0e3fb8e25db40aa4bb666850605f96158f85226dbd291a`  
		Last Modified: Tue, 29 Jun 2021 04:02:08 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:e9f83e327a1e43b6650e09d9e5c48bd779b3a863bc75bcfe187202f6dd6da51a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114697435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f0a0bd2e5cf4d62b48390c9792a0fe04c8aa4e1ed909d279e13f5360044e4a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:55 GMT
ADD file:02285d0bd3ea996a7ebbe069a83e508701cbaf14f53fdeaa123775acd7e0537f in / 
# Tue, 22 Jun 2021 23:50:56 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 04:01:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 04:01:27 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 29 Jun 2021 04:01:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 04:01:31 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 04:01:32 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 04:01:32 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 04:01:32 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 04:01:32 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 04:01:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 04:01:33 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0789e4a342a11c7c57a241829a41af53fbd194e6dede60c6d6f63d69e403b2cd`  
		Last Modified: Tue, 22 Jun 2021 23:57:52 GMT  
		Size: 43.2 MB (43177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd2ed69368e8a7d296f1c91060e897753bed4a79ab68ed47c544e1f4d6fadcd`  
		Last Modified: Wed, 23 Jun 2021 00:35:58 GMT  
		Size: 10.2 MB (10214577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c76e514669ff971481e0d19dc0581f90d72eab2d0e117a5761ae016e14f213`  
		Last Modified: Wed, 23 Jun 2021 00:35:57 GMT  
		Size: 4.1 MB (4096534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662bae9a83b25173fc68e4cb5047c90674a050340f21fde0342f410db310c17`  
		Last Modified: Tue, 29 Jun 2021 04:02:25 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a288cb2639c794b5f6489ec57512ac44c7492faa9202628dd652009705b3999b`  
		Last Modified: Tue, 29 Jun 2021 04:02:34 GMT  
		Size: 57.2 MB (57204334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae79ff486b9d2843c495e6fc59652ece6fdb1812b314c4ba76f42af0d8083a19`  
		Last Modified: Tue, 29 Jun 2021 04:02:25 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b8d93474d559c2ab7d39c774953eea7cb503339e7362c09c0bd89f9babb568`  
		Last Modified: Tue, 29 Jun 2021 04:02:25 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512a144257344d994b00b90c519692d24d15210c282ee68c2c7e7c30a0d34760`  
		Last Modified: Tue, 29 Jun 2021 04:02:25 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-alpine`

```console
$ docker pull influxdb@sha256:8bac42efda822b46efd622e24904910b38d754ecfcd64010c78edcd83b59dfc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ed05281ac54d7028366de26daf3ec72691fc911d2a31b9a4b9d2424f7d0c0152
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65268072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21019e48a3f4c20a7c22c79ce8b9d1121687d6335af7d8b4ac1ba0a6d5f0db79`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:19 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 29 Jun 2021 02:46:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:46:19 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:46:19 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:46:19 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:46:19 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:46:20 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:46:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:46:20 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfd9d500df8351ee2d1b6c9fba08ca61ddb69508dcc0e6c796026e50a6bf853`  
		Last Modified: Tue, 29 Jun 2021 02:50:55 GMT  
		Size: 61.0 MB (61034826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966bae33322b4bd6968ac47b418c20526b05732b8f18a822e27808505197424c`  
		Last Modified: Tue, 29 Jun 2021 02:50:46 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef3fb1002ad583d847b4e1466f968786dec78abd83a2aa6b53dd742998adbca`  
		Last Modified: Tue, 29 Jun 2021 02:50:46 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171e56064c9b87e0ceee549f3255b11eb4d2a47a8e2e95240bccb15866d66ba9`  
		Last Modified: Tue, 29 Jun 2021 02:50:46 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data`

```console
$ docker pull influxdb@sha256:805150f4349b5f177e7cfd65bb3ab25bbac13cccd7fb7f790d92eac962bbd96a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:b7cb9af9311cb0d6300149135c32e72a3afafa1640a651827f559d4b2873f019
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148970616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b4feed13bec3152b25070d09dd0a20b16bad46fb6f106f1d31f58672f4584f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:46:24 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Tue, 29 Jun 2021 02:46:33 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:46:33 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:46:34 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:46:34 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:46:34 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:46:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:46:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:46:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a83adfa11ff6fce2f61e6cc24f8aa5b87c5622584b7013879cdb9c884180f6e`  
		Last Modified: Tue, 29 Jun 2021 02:51:18 GMT  
		Size: 87.9 MB (87949038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1f8fd427194be6f3d3fc28d3f635bf30c5b0ca8dda32b61a0abc0b1508cb06`  
		Last Modified: Tue, 29 Jun 2021 02:51:05 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a12b17a629649fac1a0cee21540c1c4b1bc48e23ca32f1adb37d758e49334a`  
		Last Modified: Tue, 29 Jun 2021 02:51:06 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5a99874ce97657b57612e39df6b5ce2c2f88f40ce6470be84a25e143defcd4`  
		Last Modified: Tue, 29 Jun 2021 02:51:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data-alpine`

```console
$ docker pull influxdb@sha256:656c0b783d69f899d250797d79d2d6972b37ea2339be8394bd3fc9eec38267e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:10c0f22b11d8ed5c617b9407ad583ae26238c90685cd200cf30897bf84b61f35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91872120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6763179ef9052b94e7a106652666400b8250da008f49e231e787259e1701aa29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Tue, 29 Jun 2021 02:46:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:46:48 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:46:48 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:46:49 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:46:49 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:46:49 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:46:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:46:50 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcffaeb4c3ddd9e885a4fceb5bf51ce701b0c94e3c026caa8cc4267480684790`  
		Last Modified: Tue, 29 Jun 2021 02:51:42 GMT  
		Size: 87.6 MB (87638817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae2edb0b905d82f68bbf13bc240d6529e6aabf2023d5d9758b476ede8796e8e`  
		Last Modified: Tue, 29 Jun 2021 02:51:29 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30f50d155be84aeebbaaa793b9c5deeb18a0d026a126130f25a5af8ab5b26be`  
		Last Modified: Tue, 29 Jun 2021 02:51:29 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6103ac0379d35c877bbd2b0dea8a54b5a0a589bae601db97c88d97ae110d2730`  
		Last Modified: Tue, 29 Jun 2021 02:51:29 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta`

```console
$ docker pull influxdb@sha256:d186c27511e8c04ed0e5e3aee01922c5c2e597b71100aad04bde7620410ad584
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:19cd43bbc247bb12de66db8833af1e30e9c1c995d8762ac7eb091f290bc3b13c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84153984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ddd20ec8cba4f9340ce6926a92f2320f8cd08489d15cd67f4fd8d000b8ba502`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:46:24 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Tue, 29 Jun 2021 02:46:55 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:46:56 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:46:56 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:46:56 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:46:56 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:46:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:46:57 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2523bbd4e0866324ab74cfad5f15669fd47c8e45f8e04953357b90dc65bee5d8`  
		Last Modified: Tue, 29 Jun 2021 02:51:56 GMT  
		Size: 23.1 MB (23133610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046c67faac6934076e06e6a44d92e63a771fdec7ea1fe78b8834b26b20f5f776`  
		Last Modified: Tue, 29 Jun 2021 02:51:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3faa3e213a6c049b7034db70903db3a4a3e59d63ecfa4197d52f3debb8a6c7`  
		Last Modified: Tue, 29 Jun 2021 02:51:53 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta-alpine`

```console
$ docker pull influxdb@sha256:4ba4d614939eebb65c47141be3e9d585f0dcc62f1ad54dd13e1a7fe33f548607
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:c00bf82b825775a152e566ab0efbcb90ae50bcbaec979c99e5d61b17ba37ca71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27235057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:072d6bd4992e7ce8b48ccbb7eceb94eaeae74fa98d2bac4bd0d65836e5ec094a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:56:32 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Tue, 29 Jun 2021 02:47:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:47:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:47:05 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:47:05 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:47:06 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcd198100cc930b2daf7cc185ac6a6ae000ac641b7ddabacdc0471d36792afe`  
		Last Modified: Tue, 29 Jun 2021 02:52:10 GMT  
		Size: 23.0 MB (23002960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12eccdc7211c5d880848652f6e47bdd0f9eda58797bbacfe795cc9a9f6c33eda`  
		Last Modified: Tue, 29 Jun 2021 02:52:06 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20eb9c3296fedeae155393dcc058b9865975d70f7bf5d231e7f07b535e2a0ff6`  
		Last Modified: Tue, 29 Jun 2021 02:52:06 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:6dd578a74616d4194782c07402dbdca5fe91d8aaf8388da3975742f11f429f24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:b3baa6ce9f7a578105be9ddf2e045e5727b5198480a66e01c31fd1c5209d5d7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126069245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69932c3841cc8a5456297e0263003fbecb127a1e63d2db09754d9322d3ba39f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:47:10 GMT
ENV INFLUXDB_VERSION=1.8.6
# Tue, 29 Jun 2021 02:47:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 02:47:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:47:17 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:47:18 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:18 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:18 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:47:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:47:19 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ade3a783c8ff98f4e58ca612e2a2bd13500e23c9bdfe93cffb4a6885785a8c`  
		Last Modified: Tue, 29 Jun 2021 02:52:30 GMT  
		Size: 65.0 MB (65047730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddc7d5fa34f9a0da8802e12fc44f5be0056dbc3835c8fb01dee03adec8956be`  
		Last Modified: Tue, 29 Jun 2021 02:52:20 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297585df8a9b2ddb6121a22aeaff0528284411e7a37608586d6e4ba2765ceb4f`  
		Last Modified: Tue, 29 Jun 2021 02:52:21 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb505cff3d6a9dd5f6eb85d3d6b620f7fb979b4024feebe033d6443b93334cf`  
		Last Modified: Tue, 29 Jun 2021 02:52:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:682b9d24e44de479e73ccb758d4263ad6a2e04d2e733b967b0d28054622d762b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117133051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ff50fae9b546cd1fef68c390558b55ef77f0e192b6da9dd29fc77dc58490831`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:06 GMT
ADD file:8c289b4c3c40ee076e3b3563f38ccd72dee8b2ee3122170cf1bdd417ae9e03c0 in / 
# Wed, 23 Jun 2021 00:23:08 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:53:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 04:00:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 04:01:21 GMT
ENV INFLUXDB_VERSION=1.8.6
# Tue, 29 Jun 2021 04:01:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 04:01:36 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 04:01:37 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 04:01:37 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 04:01:37 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 04:01:38 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 04:01:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 04:01:39 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d2f34e8839b40d84b70d62e2c8a6909422dad9688919bf387ad4a092d38ab62f`  
		Last Modified: Wed, 23 Jun 2021 00:36:08 GMT  
		Size: 42.1 MB (42119988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327954c584e8a66a22440b9a731a29ecccc047aa5f3477d6191e1c7167a37503`  
		Last Modified: Wed, 23 Jun 2021 06:24:47 GMT  
		Size: 10.0 MB (9950929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7274a619e45e9e714e599f6ae62b529f504ec947a07a58908ad99c464907420`  
		Last Modified: Wed, 23 Jun 2021 06:24:44 GMT  
		Size: 3.9 MB (3921297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889e41b8ac9d00748aefaab9b3862dacd7137084b28ed2594b49a1cbd5159065`  
		Last Modified: Tue, 29 Jun 2021 04:02:08 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517b7931663babc5997f0e018cb0890d9fce363693760c0e10424ad1c4fc2866`  
		Last Modified: Tue, 29 Jun 2021 04:03:29 GMT  
		Size: 61.1 MB (61136266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e913e33fedc589f9a40031ab3043b6c5d9059f2510973ea24f060335f4c75e62`  
		Last Modified: Tue, 29 Jun 2021 04:02:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fe68b1e4a990e1c5cc0e5ac0a3e24c823c7ccdd2503a3c5e4e8f0d6a7cdc10`  
		Last Modified: Tue, 29 Jun 2021 04:02:53 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48328e739317853ab767d073aab69592f2094b305e1b563150d26e4c5bb82600`  
		Last Modified: Tue, 29 Jun 2021 04:02:53 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f52dd3fcf76f889e04f7992143d57730bfebc13f25ec93c1e9dd9ac298075ce3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118189720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0515e29240a94c6d4f7539d9ea8a1fb63da67a556ddf04617ce9ee7d4e14c149`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:55 GMT
ADD file:02285d0bd3ea996a7ebbe069a83e508701cbaf14f53fdeaa123775acd7e0537f in / 
# Tue, 22 Jun 2021 23:50:56 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 04:01:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 04:01:38 GMT
ENV INFLUXDB_VERSION=1.8.6
# Tue, 29 Jun 2021 04:01:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 04:01:44 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 04:01:44 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 04:01:44 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 04:01:45 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 04:01:45 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 04:01:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 04:01:45 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0789e4a342a11c7c57a241829a41af53fbd194e6dede60c6d6f63d69e403b2cd`  
		Last Modified: Tue, 22 Jun 2021 23:57:52 GMT  
		Size: 43.2 MB (43177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd2ed69368e8a7d296f1c91060e897753bed4a79ab68ed47c544e1f4d6fadcd`  
		Last Modified: Wed, 23 Jun 2021 00:35:58 GMT  
		Size: 10.2 MB (10214577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c76e514669ff971481e0d19dc0581f90d72eab2d0e117a5761ae016e14f213`  
		Last Modified: Wed, 23 Jun 2021 00:35:57 GMT  
		Size: 4.1 MB (4096534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662bae9a83b25173fc68e4cb5047c90674a050340f21fde0342f410db310c17`  
		Last Modified: Tue, 29 Jun 2021 04:02:25 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fd1077af50ce49e3016cc63893cdf517d1277ab1debb95e6d96da182ff0748`  
		Last Modified: Tue, 29 Jun 2021 04:02:55 GMT  
		Size: 60.7 MB (60696620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdbbb3d1ea1dee8b543704fe660c1dad426d5fa2ed5457a88cd64a062aa92af`  
		Last Modified: Tue, 29 Jun 2021 04:02:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4904a637145aca6604d33e2060480e0b933f3463239fbba23f44f2b5db5b28`  
		Last Modified: Tue, 29 Jun 2021 04:02:46 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e386bb00a8fd286736cfec231a92bb995e0abe92ea90c03fb89c2260dacb352`  
		Last Modified: Tue, 29 Jun 2021 04:02:46 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:af9d06269631fbba543216de88ebdb028b0e8e27e26f66233bc3b92e707a1eb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b7a000c70584cf973b06fe45c0072b7e70e51c6b654d14a7d71f12c84eae1b33
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69024535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a4a7c8e74ff9696487428a78c80be5b2a25b7c95c07bdc4d24d97a179106ae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:20:50 GMT
ENV INFLUXDB_VERSION=1.8.6
# Tue, 29 Jun 2021 02:47:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:47:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:47:30 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:47:30 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:31 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:31 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:47:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:47:32 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df10c6d81162718a9636791bed21265b364322436eb8484b67f879c3735305ea`  
		Last Modified: Tue, 29 Jun 2021 02:52:50 GMT  
		Size: 64.8 MB (64791289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bdda3cf6ff08b5cc5594af9316695aaa83ab47ad19305113023fa53d9ca361`  
		Last Modified: Tue, 29 Jun 2021 02:52:41 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a8868d42816cf4292511526154cbdde3bcbb0c255ecfa3c0035291e7818794`  
		Last Modified: Tue, 29 Jun 2021 02:52:41 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a99666c872719e833ce2d4b26f387c6bd98d89fff5e979c8a1d1ce6ac76309d`  
		Last Modified: Tue, 29 Jun 2021 02:52:41 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:4fb0dfef21ec768d604daa11c79353813af0f6bd7cc9c0f8d8829129254bc353
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:3e1303bc26c2b90eed88a89f1956a861085ee58a766cff8c4435a4129b21ffee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127804266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2883ca6aac47f1258dd7992e6b903d9a20198641207c23ca397f6423e2cae30c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:47:36 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:47:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:47:44 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:47:45 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:47:45 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:45 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:45 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:47:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:47:46 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2484aa1c72408db7db17fa7189dd8c9dbfc4ed0e8f5c0ccaf40d895b5beb35b4`  
		Last Modified: Tue, 29 Jun 2021 02:53:10 GMT  
		Size: 66.8 MB (66782689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44340132df85be8500d6ed41e6c2a3b02ac4e15b60baeb764a385fe005f0beb`  
		Last Modified: Tue, 29 Jun 2021 02:53:00 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd26a07fb714838a75eec2248ff9247c84f3ee812c405e7ed2497b147dbe6323`  
		Last Modified: Tue, 29 Jun 2021 02:53:00 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e865b0393dce51a350a72ba0cc6106fc12bd632a114a9d0e18185e1bae23f36a`  
		Last Modified: Tue, 29 Jun 2021 02:53:00 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:5d7984b19ebeae696e3a72d0d3be4d8f8ae98a26a059c30cd514d7327b328a1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:e84363979b5ea93eb60066bdc93d41b14d17c4f34b1f9f01f64b5fbe726df1cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70748308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e4a2b986dd07e77d8096bc74a754722028e44638e034361d54b091bf393c3cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:47:56 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:47:57 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:47:57 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:47:58 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:59 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:47:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97a8d8f09c90b1a78add4731e617075475228aa15ebd842f786082506157d4b`  
		Last Modified: Tue, 29 Jun 2021 02:53:33 GMT  
		Size: 66.5 MB (66515006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b888d7236b6084c80f45090dcc6b19a6c5ea223bb98fabfe8c28c1f1720e016`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0257283109ba2c40cae5ec75d6b30432c2b68de3ff5d79273c97cde6a6cc9c1`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446dae2e30b64005cca683af402f69f5c94573556a3ec08cd3784bd7069f74df`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:81b0672b04d307d8d82d5d129dd6beaf90041bb024e9cb4e0c24ef267ce7e2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:be294edf8c9a733ae7f26f34033175a589be9a7f2134598e880af2215364dc30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84226320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6ac069304e5cf8fa2a2e01cb6ac5a02021451b00c126089e7656aa49c487d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:47:36 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:48:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:48:12 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:48:13 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:48:13 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:48:14 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:48:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:14 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9de407994c8853a1596a41ee0ced55922407313243da6ba18b9d9d11025802`  
		Last Modified: Tue, 29 Jun 2021 02:53:49 GMT  
		Size: 23.2 MB (23205949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48295ea472331c2f682539b6c3baeae5c287ff9457276e4a2106b7a0dc47221f`  
		Last Modified: Tue, 29 Jun 2021 02:53:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb8d5d4b45a9b182593c6f8eecbc172ed4a8a0eda344b11590e38145a5e7814`  
		Last Modified: Tue, 29 Jun 2021 02:53:46 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:ca1e61a34022562abfd681504f9c15299de25f62d568a3a6cefebd2c7e64c581
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:05be70bb791eba3706e6508474ca275411194aa09d49e6a5dbb11ffbe4482bac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27306930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc98141e784ebcdd83f60cdda2926428a114858aea72884487f2460cd71aedc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:48:27 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:48:27 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:48:28 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:48:28 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:48:29 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:48:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:30 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a454dabfdc9badc7b06cbadac755be9de59234e022dbd19e0bc02fed5c8379`  
		Last Modified: Tue, 29 Jun 2021 02:54:06 GMT  
		Size: 23.1 MB (23074833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34742c348a4bf98acecce3f2a81f4d7d4ba5d68ac3cb5cf64bb258bc3f088d2`  
		Last Modified: Tue, 29 Jun 2021 02:54:02 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db545df212f2a7d0df6c34a87fb022e869adfacb8aef3c7be3b8b00133790f`  
		Last Modified: Tue, 29 Jun 2021 02:54:02 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6`

```console
$ docker pull influxdb@sha256:6dd578a74616d4194782c07402dbdca5fe91d8aaf8388da3975742f11f429f24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.6` - linux; amd64

```console
$ docker pull influxdb@sha256:b3baa6ce9f7a578105be9ddf2e045e5727b5198480a66e01c31fd1c5209d5d7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126069245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69932c3841cc8a5456297e0263003fbecb127a1e63d2db09754d9322d3ba39f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:47:10 GMT
ENV INFLUXDB_VERSION=1.8.6
# Tue, 29 Jun 2021 02:47:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 02:47:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:47:17 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:47:18 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:18 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:18 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:47:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:47:19 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ade3a783c8ff98f4e58ca612e2a2bd13500e23c9bdfe93cffb4a6885785a8c`  
		Last Modified: Tue, 29 Jun 2021 02:52:30 GMT  
		Size: 65.0 MB (65047730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddc7d5fa34f9a0da8802e12fc44f5be0056dbc3835c8fb01dee03adec8956be`  
		Last Modified: Tue, 29 Jun 2021 02:52:20 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297585df8a9b2ddb6121a22aeaff0528284411e7a37608586d6e4ba2765ceb4f`  
		Last Modified: Tue, 29 Jun 2021 02:52:21 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb505cff3d6a9dd5f6eb85d3d6b620f7fb979b4024feebe033d6443b93334cf`  
		Last Modified: Tue, 29 Jun 2021 02:52:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.6` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:682b9d24e44de479e73ccb758d4263ad6a2e04d2e733b967b0d28054622d762b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117133051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ff50fae9b546cd1fef68c390558b55ef77f0e192b6da9dd29fc77dc58490831`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:06 GMT
ADD file:8c289b4c3c40ee076e3b3563f38ccd72dee8b2ee3122170cf1bdd417ae9e03c0 in / 
# Wed, 23 Jun 2021 00:23:08 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:53:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 04:00:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 04:01:21 GMT
ENV INFLUXDB_VERSION=1.8.6
# Tue, 29 Jun 2021 04:01:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 04:01:36 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 04:01:37 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 04:01:37 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 04:01:37 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 04:01:38 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 04:01:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 04:01:39 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d2f34e8839b40d84b70d62e2c8a6909422dad9688919bf387ad4a092d38ab62f`  
		Last Modified: Wed, 23 Jun 2021 00:36:08 GMT  
		Size: 42.1 MB (42119988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327954c584e8a66a22440b9a731a29ecccc047aa5f3477d6191e1c7167a37503`  
		Last Modified: Wed, 23 Jun 2021 06:24:47 GMT  
		Size: 10.0 MB (9950929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7274a619e45e9e714e599f6ae62b529f504ec947a07a58908ad99c464907420`  
		Last Modified: Wed, 23 Jun 2021 06:24:44 GMT  
		Size: 3.9 MB (3921297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889e41b8ac9d00748aefaab9b3862dacd7137084b28ed2594b49a1cbd5159065`  
		Last Modified: Tue, 29 Jun 2021 04:02:08 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517b7931663babc5997f0e018cb0890d9fce363693760c0e10424ad1c4fc2866`  
		Last Modified: Tue, 29 Jun 2021 04:03:29 GMT  
		Size: 61.1 MB (61136266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e913e33fedc589f9a40031ab3043b6c5d9059f2510973ea24f060335f4c75e62`  
		Last Modified: Tue, 29 Jun 2021 04:02:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fe68b1e4a990e1c5cc0e5ac0a3e24c823c7ccdd2503a3c5e4e8f0d6a7cdc10`  
		Last Modified: Tue, 29 Jun 2021 04:02:53 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48328e739317853ab767d073aab69592f2094b305e1b563150d26e4c5bb82600`  
		Last Modified: Tue, 29 Jun 2021 04:02:53 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.6` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f52dd3fcf76f889e04f7992143d57730bfebc13f25ec93c1e9dd9ac298075ce3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118189720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0515e29240a94c6d4f7539d9ea8a1fb63da67a556ddf04617ce9ee7d4e14c149`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:55 GMT
ADD file:02285d0bd3ea996a7ebbe069a83e508701cbaf14f53fdeaa123775acd7e0537f in / 
# Tue, 22 Jun 2021 23:50:56 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 04:01:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 04:01:38 GMT
ENV INFLUXDB_VERSION=1.8.6
# Tue, 29 Jun 2021 04:01:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 29 Jun 2021 04:01:44 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 04:01:44 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 04:01:44 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 04:01:45 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 04:01:45 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 04:01:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 04:01:45 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0789e4a342a11c7c57a241829a41af53fbd194e6dede60c6d6f63d69e403b2cd`  
		Last Modified: Tue, 22 Jun 2021 23:57:52 GMT  
		Size: 43.2 MB (43177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd2ed69368e8a7d296f1c91060e897753bed4a79ab68ed47c544e1f4d6fadcd`  
		Last Modified: Wed, 23 Jun 2021 00:35:58 GMT  
		Size: 10.2 MB (10214577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c76e514669ff971481e0d19dc0581f90d72eab2d0e117a5761ae016e14f213`  
		Last Modified: Wed, 23 Jun 2021 00:35:57 GMT  
		Size: 4.1 MB (4096534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662bae9a83b25173fc68e4cb5047c90674a050340f21fde0342f410db310c17`  
		Last Modified: Tue, 29 Jun 2021 04:02:25 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fd1077af50ce49e3016cc63893cdf517d1277ab1debb95e6d96da182ff0748`  
		Last Modified: Tue, 29 Jun 2021 04:02:55 GMT  
		Size: 60.7 MB (60696620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdbbb3d1ea1dee8b543704fe660c1dad426d5fa2ed5457a88cd64a062aa92af`  
		Last Modified: Tue, 29 Jun 2021 04:02:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4904a637145aca6604d33e2060480e0b933f3463239fbba23f44f2b5db5b28`  
		Last Modified: Tue, 29 Jun 2021 04:02:46 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e386bb00a8fd286736cfec231a92bb995e0abe92ea90c03fb89c2260dacb352`  
		Last Modified: Tue, 29 Jun 2021 04:02:46 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6-alpine`

```console
$ docker pull influxdb@sha256:af9d06269631fbba543216de88ebdb028b0e8e27e26f66233bc3b92e707a1eb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.6-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b7a000c70584cf973b06fe45c0072b7e70e51c6b654d14a7d71f12c84eae1b33
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69024535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a4a7c8e74ff9696487428a78c80be5b2a25b7c95c07bdc4d24d97a179106ae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:20:50 GMT
ENV INFLUXDB_VERSION=1.8.6
# Tue, 29 Jun 2021 02:47:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:47:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:47:30 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:47:30 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:31 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:31 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:47:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:47:32 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df10c6d81162718a9636791bed21265b364322436eb8484b67f879c3735305ea`  
		Last Modified: Tue, 29 Jun 2021 02:52:50 GMT  
		Size: 64.8 MB (64791289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bdda3cf6ff08b5cc5594af9316695aaa83ab47ad19305113023fa53d9ca361`  
		Last Modified: Tue, 29 Jun 2021 02:52:41 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a8868d42816cf4292511526154cbdde3bcbb0c255ecfa3c0035291e7818794`  
		Last Modified: Tue, 29 Jun 2021 02:52:41 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a99666c872719e833ce2d4b26f387c6bd98d89fff5e979c8a1d1ce6ac76309d`  
		Last Modified: Tue, 29 Jun 2021 02:52:41 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6-data`

```console
$ docker pull influxdb@sha256:4fb0dfef21ec768d604daa11c79353813af0f6bd7cc9c0f8d8829129254bc353
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.6-data` - linux; amd64

```console
$ docker pull influxdb@sha256:3e1303bc26c2b90eed88a89f1956a861085ee58a766cff8c4435a4129b21ffee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127804266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2883ca6aac47f1258dd7992e6b903d9a20198641207c23ca397f6423e2cae30c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:47:36 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:47:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:47:44 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:47:45 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:47:45 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:45 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:45 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:47:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:47:46 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2484aa1c72408db7db17fa7189dd8c9dbfc4ed0e8f5c0ccaf40d895b5beb35b4`  
		Last Modified: Tue, 29 Jun 2021 02:53:10 GMT  
		Size: 66.8 MB (66782689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44340132df85be8500d6ed41e6c2a3b02ac4e15b60baeb764a385fe005f0beb`  
		Last Modified: Tue, 29 Jun 2021 02:53:00 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd26a07fb714838a75eec2248ff9247c84f3ee812c405e7ed2497b147dbe6323`  
		Last Modified: Tue, 29 Jun 2021 02:53:00 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e865b0393dce51a350a72ba0cc6106fc12bd632a114a9d0e18185e1bae23f36a`  
		Last Modified: Tue, 29 Jun 2021 02:53:00 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6-data-alpine`

```console
$ docker pull influxdb@sha256:5d7984b19ebeae696e3a72d0d3be4d8f8ae98a26a059c30cd514d7327b328a1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.6-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:e84363979b5ea93eb60066bdc93d41b14d17c4f34b1f9f01f64b5fbe726df1cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70748308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e4a2b986dd07e77d8096bc74a754722028e44638e034361d54b091bf393c3cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:47:56 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:47:57 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:47:57 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:47:58 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:59 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:47:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97a8d8f09c90b1a78add4731e617075475228aa15ebd842f786082506157d4b`  
		Last Modified: Tue, 29 Jun 2021 02:53:33 GMT  
		Size: 66.5 MB (66515006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b888d7236b6084c80f45090dcc6b19a6c5ea223bb98fabfe8c28c1f1720e016`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0257283109ba2c40cae5ec75d6b30432c2b68de3ff5d79273c97cde6a6cc9c1`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446dae2e30b64005cca683af402f69f5c94573556a3ec08cd3784bd7069f74df`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6-meta`

```console
$ docker pull influxdb@sha256:81b0672b04d307d8d82d5d129dd6beaf90041bb024e9cb4e0c24ef267ce7e2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.6-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:be294edf8c9a733ae7f26f34033175a589be9a7f2134598e880af2215364dc30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84226320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6ac069304e5cf8fa2a2e01cb6ac5a02021451b00c126089e7656aa49c487d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:47:36 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:48:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:48:12 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:48:13 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:48:13 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:48:14 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:48:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:14 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9de407994c8853a1596a41ee0ced55922407313243da6ba18b9d9d11025802`  
		Last Modified: Tue, 29 Jun 2021 02:53:49 GMT  
		Size: 23.2 MB (23205949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48295ea472331c2f682539b6c3baeae5c287ff9457276e4a2106b7a0dc47221f`  
		Last Modified: Tue, 29 Jun 2021 02:53:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb8d5d4b45a9b182593c6f8eecbc172ed4a8a0eda344b11590e38145a5e7814`  
		Last Modified: Tue, 29 Jun 2021 02:53:46 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.6-meta-alpine`

```console
$ docker pull influxdb@sha256:ca1e61a34022562abfd681504f9c15299de25f62d568a3a6cefebd2c7e64c581
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.6-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:05be70bb791eba3706e6508474ca275411194aa09d49e6a5dbb11ffbe4482bac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27306930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc98141e784ebcdd83f60cdda2926428a114858aea72884487f2460cd71aedc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:48:27 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:48:27 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:48:28 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:48:28 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:48:29 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:48:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:30 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a454dabfdc9badc7b06cbadac755be9de59234e022dbd19e0bc02fed5c8379`  
		Last Modified: Tue, 29 Jun 2021 02:54:06 GMT  
		Size: 23.1 MB (23074833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34742c348a4bf98acecce3f2a81f4d7d4ba5d68ac3cb5cf64bb258bc3f088d2`  
		Last Modified: Tue, 29 Jun 2021 02:54:02 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db545df212f2a7d0df6c34a87fb022e869adfacb8aef3c7be3b8b00133790f`  
		Last Modified: Tue, 29 Jun 2021 02:54:02 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data`

```console
$ docker pull influxdb@sha256:828e1637d867e9b13cd86e5634547890ad79e89c1efb3e0f07e6bd7b90a795ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:c714d9bdd4ee40d41b0f889961fe65eab50f57b593f653f41553b8160ea5a126
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125534072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c661805e3faba2843df3c56d5ef01e543d7dbf326bbc3d9a322241506c7233`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:48:36 GMT
ENV INFLUXDB_VERSION=1.9.2-c1.9.2
# Tue, 29 Jun 2021 02:48:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:48:45 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:48:45 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:48:46 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:48:46 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:48:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:48:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b654ad9216f1d8315977074ca494e1f01650641ec571347b67deb87cb1511b22`  
		Last Modified: Tue, 29 Jun 2021 02:54:32 GMT  
		Size: 64.5 MB (64512497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34bfd8f16555b5f8032bd22f772052ec496329dcaec697343dbfcedd8c0d5c5`  
		Last Modified: Tue, 29 Jun 2021 02:54:20 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa965c27f5f683828aeb777d899c08e54e52e256e02e98e34a8b19db8d47967`  
		Last Modified: Tue, 29 Jun 2021 02:54:20 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8711997cf18a6cb632130a030fbb9ceb435e25f00609df23ae4515f1015e881`  
		Last Modified: Tue, 29 Jun 2021 02:54:20 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:f16ef7db372634e3ac3c8b60a49384b111d919ba173496b709fcc8d94893e915
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:20e21dcb30b74922fa4ab1ec3fbff8806b54903db874f844aced1949b6c890a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68708857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc75725e424eaa444ba19c4ca8686afe3e3a4a3e79f066041e61f57a0bee09d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 29 Jun 2021 02:48:52 GMT
ENV INFLUXDB_VERSION=1.9.2-c1.9.2
# Tue, 29 Jun 2021 02:49:05 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:49:05 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:49:06 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:49:06 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:49:07 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:49:08 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:49:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:49:08 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b2661d4ae847f77e6c3d8c6db39d401720974edc39be20e06055fb574b0d61`  
		Last Modified: Tue, 29 Jun 2021 02:54:56 GMT  
		Size: 64.5 MB (64475557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c60158690e6a7eade3d1df8994a39db434fa99ae9573273a3b680013bedb5ef`  
		Last Modified: Tue, 29 Jun 2021 02:54:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ea1affccb8e734e278295edf63085fdf224e5a8f91a23546fa22b83859bbdd`  
		Last Modified: Tue, 29 Jun 2021 02:54:44 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf23ed89958e94de7292610239abb1d987fd8e4edaff7e5fbcd61efd6e0931b`  
		Last Modified: Tue, 29 Jun 2021 02:54:44 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:fa31842985b38ee8e45bd20dcdf1165769dc2c37f8001ddf64775319df7978f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:6061ec68e8e01ed86a6da866f8ec3e79ccd201a90bcfbfbf9d2f1b63f4d0cd9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85600959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d289a68aa5842515a9dce320980bea1ec8eb535aedcd86930339944c57e05731`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:48:36 GMT
ENV INFLUXDB_VERSION=1.9.2-c1.9.2
# Tue, 29 Jun 2021 02:49:21 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:49:22 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:49:22 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:49:23 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:49:23 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:49:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:49:24 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8cc87f7722ce26add0c2c2d887b52f48a7b828fd5ca07248f882a14bf52dc6`  
		Last Modified: Tue, 29 Jun 2021 02:55:10 GMT  
		Size: 24.6 MB (24580588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a36c718fc3f40c0d62d09214e32245b789f014eaa870cdb7f7518530aa8a21d`  
		Last Modified: Tue, 29 Jun 2021 02:55:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c60404204f9681c9b6900f03fe4fabcf7c29b208e5e9fc6f5968cf02172fa19`  
		Last Modified: Tue, 29 Jun 2021 02:55:06 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:83f4f88775034a52b472daffee6b9bcfdba7303112927cb902fc27676fd63075
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:dc6f27ad51ab3b4257d4cbff7285d1ae28958e60be54165e65f1a3c255cc9cf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28781165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad3d046a47d491221bdec239f0a4ae4eee2cf31f3dbb49ccf7483a34895f2e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 29 Jun 2021 02:48:52 GMT
ENV INFLUXDB_VERSION=1.9.2-c1.9.2
# Tue, 29 Jun 2021 02:49:33 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:49:33 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:49:33 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:49:33 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:49:34 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:49:34 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea644f2e6924b15050e8a9603287ff5cc37c5c8ef13d6dfcef8f217deef8a8f`  
		Last Modified: Tue, 29 Jun 2021 02:55:24 GMT  
		Size: 24.5 MB (24549067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9202c1c94dcaa654577dfc221ed19f575c07977ce8b9b375b01e04a459baffe`  
		Last Modified: Tue, 29 Jun 2021 02:55:20 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d2427deaf8a9f6113de6d25c69808aa983e37691dd07c80ebb44eec6294eb1`  
		Last Modified: Tue, 29 Jun 2021 02:55:21 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.2-data`

```console
$ docker pull influxdb@sha256:828e1637d867e9b13cd86e5634547890ad79e89c1efb3e0f07e6bd7b90a795ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.2-data` - linux; amd64

```console
$ docker pull influxdb@sha256:c714d9bdd4ee40d41b0f889961fe65eab50f57b593f653f41553b8160ea5a126
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125534072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c661805e3faba2843df3c56d5ef01e543d7dbf326bbc3d9a322241506c7233`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:48:36 GMT
ENV INFLUXDB_VERSION=1.9.2-c1.9.2
# Tue, 29 Jun 2021 02:48:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:48:45 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:48:45 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:48:46 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:48:46 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:48:47 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:48:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:47 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b654ad9216f1d8315977074ca494e1f01650641ec571347b67deb87cb1511b22`  
		Last Modified: Tue, 29 Jun 2021 02:54:32 GMT  
		Size: 64.5 MB (64512497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34bfd8f16555b5f8032bd22f772052ec496329dcaec697343dbfcedd8c0d5c5`  
		Last Modified: Tue, 29 Jun 2021 02:54:20 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa965c27f5f683828aeb777d899c08e54e52e256e02e98e34a8b19db8d47967`  
		Last Modified: Tue, 29 Jun 2021 02:54:20 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8711997cf18a6cb632130a030fbb9ceb435e25f00609df23ae4515f1015e881`  
		Last Modified: Tue, 29 Jun 2021 02:54:20 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.2-data-alpine`

```console
$ docker pull influxdb@sha256:f16ef7db372634e3ac3c8b60a49384b111d919ba173496b709fcc8d94893e915
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.2-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:20e21dcb30b74922fa4ab1ec3fbff8806b54903db874f844aced1949b6c890a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68708857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc75725e424eaa444ba19c4ca8686afe3e3a4a3e79f066041e61f57a0bee09d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 29 Jun 2021 02:48:52 GMT
ENV INFLUXDB_VERSION=1.9.2-c1.9.2
# Tue, 29 Jun 2021 02:49:05 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:49:05 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:49:06 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:49:06 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:49:07 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:49:08 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:49:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:49:08 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b2661d4ae847f77e6c3d8c6db39d401720974edc39be20e06055fb574b0d61`  
		Last Modified: Tue, 29 Jun 2021 02:54:56 GMT  
		Size: 64.5 MB (64475557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c60158690e6a7eade3d1df8994a39db434fa99ae9573273a3b680013bedb5ef`  
		Last Modified: Tue, 29 Jun 2021 02:54:44 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ea1affccb8e734e278295edf63085fdf224e5a8f91a23546fa22b83859bbdd`  
		Last Modified: Tue, 29 Jun 2021 02:54:44 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf23ed89958e94de7292610239abb1d987fd8e4edaff7e5fbcd61efd6e0931b`  
		Last Modified: Tue, 29 Jun 2021 02:54:44 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.2-meta`

```console
$ docker pull influxdb@sha256:fa31842985b38ee8e45bd20dcdf1165769dc2c37f8001ddf64775319df7978f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.2-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:6061ec68e8e01ed86a6da866f8ec3e79ccd201a90bcfbfbf9d2f1b63f4d0cd9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85600959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d289a68aa5842515a9dce320980bea1ec8eb535aedcd86930339944c57e05731`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:48:36 GMT
ENV INFLUXDB_VERSION=1.9.2-c1.9.2
# Tue, 29 Jun 2021 02:49:21 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:49:22 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:49:22 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:49:23 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:49:23 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:49:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:49:24 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8cc87f7722ce26add0c2c2d887b52f48a7b828fd5ca07248f882a14bf52dc6`  
		Last Modified: Tue, 29 Jun 2021 02:55:10 GMT  
		Size: 24.6 MB (24580588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a36c718fc3f40c0d62d09214e32245b789f014eaa870cdb7f7518530aa8a21d`  
		Last Modified: Tue, 29 Jun 2021 02:55:06 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c60404204f9681c9b6900f03fe4fabcf7c29b208e5e9fc6f5968cf02172fa19`  
		Last Modified: Tue, 29 Jun 2021 02:55:06 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.2-meta-alpine`

```console
$ docker pull influxdb@sha256:83f4f88775034a52b472daffee6b9bcfdba7303112927cb902fc27676fd63075
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.2-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:dc6f27ad51ab3b4257d4cbff7285d1ae28958e60be54165e65f1a3c255cc9cf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28781165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad3d046a47d491221bdec239f0a4ae4eee2cf31f3dbb49ccf7483a34895f2e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Tue, 29 Jun 2021 02:48:52 GMT
ENV INFLUXDB_VERSION=1.9.2-c1.9.2
# Tue, 29 Jun 2021 02:49:33 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:49:33 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:49:33 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:49:33 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:49:34 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:49:34 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea644f2e6924b15050e8a9603287ff5cc37c5c8ef13d6dfcef8f217deef8a8f`  
		Last Modified: Tue, 29 Jun 2021 02:55:24 GMT  
		Size: 24.5 MB (24549067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9202c1c94dcaa654577dfc221ed19f575c07977ce8b9b375b01e04a459baffe`  
		Last Modified: Tue, 29 Jun 2021 02:55:20 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d2427deaf8a9f6113de6d25c69808aa983e37691dd07c80ebb44eec6294eb1`  
		Last Modified: Tue, 29 Jun 2021 02:55:21 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0`

```console
$ docker pull influxdb@sha256:7d6dcce155a3a09d2c29e0d03c8f26514081b730938aab560df3d40044a9a9f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:eb77f0b6b3aa3bd48b85a13901d15ab14f45886139726e62749a26361bb9fad6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178699726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f26c7e4d38bc7c7152149e875c156ea37b264cad7ab9c8dcd870f3b36c56fa4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:52:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:53:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 24 Jun 2021 01:34:12 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 24 Jun 2021 01:34:12 GMT
ENV GOSU_VER=1.12
# Thu, 24 Jun 2021 01:34:16 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Thu, 24 Jun 2021 01:34:16 GMT
ENV INFLUXDB_VERSION=2.0.7
# Thu, 24 Jun 2021 01:34:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Thu, 24 Jun 2021 01:34:24 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 24 Jun 2021 01:34:24 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 24 Jun 2021 01:34:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 24 Jun 2021 01:34:25 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Thu, 24 Jun 2021 01:34:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:25 GMT
CMD ["influxd"]
# Thu, 24 Jun 2021 01:34:25 GMT
EXPOSE 8086
# Thu, 24 Jun 2021 01:34:25 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 24 Jun 2021 01:34:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 24 Jun 2021 01:34:26 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110e58716600c199fc95f633b30735c33a25b5adcfb16d1d7edbcb78a3f1b62`  
		Last Modified: Wed, 23 Jun 2021 01:01:46 GMT  
		Size: 7.8 MB (7832997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c0fa203acbade733bff627daa75b84c97f9d0553bcdf967a3f1d37471277`  
		Last Modified: Wed, 23 Jun 2021 01:01:47 GMT  
		Size: 10.0 MB (9997255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe08b7c7bd34fd2cc223ec3dfd86c583df78662452299ef0b9a600029277aa4`  
		Last Modified: Thu, 24 Jun 2021 01:37:16 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a752c953de6a8c86fd67cb69bc183cdded89c24ed14841e10e7940e368e70e`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 961.0 KB (960991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fee0b4534651e45a7733ad0a8f540ba6fbd8244fe01d2ef2f40de41592d00b`  
		Last Modified: Thu, 24 Jun 2021 01:37:24 GMT  
		Size: 109.5 MB (109466206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d853369c0c65d10005eb5b355804eee81fadd95f33c395921e83bb9dbe45ea`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fd4c49d9b93bd5c6e45ae0d18613bedcdaabaf2d18c8aa29a601ba1f8beefb`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f535b15085d744218e83e7393e9e3b586063a472fa97ed6af28157042b1dcb1`  
		Last Modified: Thu, 24 Jun 2021 01:37:15 GMT  
		Size: 4.3 KB (4316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:d9825b3d372ad663f34bf92a3ebc1b9022906062b06986a0f203c5ab8670fec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180628536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcdad0ed3f5fbd15e87467aad894389fa02f9ecb82c2710bc7bd62d50db96409`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:34:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 23 Jun 2021 18:34:17 GMT
ENV GOSU_VER=1.12
# Wed, 23 Jun 2021 18:34:20 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 23 Jun 2021 18:34:20 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 23 Jun 2021 18:34:28 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 23 Jun 2021 18:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 23 Jun 2021 18:34:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 23 Jun 2021 18:34:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 23 Jun 2021 18:34:30 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 23 Jun 2021 18:34:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:34:30 GMT
CMD ["influxd"]
# Wed, 23 Jun 2021 18:34:30 GMT
EXPOSE 8086
# Wed, 23 Jun 2021 18:34:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b86f0fed5df426869e08ab884f79326e9a310498fb9c49929e08f9ef9002b`  
		Last Modified: Wed, 23 Jun 2021 18:35:51 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f865c284b0e6b32bd1f1dd14ec1e334cbadc7d6292712190efa42f4718b8dd`  
		Last Modified: Wed, 23 Jun 2021 18:35:48 GMT  
		Size: 896.4 KB (896380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea300fef38e2d57c2657aaad371813835137c72d9f2c258e56af5006e4e5797`  
		Last Modified: Wed, 23 Jun 2021 18:36:00 GMT  
		Size: 112.8 MB (112824510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0fc3d9ce52b5368331dd5726abd82bd12ed7c3e8a23a33cdc89f2fbf64ab73`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f091d2bde4f35ffdd2cb09c6e1bdce03228e14e72564adc636b11ddf9829ce`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b9b006308f765debe388af66277c827d88a43a1cc4a90dee951af142b3d1d0`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0-alpine`

```console
$ docker pull influxdb@sha256:7630ad8caae177fe5442cce81068b944c13e2daa7ec289d6d3710b836824cd79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9c2e3774aca3f2ee9675a1e0121836ab6b094f3ff4b2b0fae03dc2dd5c3f8378
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122946151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5ab4e012ccdc738b8b78a3095905324f5e6e785f25dac93203a50321ca2039`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:57:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:57:47 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 14 Apr 2021 22:57:48 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 14 Apr 2021 22:57:49 GMT
ENV GOSU_VER=1.12
# Wed, 14 Apr 2021 22:57:52 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Jun 2021 00:31:40 GMT
ENV INFLUXDB_VERSION=2.0.7
# Sat, 05 Jun 2021 00:31:49 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 05 Jun 2021 00:31:50 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 05 Jun 2021 00:31:50 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Sat, 05 Jun 2021 00:31:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Jun 2021 00:31:51 GMT
CMD ["influxd"]
# Sat, 05 Jun 2021 00:31:51 GMT
EXPOSE 8086
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 05 Jun 2021 00:31:52 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70fcedbcfb9328a87e76b312a1996118fac6b73a1dea800c39df8d00207148`  
		Last Modified: Wed, 14 Apr 2021 23:01:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e50c2af4ce019b31b8f9df4781ebe41c99a903cd661ad9231e08773b029cfec`  
		Last Modified: Wed, 14 Apr 2021 23:01:05 GMT  
		Size: 9.7 MB (9701057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99cdb09e5aee3ab8869581dee7b389f6ebd9507ff9613cbc03683586b99eb96`  
		Last Modified: Wed, 14 Apr 2021 23:00:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4633d963d8e54bd89ef20119577189c164929c6451ec7be1f4cf45d26c3bb283`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 960.6 KB (960616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8520535bd417b8e9823de3f2c784aaa5ee76600551afc6b859eeeba6f96d7687`  
		Last Modified: Sat, 05 Jun 2021 00:33:13 GMT  
		Size: 109.5 MB (109466245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c09337d0dcff42440f468734b71a602c359686958498e9880747a5ab008e47`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d17425d58200c18e5d27020d669313a6da4c073674fa9f07fa9618857b39f3`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67868fd95f4078c1eafb60e477d23b3c44ade51937a76f0854ebe16887fdd33`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4eb31630932f0863ea90024beed6e95ad728eff5ff808ed860a9b6053e69e5ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125980529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e83b89b6cbd0d3cb85dd391739622d356bf8c255c4d79db34aaf80057183bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:52:29 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 16 Jun 2021 00:52:31 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 16 Jun 2021 00:52:32 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Jun 2021 00:52:32 GMT
ENV GOSU_VER=1.12
# Wed, 16 Jun 2021 00:52:35 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Jun 2021 00:52:35 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 16 Jun 2021 00:53:07 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 16 Jun 2021 00:53:08 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Jun 2021 00:53:08 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Jun 2021 00:53:08 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Jun 2021 00:53:09 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 16 Jun 2021 00:53:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Jun 2021 00:53:09 GMT
CMD ["influxd"]
# Wed, 16 Jun 2021 00:53:09 GMT
EXPOSE 8086
# Wed, 16 Jun 2021 00:53:09 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe30e69de6b45dfd810d5a55e1bca8f29e9400e80960f59b78b1b708d4870ce`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db672e7bc210adf1e3b27670230d2aff87b3f7a7010d104a76386659263199a`  
		Last Modified: Wed, 16 Jun 2021 00:53:50 GMT  
		Size: 9.5 MB (9541646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bdc8b41c00d800f0b805f5e77f19a84e2ed27590d2bd4c4c6bd5f0acd42696`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa53e1ed7ae59baa7209d2ea5fc38c68534e7c0874e5049a328d5773fa5fd52`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 896.1 KB (896102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363de3b3909450074472d83e29bdc1ed5bae16c0c7b418d2a6dd3a2fc7a6c4b9`  
		Last Modified: Wed, 16 Jun 2021 00:54:01 GMT  
		Size: 112.8 MB (112824492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5833ddaacbfb7d8dc60578a7fde752675eb2fe1afd84df0aa0e6f79376420237`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b25df44481a6e552072d4a95867ba255251639aaf14ce4541b3556623c8f87`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e1ceabc2f222ffe7be59784f0bfe551e8e322ebe7c1b40967cfb50bb2f30c`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.7`

```console
$ docker pull influxdb@sha256:7d6dcce155a3a09d2c29e0d03c8f26514081b730938aab560df3d40044a9a9f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.7` - linux; amd64

```console
$ docker pull influxdb@sha256:eb77f0b6b3aa3bd48b85a13901d15ab14f45886139726e62749a26361bb9fad6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178699726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f26c7e4d38bc7c7152149e875c156ea37b264cad7ab9c8dcd870f3b36c56fa4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:52:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:53:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 24 Jun 2021 01:34:12 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 24 Jun 2021 01:34:12 GMT
ENV GOSU_VER=1.12
# Thu, 24 Jun 2021 01:34:16 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Thu, 24 Jun 2021 01:34:16 GMT
ENV INFLUXDB_VERSION=2.0.7
# Thu, 24 Jun 2021 01:34:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Thu, 24 Jun 2021 01:34:24 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 24 Jun 2021 01:34:24 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 24 Jun 2021 01:34:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 24 Jun 2021 01:34:25 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Thu, 24 Jun 2021 01:34:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:25 GMT
CMD ["influxd"]
# Thu, 24 Jun 2021 01:34:25 GMT
EXPOSE 8086
# Thu, 24 Jun 2021 01:34:25 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 24 Jun 2021 01:34:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 24 Jun 2021 01:34:26 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110e58716600c199fc95f633b30735c33a25b5adcfb16d1d7edbcb78a3f1b62`  
		Last Modified: Wed, 23 Jun 2021 01:01:46 GMT  
		Size: 7.8 MB (7832997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c0fa203acbade733bff627daa75b84c97f9d0553bcdf967a3f1d37471277`  
		Last Modified: Wed, 23 Jun 2021 01:01:47 GMT  
		Size: 10.0 MB (9997255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe08b7c7bd34fd2cc223ec3dfd86c583df78662452299ef0b9a600029277aa4`  
		Last Modified: Thu, 24 Jun 2021 01:37:16 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a752c953de6a8c86fd67cb69bc183cdded89c24ed14841e10e7940e368e70e`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 961.0 KB (960991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fee0b4534651e45a7733ad0a8f540ba6fbd8244fe01d2ef2f40de41592d00b`  
		Last Modified: Thu, 24 Jun 2021 01:37:24 GMT  
		Size: 109.5 MB (109466206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d853369c0c65d10005eb5b355804eee81fadd95f33c395921e83bb9dbe45ea`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fd4c49d9b93bd5c6e45ae0d18613bedcdaabaf2d18c8aa29a601ba1f8beefb`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f535b15085d744218e83e7393e9e3b586063a472fa97ed6af28157042b1dcb1`  
		Last Modified: Thu, 24 Jun 2021 01:37:15 GMT  
		Size: 4.3 KB (4316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:d9825b3d372ad663f34bf92a3ebc1b9022906062b06986a0f203c5ab8670fec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180628536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcdad0ed3f5fbd15e87467aad894389fa02f9ecb82c2710bc7bd62d50db96409`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:34:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 23 Jun 2021 18:34:17 GMT
ENV GOSU_VER=1.12
# Wed, 23 Jun 2021 18:34:20 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 23 Jun 2021 18:34:20 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 23 Jun 2021 18:34:28 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 23 Jun 2021 18:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 23 Jun 2021 18:34:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 23 Jun 2021 18:34:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 23 Jun 2021 18:34:30 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 23 Jun 2021 18:34:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:34:30 GMT
CMD ["influxd"]
# Wed, 23 Jun 2021 18:34:30 GMT
EXPOSE 8086
# Wed, 23 Jun 2021 18:34:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b86f0fed5df426869e08ab884f79326e9a310498fb9c49929e08f9ef9002b`  
		Last Modified: Wed, 23 Jun 2021 18:35:51 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f865c284b0e6b32bd1f1dd14ec1e334cbadc7d6292712190efa42f4718b8dd`  
		Last Modified: Wed, 23 Jun 2021 18:35:48 GMT  
		Size: 896.4 KB (896380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea300fef38e2d57c2657aaad371813835137c72d9f2c258e56af5006e4e5797`  
		Last Modified: Wed, 23 Jun 2021 18:36:00 GMT  
		Size: 112.8 MB (112824510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0fc3d9ce52b5368331dd5726abd82bd12ed7c3e8a23a33cdc89f2fbf64ab73`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f091d2bde4f35ffdd2cb09c6e1bdce03228e14e72564adc636b11ddf9829ce`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b9b006308f765debe388af66277c827d88a43a1cc4a90dee951af142b3d1d0`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.7-alpine`

```console
$ docker pull influxdb@sha256:7630ad8caae177fe5442cce81068b944c13e2daa7ec289d6d3710b836824cd79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9c2e3774aca3f2ee9675a1e0121836ab6b094f3ff4b2b0fae03dc2dd5c3f8378
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122946151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5ab4e012ccdc738b8b78a3095905324f5e6e785f25dac93203a50321ca2039`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:57:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:57:47 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 14 Apr 2021 22:57:48 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 14 Apr 2021 22:57:49 GMT
ENV GOSU_VER=1.12
# Wed, 14 Apr 2021 22:57:52 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Jun 2021 00:31:40 GMT
ENV INFLUXDB_VERSION=2.0.7
# Sat, 05 Jun 2021 00:31:49 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 05 Jun 2021 00:31:50 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 05 Jun 2021 00:31:50 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Sat, 05 Jun 2021 00:31:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Jun 2021 00:31:51 GMT
CMD ["influxd"]
# Sat, 05 Jun 2021 00:31:51 GMT
EXPOSE 8086
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 05 Jun 2021 00:31:52 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70fcedbcfb9328a87e76b312a1996118fac6b73a1dea800c39df8d00207148`  
		Last Modified: Wed, 14 Apr 2021 23:01:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e50c2af4ce019b31b8f9df4781ebe41c99a903cd661ad9231e08773b029cfec`  
		Last Modified: Wed, 14 Apr 2021 23:01:05 GMT  
		Size: 9.7 MB (9701057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99cdb09e5aee3ab8869581dee7b389f6ebd9507ff9613cbc03683586b99eb96`  
		Last Modified: Wed, 14 Apr 2021 23:00:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4633d963d8e54bd89ef20119577189c164929c6451ec7be1f4cf45d26c3bb283`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 960.6 KB (960616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8520535bd417b8e9823de3f2c784aaa5ee76600551afc6b859eeeba6f96d7687`  
		Last Modified: Sat, 05 Jun 2021 00:33:13 GMT  
		Size: 109.5 MB (109466245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c09337d0dcff42440f468734b71a602c359686958498e9880747a5ab008e47`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d17425d58200c18e5d27020d669313a6da4c073674fa9f07fa9618857b39f3`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67868fd95f4078c1eafb60e477d23b3c44ade51937a76f0854ebe16887fdd33`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.7-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4eb31630932f0863ea90024beed6e95ad728eff5ff808ed860a9b6053e69e5ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125980529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e83b89b6cbd0d3cb85dd391739622d356bf8c255c4d79db34aaf80057183bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:52:29 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 16 Jun 2021 00:52:31 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 16 Jun 2021 00:52:32 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Jun 2021 00:52:32 GMT
ENV GOSU_VER=1.12
# Wed, 16 Jun 2021 00:52:35 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Jun 2021 00:52:35 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 16 Jun 2021 00:53:07 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 16 Jun 2021 00:53:08 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Jun 2021 00:53:08 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Jun 2021 00:53:08 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Jun 2021 00:53:09 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 16 Jun 2021 00:53:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Jun 2021 00:53:09 GMT
CMD ["influxd"]
# Wed, 16 Jun 2021 00:53:09 GMT
EXPOSE 8086
# Wed, 16 Jun 2021 00:53:09 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe30e69de6b45dfd810d5a55e1bca8f29e9400e80960f59b78b1b708d4870ce`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db672e7bc210adf1e3b27670230d2aff87b3f7a7010d104a76386659263199a`  
		Last Modified: Wed, 16 Jun 2021 00:53:50 GMT  
		Size: 9.5 MB (9541646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bdc8b41c00d800f0b805f5e77f19a84e2ed27590d2bd4c4c6bd5f0acd42696`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa53e1ed7ae59baa7209d2ea5fc38c68534e7c0874e5049a328d5773fa5fd52`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 896.1 KB (896102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363de3b3909450074472d83e29bdc1ed5bae16c0c7b418d2a6dd3a2fc7a6c4b9`  
		Last Modified: Wed, 16 Jun 2021 00:54:01 GMT  
		Size: 112.8 MB (112824492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5833ddaacbfb7d8dc60578a7fde752675eb2fe1afd84df0aa0e6f79376420237`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b25df44481a6e552072d4a95867ba255251639aaf14ce4541b3556623c8f87`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e1ceabc2f222ffe7be59784f0bfe551e8e322ebe7c1b40967cfb50bb2f30c`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:7630ad8caae177fe5442cce81068b944c13e2daa7ec289d6d3710b836824cd79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9c2e3774aca3f2ee9675a1e0121836ab6b094f3ff4b2b0fae03dc2dd5c3f8378
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122946151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5ab4e012ccdc738b8b78a3095905324f5e6e785f25dac93203a50321ca2039`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:57:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:57:47 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 14 Apr 2021 22:57:48 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 14 Apr 2021 22:57:49 GMT
ENV GOSU_VER=1.12
# Wed, 14 Apr 2021 22:57:52 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Jun 2021 00:31:40 GMT
ENV INFLUXDB_VERSION=2.0.7
# Sat, 05 Jun 2021 00:31:49 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 05 Jun 2021 00:31:50 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 05 Jun 2021 00:31:50 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 05 Jun 2021 00:31:50 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Sat, 05 Jun 2021 00:31:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Jun 2021 00:31:51 GMT
CMD ["influxd"]
# Sat, 05 Jun 2021 00:31:51 GMT
EXPOSE 8086
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 05 Jun 2021 00:31:51 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 05 Jun 2021 00:31:52 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70fcedbcfb9328a87e76b312a1996118fac6b73a1dea800c39df8d00207148`  
		Last Modified: Wed, 14 Apr 2021 23:01:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e50c2af4ce019b31b8f9df4781ebe41c99a903cd661ad9231e08773b029cfec`  
		Last Modified: Wed, 14 Apr 2021 23:01:05 GMT  
		Size: 9.7 MB (9701057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99cdb09e5aee3ab8869581dee7b389f6ebd9507ff9613cbc03683586b99eb96`  
		Last Modified: Wed, 14 Apr 2021 23:00:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4633d963d8e54bd89ef20119577189c164929c6451ec7be1f4cf45d26c3bb283`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 960.6 KB (960616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8520535bd417b8e9823de3f2c784aaa5ee76600551afc6b859eeeba6f96d7687`  
		Last Modified: Sat, 05 Jun 2021 00:33:13 GMT  
		Size: 109.5 MB (109466245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c09337d0dcff42440f468734b71a602c359686958498e9880747a5ab008e47`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d17425d58200c18e5d27020d669313a6da4c073674fa9f07fa9618857b39f3`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67868fd95f4078c1eafb60e477d23b3c44ade51937a76f0854ebe16887fdd33`  
		Last Modified: Sat, 05 Jun 2021 00:33:03 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4eb31630932f0863ea90024beed6e95ad728eff5ff808ed860a9b6053e69e5ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125980529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e83b89b6cbd0d3cb85dd391739622d356bf8c255c4d79db34aaf80057183bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:52:29 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 16 Jun 2021 00:52:31 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 16 Jun 2021 00:52:32 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 16 Jun 2021 00:52:32 GMT
ENV GOSU_VER=1.12
# Wed, 16 Jun 2021 00:52:35 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Jun 2021 00:52:35 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 16 Jun 2021 00:53:07 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 16 Jun 2021 00:53:08 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 16 Jun 2021 00:53:08 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 16 Jun 2021 00:53:08 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 16 Jun 2021 00:53:09 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 16 Jun 2021 00:53:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Jun 2021 00:53:09 GMT
CMD ["influxd"]
# Wed, 16 Jun 2021 00:53:09 GMT
EXPOSE 8086
# Wed, 16 Jun 2021 00:53:09 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 16 Jun 2021 00:53:10 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe30e69de6b45dfd810d5a55e1bca8f29e9400e80960f59b78b1b708d4870ce`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db672e7bc210adf1e3b27670230d2aff87b3f7a7010d104a76386659263199a`  
		Last Modified: Wed, 16 Jun 2021 00:53:50 GMT  
		Size: 9.5 MB (9541646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bdc8b41c00d800f0b805f5e77f19a84e2ed27590d2bd4c4c6bd5f0acd42696`  
		Last Modified: Wed, 16 Jun 2021 00:53:48 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa53e1ed7ae59baa7209d2ea5fc38c68534e7c0874e5049a328d5773fa5fd52`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 896.1 KB (896102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363de3b3909450074472d83e29bdc1ed5bae16c0c7b418d2a6dd3a2fc7a6c4b9`  
		Last Modified: Wed, 16 Jun 2021 00:54:01 GMT  
		Size: 112.8 MB (112824492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5833ddaacbfb7d8dc60578a7fde752675eb2fe1afd84df0aa0e6f79376420237`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b25df44481a6e552072d4a95867ba255251639aaf14ce4541b3556623c8f87`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e1ceabc2f222ffe7be59784f0bfe551e8e322ebe7c1b40967cfb50bb2f30c`  
		Last Modified: Wed, 16 Jun 2021 00:53:46 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:4fb0dfef21ec768d604daa11c79353813af0f6bd7cc9c0f8d8829129254bc353
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:3e1303bc26c2b90eed88a89f1956a861085ee58a766cff8c4435a4129b21ffee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127804266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2883ca6aac47f1258dd7992e6b903d9a20198641207c23ca397f6423e2cae30c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:47:36 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:47:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:47:44 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:47:45 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:47:45 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:45 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:45 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:47:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:47:46 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2484aa1c72408db7db17fa7189dd8c9dbfc4ed0e8f5c0ccaf40d895b5beb35b4`  
		Last Modified: Tue, 29 Jun 2021 02:53:10 GMT  
		Size: 66.8 MB (66782689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44340132df85be8500d6ed41e6c2a3b02ac4e15b60baeb764a385fe005f0beb`  
		Last Modified: Tue, 29 Jun 2021 02:53:00 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd26a07fb714838a75eec2248ff9247c84f3ee812c405e7ed2497b147dbe6323`  
		Last Modified: Tue, 29 Jun 2021 02:53:00 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e865b0393dce51a350a72ba0cc6106fc12bd632a114a9d0e18185e1bae23f36a`  
		Last Modified: Tue, 29 Jun 2021 02:53:00 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:5d7984b19ebeae696e3a72d0d3be4d8f8ae98a26a059c30cd514d7327b328a1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:e84363979b5ea93eb60066bdc93d41b14d17c4f34b1f9f01f64b5fbe726df1cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70748308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e4a2b986dd07e77d8096bc74a754722028e44638e034361d54b091bf393c3cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:47:56 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:47:57 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Tue, 29 Jun 2021 02:47:57 GMT
EXPOSE 8086
# Tue, 29 Jun 2021 02:47:58 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:47:59 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:47:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 29 Jun 2021 02:47:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97a8d8f09c90b1a78add4731e617075475228aa15ebd842f786082506157d4b`  
		Last Modified: Tue, 29 Jun 2021 02:53:33 GMT  
		Size: 66.5 MB (66515006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b888d7236b6084c80f45090dcc6b19a6c5ea223bb98fabfe8c28c1f1720e016`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0257283109ba2c40cae5ec75d6b30432c2b68de3ff5d79273c97cde6a6cc9c1`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446dae2e30b64005cca683af402f69f5c94573556a3ec08cd3784bd7069f74df`  
		Last Modified: Tue, 29 Jun 2021 02:53:23 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:7d6dcce155a3a09d2c29e0d03c8f26514081b730938aab560df3d40044a9a9f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:eb77f0b6b3aa3bd48b85a13901d15ab14f45886139726e62749a26361bb9fad6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178699726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f26c7e4d38bc7c7152149e875c156ea37b264cad7ab9c8dcd870f3b36c56fa4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:52:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:53:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 24 Jun 2021 01:34:12 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 24 Jun 2021 01:34:12 GMT
ENV GOSU_VER=1.12
# Thu, 24 Jun 2021 01:34:16 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Thu, 24 Jun 2021 01:34:16 GMT
ENV INFLUXDB_VERSION=2.0.7
# Thu, 24 Jun 2021 01:34:23 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Thu, 24 Jun 2021 01:34:24 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 24 Jun 2021 01:34:24 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 24 Jun 2021 01:34:24 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 24 Jun 2021 01:34:25 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Thu, 24 Jun 2021 01:34:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:25 GMT
CMD ["influxd"]
# Thu, 24 Jun 2021 01:34:25 GMT
EXPOSE 8086
# Thu, 24 Jun 2021 01:34:25 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 24 Jun 2021 01:34:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 24 Jun 2021 01:34:26 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110e58716600c199fc95f633b30735c33a25b5adcfb16d1d7edbcb78a3f1b62`  
		Last Modified: Wed, 23 Jun 2021 01:01:46 GMT  
		Size: 7.8 MB (7832997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c0fa203acbade733bff627daa75b84c97f9d0553bcdf967a3f1d37471277`  
		Last Modified: Wed, 23 Jun 2021 01:01:47 GMT  
		Size: 10.0 MB (9997255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe08b7c7bd34fd2cc223ec3dfd86c583df78662452299ef0b9a600029277aa4`  
		Last Modified: Thu, 24 Jun 2021 01:37:16 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a752c953de6a8c86fd67cb69bc183cdded89c24ed14841e10e7940e368e70e`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 961.0 KB (960991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fee0b4534651e45a7733ad0a8f540ba6fbd8244fe01d2ef2f40de41592d00b`  
		Last Modified: Thu, 24 Jun 2021 01:37:24 GMT  
		Size: 109.5 MB (109466206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d853369c0c65d10005eb5b355804eee81fadd95f33c395921e83bb9dbe45ea`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fd4c49d9b93bd5c6e45ae0d18613bedcdaabaf2d18c8aa29a601ba1f8beefb`  
		Last Modified: Thu, 24 Jun 2021 01:37:14 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f535b15085d744218e83e7393e9e3b586063a472fa97ed6af28157042b1dcb1`  
		Last Modified: Thu, 24 Jun 2021 01:37:15 GMT  
		Size: 4.3 KB (4316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:d9825b3d372ad663f34bf92a3ebc1b9022906062b06986a0f203c5ab8670fec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180628536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcdad0ed3f5fbd15e87467aad894389fa02f9ecb82c2710bc7bd62d50db96409`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 18:34:17 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 23 Jun 2021 18:34:17 GMT
ENV GOSU_VER=1.12
# Wed, 23 Jun 2021 18:34:20 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 23 Jun 2021 18:34:20 GMT
ENV INFLUXDB_VERSION=2.0.7
# Wed, 23 Jun 2021 18:34:28 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 23 Jun 2021 18:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 23 Jun 2021 18:34:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 23 Jun 2021 18:34:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 23 Jun 2021 18:34:30 GMT
COPY file:aed864fe2ff542ad0befc1e02894ef6f2c81f22dcc9d0048882c779bb7c1fcd8 in /entrypoint.sh 
# Wed, 23 Jun 2021 18:34:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Jun 2021 18:34:30 GMT
CMD ["influxd"]
# Wed, 23 Jun 2021 18:34:30 GMT
EXPOSE 8086
# Wed, 23 Jun 2021 18:34:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 23 Jun 2021 18:34:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b86f0fed5df426869e08ab884f79326e9a310498fb9c49929e08f9ef9002b`  
		Last Modified: Wed, 23 Jun 2021 18:35:51 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f865c284b0e6b32bd1f1dd14ec1e334cbadc7d6292712190efa42f4718b8dd`  
		Last Modified: Wed, 23 Jun 2021 18:35:48 GMT  
		Size: 896.4 KB (896380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea300fef38e2d57c2657aaad371813835137c72d9f2c258e56af5006e4e5797`  
		Last Modified: Wed, 23 Jun 2021 18:36:00 GMT  
		Size: 112.8 MB (112824510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0fc3d9ce52b5368331dd5726abd82bd12ed7c3e8a23a33cdc89f2fbf64ab73`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f091d2bde4f35ffdd2cb09c6e1bdce03228e14e72564adc636b11ddf9829ce`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b9b006308f765debe388af66277c827d88a43a1cc4a90dee951af142b3d1d0`  
		Last Modified: Wed, 23 Jun 2021 18:35:47 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:81b0672b04d307d8d82d5d129dd6beaf90041bb024e9cb4e0c24ef267ce7e2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:be294edf8c9a733ae7f26f34033175a589be9a7f2134598e880af2215364dc30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84226320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6ac069304e5cf8fa2a2e01cb6ac5a02021451b00c126089e7656aa49c487d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Jun 2021 02:45:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Jun 2021 02:47:36 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:48:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Tue, 29 Jun 2021 02:48:12 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:48:13 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:48:13 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:48:14 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:48:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:14 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53c08fc236dd31803b3edc0786cc3311441a845a4b831b448f27bf55ffe3aa`  
		Last Modified: Tue, 29 Jun 2021 02:50:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9de407994c8853a1596a41ee0ced55922407313243da6ba18b9d9d11025802`  
		Last Modified: Tue, 29 Jun 2021 02:53:49 GMT  
		Size: 23.2 MB (23205949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48295ea472331c2f682539b6c3baeae5c287ff9457276e4a2106b7a0dc47221f`  
		Last Modified: Tue, 29 Jun 2021 02:53:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb8d5d4b45a9b182593c6f8eecbc172ed4a8a0eda344b11590e38145a5e7814`  
		Last Modified: Tue, 29 Jun 2021 02:53:46 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:ca1e61a34022562abfd681504f9c15299de25f62d568a3a6cefebd2c7e64c581
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:05be70bb791eba3706e6508474ca275411194aa09d49e6a5dbb11ffbe4482bac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27306930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc98141e784ebcdd83f60cdda2926428a114858aea72884487f2460cd71aedc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 24 May 2021 19:21:17 GMT
ENV INFLUXDB_VERSION=1.8.6-c1.8.6
# Tue, 29 Jun 2021 02:48:27 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 29 Jun 2021 02:48:27 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Tue, 29 Jun 2021 02:48:28 GMT
EXPOSE 8091
# Tue, 29 Jun 2021 02:48:28 GMT
VOLUME [/var/lib/influxdb]
# Tue, 29 Jun 2021 02:48:29 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Tue, 29 Jun 2021 02:48:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:48:30 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a454dabfdc9badc7b06cbadac755be9de59234e022dbd19e0bc02fed5c8379`  
		Last Modified: Tue, 29 Jun 2021 02:54:06 GMT  
		Size: 23.1 MB (23074833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34742c348a4bf98acecce3f2a81f4d7d4ba5d68ac3cb5cf64bb258bc3f088d2`  
		Last Modified: Tue, 29 Jun 2021 02:54:02 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db545df212f2a7d0df6c34a87fb022e869adfacb8aef3c7be3b8b00133790f`  
		Last Modified: Tue, 29 Jun 2021 02:54:02 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
