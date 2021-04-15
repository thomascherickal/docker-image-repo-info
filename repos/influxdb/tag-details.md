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
$ docker pull influxdb@sha256:847147c8462879296fc5c770eec56f83ecf0b7e855034e5fdbf297c751fb1234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7` - linux; amd64

```console
$ docker pull influxdb@sha256:544776c82cba2072999e3d450b01a3920979ef9021560ca27890257a22feaafd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122298578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9fc0838f1aeee7051a433a8c090aec1a4678e3653e97fbb57a70e3508e1a47`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:13:40 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 10 Apr 2021 19:13:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 19:13:45 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 19:13:45 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:13:46 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:13:46 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:13:46 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 19:13:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:13:46 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae77db513abc12894d4d9788c11d0d0403adeac2022b0f847d1f4defdc80754c`  
		Last Modified: Sat, 10 Apr 2021 19:16:07 GMT  
		Size: 61.3 MB (61285139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eaae51f0ee2efa3035e6e4e73585501c61955ef0ebdb4a4adc4dd0dae7310a`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe2cb523d09fe04648a473b55b436a7923163529508a92feedcd28ac5db93f7`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239ec67286145b6f876712d35d328912c7e9c2fada69d4928d53059603f924a0`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:2bdf61ce964ab9644383d1136d74efe2f585fe3b0c725c131a00160a489c1321
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113454991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e51bd3a8e0dd6d6708ad5f4a028227dbbb051181e0c6db3492dcb0678dc6a2f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:02:42 GMT
ADD file:4c101c517b88a8d25a4997ab4d938ea50aaa265c7f88a4e63edaaed37d89a288 in / 
# Sat, 10 Apr 2021 01:02:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:12:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:16:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:16:42 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 10 Apr 2021 22:16:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 22:16:54 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 22:16:56 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 22:16:57 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 22:16:58 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 22:16:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 22:17:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:17:01 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:533b099902e847172558070703785f6c70f0c6912fefcfd283f3b0e3ebc306c5`  
		Last Modified: Sat, 10 Apr 2021 01:10:12 GMT  
		Size: 42.1 MB (42120304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba1eda48434fdafc900e072c3d26755397eb33edd3403430befc06bf5ebfe0d`  
		Last Modified: Sat, 10 Apr 2021 06:22:42 GMT  
		Size: 9.9 MB (9939854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436419ab83cc68fde8e9c3d51a90fcb8c9874db9093ff594532fd4f5f4e54b8`  
		Last Modified: Sat, 10 Apr 2021 06:22:40 GMT  
		Size: 3.9 MB (3921286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76140bc19f592b5201423519222671e95abc93c446dbf7b6f920df2916214565`  
		Last Modified: Sat, 10 Apr 2021 22:17:48 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a11faa62a7a7ac6124e369ee568ba0ca004fff7af16f36713bf2685dfc99415`  
		Last Modified: Sat, 10 Apr 2021 22:18:03 GMT  
		Size: 57.5 MB (57468974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0315a5599687eb2abaa5c82e61345ebb323c1b377a6fd5cb4fb0c8a5b688990`  
		Last Modified: Sat, 10 Apr 2021 22:17:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e762cf6bcb022e8ff42c861003fdd860a5398be4f3faeb242418909f864a8c2`  
		Last Modified: Sat, 10 Apr 2021 22:17:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f82ee79cc1bd245202764e7804d79529dac377ac0b7ec7541571204a7f8666f`  
		Last Modified: Sat, 10 Apr 2021 22:17:48 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a10406e70a6e58cb9e533fa1048c312efd9159091dd9c6727bc94743eb19d33a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114684333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21d336354a3206d783d2d1f975a9b68b49c4e6b7f08c2a97e0e010731baf3b4a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 00:43:48 GMT
ADD file:64990d14743657dbcbe885739e43ac964a0239a63e4693e6401b0884ab96e09b in / 
# Sat, 10 Apr 2021 00:43:50 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:53:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:53:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:57:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:57:12 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 10 Apr 2021 22:57:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 22:57:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 22:57:31 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 22:57:32 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 22:57:33 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 22:57:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 22:57:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:57:36 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:30bd672115ff6f225cb98d2d7f1ed62feb72c2612297b2ac615e762e436c64ec`  
		Last Modified: Sat, 10 Apr 2021 00:49:51 GMT  
		Size: 43.2 MB (43177772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7d38e5813e5a59ee1d86fb1c7c8c344342d0ec418aa440509260354958f9ad`  
		Last Modified: Sat, 10 Apr 2021 02:03:48 GMT  
		Size: 10.2 MB (10200972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8ce7d8aff50ac8c0f7baa508791ea69df0fa3c7dac0ab9be8933ce3ef5b68a`  
		Last Modified: Sat, 10 Apr 2021 02:03:46 GMT  
		Size: 4.1 MB (4096630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6013e6f034ca76b4efc42a5079012e11dad3a296baf967d6e2ef766c3442442c`  
		Last Modified: Sat, 10 Apr 2021 22:59:15 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04935672804428b7b97325b57c115d38f1eef01b9d0c874896a079297f4fac6`  
		Last Modified: Sat, 10 Apr 2021 22:59:28 GMT  
		Size: 57.2 MB (57204390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076a26cb6b257f5fa3e187a02fb22e00267966bca355899376e6140c6ec48db9`  
		Last Modified: Sat, 10 Apr 2021 22:59:15 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2333a8aacf455e188976c61e327967e9d77536e7ec9120c4700cc3406040ec`  
		Last Modified: Sat, 10 Apr 2021 22:59:15 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c95d8eecb3ef06697a51e4079f961cdacfd0c43e022b211b710aca4d1306bb`  
		Last Modified: Sat, 10 Apr 2021 22:59:15 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-alpine`

```console
$ docker pull influxdb@sha256:019ffe9b1959d8a9a96ecb4d508e22024a0747008029265179be02b19b9c907d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:497cc2e6dd209b9cded65e0189ff389060f2786e7f2f1666889026a8beb0135d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65268062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a2f90d367a1c53920888d296e840fd0924b4b2f020ed4afd70ebab0fd4084d`
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
# Wed, 14 Apr 2021 22:56:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:56:26 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:56:26 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:56:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:27 GMT
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
	-	`sha256:ffdfcbb00141ab55c6d38419b5322b874030c5aa73d693a598a2b28ce0e17081`  
		Last Modified: Wed, 14 Apr 2021 22:58:49 GMT  
		Size: 61.0 MB (61034818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19c2e634090909c8b92a0bc6963538e530570f798f2d9fed2be84648f6e66df`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512843e4c495158d090efbaa5625e4123a8aa5978df645e3a86e941f2c478a8`  
		Last Modified: Wed, 14 Apr 2021 22:58:44 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd288200021e8c620e82728a414657c33d78a2bd6f17adc456286e2c471c362`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data`

```console
$ docker pull influxdb@sha256:c3648bf88b6cee96637aef84f857892fc793326150858f7f214df35db7d5404c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:59da322423db1c9f38eeb4002c35df9a2464619c195db486994ac218a6852f1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148962533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27a3354ed96eef80a982383b7057a9a1eb3b13100b37adef5c4b0a95d3fbe79a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:13:54 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 10 Apr 2021 19:14:02 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 10 Apr 2021 19:14:03 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 19:14:03 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:14:03 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:03 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:03 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 19:14:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:04 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d2e86252bcf84f1adfcd498c12b4c08050deb888663760ac66f87d514dde12`  
		Last Modified: Sat, 10 Apr 2021 19:16:47 GMT  
		Size: 87.9 MB (87949035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95aa55e40f4f1dd8861b61195f1b5c3eb8dfd7dd26ada5c2c9102257f97897`  
		Last Modified: Sat, 10 Apr 2021 19:16:32 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0525a0472de3c0091b4e3e85c8ac55cc2eabf9a14823c7aee210e772dc7a5edc`  
		Last Modified: Sat, 10 Apr 2021 19:16:32 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa08ba23218161de62dec1cfb78c16035fc5e32cd65c6873843aee448707d9fe`  
		Last Modified: Sat, 10 Apr 2021 19:16:33 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data-alpine`

```console
$ docker pull influxdb@sha256:953218e27826969473de77140a6e8e36635bc9598fb53e87520da576a4714697
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:59f66a260ca6ac25da45231834f1ba1f5cbd13db57112b39a1eaf3d89418eb1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91872207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6de1bd45ba333a7fa2b42d112e649986e5df7ccfb6e5d61b4708ed0c96a95770`
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
# Wed, 14 Apr 2021 22:56:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:42 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:56:42 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:56:43 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:43 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:43 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:56:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:43 GMT
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
	-	`sha256:50d72c8962115b8fbd20d5a78dd48e575abcd35f896096c95e0b579a8dbd4336`  
		Last Modified: Wed, 14 Apr 2021 22:59:12 GMT  
		Size: 87.6 MB (87638906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0493fd864febd60f65cd5502bd7fcba1d872989c033068c72632717ea9b5137c`  
		Last Modified: Wed, 14 Apr 2021 22:59:01 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd7b30f761adf01ac672b68e8634efcdbcaed5cadd4e8fd9b997c0537ec7a65`  
		Last Modified: Wed, 14 Apr 2021 22:59:00 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0880938167776dea94134027e0bc04f2f881b2fab628ec37a41a325af8ed0`  
		Last Modified: Wed, 14 Apr 2021 22:59:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta`

```console
$ docker pull influxdb@sha256:337aea983f3da7180d365cc11cc6f3aca6d53f24a0c78ab30cff639d6cce5061
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:2905d77f1445f3175b67862a9bb9488c523667871574234e45dea19dd50fa008
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.1 MB (84145902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06f271e73df348c6da1b34fa2c785a9f756964b50eba1b7fade6a83816033b8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:13:54 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 10 Apr 2021 19:14:14 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 10 Apr 2021 19:14:14 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 10 Apr 2021 19:14:14 GMT
EXPOSE 8091
# Sat, 10 Apr 2021 19:14:14 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:14 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:15 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eeaf8f6e64ce1140bd91c25b04410ff3be1f9dd7496b959bbfbf4810a10a0df`  
		Last Modified: Sat, 10 Apr 2021 19:17:02 GMT  
		Size: 23.1 MB (23133610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bd3fa1a024ea76e33e00251ca3a55fdad98865d6fc87802a1352e40d49e2`  
		Last Modified: Sat, 10 Apr 2021 19:16:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e423aede590af38b52c626f7f97d3b585aef872e84115b5d9c4adabd0309979`  
		Last Modified: Sat, 10 Apr 2021 19:16:59 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta-alpine`

```console
$ docker pull influxdb@sha256:f997194721a978be18e2db6310fc4f20d4e8ae1a13158de1cd7dc6b042ebe98b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:88915c86ce7afd69b101ba5a4dd8d1dfce23bfa760dd74fbb8fec36b562a3909
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27235086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0485099136dd77a780e637f002a9399df5468f2609d126e85c977208798adaac`
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
# Wed, 14 Apr 2021 22:56:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:55 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 14 Apr 2021 22:56:55 GMT
EXPOSE 8091
# Wed, 14 Apr 2021 22:56:55 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:55 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:56 GMT
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
	-	`sha256:1b8177497e45bcdf4f69a9c9e31aa09286c8157b7e3918ca418f2a8792b98791`  
		Last Modified: Wed, 14 Apr 2021 22:59:27 GMT  
		Size: 23.0 MB (23002988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ea6921490482ed769782ef5ab560e586b844b845bd40314224130d55910a45`  
		Last Modified: Wed, 14 Apr 2021 22:59:24 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bb5766ed91f5ba3565a638433f21786c10951ed30c32133153d1e11a7826c0`  
		Last Modified: Wed, 14 Apr 2021 22:59:28 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11`

```console
$ docker pull influxdb@sha256:847147c8462879296fc5c770eec56f83ecf0b7e855034e5fdbf297c751fb1234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7.11` - linux; amd64

```console
$ docker pull influxdb@sha256:544776c82cba2072999e3d450b01a3920979ef9021560ca27890257a22feaafd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122298578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9fc0838f1aeee7051a433a8c090aec1a4678e3653e97fbb57a70e3508e1a47`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:13:40 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 10 Apr 2021 19:13:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 19:13:45 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 19:13:45 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:13:46 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:13:46 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:13:46 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 19:13:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:13:46 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae77db513abc12894d4d9788c11d0d0403adeac2022b0f847d1f4defdc80754c`  
		Last Modified: Sat, 10 Apr 2021 19:16:07 GMT  
		Size: 61.3 MB (61285139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eaae51f0ee2efa3035e6e4e73585501c61955ef0ebdb4a4adc4dd0dae7310a`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe2cb523d09fe04648a473b55b436a7923163529508a92feedcd28ac5db93f7`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239ec67286145b6f876712d35d328912c7e9c2fada69d4928d53059603f924a0`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:2bdf61ce964ab9644383d1136d74efe2f585fe3b0c725c131a00160a489c1321
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113454991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e51bd3a8e0dd6d6708ad5f4a028227dbbb051181e0c6db3492dcb0678dc6a2f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:02:42 GMT
ADD file:4c101c517b88a8d25a4997ab4d938ea50aaa265c7f88a4e63edaaed37d89a288 in / 
# Sat, 10 Apr 2021 01:02:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:12:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:16:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:16:42 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 10 Apr 2021 22:16:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 22:16:54 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 22:16:56 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 22:16:57 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 22:16:58 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 22:16:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 22:17:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:17:01 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:533b099902e847172558070703785f6c70f0c6912fefcfd283f3b0e3ebc306c5`  
		Last Modified: Sat, 10 Apr 2021 01:10:12 GMT  
		Size: 42.1 MB (42120304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba1eda48434fdafc900e072c3d26755397eb33edd3403430befc06bf5ebfe0d`  
		Last Modified: Sat, 10 Apr 2021 06:22:42 GMT  
		Size: 9.9 MB (9939854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436419ab83cc68fde8e9c3d51a90fcb8c9874db9093ff594532fd4f5f4e54b8`  
		Last Modified: Sat, 10 Apr 2021 06:22:40 GMT  
		Size: 3.9 MB (3921286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76140bc19f592b5201423519222671e95abc93c446dbf7b6f920df2916214565`  
		Last Modified: Sat, 10 Apr 2021 22:17:48 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a11faa62a7a7ac6124e369ee568ba0ca004fff7af16f36713bf2685dfc99415`  
		Last Modified: Sat, 10 Apr 2021 22:18:03 GMT  
		Size: 57.5 MB (57468974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0315a5599687eb2abaa5c82e61345ebb323c1b377a6fd5cb4fb0c8a5b688990`  
		Last Modified: Sat, 10 Apr 2021 22:17:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e762cf6bcb022e8ff42c861003fdd860a5398be4f3faeb242418909f864a8c2`  
		Last Modified: Sat, 10 Apr 2021 22:17:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f82ee79cc1bd245202764e7804d79529dac377ac0b7ec7541571204a7f8666f`  
		Last Modified: Sat, 10 Apr 2021 22:17:48 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:a10406e70a6e58cb9e533fa1048c312efd9159091dd9c6727bc94743eb19d33a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114684333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21d336354a3206d783d2d1f975a9b68b49c4e6b7f08c2a97e0e010731baf3b4a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 00:43:48 GMT
ADD file:64990d14743657dbcbe885739e43ac964a0239a63e4693e6401b0884ab96e09b in / 
# Sat, 10 Apr 2021 00:43:50 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:53:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:53:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:57:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:57:12 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 10 Apr 2021 22:57:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 22:57:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 22:57:31 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 22:57:32 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 22:57:33 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 22:57:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 22:57:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:57:36 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:30bd672115ff6f225cb98d2d7f1ed62feb72c2612297b2ac615e762e436c64ec`  
		Last Modified: Sat, 10 Apr 2021 00:49:51 GMT  
		Size: 43.2 MB (43177772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7d38e5813e5a59ee1d86fb1c7c8c344342d0ec418aa440509260354958f9ad`  
		Last Modified: Sat, 10 Apr 2021 02:03:48 GMT  
		Size: 10.2 MB (10200972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8ce7d8aff50ac8c0f7baa508791ea69df0fa3c7dac0ab9be8933ce3ef5b68a`  
		Last Modified: Sat, 10 Apr 2021 02:03:46 GMT  
		Size: 4.1 MB (4096630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6013e6f034ca76b4efc42a5079012e11dad3a296baf967d6e2ef766c3442442c`  
		Last Modified: Sat, 10 Apr 2021 22:59:15 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04935672804428b7b97325b57c115d38f1eef01b9d0c874896a079297f4fac6`  
		Last Modified: Sat, 10 Apr 2021 22:59:28 GMT  
		Size: 57.2 MB (57204390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076a26cb6b257f5fa3e187a02fb22e00267966bca355899376e6140c6ec48db9`  
		Last Modified: Sat, 10 Apr 2021 22:59:15 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2333a8aacf455e188976c61e327967e9d77536e7ec9120c4700cc3406040ec`  
		Last Modified: Sat, 10 Apr 2021 22:59:15 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c95d8eecb3ef06697a51e4079f961cdacfd0c43e022b211b710aca4d1306bb`  
		Last Modified: Sat, 10 Apr 2021 22:59:15 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-alpine`

```console
$ docker pull influxdb@sha256:019ffe9b1959d8a9a96ecb4d508e22024a0747008029265179be02b19b9c907d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:497cc2e6dd209b9cded65e0189ff389060f2786e7f2f1666889026a8beb0135d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65268062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a2f90d367a1c53920888d296e840fd0924b4b2f020ed4afd70ebab0fd4084d`
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
# Wed, 14 Apr 2021 22:56:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:56:26 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:56:26 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:56:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:27 GMT
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
	-	`sha256:ffdfcbb00141ab55c6d38419b5322b874030c5aa73d693a598a2b28ce0e17081`  
		Last Modified: Wed, 14 Apr 2021 22:58:49 GMT  
		Size: 61.0 MB (61034818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19c2e634090909c8b92a0bc6963538e530570f798f2d9fed2be84648f6e66df`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512843e4c495158d090efbaa5625e4123a8aa5978df645e3a86e941f2c478a8`  
		Last Modified: Wed, 14 Apr 2021 22:58:44 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd288200021e8c620e82728a414657c33d78a2bd6f17adc456286e2c471c362`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data`

```console
$ docker pull influxdb@sha256:c3648bf88b6cee96637aef84f857892fc793326150858f7f214df35db7d5404c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:59da322423db1c9f38eeb4002c35df9a2464619c195db486994ac218a6852f1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148962533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27a3354ed96eef80a982383b7057a9a1eb3b13100b37adef5c4b0a95d3fbe79a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:13:54 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 10 Apr 2021 19:14:02 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 10 Apr 2021 19:14:03 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 19:14:03 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:14:03 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:03 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:03 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 19:14:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:04 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d2e86252bcf84f1adfcd498c12b4c08050deb888663760ac66f87d514dde12`  
		Last Modified: Sat, 10 Apr 2021 19:16:47 GMT  
		Size: 87.9 MB (87949035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95aa55e40f4f1dd8861b61195f1b5c3eb8dfd7dd26ada5c2c9102257f97897`  
		Last Modified: Sat, 10 Apr 2021 19:16:32 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0525a0472de3c0091b4e3e85c8ac55cc2eabf9a14823c7aee210e772dc7a5edc`  
		Last Modified: Sat, 10 Apr 2021 19:16:32 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa08ba23218161de62dec1cfb78c16035fc5e32cd65c6873843aee448707d9fe`  
		Last Modified: Sat, 10 Apr 2021 19:16:33 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data-alpine`

```console
$ docker pull influxdb@sha256:953218e27826969473de77140a6e8e36635bc9598fb53e87520da576a4714697
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:59f66a260ca6ac25da45231834f1ba1f5cbd13db57112b39a1eaf3d89418eb1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91872207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6de1bd45ba333a7fa2b42d112e649986e5df7ccfb6e5d61b4708ed0c96a95770`
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
# Wed, 14 Apr 2021 22:56:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:42 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:56:42 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:56:43 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:43 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:43 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:56:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:43 GMT
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
	-	`sha256:50d72c8962115b8fbd20d5a78dd48e575abcd35f896096c95e0b579a8dbd4336`  
		Last Modified: Wed, 14 Apr 2021 22:59:12 GMT  
		Size: 87.6 MB (87638906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0493fd864febd60f65cd5502bd7fcba1d872989c033068c72632717ea9b5137c`  
		Last Modified: Wed, 14 Apr 2021 22:59:01 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd7b30f761adf01ac672b68e8634efcdbcaed5cadd4e8fd9b997c0537ec7a65`  
		Last Modified: Wed, 14 Apr 2021 22:59:00 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0880938167776dea94134027e0bc04f2f881b2fab628ec37a41a325af8ed0`  
		Last Modified: Wed, 14 Apr 2021 22:59:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta`

```console
$ docker pull influxdb@sha256:337aea983f3da7180d365cc11cc6f3aca6d53f24a0c78ab30cff639d6cce5061
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:2905d77f1445f3175b67862a9bb9488c523667871574234e45dea19dd50fa008
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.1 MB (84145902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06f271e73df348c6da1b34fa2c785a9f756964b50eba1b7fade6a83816033b8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:13:54 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 10 Apr 2021 19:14:14 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 10 Apr 2021 19:14:14 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 10 Apr 2021 19:14:14 GMT
EXPOSE 8091
# Sat, 10 Apr 2021 19:14:14 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:14 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:15 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eeaf8f6e64ce1140bd91c25b04410ff3be1f9dd7496b959bbfbf4810a10a0df`  
		Last Modified: Sat, 10 Apr 2021 19:17:02 GMT  
		Size: 23.1 MB (23133610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de82bd3fa1a024ea76e33e00251ca3a55fdad98865d6fc87802a1352e40d49e2`  
		Last Modified: Sat, 10 Apr 2021 19:16:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e423aede590af38b52c626f7f97d3b585aef872e84115b5d9c4adabd0309979`  
		Last Modified: Sat, 10 Apr 2021 19:16:59 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta-alpine`

```console
$ docker pull influxdb@sha256:f997194721a978be18e2db6310fc4f20d4e8ae1a13158de1cd7dc6b042ebe98b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.7.11-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:88915c86ce7afd69b101ba5a4dd8d1dfce23bfa760dd74fbb8fec36b562a3909
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27235086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0485099136dd77a780e637f002a9399df5468f2609d126e85c977208798adaac`
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
# Wed, 14 Apr 2021 22:56:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:56:55 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 14 Apr 2021 22:56:55 GMT
EXPOSE 8091
# Wed, 14 Apr 2021 22:56:55 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:56:55 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:56:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:56:56 GMT
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
	-	`sha256:1b8177497e45bcdf4f69a9c9e31aa09286c8157b7e3918ca418f2a8792b98791`  
		Last Modified: Wed, 14 Apr 2021 22:59:27 GMT  
		Size: 23.0 MB (23002988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ea6921490482ed769782ef5ab560e586b844b845bd40314224130d55910a45`  
		Last Modified: Wed, 14 Apr 2021 22:59:24 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bb5766ed91f5ba3565a638433f21786c10951ed30c32133153d1e11a7826c0`  
		Last Modified: Wed, 14 Apr 2021 22:59:28 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:72b1b24a028878162ba61140f70baef70d9e1409682583f0acac034f9531d4f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:1ab363ccda86fd2a585a4ddb4f9dfda01305a92ba661155faa4d9ef614a9a067
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125980189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ffbb8ff883fa16536d88e143aa98c1d6d10adf5095f23ebeb76be2e837b27f0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:14:22 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 10 Apr 2021 19:14:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 19:14:27 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 19:14:27 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:14:27 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:28 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 19:14:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74821cc1518f4e93b542c9e2a779912f92b0515b59e69b57bf13d9b77a91fda4`  
		Last Modified: Sat, 10 Apr 2021 19:17:28 GMT  
		Size: 65.0 MB (64966750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef8dd3f2bbc7cd097d082698f468d3f07c08349426c2227d4bd514b516136b4`  
		Last Modified: Sat, 10 Apr 2021 19:17:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e12d80ed3d7bc4e71e34ff3f841abeda609eb24859ab27fcadf595f1798213`  
		Last Modified: Sat, 10 Apr 2021 19:17:15 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa128a258a46e8c45abd7fa761980cf3707d2b72049ee01cee71e84fb8e08f8`  
		Last Modified: Sat, 10 Apr 2021 19:17:15 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:08111a6d92ad219885669b0d57ed27fa30c5386f410a8891744973da8c987563
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117045986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aeb3b9c435d7c8e282baf31f69e6499c54ccd0b594f61ba90ebf97c528c2113`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:02:42 GMT
ADD file:4c101c517b88a8d25a4997ab4d938ea50aaa265c7f88a4e63edaaed37d89a288 in / 
# Sat, 10 Apr 2021 01:02:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:12:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:16:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:17:11 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 10 Apr 2021 22:17:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 22:17:25 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 22:17:26 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 22:17:27 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 22:17:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 22:17:29 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 22:17:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:17:32 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:533b099902e847172558070703785f6c70f0c6912fefcfd283f3b0e3ebc306c5`  
		Last Modified: Sat, 10 Apr 2021 01:10:12 GMT  
		Size: 42.1 MB (42120304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba1eda48434fdafc900e072c3d26755397eb33edd3403430befc06bf5ebfe0d`  
		Last Modified: Sat, 10 Apr 2021 06:22:42 GMT  
		Size: 9.9 MB (9939854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436419ab83cc68fde8e9c3d51a90fcb8c9874db9093ff594532fd4f5f4e54b8`  
		Last Modified: Sat, 10 Apr 2021 06:22:40 GMT  
		Size: 3.9 MB (3921286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76140bc19f592b5201423519222671e95abc93c446dbf7b6f920df2916214565`  
		Last Modified: Sat, 10 Apr 2021 22:17:48 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4313d1fb57169bae7b8f919122864d0bf6369df64605d945cb09566d46188fa2`  
		Last Modified: Sat, 10 Apr 2021 22:18:25 GMT  
		Size: 61.1 MB (61059964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c6d279e60715188be34eb31057286a873c197cb247f711ebbcbc22cbba83bf`  
		Last Modified: Sat, 10 Apr 2021 22:18:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a97d61a30788f490f9f2def6b7f1a235b5c6b90e7c3cac70061a1e5e31f7b27`  
		Last Modified: Sat, 10 Apr 2021 22:18:10 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3631c703e8a8e85072bcc6e1be534d68102ff34d2cae368874f53da79ebaa667`  
		Last Modified: Sat, 10 Apr 2021 22:18:11 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:0a74296d2d81452abf42cd49c856831f54087fcd6dc3e8752c9edb7492916c20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.1 MB (118109160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a13abe0c142050da51250eef6a9de93696d33b62381b4e2d1d129a5695ae4651`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 00:43:48 GMT
ADD file:64990d14743657dbcbe885739e43ac964a0239a63e4693e6401b0884ab96e09b in / 
# Sat, 10 Apr 2021 00:43:50 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:53:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:53:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:57:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:57:47 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 10 Apr 2021 22:57:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 22:57:56 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 22:57:57 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 22:57:58 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 22:57:59 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 22:58:01 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 22:58:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:58:02 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:30bd672115ff6f225cb98d2d7f1ed62feb72c2612297b2ac615e762e436c64ec`  
		Last Modified: Sat, 10 Apr 2021 00:49:51 GMT  
		Size: 43.2 MB (43177772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7d38e5813e5a59ee1d86fb1c7c8c344342d0ec418aa440509260354958f9ad`  
		Last Modified: Sat, 10 Apr 2021 02:03:48 GMT  
		Size: 10.2 MB (10200972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8ce7d8aff50ac8c0f7baa508791ea69df0fa3c7dac0ab9be8933ce3ef5b68a`  
		Last Modified: Sat, 10 Apr 2021 02:03:46 GMT  
		Size: 4.1 MB (4096630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6013e6f034ca76b4efc42a5079012e11dad3a296baf967d6e2ef766c3442442c`  
		Last Modified: Sat, 10 Apr 2021 22:59:15 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c5c6a3a4f4b52c2f385075ba3a8b8e21ce26e61847f270a8774bfa67b708e8`  
		Last Modified: Sat, 10 Apr 2021 22:59:48 GMT  
		Size: 60.6 MB (60629215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d89577de6aa8b7faa03a966279a59c707ec7bb029198b0e8c35ef45b1d038c`  
		Last Modified: Sat, 10 Apr 2021 22:59:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39322675f8f8b9b8dbc7e697438ec50b8e986b7bf104f4c9c3135aa9e661516`  
		Last Modified: Sat, 10 Apr 2021 22:59:35 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399cf6254f91219d639d95e71ac14500665c7a92b4545afa3be28220a72a873a`  
		Last Modified: Sat, 10 Apr 2021 22:59:35 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:c9eae3860cab958a3e96f2b5ac84aa9460ca6c7d002a67ebc4fd2ba0b843c8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9f9f168ed71b91f06f922f3269bb4b422866d50da93caeedacd39ddf3e3f3e65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68939925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcbef068455c3ded6ab4513ef6ffa479fc84ac810d7a0c5b94e4777670c42741`
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
# Wed, 14 Apr 2021 22:57:01 GMT
ENV INFLUXDB_VERSION=1.8.4
# Wed, 14 Apr 2021 22:57:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:57:10 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:57:10 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:57:10 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:57:10 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:57:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:57:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:57:11 GMT
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
	-	`sha256:28299736dea79a8071f3a9116b60b0f0f073763bc9d379ed8f1e4bee2abf0e88`  
		Last Modified: Wed, 14 Apr 2021 22:59:51 GMT  
		Size: 64.7 MB (64706679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e2d412750af820f6af473dbfa077610bae95e1918a85f9699b33ddd30c740d`  
		Last Modified: Wed, 14 Apr 2021 22:59:42 GMT  
		Size: 253.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5fb71304ab7e30a90f4c13d96fa55458f9c0d243ad064844e6b59834e35600`  
		Last Modified: Wed, 14 Apr 2021 22:59:42 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51463d341f2b4db83588f5d576f36354e64513560764c9b6f1af1c11f0bfb883`  
		Last Modified: Wed, 14 Apr 2021 22:59:43 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:00486245118cb28f2f59f12bcdf4898aa547bd0bf4dd3d1108ce4bb2e41d4634
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:c0e1f20f8eb6d514732e953e346f5094b7b073b62b453c0ad9467bd9bafcf623
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126809910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66196416c6c50082685dfc18906aa5efb7f661804ff4cecea38a8ce02ad877c5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:14:35 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 10 Apr 2021 19:14:42 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 10 Apr 2021 19:14:42 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 19:14:43 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:14:43 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:43 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:43 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 19:14:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:43 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e93546ebb597d763f590fb64f0fd04130ed54d7437c41f8fb2e142e7f186644`  
		Last Modified: Sat, 10 Apr 2021 19:17:49 GMT  
		Size: 65.8 MB (65796413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f657fadbed9c3501434ececc43ebd585eb28d94c0a2ff4ee94663a6a08b1cb1`  
		Last Modified: Sat, 10 Apr 2021 19:17:40 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058e9efdb50e78a7024a24b0041660ec0762ea4217af6cd7ee53810135a78d9d`  
		Last Modified: Sat, 10 Apr 2021 19:17:40 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f790e114555d22f2f3d2de8ac2c7966e422e196c54acf802cd5d962a4fdaea`  
		Last Modified: Sat, 10 Apr 2021 19:17:40 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:8443ef7efdf25b2e649486ee5960b78a020096560c6fe79faee9f209bc7b44b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8a52d04da9a47a536a2a36806940d602e1004a2da63bc2c29024567843eb7d17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69773942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04efee4d4c00fdbc1933b236b477df80ab199ec32c6ec6d14018bfb32ccd7cfa`
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
# Wed, 14 Apr 2021 22:57:17 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Wed, 14 Apr 2021 22:57:25 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:57:25 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:57:26 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:57:26 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:57:26 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:57:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:57:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:57:27 GMT
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
	-	`sha256:2cd09e6c21a9c381749ca1c4c2297748fe31682c186fc844a6c62e2629494885`  
		Last Modified: Wed, 14 Apr 2021 23:00:15 GMT  
		Size: 65.5 MB (65540639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bfda1aab8d5d1a97c0611d2faf1b2af485aa8c6efa0a7491f124ef5354dc9c`  
		Last Modified: Wed, 14 Apr 2021 23:00:08 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949c56c4d23ab81ec9e9c7e11cde367e05a465c240d71d6033a862a507a1af9e`  
		Last Modified: Wed, 14 Apr 2021 23:00:07 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3ec97331674288a09e2cc041cf31424b9ae56cc8c68f01c44c54a78ab4ebd8`  
		Last Modified: Wed, 14 Apr 2021 23:00:06 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:780d06c7cb6e61dc48ee11bb287e4f489e09aab77fcf1053cb32086c8cdba340
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:a26652e1053dae13fd1545c06d4881536f840199338f31cf173a690fa65e73b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83878536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7b48b4f346c5efced4ab74782074cb0be7b5f079de1690161f335f96b31f6a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:14:35 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 10 Apr 2021 19:14:54 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 10 Apr 2021 19:14:54 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 10 Apr 2021 19:14:54 GMT
EXPOSE 8091
# Sat, 10 Apr 2021 19:14:54 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:54 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:55 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d959ec500858a4f95780322c2dd61e95ba7e6921cf5fed504f25e342d8efa13c`  
		Last Modified: Sat, 10 Apr 2021 19:18:08 GMT  
		Size: 22.9 MB (22866244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6d0fd17f970ab0898594b873c16a4fb0b0a31d0a455a58dc07c83bb28a84d9`  
		Last Modified: Sat, 10 Apr 2021 19:18:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab68c359f5d557440de5224f19e72cbe2c01453f83ef7dcf10f9562e59eb5491`  
		Last Modified: Sat, 10 Apr 2021 19:18:05 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:50f6415fbcb9090b6f0137c3cc38c44958e3d817243fbb5d1c1fc47ad1ba0582
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f205bb2774db90735f516a996e01b953c85782db1d1f2c219a1747254ba29b08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26967499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:983e17d469ce4282fb747e4ed26a58357a467dfeff0b983e57864d550b93532a`
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
# Wed, 14 Apr 2021 22:57:17 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Wed, 14 Apr 2021 22:57:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:57:38 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 14 Apr 2021 22:57:38 GMT
EXPOSE 8091
# Wed, 14 Apr 2021 22:57:38 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:57:38 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:57:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:57:39 GMT
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
	-	`sha256:6842848fd72dae543e9cec2ee9a02273eb56bccb98e1df7a67ec462226702ff5`  
		Last Modified: Wed, 14 Apr 2021 23:00:39 GMT  
		Size: 22.7 MB (22735398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85af523caa3353e737b367b7ccf17b422372bf45cfcb707599dde1ef0ff30c0`  
		Last Modified: Wed, 14 Apr 2021 23:00:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff836b13b8350c6a99c8831862153092f5247e2e274d72ef884bbd98a46263c`  
		Last Modified: Wed, 14 Apr 2021 23:00:35 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-data`

```console
$ docker pull influxdb@sha256:00486245118cb28f2f59f12bcdf4898aa547bd0bf4dd3d1108ce4bb2e41d4634
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-data` - linux; amd64

```console
$ docker pull influxdb@sha256:c0e1f20f8eb6d514732e953e346f5094b7b073b62b453c0ad9467bd9bafcf623
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126809910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66196416c6c50082685dfc18906aa5efb7f661804ff4cecea38a8ce02ad877c5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:14:35 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 10 Apr 2021 19:14:42 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 10 Apr 2021 19:14:42 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 19:14:43 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:14:43 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:43 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:43 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 19:14:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:43 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e93546ebb597d763f590fb64f0fd04130ed54d7437c41f8fb2e142e7f186644`  
		Last Modified: Sat, 10 Apr 2021 19:17:49 GMT  
		Size: 65.8 MB (65796413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f657fadbed9c3501434ececc43ebd585eb28d94c0a2ff4ee94663a6a08b1cb1`  
		Last Modified: Sat, 10 Apr 2021 19:17:40 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058e9efdb50e78a7024a24b0041660ec0762ea4217af6cd7ee53810135a78d9d`  
		Last Modified: Sat, 10 Apr 2021 19:17:40 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f790e114555d22f2f3d2de8ac2c7966e422e196c54acf802cd5d962a4fdaea`  
		Last Modified: Sat, 10 Apr 2021 19:17:40 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-data-alpine`

```console
$ docker pull influxdb@sha256:8443ef7efdf25b2e649486ee5960b78a020096560c6fe79faee9f209bc7b44b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8a52d04da9a47a536a2a36806940d602e1004a2da63bc2c29024567843eb7d17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69773942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04efee4d4c00fdbc1933b236b477df80ab199ec32c6ec6d14018bfb32ccd7cfa`
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
# Wed, 14 Apr 2021 22:57:17 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Wed, 14 Apr 2021 22:57:25 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:57:25 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:57:26 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:57:26 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:57:26 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:57:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:57:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:57:27 GMT
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
	-	`sha256:2cd09e6c21a9c381749ca1c4c2297748fe31682c186fc844a6c62e2629494885`  
		Last Modified: Wed, 14 Apr 2021 23:00:15 GMT  
		Size: 65.5 MB (65540639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bfda1aab8d5d1a97c0611d2faf1b2af485aa8c6efa0a7491f124ef5354dc9c`  
		Last Modified: Wed, 14 Apr 2021 23:00:08 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949c56c4d23ab81ec9e9c7e11cde367e05a465c240d71d6033a862a507a1af9e`  
		Last Modified: Wed, 14 Apr 2021 23:00:07 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3ec97331674288a09e2cc041cf31424b9ae56cc8c68f01c44c54a78ab4ebd8`  
		Last Modified: Wed, 14 Apr 2021 23:00:06 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-meta`

```console
$ docker pull influxdb@sha256:780d06c7cb6e61dc48ee11bb287e4f489e09aab77fcf1053cb32086c8cdba340
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:a26652e1053dae13fd1545c06d4881536f840199338f31cf173a690fa65e73b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83878536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7b48b4f346c5efced4ab74782074cb0be7b5f079de1690161f335f96b31f6a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:14:35 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 10 Apr 2021 19:14:54 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 10 Apr 2021 19:14:54 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 10 Apr 2021 19:14:54 GMT
EXPOSE 8091
# Sat, 10 Apr 2021 19:14:54 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:54 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:55 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d959ec500858a4f95780322c2dd61e95ba7e6921cf5fed504f25e342d8efa13c`  
		Last Modified: Sat, 10 Apr 2021 19:18:08 GMT  
		Size: 22.9 MB (22866244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6d0fd17f970ab0898594b873c16a4fb0b0a31d0a455a58dc07c83bb28a84d9`  
		Last Modified: Sat, 10 Apr 2021 19:18:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab68c359f5d557440de5224f19e72cbe2c01453f83ef7dcf10f9562e59eb5491`  
		Last Modified: Sat, 10 Apr 2021 19:18:05 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.3-meta-alpine`

```console
$ docker pull influxdb@sha256:50f6415fbcb9090b6f0137c3cc38c44958e3d817243fbb5d1c1fc47ad1ba0582
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.3-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f205bb2774db90735f516a996e01b953c85782db1d1f2c219a1747254ba29b08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26967499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:983e17d469ce4282fb747e4ed26a58357a467dfeff0b983e57864d550b93532a`
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
# Wed, 14 Apr 2021 22:57:17 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Wed, 14 Apr 2021 22:57:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:57:38 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 14 Apr 2021 22:57:38 GMT
EXPOSE 8091
# Wed, 14 Apr 2021 22:57:38 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:57:38 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:57:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:57:39 GMT
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
	-	`sha256:6842848fd72dae543e9cec2ee9a02273eb56bccb98e1df7a67ec462226702ff5`  
		Last Modified: Wed, 14 Apr 2021 23:00:39 GMT  
		Size: 22.7 MB (22735398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85af523caa3353e737b367b7ccf17b422372bf45cfcb707599dde1ef0ff30c0`  
		Last Modified: Wed, 14 Apr 2021 23:00:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff836b13b8350c6a99c8831862153092f5247e2e274d72ef884bbd98a46263c`  
		Last Modified: Wed, 14 Apr 2021 23:00:35 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.4`

```console
$ docker pull influxdb@sha256:72b1b24a028878162ba61140f70baef70d9e1409682583f0acac034f9531d4f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.4` - linux; amd64

```console
$ docker pull influxdb@sha256:1ab363ccda86fd2a585a4ddb4f9dfda01305a92ba661155faa4d9ef614a9a067
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125980189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ffbb8ff883fa16536d88e143aa98c1d6d10adf5095f23ebeb76be2e837b27f0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:14:22 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 10 Apr 2021 19:14:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 19:14:27 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 19:14:27 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:14:27 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:28 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 19:14:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74821cc1518f4e93b542c9e2a779912f92b0515b59e69b57bf13d9b77a91fda4`  
		Last Modified: Sat, 10 Apr 2021 19:17:28 GMT  
		Size: 65.0 MB (64966750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef8dd3f2bbc7cd097d082698f468d3f07c08349426c2227d4bd514b516136b4`  
		Last Modified: Sat, 10 Apr 2021 19:17:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e12d80ed3d7bc4e71e34ff3f841abeda609eb24859ab27fcadf595f1798213`  
		Last Modified: Sat, 10 Apr 2021 19:17:15 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa128a258a46e8c45abd7fa761980cf3707d2b72049ee01cee71e84fb8e08f8`  
		Last Modified: Sat, 10 Apr 2021 19:17:15 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.4` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:08111a6d92ad219885669b0d57ed27fa30c5386f410a8891744973da8c987563
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117045986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aeb3b9c435d7c8e282baf31f69e6499c54ccd0b594f61ba90ebf97c528c2113`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:02:42 GMT
ADD file:4c101c517b88a8d25a4997ab4d938ea50aaa265c7f88a4e63edaaed37d89a288 in / 
# Sat, 10 Apr 2021 01:02:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:12:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:16:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:17:11 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 10 Apr 2021 22:17:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 22:17:25 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 22:17:26 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 22:17:27 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 22:17:28 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 22:17:29 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 22:17:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:17:32 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:533b099902e847172558070703785f6c70f0c6912fefcfd283f3b0e3ebc306c5`  
		Last Modified: Sat, 10 Apr 2021 01:10:12 GMT  
		Size: 42.1 MB (42120304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba1eda48434fdafc900e072c3d26755397eb33edd3403430befc06bf5ebfe0d`  
		Last Modified: Sat, 10 Apr 2021 06:22:42 GMT  
		Size: 9.9 MB (9939854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436419ab83cc68fde8e9c3d51a90fcb8c9874db9093ff594532fd4f5f4e54b8`  
		Last Modified: Sat, 10 Apr 2021 06:22:40 GMT  
		Size: 3.9 MB (3921286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76140bc19f592b5201423519222671e95abc93c446dbf7b6f920df2916214565`  
		Last Modified: Sat, 10 Apr 2021 22:17:48 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4313d1fb57169bae7b8f919122864d0bf6369df64605d945cb09566d46188fa2`  
		Last Modified: Sat, 10 Apr 2021 22:18:25 GMT  
		Size: 61.1 MB (61059964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c6d279e60715188be34eb31057286a873c197cb247f711ebbcbc22cbba83bf`  
		Last Modified: Sat, 10 Apr 2021 22:18:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a97d61a30788f490f9f2def6b7f1a235b5c6b90e7c3cac70061a1e5e31f7b27`  
		Last Modified: Sat, 10 Apr 2021 22:18:10 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3631c703e8a8e85072bcc6e1be534d68102ff34d2cae368874f53da79ebaa667`  
		Last Modified: Sat, 10 Apr 2021 22:18:11 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.4` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:0a74296d2d81452abf42cd49c856831f54087fcd6dc3e8752c9edb7492916c20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.1 MB (118109160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a13abe0c142050da51250eef6a9de93696d33b62381b4e2d1d129a5695ae4651`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 00:43:48 GMT
ADD file:64990d14743657dbcbe885739e43ac964a0239a63e4693e6401b0884ab96e09b in / 
# Sat, 10 Apr 2021 00:43:50 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:53:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:53:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:57:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:57:47 GMT
ENV INFLUXDB_VERSION=1.8.4
# Sat, 10 Apr 2021 22:57:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 22:57:56 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 22:57:57 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 22:57:58 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 22:57:59 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 10 Apr 2021 22:58:01 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 22:58:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:58:02 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:30bd672115ff6f225cb98d2d7f1ed62feb72c2612297b2ac615e762e436c64ec`  
		Last Modified: Sat, 10 Apr 2021 00:49:51 GMT  
		Size: 43.2 MB (43177772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7d38e5813e5a59ee1d86fb1c7c8c344342d0ec418aa440509260354958f9ad`  
		Last Modified: Sat, 10 Apr 2021 02:03:48 GMT  
		Size: 10.2 MB (10200972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8ce7d8aff50ac8c0f7baa508791ea69df0fa3c7dac0ab9be8933ce3ef5b68a`  
		Last Modified: Sat, 10 Apr 2021 02:03:46 GMT  
		Size: 4.1 MB (4096630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6013e6f034ca76b4efc42a5079012e11dad3a296baf967d6e2ef766c3442442c`  
		Last Modified: Sat, 10 Apr 2021 22:59:15 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c5c6a3a4f4b52c2f385075ba3a8b8e21ce26e61847f270a8774bfa67b708e8`  
		Last Modified: Sat, 10 Apr 2021 22:59:48 GMT  
		Size: 60.6 MB (60629215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d89577de6aa8b7faa03a966279a59c707ec7bb029198b0e8c35ef45b1d038c`  
		Last Modified: Sat, 10 Apr 2021 22:59:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39322675f8f8b9b8dbc7e697438ec50b8e986b7bf104f4c9c3135aa9e661516`  
		Last Modified: Sat, 10 Apr 2021 22:59:35 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399cf6254f91219d639d95e71ac14500665c7a92b4545afa3be28220a72a873a`  
		Last Modified: Sat, 10 Apr 2021 22:59:35 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.4-alpine`

```console
$ docker pull influxdb@sha256:c9eae3860cab958a3e96f2b5ac84aa9460ca6c7d002a67ebc4fd2ba0b843c8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:1.8.4-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:9f9f168ed71b91f06f922f3269bb4b422866d50da93caeedacd39ddf3e3f3e65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68939925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcbef068455c3ded6ab4513ef6ffa479fc84ac810d7a0c5b94e4777670c42741`
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
# Wed, 14 Apr 2021 22:57:01 GMT
ENV INFLUXDB_VERSION=1.8.4
# Wed, 14 Apr 2021 22:57:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:57:10 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:57:10 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:57:10 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:57:10 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:57:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:57:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:57:11 GMT
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
	-	`sha256:28299736dea79a8071f3a9116b60b0f0f073763bc9d379ed8f1e4bee2abf0e88`  
		Last Modified: Wed, 14 Apr 2021 22:59:51 GMT  
		Size: 64.7 MB (64706679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e2d412750af820f6af473dbfa077610bae95e1918a85f9699b33ddd30c740d`  
		Last Modified: Wed, 14 Apr 2021 22:59:42 GMT  
		Size: 253.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5fb71304ab7e30a90f4c13d96fa55458f9c0d243ad064844e6b59834e35600`  
		Last Modified: Wed, 14 Apr 2021 22:59:42 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51463d341f2b4db83588f5d576f36354e64513560764c9b6f1af1c11f0bfb883`  
		Last Modified: Wed, 14 Apr 2021 22:59:43 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0`

```console
$ docker pull influxdb@sha256:142700dfdfb0d63b683c8b30a8571602c5be410cacde7d6a2faf6c71773cfe6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:30d2b24b36c0d763de6be494e4caacc9f7c32f99a50a359569bc52aa51f0da03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116231917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:129820bf5dd739acef3cdecb79f2fc6dbcfab47c88ca424906f8fa4a1060fef9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:54:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:54:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:15:02 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 10 Apr 2021 19:15:02 GMT
ENV GOSU_VER=1.12
# Sat, 10 Apr 2021 19:15:06 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 10 Apr 2021 19:15:07 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 10 Apr 2021 19:15:12 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 10 Apr 2021 19:15:13 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 10 Apr 2021 19:15:13 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 10 Apr 2021 19:15:13 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 10 Apr 2021 19:15:14 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 10 Apr 2021 19:15:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:15:14 GMT
CMD ["influxd"]
# Sat, 10 Apr 2021 19:15:14 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:15:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 10 Apr 2021 19:15:15 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44718e6d535d365250316b02459f98a1b0fa490158cc53057d18858507504d60`  
		Last Modified: Sat, 10 Apr 2021 02:01:57 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe9738af0cb2184ee8f3fb3dcb130455385aa428a27d14e1e07a5587ff16e64`  
		Last Modified: Sat, 10 Apr 2021 02:01:59 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a23e1225dc83c683776f535e68ad815ca7fd88c6c5604c26e020658bef6e67`  
		Last Modified: Sat, 10 Apr 2021 19:18:26 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6503eaa7838769ede3a9772dbb56a771ffcff6780cf948129d329992abe7d160`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 961.0 KB (960989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443db3bed31e3f6fb984281dfa7d2c8d15be4e5ca07ceed2cadee242a1ba9611`  
		Last Modified: Sat, 10 Apr 2021 19:18:30 GMT  
		Size: 47.0 MB (47001563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4eebf6b1be91780c0adad84076fcdc0d6b27a0e9e3dd2beccff3ab43f0430d`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e2dd6edd49acb591991bb34a60adcfd18f8538758a4e05b63a3ea17b3e2fb5`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17634653b3b73c75dfed114a62745f36b2953b61c7710c09960d3faba927a39c`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:8e805709bdef3c92880619629c2ac087f482db20b49bc11bad61ac40ad697b5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112211926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec907ca33dcbfb3d7e886f53b99d28b14c254e1d07929c2371ede4c292f77dcf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 00:40:59 GMT
ADD file:320ad0e2a3d6c676ddb8ce5646b5a94d18d82a8868955da3a9379a261dfe1ffe in / 
# Sat, 10 Apr 2021 00:41:01 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:46:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:46:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:58:18 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 10 Apr 2021 22:58:20 GMT
ENV GOSU_VER=1.12
# Sat, 10 Apr 2021 22:58:25 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 10 Apr 2021 22:58:26 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 10 Apr 2021 22:58:35 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 10 Apr 2021 22:58:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 10 Apr 2021 22:58:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 10 Apr 2021 22:58:41 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 10 Apr 2021 22:58:42 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 10 Apr 2021 22:58:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:58:44 GMT
CMD ["influxd"]
# Sat, 10 Apr 2021 22:58:45 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 22:58:46 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 10 Apr 2021 22:58:47 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:01cf0f0da10ede0eec0fc1c5fbfdeb63a447dfcc0a3c4419c0a4c3f0a2826636`  
		Last Modified: Sat, 10 Apr 2021 00:47:28 GMT  
		Size: 49.2 MB (49225782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c667eb56cd05909001c1c50e81cbc75e290fd8e353f974bab4246a0d4fc484ca`  
		Last Modified: Sat, 10 Apr 2021 02:01:00 GMT  
		Size: 7.7 MB (7695101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ca15a4cef673e0e1a7bc3e659f4653df9bce82b945e367475e436852cc7880`  
		Last Modified: Sat, 10 Apr 2021 02:00:59 GMT  
		Size: 10.0 MB (9984406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dfb0a0dcecdedcb4c30762da81dd0e998ea09d73fe9a3a7c021f3ebde894a5`  
		Last Modified: Sat, 10 Apr 2021 22:59:57 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48c642dee557d637359d24782b535f60582393a664634a93afdfd996262e650`  
		Last Modified: Sat, 10 Apr 2021 22:59:56 GMT  
		Size: 896.4 KB (896378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ebe1ecb38ab675ff87fbda5ea858df472a25b1b107bae217ef2a793640a8fd`  
		Last Modified: Sat, 10 Apr 2021 23:00:05 GMT  
		Size: 44.4 MB (44403985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2013163064671010d6b82410fb662ba816e43c8f51e5f5f891d733c7c49a97`  
		Last Modified: Sat, 10 Apr 2021 22:59:56 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc311114a04880ecf8c64c799292cd80e9d8411dbc47e02710944eb6c641e93`  
		Last Modified: Sat, 10 Apr 2021 22:59:56 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafb284b64f4aab2f74ab25c5eeafedcdcc23fd5ece787255f9aee185a37a8b7`  
		Last Modified: Sat, 10 Apr 2021 22:59:55 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0-alpine`

```console
$ docker pull influxdb@sha256:eebc0eb585c47d5b476dfa25d3a96392856f35748acaccff9c166097c5123717
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:325e936bd4cfb6a18439871bbe90ff87fd777767dfcbce3b0ad2d68003feafd3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60481093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae1dd72d1cbeb93fd570c7534125b66c4fb9a46ad6b6b0f9d03b39cfaaa0ff2c`
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
# Wed, 14 Apr 2021 22:57:52 GMT
ENV INFLUXDB_VERSION=2.0.4
# Wed, 14 Apr 2021 22:57:59 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 14 Apr 2021 22:58:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 14 Apr 2021 22:58:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 14 Apr 2021 22:58:00 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 14 Apr 2021 22:58:01 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Wed, 14 Apr 2021 22:58:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:58:01 GMT
CMD ["influxd"]
# Wed, 14 Apr 2021 22:58:01 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:58:01 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 14 Apr 2021 22:58:02 GMT
ENV INFLUXD_INIT_PORT=9999
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
	-	`sha256:f2e8dc2c5afdfefb911db2feb20e9a30a5fd45493576e9ce75b2bd3c83e5492e`  
		Last Modified: Wed, 14 Apr 2021 23:01:03 GMT  
		Size: 47.0 MB (47001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accbdfcc5a0b81ca72a6280666a19c98f8aac68deaa93482d707491460f7e4c6`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309000718bdce254d72f252239df89b6e3ab9a7fbbe015fc1fb5d7c34d0d4304`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da6b6f6928cb8eadaa51d238e6724b6de074849783c2a11b44361979bb1bc2e`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4469367e5ffb0a9d2a3279f1b463e27fa2627d51aa2842db8c0a174001625880
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57559670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b34ad33ce9f8803a5ed1c6e4a36c60ee810ab894c66bc3a6f20ca16d951487`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:35:11 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 23:35:16 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 14 Apr 2021 23:35:19 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 14 Apr 2021 23:35:20 GMT
ENV GOSU_VER=1.12
# Wed, 14 Apr 2021 23:35:25 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Apr 2021 23:35:26 GMT
ENV INFLUXDB_VERSION=2.0.4
# Wed, 14 Apr 2021 23:35:40 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 14 Apr 2021 23:35:46 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 14 Apr 2021 23:35:47 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 14 Apr 2021 23:35:48 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 14 Apr 2021 23:35:49 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Wed, 14 Apr 2021 23:35:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 23:35:51 GMT
CMD ["influxd"]
# Wed, 14 Apr 2021 23:35:54 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 23:35:56 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 14 Apr 2021 23:35:59 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35940a9c5a13039e953be6bbca73c22954a237641c4881ca4504503b9574469`  
		Last Modified: Wed, 14 Apr 2021 23:36:27 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a289b7dc5e9293f975c801edc34b42ff3160252abdfdac7b9434099518e592bf`  
		Last Modified: Wed, 14 Apr 2021 23:36:30 GMT  
		Size: 9.5 MB (9541707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5346d594da33a77ca1fc238adf6397d1a20af9f219ee01e79750ebd85810fee`  
		Last Modified: Wed, 14 Apr 2021 23:36:29 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd71d02f10a42edeb33b50244220eb0878636fdfa455615cae0a7bbf24c33c0e`  
		Last Modified: Wed, 14 Apr 2021 23:36:26 GMT  
		Size: 896.1 KB (896100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00df5389cdd7ca781f34aad318585dec59ba12b21fb42b42a66991a795f31987`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 44.4 MB (44403964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244485510737e087992d685318dc99fb965414863f808d68be446017c550cfeb`  
		Last Modified: Wed, 14 Apr 2021 23:36:25 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7905ce6087715dc66fc677b64f6edb6643956c6dace633cf4f6013db1ba636`  
		Last Modified: Wed, 14 Apr 2021 23:36:25 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ffc0674eb640a7756adac66b83a1203ef7d59d0956726c18877bc3218e5ff3`  
		Last Modified: Wed, 14 Apr 2021 23:36:24 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.4`

```console
$ docker pull influxdb@sha256:142700dfdfb0d63b683c8b30a8571602c5be410cacde7d6a2faf6c71773cfe6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.4` - linux; amd64

```console
$ docker pull influxdb@sha256:30d2b24b36c0d763de6be494e4caacc9f7c32f99a50a359569bc52aa51f0da03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116231917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:129820bf5dd739acef3cdecb79f2fc6dbcfab47c88ca424906f8fa4a1060fef9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:54:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:54:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:15:02 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 10 Apr 2021 19:15:02 GMT
ENV GOSU_VER=1.12
# Sat, 10 Apr 2021 19:15:06 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 10 Apr 2021 19:15:07 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 10 Apr 2021 19:15:12 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 10 Apr 2021 19:15:13 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 10 Apr 2021 19:15:13 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 10 Apr 2021 19:15:13 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 10 Apr 2021 19:15:14 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 10 Apr 2021 19:15:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:15:14 GMT
CMD ["influxd"]
# Sat, 10 Apr 2021 19:15:14 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:15:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 10 Apr 2021 19:15:15 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44718e6d535d365250316b02459f98a1b0fa490158cc53057d18858507504d60`  
		Last Modified: Sat, 10 Apr 2021 02:01:57 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe9738af0cb2184ee8f3fb3dcb130455385aa428a27d14e1e07a5587ff16e64`  
		Last Modified: Sat, 10 Apr 2021 02:01:59 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a23e1225dc83c683776f535e68ad815ca7fd88c6c5604c26e020658bef6e67`  
		Last Modified: Sat, 10 Apr 2021 19:18:26 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6503eaa7838769ede3a9772dbb56a771ffcff6780cf948129d329992abe7d160`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 961.0 KB (960989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443db3bed31e3f6fb984281dfa7d2c8d15be4e5ca07ceed2cadee242a1ba9611`  
		Last Modified: Sat, 10 Apr 2021 19:18:30 GMT  
		Size: 47.0 MB (47001563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4eebf6b1be91780c0adad84076fcdc0d6b27a0e9e3dd2beccff3ab43f0430d`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e2dd6edd49acb591991bb34a60adcfd18f8538758a4e05b63a3ea17b3e2fb5`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17634653b3b73c75dfed114a62745f36b2953b61c7710c09960d3faba927a39c`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.4` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:8e805709bdef3c92880619629c2ac087f482db20b49bc11bad61ac40ad697b5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112211926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec907ca33dcbfb3d7e886f53b99d28b14c254e1d07929c2371ede4c292f77dcf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 00:40:59 GMT
ADD file:320ad0e2a3d6c676ddb8ce5646b5a94d18d82a8868955da3a9379a261dfe1ffe in / 
# Sat, 10 Apr 2021 00:41:01 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:46:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:46:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:58:18 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 10 Apr 2021 22:58:20 GMT
ENV GOSU_VER=1.12
# Sat, 10 Apr 2021 22:58:25 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 10 Apr 2021 22:58:26 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 10 Apr 2021 22:58:35 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 10 Apr 2021 22:58:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 10 Apr 2021 22:58:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 10 Apr 2021 22:58:41 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 10 Apr 2021 22:58:42 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 10 Apr 2021 22:58:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:58:44 GMT
CMD ["influxd"]
# Sat, 10 Apr 2021 22:58:45 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 22:58:46 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 10 Apr 2021 22:58:47 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:01cf0f0da10ede0eec0fc1c5fbfdeb63a447dfcc0a3c4419c0a4c3f0a2826636`  
		Last Modified: Sat, 10 Apr 2021 00:47:28 GMT  
		Size: 49.2 MB (49225782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c667eb56cd05909001c1c50e81cbc75e290fd8e353f974bab4246a0d4fc484ca`  
		Last Modified: Sat, 10 Apr 2021 02:01:00 GMT  
		Size: 7.7 MB (7695101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ca15a4cef673e0e1a7bc3e659f4653df9bce82b945e367475e436852cc7880`  
		Last Modified: Sat, 10 Apr 2021 02:00:59 GMT  
		Size: 10.0 MB (9984406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dfb0a0dcecdedcb4c30762da81dd0e998ea09d73fe9a3a7c021f3ebde894a5`  
		Last Modified: Sat, 10 Apr 2021 22:59:57 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48c642dee557d637359d24782b535f60582393a664634a93afdfd996262e650`  
		Last Modified: Sat, 10 Apr 2021 22:59:56 GMT  
		Size: 896.4 KB (896378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ebe1ecb38ab675ff87fbda5ea858df472a25b1b107bae217ef2a793640a8fd`  
		Last Modified: Sat, 10 Apr 2021 23:00:05 GMT  
		Size: 44.4 MB (44403985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2013163064671010d6b82410fb662ba816e43c8f51e5f5f891d733c7c49a97`  
		Last Modified: Sat, 10 Apr 2021 22:59:56 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc311114a04880ecf8c64c799292cd80e9d8411dbc47e02710944eb6c641e93`  
		Last Modified: Sat, 10 Apr 2021 22:59:56 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafb284b64f4aab2f74ab25c5eeafedcdcc23fd5ece787255f9aee185a37a8b7`  
		Last Modified: Sat, 10 Apr 2021 22:59:55 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.4-alpine`

```console
$ docker pull influxdb@sha256:eebc0eb585c47d5b476dfa25d3a96392856f35748acaccff9c166097c5123717
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.4-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:325e936bd4cfb6a18439871bbe90ff87fd777767dfcbce3b0ad2d68003feafd3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60481093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae1dd72d1cbeb93fd570c7534125b66c4fb9a46ad6b6b0f9d03b39cfaaa0ff2c`
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
# Wed, 14 Apr 2021 22:57:52 GMT
ENV INFLUXDB_VERSION=2.0.4
# Wed, 14 Apr 2021 22:57:59 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 14 Apr 2021 22:58:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 14 Apr 2021 22:58:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 14 Apr 2021 22:58:00 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 14 Apr 2021 22:58:01 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Wed, 14 Apr 2021 22:58:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:58:01 GMT
CMD ["influxd"]
# Wed, 14 Apr 2021 22:58:01 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:58:01 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 14 Apr 2021 22:58:02 GMT
ENV INFLUXD_INIT_PORT=9999
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
	-	`sha256:f2e8dc2c5afdfefb911db2feb20e9a30a5fd45493576e9ce75b2bd3c83e5492e`  
		Last Modified: Wed, 14 Apr 2021 23:01:03 GMT  
		Size: 47.0 MB (47001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accbdfcc5a0b81ca72a6280666a19c98f8aac68deaa93482d707491460f7e4c6`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309000718bdce254d72f252239df89b6e3ab9a7fbbe015fc1fb5d7c34d0d4304`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da6b6f6928cb8eadaa51d238e6724b6de074849783c2a11b44361979bb1bc2e`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.4-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4469367e5ffb0a9d2a3279f1b463e27fa2627d51aa2842db8c0a174001625880
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57559670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b34ad33ce9f8803a5ed1c6e4a36c60ee810ab894c66bc3a6f20ca16d951487`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:35:11 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 23:35:16 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 14 Apr 2021 23:35:19 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 14 Apr 2021 23:35:20 GMT
ENV GOSU_VER=1.12
# Wed, 14 Apr 2021 23:35:25 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Apr 2021 23:35:26 GMT
ENV INFLUXDB_VERSION=2.0.4
# Wed, 14 Apr 2021 23:35:40 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 14 Apr 2021 23:35:46 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 14 Apr 2021 23:35:47 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 14 Apr 2021 23:35:48 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 14 Apr 2021 23:35:49 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Wed, 14 Apr 2021 23:35:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 23:35:51 GMT
CMD ["influxd"]
# Wed, 14 Apr 2021 23:35:54 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 23:35:56 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 14 Apr 2021 23:35:59 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35940a9c5a13039e953be6bbca73c22954a237641c4881ca4504503b9574469`  
		Last Modified: Wed, 14 Apr 2021 23:36:27 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a289b7dc5e9293f975c801edc34b42ff3160252abdfdac7b9434099518e592bf`  
		Last Modified: Wed, 14 Apr 2021 23:36:30 GMT  
		Size: 9.5 MB (9541707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5346d594da33a77ca1fc238adf6397d1a20af9f219ee01e79750ebd85810fee`  
		Last Modified: Wed, 14 Apr 2021 23:36:29 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd71d02f10a42edeb33b50244220eb0878636fdfa455615cae0a7bbf24c33c0e`  
		Last Modified: Wed, 14 Apr 2021 23:36:26 GMT  
		Size: 896.1 KB (896100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00df5389cdd7ca781f34aad318585dec59ba12b21fb42b42a66991a795f31987`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 44.4 MB (44403964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244485510737e087992d685318dc99fb965414863f808d68be446017c550cfeb`  
		Last Modified: Wed, 14 Apr 2021 23:36:25 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7905ce6087715dc66fc677b64f6edb6643956c6dace633cf4f6013db1ba636`  
		Last Modified: Wed, 14 Apr 2021 23:36:25 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ffc0674eb640a7756adac66b83a1203ef7d59d0956726c18877bc3218e5ff3`  
		Last Modified: Wed, 14 Apr 2021 23:36:24 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:eebc0eb585c47d5b476dfa25d3a96392856f35748acaccff9c166097c5123717
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:325e936bd4cfb6a18439871bbe90ff87fd777767dfcbce3b0ad2d68003feafd3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60481093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae1dd72d1cbeb93fd570c7534125b66c4fb9a46ad6b6b0f9d03b39cfaaa0ff2c`
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
# Wed, 14 Apr 2021 22:57:52 GMT
ENV INFLUXDB_VERSION=2.0.4
# Wed, 14 Apr 2021 22:57:59 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 14 Apr 2021 22:58:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 14 Apr 2021 22:58:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 14 Apr 2021 22:58:00 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 14 Apr 2021 22:58:01 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Wed, 14 Apr 2021 22:58:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:58:01 GMT
CMD ["influxd"]
# Wed, 14 Apr 2021 22:58:01 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:58:01 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 14 Apr 2021 22:58:02 GMT
ENV INFLUXD_INIT_PORT=9999
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
	-	`sha256:f2e8dc2c5afdfefb911db2feb20e9a30a5fd45493576e9ce75b2bd3c83e5492e`  
		Last Modified: Wed, 14 Apr 2021 23:01:03 GMT  
		Size: 47.0 MB (47001577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accbdfcc5a0b81ca72a6280666a19c98f8aac68deaa93482d707491460f7e4c6`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309000718bdce254d72f252239df89b6e3ab9a7fbbe015fc1fb5d7c34d0d4304`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da6b6f6928cb8eadaa51d238e6724b6de074849783c2a11b44361979bb1bc2e`  
		Last Modified: Wed, 14 Apr 2021 23:00:56 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4469367e5ffb0a9d2a3279f1b463e27fa2627d51aa2842db8c0a174001625880
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57559670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b34ad33ce9f8803a5ed1c6e4a36c60ee810ab894c66bc3a6f20ca16d951487`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:35:11 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 23:35:16 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Wed, 14 Apr 2021 23:35:19 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 14 Apr 2021 23:35:20 GMT
ENV GOSU_VER=1.12
# Wed, 14 Apr 2021 23:35:25 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Apr 2021 23:35:26 GMT
ENV INFLUXDB_VERSION=2.0.4
# Wed, 14 Apr 2021 23:35:40 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 14 Apr 2021 23:35:46 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 14 Apr 2021 23:35:47 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 14 Apr 2021 23:35:48 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 14 Apr 2021 23:35:49 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Wed, 14 Apr 2021 23:35:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 23:35:51 GMT
CMD ["influxd"]
# Wed, 14 Apr 2021 23:35:54 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 23:35:56 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 14 Apr 2021 23:35:59 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35940a9c5a13039e953be6bbca73c22954a237641c4881ca4504503b9574469`  
		Last Modified: Wed, 14 Apr 2021 23:36:27 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a289b7dc5e9293f975c801edc34b42ff3160252abdfdac7b9434099518e592bf`  
		Last Modified: Wed, 14 Apr 2021 23:36:30 GMT  
		Size: 9.5 MB (9541707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5346d594da33a77ca1fc238adf6397d1a20af9f219ee01e79750ebd85810fee`  
		Last Modified: Wed, 14 Apr 2021 23:36:29 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd71d02f10a42edeb33b50244220eb0878636fdfa455615cae0a7bbf24c33c0e`  
		Last Modified: Wed, 14 Apr 2021 23:36:26 GMT  
		Size: 896.1 KB (896100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00df5389cdd7ca781f34aad318585dec59ba12b21fb42b42a66991a795f31987`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 44.4 MB (44403964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244485510737e087992d685318dc99fb965414863f808d68be446017c550cfeb`  
		Last Modified: Wed, 14 Apr 2021 23:36:25 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7905ce6087715dc66fc677b64f6edb6643956c6dace633cf4f6013db1ba636`  
		Last Modified: Wed, 14 Apr 2021 23:36:25 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ffc0674eb640a7756adac66b83a1203ef7d59d0956726c18877bc3218e5ff3`  
		Last Modified: Wed, 14 Apr 2021 23:36:24 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:00486245118cb28f2f59f12bcdf4898aa547bd0bf4dd3d1108ce4bb2e41d4634
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:c0e1f20f8eb6d514732e953e346f5094b7b073b62b453c0ad9467bd9bafcf623
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126809910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66196416c6c50082685dfc18906aa5efb7f661804ff4cecea38a8ce02ad877c5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:14:35 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 10 Apr 2021 19:14:42 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 10 Apr 2021 19:14:42 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 10 Apr 2021 19:14:43 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:14:43 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:43 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:43 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 10 Apr 2021 19:14:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:43 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e93546ebb597d763f590fb64f0fd04130ed54d7437c41f8fb2e142e7f186644`  
		Last Modified: Sat, 10 Apr 2021 19:17:49 GMT  
		Size: 65.8 MB (65796413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f657fadbed9c3501434ececc43ebd585eb28d94c0a2ff4ee94663a6a08b1cb1`  
		Last Modified: Sat, 10 Apr 2021 19:17:40 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058e9efdb50e78a7024a24b0041660ec0762ea4217af6cd7ee53810135a78d9d`  
		Last Modified: Sat, 10 Apr 2021 19:17:40 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f790e114555d22f2f3d2de8ac2c7966e422e196c54acf802cd5d962a4fdaea`  
		Last Modified: Sat, 10 Apr 2021 19:17:40 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:8443ef7efdf25b2e649486ee5960b78a020096560c6fe79faee9f209bc7b44b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:8a52d04da9a47a536a2a36806940d602e1004a2da63bc2c29024567843eb7d17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69773942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04efee4d4c00fdbc1933b236b477df80ab199ec32c6ec6d14018bfb32ccd7cfa`
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
# Wed, 14 Apr 2021 22:57:17 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Wed, 14 Apr 2021 22:57:25 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:57:25 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 14 Apr 2021 22:57:26 GMT
EXPOSE 8086
# Wed, 14 Apr 2021 22:57:26 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:57:26 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:57:26 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 14 Apr 2021 22:57:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:57:27 GMT
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
	-	`sha256:2cd09e6c21a9c381749ca1c4c2297748fe31682c186fc844a6c62e2629494885`  
		Last Modified: Wed, 14 Apr 2021 23:00:15 GMT  
		Size: 65.5 MB (65540639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bfda1aab8d5d1a97c0611d2faf1b2af485aa8c6efa0a7491f124ef5354dc9c`  
		Last Modified: Wed, 14 Apr 2021 23:00:08 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949c56c4d23ab81ec9e9c7e11cde367e05a465c240d71d6033a862a507a1af9e`  
		Last Modified: Wed, 14 Apr 2021 23:00:07 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3ec97331674288a09e2cc041cf31424b9ae56cc8c68f01c44c54a78ab4ebd8`  
		Last Modified: Wed, 14 Apr 2021 23:00:06 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:142700dfdfb0d63b683c8b30a8571602c5be410cacde7d6a2faf6c71773cfe6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:30d2b24b36c0d763de6be494e4caacc9f7c32f99a50a359569bc52aa51f0da03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116231917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:129820bf5dd739acef3cdecb79f2fc6dbcfab47c88ca424906f8fa4a1060fef9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:54:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:54:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:15:02 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 10 Apr 2021 19:15:02 GMT
ENV GOSU_VER=1.12
# Sat, 10 Apr 2021 19:15:06 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 10 Apr 2021 19:15:07 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 10 Apr 2021 19:15:12 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 10 Apr 2021 19:15:13 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 10 Apr 2021 19:15:13 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 10 Apr 2021 19:15:13 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 10 Apr 2021 19:15:14 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 10 Apr 2021 19:15:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:15:14 GMT
CMD ["influxd"]
# Sat, 10 Apr 2021 19:15:14 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 19:15:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 10 Apr 2021 19:15:15 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44718e6d535d365250316b02459f98a1b0fa490158cc53057d18858507504d60`  
		Last Modified: Sat, 10 Apr 2021 02:01:57 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe9738af0cb2184ee8f3fb3dcb130455385aa428a27d14e1e07a5587ff16e64`  
		Last Modified: Sat, 10 Apr 2021 02:01:59 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a23e1225dc83c683776f535e68ad815ca7fd88c6c5604c26e020658bef6e67`  
		Last Modified: Sat, 10 Apr 2021 19:18:26 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6503eaa7838769ede3a9772dbb56a771ffcff6780cf948129d329992abe7d160`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 961.0 KB (960989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443db3bed31e3f6fb984281dfa7d2c8d15be4e5ca07ceed2cadee242a1ba9611`  
		Last Modified: Sat, 10 Apr 2021 19:18:30 GMT  
		Size: 47.0 MB (47001563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4eebf6b1be91780c0adad84076fcdc0d6b27a0e9e3dd2beccff3ab43f0430d`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e2dd6edd49acb591991bb34a60adcfd18f8538758a4e05b63a3ea17b3e2fb5`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17634653b3b73c75dfed114a62745f36b2953b61c7710c09960d3faba927a39c`  
		Last Modified: Sat, 10 Apr 2021 19:18:23 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:8e805709bdef3c92880619629c2ac087f482db20b49bc11bad61ac40ad697b5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112211926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec907ca33dcbfb3d7e886f53b99d28b14c254e1d07929c2371ede4c292f77dcf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 10 Apr 2021 00:40:59 GMT
ADD file:320ad0e2a3d6c676ddb8ce5646b5a94d18d82a8868955da3a9379a261dfe1ffe in / 
# Sat, 10 Apr 2021 00:41:01 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:46:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:46:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:58:18 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 10 Apr 2021 22:58:20 GMT
ENV GOSU_VER=1.12
# Sat, 10 Apr 2021 22:58:25 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 10 Apr 2021 22:58:26 GMT
ENV INFLUXDB_VERSION=2.0.4
# Sat, 10 Apr 2021 22:58:35 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 10 Apr 2021 22:58:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 10 Apr 2021 22:58:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 10 Apr 2021 22:58:41 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 10 Apr 2021 22:58:42 GMT
COPY file:f9664ff5942fcf872d1fcd8f91b28e3f7a4c39246a1a9f538b22029c8aa1490f in /entrypoint.sh 
# Sat, 10 Apr 2021 22:58:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:58:44 GMT
CMD ["influxd"]
# Sat, 10 Apr 2021 22:58:45 GMT
EXPOSE 8086
# Sat, 10 Apr 2021 22:58:46 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 10 Apr 2021 22:58:47 GMT
ENV INFLUXD_INIT_PORT=9999
```

-	Layers:
	-	`sha256:01cf0f0da10ede0eec0fc1c5fbfdeb63a447dfcc0a3c4419c0a4c3f0a2826636`  
		Last Modified: Sat, 10 Apr 2021 00:47:28 GMT  
		Size: 49.2 MB (49225782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c667eb56cd05909001c1c50e81cbc75e290fd8e353f974bab4246a0d4fc484ca`  
		Last Modified: Sat, 10 Apr 2021 02:01:00 GMT  
		Size: 7.7 MB (7695101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ca15a4cef673e0e1a7bc3e659f4653df9bce82b945e367475e436852cc7880`  
		Last Modified: Sat, 10 Apr 2021 02:00:59 GMT  
		Size: 10.0 MB (9984406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dfb0a0dcecdedcb4c30762da81dd0e998ea09d73fe9a3a7c021f3ebde894a5`  
		Last Modified: Sat, 10 Apr 2021 22:59:57 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48c642dee557d637359d24782b535f60582393a664634a93afdfd996262e650`  
		Last Modified: Sat, 10 Apr 2021 22:59:56 GMT  
		Size: 896.4 KB (896378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ebe1ecb38ab675ff87fbda5ea858df472a25b1b107bae217ef2a793640a8fd`  
		Last Modified: Sat, 10 Apr 2021 23:00:05 GMT  
		Size: 44.4 MB (44403985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2013163064671010d6b82410fb662ba816e43c8f51e5f5f891d733c7c49a97`  
		Last Modified: Sat, 10 Apr 2021 22:59:56 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc311114a04880ecf8c64c799292cd80e9d8411dbc47e02710944eb6c641e93`  
		Last Modified: Sat, 10 Apr 2021 22:59:56 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafb284b64f4aab2f74ab25c5eeafedcdcc23fd5ece787255f9aee185a37a8b7`  
		Last Modified: Sat, 10 Apr 2021 22:59:55 GMT  
		Size: 3.9 KB (3926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:780d06c7cb6e61dc48ee11bb287e4f489e09aab77fcf1053cb32086c8cdba340
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:a26652e1053dae13fd1545c06d4881536f840199338f31cf173a690fa65e73b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.9 MB (83878536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7b48b4f346c5efced4ab74782074cb0be7b5f079de1690161f335f96b31f6a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 19:13:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 19:14:35 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Sat, 10 Apr 2021 19:14:54 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 10 Apr 2021 19:14:54 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 10 Apr 2021 19:14:54 GMT
EXPOSE 8091
# Sat, 10 Apr 2021 19:14:54 GMT
VOLUME [/var/lib/influxdb]
# Sat, 10 Apr 2021 19:14:54 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 10 Apr 2021 19:14:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 19:14:55 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d661fe5a6d03bcbf4c331f5baa050071efd4e152404ba66693d31e11177a5`  
		Last Modified: Sat, 10 Apr 2021 19:15:58 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d959ec500858a4f95780322c2dd61e95ba7e6921cf5fed504f25e342d8efa13c`  
		Last Modified: Sat, 10 Apr 2021 19:18:08 GMT  
		Size: 22.9 MB (22866244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6d0fd17f970ab0898594b873c16a4fb0b0a31d0a455a58dc07c83bb28a84d9`  
		Last Modified: Sat, 10 Apr 2021 19:18:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab68c359f5d557440de5224f19e72cbe2c01453f83ef7dcf10f9562e59eb5491`  
		Last Modified: Sat, 10 Apr 2021 19:18:05 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:50f6415fbcb9090b6f0137c3cc38c44958e3d817243fbb5d1c1fc47ad1ba0582
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f205bb2774db90735f516a996e01b953c85782db1d1f2c219a1747254ba29b08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26967499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:983e17d469ce4282fb747e4ed26a58357a467dfeff0b983e57864d550b93532a`
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
# Wed, 14 Apr 2021 22:57:17 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Wed, 14 Apr 2021 22:57:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:57:38 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 14 Apr 2021 22:57:38 GMT
EXPOSE 8091
# Wed, 14 Apr 2021 22:57:38 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:57:38 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:57:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:57:39 GMT
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
	-	`sha256:6842848fd72dae543e9cec2ee9a02273eb56bccb98e1df7a67ec462226702ff5`  
		Last Modified: Wed, 14 Apr 2021 23:00:39 GMT  
		Size: 22.7 MB (22735398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85af523caa3353e737b367b7ccf17b422372bf45cfcb707599dde1ef0ff30c0`  
		Last Modified: Wed, 14 Apr 2021 23:00:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff836b13b8350c6a99c8831862153092f5247e2e274d72ef884bbd98a46263c`  
		Last Modified: Wed, 14 Apr 2021 23:00:35 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
