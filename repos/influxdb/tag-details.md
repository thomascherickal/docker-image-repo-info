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
-	[`influxdb:1.9.8-data`](#influxdb198-data)
-	[`influxdb:1.9.8-data-alpine`](#influxdb198-data-alpine)
-	[`influxdb:1.9.8-meta`](#influxdb198-meta)
-	[`influxdb:1.9.8-meta-alpine`](#influxdb198-meta-alpine)
-	[`influxdb:2.1`](#influxdb21)
-	[`influxdb:2.1-alpine`](#influxdb21-alpine)
-	[`influxdb:2.1.1`](#influxdb211)
-	[`influxdb:2.1.1-alpine`](#influxdb211-alpine)
-	[`influxdb:2.2`](#influxdb22)
-	[`influxdb:2.2-alpine`](#influxdb22-alpine)
-	[`influxdb:2.2.0`](#influxdb220)
-	[`influxdb:2.2.0-alpine`](#influxdb220-alpine)
-	[`influxdb:2.3`](#influxdb23)
-	[`influxdb:2.3-alpine`](#influxdb23-alpine)
-	[`influxdb:2.3.0`](#influxdb230)
-	[`influxdb:2.3.0-alpine`](#influxdb230-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:e4a8fc195ae6b02c58e7d41cca7ab181ef9bd4c7e783d96d2d5e1dff0c26666c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:c16f40f6594609d6616ce97bca66711bfb70bc1b93f5a75399849665dfad92f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115970535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6cb414914317a702dce8e755685abcc32f8aec5d19b44ac6142792c4adbf13`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:17:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:17:59 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 23 Jun 2022 15:18:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 23 Jun 2022 15:18:08 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 23 Jun 2022 15:18:08 GMT
EXPOSE 8086
# Thu, 23 Jun 2022 15:18:08 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 15:18:08 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 23 Jun 2022 15:18:08 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 23 Jun 2022 15:18:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:18:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86e15a947f1f4c2ec5261546aba1007d9944f87c77bed2eb2cb9f38d91fe491`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62cc51cba414c3541215225647c5af4c8c3a3e36ea7561bdf4eca2049571b43`  
		Last Modified: Thu, 23 Jun 2022 15:20:38 GMT  
		Size: 54.9 MB (54890096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faaa581d54756ef7464eb5c63ef74c72aff4cfe424ede3b344b71ea3aa3b9c72`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f632aa225f7e7dca7b2e7e5374c709d730e83b6f5afcb4d815a7677b22f8a0`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ecbe6378b00513801e7c9517c5cd8d5bb1763f0d4d0c54b1d12fbaead0d78`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:febf0c5fe4cdaac4343046d77841b7be5448d45407010d895b73dc3852f09a2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107651683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f662fc3778211c5978a66077ad7c8e7929b7a2b9bf70d705cedb59e97443b21`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:04 GMT
ADD file:4f45aa06c6a1c011e41ff7e4685f05d91970973768fc88ff3e825c5ac4fd6058 in / 
# Thu, 23 Jun 2022 01:05:05 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:58:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:58:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Jun 2022 21:31:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 24 Jun 2022 21:31:27 GMT
ENV INFLUXDB_VERSION=1.8.10
# Fri, 24 Jun 2022 21:31:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 24 Jun 2022 21:31:40 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 24 Jun 2022 21:31:40 GMT
EXPOSE 8086
# Fri, 24 Jun 2022 21:31:41 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Jun 2022 21:31:41 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 24 Jun 2022 21:31:42 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 24 Jun 2022 21:31:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jun 2022 21:31:43 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:cf35481e5c316d184dac1873898948d1e8108de590a2a940c32cda34173fe7c1`  
		Last Modified: Thu, 23 Jun 2022 01:22:04 GMT  
		Size: 42.2 MB (42150850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b740b174e94fb77095522004355bb6f430f0b25308acd5fc66d325f04f99c6`  
		Last Modified: Thu, 23 Jun 2022 02:21:27 GMT  
		Size: 10.0 MB (9957097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf98bd2fdfbc26a0f8c12d47c32e612d01389ff5e4aafc52aa04b72381a6c823`  
		Last Modified: Thu, 23 Jun 2022 02:21:24 GMT  
		Size: 3.9 MB (3921761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47d44c23d29138cc77963505746aeb5e198c324f107db630815dae36a9ae314`  
		Last Modified: Fri, 24 Jun 2022 21:32:04 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf461c7998377c5f4873577c4b0c37adfc647e929ff29f933fdb0e5cacb8c9a`  
		Last Modified: Fri, 24 Jun 2022 21:32:33 GMT  
		Size: 51.6 MB (51617403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c23495e74b15f15e81a6ec00bd4a00e11b7b6106d64c23443d3da66181a55fb`  
		Last Modified: Fri, 24 Jun 2022 21:32:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba482c6b30994880b11a1ed9071a3c60e2aadc28367ab29f82d150a8942b839`  
		Last Modified: Fri, 24 Jun 2022 21:32:04 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a70e33cd3c46138a2b7273fd23bb7b2283bc9ec9f93e48d2dd4e5445ccd7cb3`  
		Last Modified: Fri, 24 Jun 2022 21:32:04 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:1c64e6f0442dd3e37e41ef6f8eefe4eed53cd333dc5bc610ef8496d1e08d06d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108545169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb8543f113ca7cef9b6c045530b0dc675e1a21e0af0cae7089042a9bec7ba16`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:45 GMT
ADD file:3d8b1da94fcec5d068e3e6465fac70cce404c331bb52e30a5bf7cbd950baa5fe in / 
# Thu, 23 Jun 2022 00:42:45 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:15:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:16:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 19:48:34 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 19:48:34 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 23 Jun 2022 19:48:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 23 Jun 2022 19:48:41 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 23 Jun 2022 19:48:41 GMT
EXPOSE 8086
# Thu, 23 Jun 2022 19:48:42 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 19:48:44 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 23 Jun 2022 19:48:45 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 23 Jun 2022 19:48:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 19:48:46 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d8ccec8a513f896fedd1d9765f3f2abf98bc8264f61cecf17919c80c9aa7ddbc`  
		Last Modified: Thu, 23 Jun 2022 00:51:18 GMT  
		Size: 43.2 MB (43213121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b40625a6bb21cb2cd6b19ef7592951f90da9ea1d8abf359196bf48300c448b2`  
		Last Modified: Thu, 23 Jun 2022 01:25:28 GMT  
		Size: 10.2 MB (10218617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414226169d0f92fdcd77314cbd06ba7613675d62a3afd63aa88afbf0072c44c2`  
		Last Modified: Thu, 23 Jun 2022 01:25:27 GMT  
		Size: 3.9 MB (3874558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d0c0dd1eef675f72de8d122b467f8e456d2c09b2b543e3ca5b64e5675bffce`  
		Last Modified: Thu, 23 Jun 2022 19:51:31 GMT  
		Size: 2.8 KB (2824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c6474f58a4fb305a76da0094b9c7d1d7e94becaefe6c2fbf58fd31cac845cc`  
		Last Modified: Thu, 23 Jun 2022 19:51:37 GMT  
		Size: 51.2 MB (51234330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd60772939842216264a6c1cf4edc5ac2554d3ab06ac828171d2643a1468b6`  
		Last Modified: Thu, 23 Jun 2022 19:51:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5307c2b3dde34fcba26bcffd16aa11e6eadcd30ef81c0c864ccf1371103f6c40`  
		Last Modified: Thu, 23 Jun 2022 19:51:31 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec356415ae67a7221e56aa64b08c9e6685db512d3a76724a746bdc999c5edb3d`  
		Last Modified: Thu, 23 Jun 2022 19:51:31 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:fb64ca8970ce9f6b4d235de14124af0c998e3960436f5fd6429daa1084179b8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:bebc8358fd24a1888e3ad376a96896693beb7539ad66f8560908e735d9661603
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117789620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d217aae6287d1db96b3e3790861ee7c4d6606f2b7bb0321ea1fd5982f2f4ed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:17:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:18:14 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 23 Jun 2022 15:18:20 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 23 Jun 2022 15:18:21 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 23 Jun 2022 15:18:21 GMT
EXPOSE 8086
# Thu, 23 Jun 2022 15:18:21 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 15:18:21 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 23 Jun 2022 15:18:21 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 23 Jun 2022 15:18:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:18:21 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86e15a947f1f4c2ec5261546aba1007d9944f87c77bed2eb2cb9f38d91fe491`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950f7b7fdaff085645293a46684da21b15044d943489a4d2c277b4b26e680e9b`  
		Last Modified: Thu, 23 Jun 2022 15:20:56 GMT  
		Size: 56.7 MB (56709124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1872d73bcff1f595b2830cd35fc5f092d8c2a50d078b790877f9118613c8e1`  
		Last Modified: Thu, 23 Jun 2022 15:20:49 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d58f2fb0c6074e97aed0e4d9ddc3a70065731436d5c1d738acac3e66f6f62f`  
		Last Modified: Thu, 23 Jun 2022 15:20:49 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9a5e047ca0e0553d8afd2a4bd60baa41783dcdb113de5cb1c656091d7e0049`  
		Last Modified: Thu, 23 Jun 2022 15:20:49 GMT  
		Size: 1.3 KB (1280 bytes)  
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
$ docker pull influxdb@sha256:22802a6c409c5cdd3bc054c2196b8320041e1be81dfa4683d21358cd832113d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:7ecfdafa61c3d2d3f057774038cf7c870861c9d1f094abb763bbccda889be0fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84496164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095bfff223c443c0e87ec288f1462d1732302060b304b9799c4b17ae4447e1b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:17:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:18:14 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 23 Jun 2022 15:18:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 23 Jun 2022 15:18:30 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 23 Jun 2022 15:18:30 GMT
EXPOSE 8091
# Thu, 23 Jun 2022 15:18:30 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 15:18:30 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 23 Jun 2022 15:18:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:18:30 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86e15a947f1f4c2ec5261546aba1007d9944f87c77bed2eb2cb9f38d91fe491`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7551c1766386d104f430be81f49cfaa95686138d88c7038f7e6cfd1e66f4c`  
		Last Modified: Thu, 23 Jun 2022 15:21:14 GMT  
		Size: 23.4 MB (23416877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535fe8a7786b0b29380c8643d4e5e61e5e5017afcfa08a3b8af6742f09dc3a68`  
		Last Modified: Thu, 23 Jun 2022 15:21:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa9e12f9123b3fb169ca58d9afa4152583f9f5531c26fa69ce35b5e7ec63667`  
		Last Modified: Thu, 23 Jun 2022 15:21:11 GMT  
		Size: 371.0 B  
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
$ docker pull influxdb@sha256:e4a8fc195ae6b02c58e7d41cca7ab181ef9bd4c7e783d96d2d5e1dff0c26666c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:c16f40f6594609d6616ce97bca66711bfb70bc1b93f5a75399849665dfad92f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115970535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6cb414914317a702dce8e755685abcc32f8aec5d19b44ac6142792c4adbf13`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:17:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:17:59 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 23 Jun 2022 15:18:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 23 Jun 2022 15:18:08 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 23 Jun 2022 15:18:08 GMT
EXPOSE 8086
# Thu, 23 Jun 2022 15:18:08 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 15:18:08 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 23 Jun 2022 15:18:08 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 23 Jun 2022 15:18:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:18:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86e15a947f1f4c2ec5261546aba1007d9944f87c77bed2eb2cb9f38d91fe491`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62cc51cba414c3541215225647c5af4c8c3a3e36ea7561bdf4eca2049571b43`  
		Last Modified: Thu, 23 Jun 2022 15:20:38 GMT  
		Size: 54.9 MB (54890096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faaa581d54756ef7464eb5c63ef74c72aff4cfe424ede3b344b71ea3aa3b9c72`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f632aa225f7e7dca7b2e7e5374c709d730e83b6f5afcb4d815a7677b22f8a0`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ecbe6378b00513801e7c9517c5cd8d5bb1763f0d4d0c54b1d12fbaead0d78`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:febf0c5fe4cdaac4343046d77841b7be5448d45407010d895b73dc3852f09a2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107651683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f662fc3778211c5978a66077ad7c8e7929b7a2b9bf70d705cedb59e97443b21`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Jun 2022 01:05:04 GMT
ADD file:4f45aa06c6a1c011e41ff7e4685f05d91970973768fc88ff3e825c5ac4fd6058 in / 
# Thu, 23 Jun 2022 01:05:05 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:58:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:58:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Jun 2022 21:31:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 24 Jun 2022 21:31:27 GMT
ENV INFLUXDB_VERSION=1.8.10
# Fri, 24 Jun 2022 21:31:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 24 Jun 2022 21:31:40 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 24 Jun 2022 21:31:40 GMT
EXPOSE 8086
# Fri, 24 Jun 2022 21:31:41 GMT
VOLUME [/var/lib/influxdb]
# Fri, 24 Jun 2022 21:31:41 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 24 Jun 2022 21:31:42 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 24 Jun 2022 21:31:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jun 2022 21:31:43 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:cf35481e5c316d184dac1873898948d1e8108de590a2a940c32cda34173fe7c1`  
		Last Modified: Thu, 23 Jun 2022 01:22:04 GMT  
		Size: 42.2 MB (42150850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b740b174e94fb77095522004355bb6f430f0b25308acd5fc66d325f04f99c6`  
		Last Modified: Thu, 23 Jun 2022 02:21:27 GMT  
		Size: 10.0 MB (9957097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf98bd2fdfbc26a0f8c12d47c32e612d01389ff5e4aafc52aa04b72381a6c823`  
		Last Modified: Thu, 23 Jun 2022 02:21:24 GMT  
		Size: 3.9 MB (3921761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47d44c23d29138cc77963505746aeb5e198c324f107db630815dae36a9ae314`  
		Last Modified: Fri, 24 Jun 2022 21:32:04 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf461c7998377c5f4873577c4b0c37adfc647e929ff29f933fdb0e5cacb8c9a`  
		Last Modified: Fri, 24 Jun 2022 21:32:33 GMT  
		Size: 51.6 MB (51617403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c23495e74b15f15e81a6ec00bd4a00e11b7b6106d64c23443d3da66181a55fb`  
		Last Modified: Fri, 24 Jun 2022 21:32:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba482c6b30994880b11a1ed9071a3c60e2aadc28367ab29f82d150a8942b839`  
		Last Modified: Fri, 24 Jun 2022 21:32:04 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a70e33cd3c46138a2b7273fd23bb7b2283bc9ec9f93e48d2dd4e5445ccd7cb3`  
		Last Modified: Fri, 24 Jun 2022 21:32:04 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:1c64e6f0442dd3e37e41ef6f8eefe4eed53cd333dc5bc610ef8496d1e08d06d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108545169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb8543f113ca7cef9b6c045530b0dc675e1a21e0af0cae7089042a9bec7ba16`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:45 GMT
ADD file:3d8b1da94fcec5d068e3e6465fac70cce404c331bb52e30a5bf7cbd950baa5fe in / 
# Thu, 23 Jun 2022 00:42:45 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:15:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:16:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 19:48:34 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 19:48:34 GMT
ENV INFLUXDB_VERSION=1.8.10
# Thu, 23 Jun 2022 19:48:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Thu, 23 Jun 2022 19:48:41 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 23 Jun 2022 19:48:41 GMT
EXPOSE 8086
# Thu, 23 Jun 2022 19:48:42 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 19:48:44 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 23 Jun 2022 19:48:45 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 23 Jun 2022 19:48:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 19:48:46 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d8ccec8a513f896fedd1d9765f3f2abf98bc8264f61cecf17919c80c9aa7ddbc`  
		Last Modified: Thu, 23 Jun 2022 00:51:18 GMT  
		Size: 43.2 MB (43213121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b40625a6bb21cb2cd6b19ef7592951f90da9ea1d8abf359196bf48300c448b2`  
		Last Modified: Thu, 23 Jun 2022 01:25:28 GMT  
		Size: 10.2 MB (10218617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414226169d0f92fdcd77314cbd06ba7613675d62a3afd63aa88afbf0072c44c2`  
		Last Modified: Thu, 23 Jun 2022 01:25:27 GMT  
		Size: 3.9 MB (3874558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d0c0dd1eef675f72de8d122b467f8e456d2c09b2b543e3ca5b64e5675bffce`  
		Last Modified: Thu, 23 Jun 2022 19:51:31 GMT  
		Size: 2.8 KB (2824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c6474f58a4fb305a76da0094b9c7d1d7e94becaefe6c2fbf58fd31cac845cc`  
		Last Modified: Thu, 23 Jun 2022 19:51:37 GMT  
		Size: 51.2 MB (51234330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd60772939842216264a6c1cf4edc5ac2554d3ab06ac828171d2643a1468b6`  
		Last Modified: Thu, 23 Jun 2022 19:51:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5307c2b3dde34fcba26bcffd16aa11e6eadcd30ef81c0c864ccf1371103f6c40`  
		Last Modified: Thu, 23 Jun 2022 19:51:31 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec356415ae67a7221e56aa64b08c9e6685db512d3a76724a746bdc999c5edb3d`  
		Last Modified: Thu, 23 Jun 2022 19:51:31 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:fb64ca8970ce9f6b4d235de14124af0c998e3960436f5fd6429daa1084179b8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:bebc8358fd24a1888e3ad376a96896693beb7539ad66f8560908e735d9661603
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117789620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d217aae6287d1db96b3e3790861ee7c4d6606f2b7bb0321ea1fd5982f2f4ed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:17:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:18:14 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 23 Jun 2022 15:18:20 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 23 Jun 2022 15:18:21 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 23 Jun 2022 15:18:21 GMT
EXPOSE 8086
# Thu, 23 Jun 2022 15:18:21 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 15:18:21 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 23 Jun 2022 15:18:21 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 23 Jun 2022 15:18:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:18:21 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86e15a947f1f4c2ec5261546aba1007d9944f87c77bed2eb2cb9f38d91fe491`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950f7b7fdaff085645293a46684da21b15044d943489a4d2c277b4b26e680e9b`  
		Last Modified: Thu, 23 Jun 2022 15:20:56 GMT  
		Size: 56.7 MB (56709124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1872d73bcff1f595b2830cd35fc5f092d8c2a50d078b790877f9118613c8e1`  
		Last Modified: Thu, 23 Jun 2022 15:20:49 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d58f2fb0c6074e97aed0e4d9ddc3a70065731436d5c1d738acac3e66f6f62f`  
		Last Modified: Thu, 23 Jun 2022 15:20:49 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9a5e047ca0e0553d8afd2a4bd60baa41783dcdb113de5cb1c656091d7e0049`  
		Last Modified: Thu, 23 Jun 2022 15:20:49 GMT  
		Size: 1.3 KB (1280 bytes)  
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
$ docker pull influxdb@sha256:22802a6c409c5cdd3bc054c2196b8320041e1be81dfa4683d21358cd832113d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:7ecfdafa61c3d2d3f057774038cf7c870861c9d1f094abb763bbccda889be0fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84496164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095bfff223c443c0e87ec288f1462d1732302060b304b9799c4b17ae4447e1b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:17:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:18:14 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 23 Jun 2022 15:18:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 23 Jun 2022 15:18:30 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 23 Jun 2022 15:18:30 GMT
EXPOSE 8091
# Thu, 23 Jun 2022 15:18:30 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 15:18:30 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 23 Jun 2022 15:18:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:18:30 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86e15a947f1f4c2ec5261546aba1007d9944f87c77bed2eb2cb9f38d91fe491`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7551c1766386d104f430be81f49cfaa95686138d88c7038f7e6cfd1e66f4c`  
		Last Modified: Thu, 23 Jun 2022 15:21:14 GMT  
		Size: 23.4 MB (23416877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535fe8a7786b0b29380c8643d4e5e61e5e5017afcfa08a3b8af6742f09dc3a68`  
		Last Modified: Thu, 23 Jun 2022 15:21:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa9e12f9123b3fb169ca58d9afa4152583f9f5531c26fa69ce35b5e7ec63667`  
		Last Modified: Thu, 23 Jun 2022 15:21:11 GMT  
		Size: 371.0 B  
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
$ docker pull influxdb@sha256:1d54a86b0bd7fcfa9aabc07fd5d154b09f739b3e576637894d15ef81e614568c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:0a84e27ca1134eb38d8ae09c832632cc1c76778b329054dd5f6b85cecec44c3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90704761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6e2b7604b07c7552b02cbd1f026de424bbb321323200eb002caad58bf1ac95`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:17:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:18:34 GMT
ENV INFLUXDB_VERSION=1.9.7-c1.9.7
# Thu, 23 Jun 2022 15:18:39 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 23 Jun 2022 15:18:39 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 23 Jun 2022 15:18:39 GMT
EXPOSE 8086
# Thu, 23 Jun 2022 15:18:39 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 15:18:40 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 23 Jun 2022 15:18:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 23 Jun 2022 15:18:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:18:40 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86e15a947f1f4c2ec5261546aba1007d9944f87c77bed2eb2cb9f38d91fe491`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04aff6c1890c46abd4003acde3b453e5b71898dbd9d769127f25311ef5d10259`  
		Last Modified: Thu, 23 Jun 2022 15:21:32 GMT  
		Size: 29.6 MB (29624267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d939fe246a2b556daa5103d3ab51ff08e2782b1fda9b1b7002875f54b882dd3`  
		Last Modified: Thu, 23 Jun 2022 15:21:27 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292f4825b351de647551aca4182dc9f79e13621e095feccfcfb34fdf1165c40c`  
		Last Modified: Thu, 23 Jun 2022 15:21:28 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055f8157df2bcf052d3e011c32350c23fbb4e13dad6530c744d04168dd6cfe55`  
		Last Modified: Thu, 23 Jun 2022 15:21:27 GMT  
		Size: 1.3 KB (1280 bytes)  
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
$ docker pull influxdb@sha256:d7601e92ba4e711f4ee3cf7d07932feae8711674c23bbe17a6a0b50710a9ca72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:5d4a3f1734cb58cb07243792530aee4b252294e3a00524b1ed95db179b9de3cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72483542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:039225233dfae14e09aaaaf799595bf09836c8abc0cca7cbc5b8d414795fd4bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:17:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:18:34 GMT
ENV INFLUXDB_VERSION=1.9.7-c1.9.7
# Thu, 23 Jun 2022 15:18:47 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 23 Jun 2022 15:18:48 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 23 Jun 2022 15:18:48 GMT
EXPOSE 8091
# Thu, 23 Jun 2022 15:18:48 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 15:18:48 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 23 Jun 2022 15:18:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:18:48 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86e15a947f1f4c2ec5261546aba1007d9944f87c77bed2eb2cb9f38d91fe491`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555f5d16489bb07a4d278b9f3ad38a4d03912e5476c27aad983ba3d4c019088a`  
		Last Modified: Thu, 23 Jun 2022 15:21:45 GMT  
		Size: 11.4 MB (11404252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175220f81e0548d4288cd6ca249df7634d2a5320e267820ca692254e87eac48`  
		Last Modified: Thu, 23 Jun 2022 15:21:43 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a9aa4a35f20cac33f164f643ad67623fe1564ee3901bc2343b52a9ca03d1ba`  
		Last Modified: Thu, 23 Jun 2022 15:21:43 GMT  
		Size: 372.0 B  
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

## `influxdb:1.9.8-data`

**does not exist** (yet?)

## `influxdb:1.9.8-data-alpine`

**does not exist** (yet?)

## `influxdb:1.9.8-meta`

**does not exist** (yet?)

## `influxdb:1.9.8-meta-alpine`

**does not exist** (yet?)

## `influxdb:2.1`

```console
$ docker pull influxdb@sha256:cae91f54aae30536e83d45004a30fdde17cf842c613a5c57ce87506d190d71ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1` - linux; amd64

```console
$ docker pull influxdb@sha256:c52714e5c4642274a001cd6312a0b7fa1f11d946277082ffb1f30fc3d36da683
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182913140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f9ac0ce7ac52f20323ca07dd60b529bd8758b201620e0649765571c7387445a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:20 GMT
ADD file:d738977543f4afc4c3040c6fca3e3f15388ec3b7263a29a6aa83f9a4bf05fed1 in / 
# Tue, 12 Jul 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:49:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:49:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jul 2022 00:48:08 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 13 Jul 2022 00:48:08 GMT
ENV GOSU_VER=1.12
# Wed, 13 Jul 2022 00:48:12 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 13 Jul 2022 00:48:12 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 13 Jul 2022 00:48:20 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 13 Jul 2022 00:48:21 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 13 Jul 2022 00:48:24 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 13 Jul 2022 00:48:25 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 13 Jul 2022 00:48:25 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 13 Jul 2022 00:48:25 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 13 Jul 2022 00:48:25 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 13 Jul 2022 00:48:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jul 2022 00:48:25 GMT
CMD ["influxd"]
# Wed, 13 Jul 2022 00:48:25 GMT
EXPOSE 8086
# Wed, 13 Jul 2022 00:48:25 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 13 Jul 2022 00:48:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 13 Jul 2022 00:48:26 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 13 Jul 2022 00:48:26 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:80b89a2b88b24e7be7c8038e2cbff99ad4fd2f07ad914da4bab80dabaadf8a99`  
		Last Modified: Tue, 12 Jul 2022 01:24:55 GMT  
		Size: 50.4 MB (50440555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0405f798f5b335d83b02371187f3be0ce2092aa0c6b6178ff11290ee6a14c9`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 7.9 MB (7856888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab80b2b0494ab26b41941fb73a028292e2e5d2070c56b3488e890eda20e04641`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 10.0 MB (9998095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99c88ddeebad2b651c3edb1be60a716c899a4fcc58c8cff5c0c880d08a4afa9`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c19bb70c8cbec52a00e4bf3a3dd775454b5ddc47e2043117e196580d12eae8d`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 961.0 KB (960956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b5a00e60ba1c7a14cefe1e47e88dcd6d47b0a85803ec408f4eb14a6a641cb5`  
		Last Modified: Wed, 13 Jul 2022 00:50:04 GMT  
		Size: 108.3 MB (108324802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a62dd84731fb18dfacdbfe8639bb69368c06911d43d0ac5f8cda3228e0d1eff`  
		Last Modified: Wed, 13 Jul 2022 00:49:57 GMT  
		Size: 5.3 MB (5324487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6f65a0720bb75a477fa6df49a27881b814c32a0b74d217d92c6fb2d2bc66ea`  
		Last Modified: Wed, 13 Jul 2022 00:49:56 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd99733aee3a4a0e2fddeba185417ccf7e072aa9a428772e4e2f13dc77ae34e1`  
		Last Modified: Wed, 13 Jul 2022 00:49:56 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf7f5f0bb696bbb3b2114078ba220cb660ab5409d415709aa5f2c58916eae91`  
		Last Modified: Wed, 13 Jul 2022 00:49:56 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ad56ee9d2aa7559be5600e1fa767c4ba7215fd98bc54e4194454073dbddd06d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183419383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:851deafca68f9d27a33fcd3a06baf03f03f443945c8ac1c64b957b98a5e16a84`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:46 GMT
ADD file:ea39534c5e9a548d7938f6b0e2459383caaf3906f3cc5eafe8bf66053b19f2d5 in / 
# Tue, 12 Jul 2022 00:40:47 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:34:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 21:30:54 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 12 Jul 2022 21:30:55 GMT
ENV GOSU_VER=1.12
# Tue, 12 Jul 2022 21:30:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 12 Jul 2022 21:31:00 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 12 Jul 2022 21:31:12 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 12 Jul 2022 21:31:12 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 12 Jul 2022 21:31:17 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 12 Jul 2022 21:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 12 Jul 2022 21:31:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 12 Jul 2022 21:31:20 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 12 Jul 2022 21:31:21 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Tue, 12 Jul 2022 21:31:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jul 2022 21:31:22 GMT
CMD ["influxd"]
# Tue, 12 Jul 2022 21:31:23 GMT
EXPOSE 8086
# Tue, 12 Jul 2022 21:31:24 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 12 Jul 2022 21:31:25 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 12 Jul 2022 21:31:26 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 12 Jul 2022 21:31:27 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:891a1587d3644a8b4b6dab3726ef380a725a0e19bfbf0eac02a275f711985862`  
		Last Modified: Tue, 12 Jul 2022 00:46:46 GMT  
		Size: 49.2 MB (49228928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d1ed6a27dab15e77b7afa9c8697a170f017a73ec9ea8f3f00d5f322e1d3ab`  
		Last Modified: Tue, 12 Jul 2022 02:43:49 GMT  
		Size: 7.7 MB (7720027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186afd5d5e89c602b988d31dd5210c9e3c19435f849f6cc4a6a22a2388e83cf`  
		Last Modified: Tue, 12 Jul 2022 02:43:46 GMT  
		Size: 9.8 MB (9768648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0df5326ac1fed63134e3c8159e5848b6b21984f5e3fcc471726138a3ad72a6`  
		Last Modified: Tue, 12 Jul 2022 21:33:32 GMT  
		Size: 1.7 KB (1657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6354ffc941f42e787a87e65c98641066c2adeab672dd2e105f4e774496dfd3`  
		Last Modified: Tue, 12 Jul 2022 21:33:33 GMT  
		Size: 896.3 KB (896337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98f0f994ea586fd05e50c5ee1a712ab04c9ff1c4ad8c5fa3323f0a9a812e940`  
		Last Modified: Tue, 12 Jul 2022 21:33:40 GMT  
		Size: 110.9 MB (110891609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d00da4550fb18ae0d3189a92e0b6e6e7ac142ee30be189eb911238cc76deb`  
		Last Modified: Tue, 12 Jul 2022 21:33:31 GMT  
		Size: 4.9 MB (4906720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5152261d8248b5856df4650c1282704c264d6e926a6f8275993d93264ae32348`  
		Last Modified: Tue, 12 Jul 2022 21:33:30 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb39a1fd7fddc7756610aa4ad15ceebebb0156ce6a5c73647940eafb6e82d34b`  
		Last Modified: Tue, 12 Jul 2022 21:33:30 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449b6c0f3a247ccb41c286f11cee73dc7a5556cd91b5434451e8e7773e7bd4e1`  
		Last Modified: Tue, 12 Jul 2022 21:33:30 GMT  
		Size: 5.0 KB (5016 bytes)  
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
$ docker pull influxdb@sha256:cae91f54aae30536e83d45004a30fdde17cf842c613a5c57ce87506d190d71ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1` - linux; amd64

```console
$ docker pull influxdb@sha256:c52714e5c4642274a001cd6312a0b7fa1f11d946277082ffb1f30fc3d36da683
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182913140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f9ac0ce7ac52f20323ca07dd60b529bd8758b201620e0649765571c7387445a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:20 GMT
ADD file:d738977543f4afc4c3040c6fca3e3f15388ec3b7263a29a6aa83f9a4bf05fed1 in / 
# Tue, 12 Jul 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:49:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:49:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jul 2022 00:48:08 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 13 Jul 2022 00:48:08 GMT
ENV GOSU_VER=1.12
# Wed, 13 Jul 2022 00:48:12 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 13 Jul 2022 00:48:12 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 13 Jul 2022 00:48:20 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 13 Jul 2022 00:48:21 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 13 Jul 2022 00:48:24 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 13 Jul 2022 00:48:25 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 13 Jul 2022 00:48:25 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 13 Jul 2022 00:48:25 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 13 Jul 2022 00:48:25 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 13 Jul 2022 00:48:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jul 2022 00:48:25 GMT
CMD ["influxd"]
# Wed, 13 Jul 2022 00:48:25 GMT
EXPOSE 8086
# Wed, 13 Jul 2022 00:48:25 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 13 Jul 2022 00:48:26 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 13 Jul 2022 00:48:26 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 13 Jul 2022 00:48:26 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:80b89a2b88b24e7be7c8038e2cbff99ad4fd2f07ad914da4bab80dabaadf8a99`  
		Last Modified: Tue, 12 Jul 2022 01:24:55 GMT  
		Size: 50.4 MB (50440555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0405f798f5b335d83b02371187f3be0ce2092aa0c6b6178ff11290ee6a14c9`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 7.9 MB (7856888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab80b2b0494ab26b41941fb73a028292e2e5d2070c56b3488e890eda20e04641`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 10.0 MB (9998095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99c88ddeebad2b651c3edb1be60a716c899a4fcc58c8cff5c0c880d08a4afa9`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c19bb70c8cbec52a00e4bf3a3dd775454b5ddc47e2043117e196580d12eae8d`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 961.0 KB (960956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b5a00e60ba1c7a14cefe1e47e88dcd6d47b0a85803ec408f4eb14a6a641cb5`  
		Last Modified: Wed, 13 Jul 2022 00:50:04 GMT  
		Size: 108.3 MB (108324802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a62dd84731fb18dfacdbfe8639bb69368c06911d43d0ac5f8cda3228e0d1eff`  
		Last Modified: Wed, 13 Jul 2022 00:49:57 GMT  
		Size: 5.3 MB (5324487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6f65a0720bb75a477fa6df49a27881b814c32a0b74d217d92c6fb2d2bc66ea`  
		Last Modified: Wed, 13 Jul 2022 00:49:56 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd99733aee3a4a0e2fddeba185417ccf7e072aa9a428772e4e2f13dc77ae34e1`  
		Last Modified: Wed, 13 Jul 2022 00:49:56 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf7f5f0bb696bbb3b2114078ba220cb660ab5409d415709aa5f2c58916eae91`  
		Last Modified: Wed, 13 Jul 2022 00:49:56 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ad56ee9d2aa7559be5600e1fa767c4ba7215fd98bc54e4194454073dbddd06d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183419383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:851deafca68f9d27a33fcd3a06baf03f03f443945c8ac1c64b957b98a5e16a84`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:46 GMT
ADD file:ea39534c5e9a548d7938f6b0e2459383caaf3906f3cc5eafe8bf66053b19f2d5 in / 
# Tue, 12 Jul 2022 00:40:47 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:34:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 21:30:54 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 12 Jul 2022 21:30:55 GMT
ENV GOSU_VER=1.12
# Tue, 12 Jul 2022 21:30:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 12 Jul 2022 21:31:00 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 12 Jul 2022 21:31:12 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 12 Jul 2022 21:31:12 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 12 Jul 2022 21:31:17 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 12 Jul 2022 21:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 12 Jul 2022 21:31:18 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 12 Jul 2022 21:31:20 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 12 Jul 2022 21:31:21 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Tue, 12 Jul 2022 21:31:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jul 2022 21:31:22 GMT
CMD ["influxd"]
# Tue, 12 Jul 2022 21:31:23 GMT
EXPOSE 8086
# Tue, 12 Jul 2022 21:31:24 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 12 Jul 2022 21:31:25 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 12 Jul 2022 21:31:26 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 12 Jul 2022 21:31:27 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:891a1587d3644a8b4b6dab3726ef380a725a0e19bfbf0eac02a275f711985862`  
		Last Modified: Tue, 12 Jul 2022 00:46:46 GMT  
		Size: 49.2 MB (49228928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d1ed6a27dab15e77b7afa9c8697a170f017a73ec9ea8f3f00d5f322e1d3ab`  
		Last Modified: Tue, 12 Jul 2022 02:43:49 GMT  
		Size: 7.7 MB (7720027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186afd5d5e89c602b988d31dd5210c9e3c19435f849f6cc4a6a22a2388e83cf`  
		Last Modified: Tue, 12 Jul 2022 02:43:46 GMT  
		Size: 9.8 MB (9768648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0df5326ac1fed63134e3c8159e5848b6b21984f5e3fcc471726138a3ad72a6`  
		Last Modified: Tue, 12 Jul 2022 21:33:32 GMT  
		Size: 1.7 KB (1657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6354ffc941f42e787a87e65c98641066c2adeab672dd2e105f4e774496dfd3`  
		Last Modified: Tue, 12 Jul 2022 21:33:33 GMT  
		Size: 896.3 KB (896337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98f0f994ea586fd05e50c5ee1a712ab04c9ff1c4ad8c5fa3323f0a9a812e940`  
		Last Modified: Tue, 12 Jul 2022 21:33:40 GMT  
		Size: 110.9 MB (110891609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d00da4550fb18ae0d3189a92e0b6e6e7ac142ee30be189eb911238cc76deb`  
		Last Modified: Tue, 12 Jul 2022 21:33:31 GMT  
		Size: 4.9 MB (4906720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5152261d8248b5856df4650c1282704c264d6e926a6f8275993d93264ae32348`  
		Last Modified: Tue, 12 Jul 2022 21:33:30 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb39a1fd7fddc7756610aa4ad15ceebebb0156ce6a5c73647940eafb6e82d34b`  
		Last Modified: Tue, 12 Jul 2022 21:33:30 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449b6c0f3a247ccb41c286f11cee73dc7a5556cd91b5434451e8e7773e7bd4e1`  
		Last Modified: Tue, 12 Jul 2022 21:33:30 GMT  
		Size: 5.0 KB (5016 bytes)  
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
$ docker pull influxdb@sha256:5ed33d5de2fcddc2185e20dd19bf4629eef16cb563f445345467a8df46cb389b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.2` - linux; amd64

```console
$ docker pull influxdb@sha256:a1541388e637c053502d73537df18a26eb4c9e689df8cb99c147e08748cb9ad4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.9 MB (181851245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0f46f9d0bd317511d2ff6b82e681c84d387a3cce882dc2ad11ed561fd9b0a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:20 GMT
ADD file:d738977543f4afc4c3040c6fca3e3f15388ec3b7263a29a6aa83f9a4bf05fed1 in / 
# Tue, 12 Jul 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:49:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:49:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jul 2022 00:48:08 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 13 Jul 2022 00:48:08 GMT
ENV GOSU_VER=1.12
# Wed, 13 Jul 2022 00:48:12 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 13 Jul 2022 00:48:33 GMT
ENV INFLUXDB_VERSION=2.2.0
# Wed, 13 Jul 2022 00:48:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 13 Jul 2022 00:48:40 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 13 Jul 2022 00:48:43 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 13 Jul 2022 00:48:44 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 13 Jul 2022 00:48:44 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 13 Jul 2022 00:48:44 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 13 Jul 2022 00:48:44 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 13 Jul 2022 00:48:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jul 2022 00:48:44 GMT
CMD ["influxd"]
# Wed, 13 Jul 2022 00:48:45 GMT
EXPOSE 8086
# Wed, 13 Jul 2022 00:48:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 13 Jul 2022 00:48:45 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 13 Jul 2022 00:48:45 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 13 Jul 2022 00:48:45 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:80b89a2b88b24e7be7c8038e2cbff99ad4fd2f07ad914da4bab80dabaadf8a99`  
		Last Modified: Tue, 12 Jul 2022 01:24:55 GMT  
		Size: 50.4 MB (50440555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0405f798f5b335d83b02371187f3be0ce2092aa0c6b6178ff11290ee6a14c9`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 7.9 MB (7856888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab80b2b0494ab26b41941fb73a028292e2e5d2070c56b3488e890eda20e04641`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 10.0 MB (9998095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99c88ddeebad2b651c3edb1be60a716c899a4fcc58c8cff5c0c880d08a4afa9`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c19bb70c8cbec52a00e4bf3a3dd775454b5ddc47e2043117e196580d12eae8d`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 961.0 KB (960956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d1ee4be5e45c250a027a0a95837b3750a21e4c21c05ffb4bc3b8b4ac393981`  
		Last Modified: Wed, 13 Jul 2022 00:50:24 GMT  
		Size: 107.2 MB (107220539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9beb19d5e5caa97c45608caeb5554e34018ab1f3550e85187c7f72e08fad8be`  
		Last Modified: Wed, 13 Jul 2022 00:50:17 GMT  
		Size: 5.4 MB (5366855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9cc32325a5a79e54131b3c311440be40faed9e500b848c7be4ccbfbbd6e8a3`  
		Last Modified: Wed, 13 Jul 2022 00:50:16 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eecba331522cd7a7c9744c3af535401350b39bca08a5eed0b8cd5607d8eb34`  
		Last Modified: Wed, 13 Jul 2022 00:50:16 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d1a3d8c1aa5dadc0d6e5956aa7f3ba331ce0a9e285bce8d3ea22ce02e3002`  
		Last Modified: Wed, 13 Jul 2022 00:50:16 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.2` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:e726f8531b5b8c8639928c0b349a90388825791366fa34196768b5b794362b7f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182451588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fefb895fd033cbfd61fa13057ab6819703bb5766c360fc7fed2b1ebfe11f499a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:46 GMT
ADD file:ea39534c5e9a548d7938f6b0e2459383caaf3906f3cc5eafe8bf66053b19f2d5 in / 
# Tue, 12 Jul 2022 00:40:47 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:34:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 21:30:54 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 12 Jul 2022 21:30:55 GMT
ENV GOSU_VER=1.12
# Tue, 12 Jul 2022 21:30:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 12 Jul 2022 21:31:41 GMT
ENV INFLUXDB_VERSION=2.2.0
# Tue, 12 Jul 2022 21:31:55 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 12 Jul 2022 21:31:55 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Tue, 12 Jul 2022 21:31:59 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 12 Jul 2022 21:31:59 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 12 Jul 2022 21:32:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 12 Jul 2022 21:32:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 12 Jul 2022 21:32:03 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Tue, 12 Jul 2022 21:32:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jul 2022 21:32:04 GMT
CMD ["influxd"]
# Tue, 12 Jul 2022 21:32:05 GMT
EXPOSE 8086
# Tue, 12 Jul 2022 21:32:06 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 12 Jul 2022 21:32:07 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 12 Jul 2022 21:32:08 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 12 Jul 2022 21:32:09 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:891a1587d3644a8b4b6dab3726ef380a725a0e19bfbf0eac02a275f711985862`  
		Last Modified: Tue, 12 Jul 2022 00:46:46 GMT  
		Size: 49.2 MB (49228928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d1ed6a27dab15e77b7afa9c8697a170f017a73ec9ea8f3f00d5f322e1d3ab`  
		Last Modified: Tue, 12 Jul 2022 02:43:49 GMT  
		Size: 7.7 MB (7720027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186afd5d5e89c602b988d31dd5210c9e3c19435f849f6cc4a6a22a2388e83cf`  
		Last Modified: Tue, 12 Jul 2022 02:43:46 GMT  
		Size: 9.8 MB (9768648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0df5326ac1fed63134e3c8159e5848b6b21984f5e3fcc471726138a3ad72a6`  
		Last Modified: Tue, 12 Jul 2022 21:33:32 GMT  
		Size: 1.7 KB (1657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6354ffc941f42e787a87e65c98641066c2adeab672dd2e105f4e774496dfd3`  
		Last Modified: Tue, 12 Jul 2022 21:33:33 GMT  
		Size: 896.3 KB (896337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a176f29b2f44c2cdb087ebd44351c964c95b7ec49e44eb5017d61b52fd090`  
		Last Modified: Tue, 12 Jul 2022 21:34:03 GMT  
		Size: 109.9 MB (109877904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8819733cfa7d8689336e48112a8efb0e0fe1d892e0aa110db3d146b5af370`  
		Last Modified: Tue, 12 Jul 2022 21:33:53 GMT  
		Size: 5.0 MB (4952627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efdb38ac112497a8690a1ae2787906dcf896385d128074300b125c53e9ade8a`  
		Last Modified: Tue, 12 Jul 2022 21:33:52 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8cdcefcb33b24e507e5709efc8bcdb7c3c75f5d3985f93a1cb99cc8220864c`  
		Last Modified: Tue, 12 Jul 2022 21:33:52 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d50757ee7568016db30fa8a1534a23987eee26efb6567f1493a661d38e6531c`  
		Last Modified: Tue, 12 Jul 2022 21:33:53 GMT  
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
$ docker pull influxdb@sha256:5ed33d5de2fcddc2185e20dd19bf4629eef16cb563f445345467a8df46cb389b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:a1541388e637c053502d73537df18a26eb4c9e689df8cb99c147e08748cb9ad4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.9 MB (181851245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0f46f9d0bd317511d2ff6b82e681c84d387a3cce882dc2ad11ed561fd9b0a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:20 GMT
ADD file:d738977543f4afc4c3040c6fca3e3f15388ec3b7263a29a6aa83f9a4bf05fed1 in / 
# Tue, 12 Jul 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:49:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:49:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jul 2022 00:48:08 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 13 Jul 2022 00:48:08 GMT
ENV GOSU_VER=1.12
# Wed, 13 Jul 2022 00:48:12 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 13 Jul 2022 00:48:33 GMT
ENV INFLUXDB_VERSION=2.2.0
# Wed, 13 Jul 2022 00:48:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 13 Jul 2022 00:48:40 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 13 Jul 2022 00:48:43 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 13 Jul 2022 00:48:44 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 13 Jul 2022 00:48:44 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 13 Jul 2022 00:48:44 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 13 Jul 2022 00:48:44 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 13 Jul 2022 00:48:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jul 2022 00:48:44 GMT
CMD ["influxd"]
# Wed, 13 Jul 2022 00:48:45 GMT
EXPOSE 8086
# Wed, 13 Jul 2022 00:48:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 13 Jul 2022 00:48:45 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 13 Jul 2022 00:48:45 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 13 Jul 2022 00:48:45 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:80b89a2b88b24e7be7c8038e2cbff99ad4fd2f07ad914da4bab80dabaadf8a99`  
		Last Modified: Tue, 12 Jul 2022 01:24:55 GMT  
		Size: 50.4 MB (50440555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0405f798f5b335d83b02371187f3be0ce2092aa0c6b6178ff11290ee6a14c9`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 7.9 MB (7856888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab80b2b0494ab26b41941fb73a028292e2e5d2070c56b3488e890eda20e04641`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 10.0 MB (9998095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99c88ddeebad2b651c3edb1be60a716c899a4fcc58c8cff5c0c880d08a4afa9`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c19bb70c8cbec52a00e4bf3a3dd775454b5ddc47e2043117e196580d12eae8d`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 961.0 KB (960956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d1ee4be5e45c250a027a0a95837b3750a21e4c21c05ffb4bc3b8b4ac393981`  
		Last Modified: Wed, 13 Jul 2022 00:50:24 GMT  
		Size: 107.2 MB (107220539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9beb19d5e5caa97c45608caeb5554e34018ab1f3550e85187c7f72e08fad8be`  
		Last Modified: Wed, 13 Jul 2022 00:50:17 GMT  
		Size: 5.4 MB (5366855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9cc32325a5a79e54131b3c311440be40faed9e500b848c7be4ccbfbbd6e8a3`  
		Last Modified: Wed, 13 Jul 2022 00:50:16 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eecba331522cd7a7c9744c3af535401350b39bca08a5eed0b8cd5607d8eb34`  
		Last Modified: Wed, 13 Jul 2022 00:50:16 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d1a3d8c1aa5dadc0d6e5956aa7f3ba331ce0a9e285bce8d3ea22ce02e3002`  
		Last Modified: Wed, 13 Jul 2022 00:50:16 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:e726f8531b5b8c8639928c0b349a90388825791366fa34196768b5b794362b7f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182451588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fefb895fd033cbfd61fa13057ab6819703bb5766c360fc7fed2b1ebfe11f499a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:46 GMT
ADD file:ea39534c5e9a548d7938f6b0e2459383caaf3906f3cc5eafe8bf66053b19f2d5 in / 
# Tue, 12 Jul 2022 00:40:47 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:34:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 21:30:54 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 12 Jul 2022 21:30:55 GMT
ENV GOSU_VER=1.12
# Tue, 12 Jul 2022 21:30:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 12 Jul 2022 21:31:41 GMT
ENV INFLUXDB_VERSION=2.2.0
# Tue, 12 Jul 2022 21:31:55 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 12 Jul 2022 21:31:55 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Tue, 12 Jul 2022 21:31:59 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 12 Jul 2022 21:31:59 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 12 Jul 2022 21:32:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 12 Jul 2022 21:32:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 12 Jul 2022 21:32:03 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Tue, 12 Jul 2022 21:32:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jul 2022 21:32:04 GMT
CMD ["influxd"]
# Tue, 12 Jul 2022 21:32:05 GMT
EXPOSE 8086
# Tue, 12 Jul 2022 21:32:06 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 12 Jul 2022 21:32:07 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 12 Jul 2022 21:32:08 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 12 Jul 2022 21:32:09 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:891a1587d3644a8b4b6dab3726ef380a725a0e19bfbf0eac02a275f711985862`  
		Last Modified: Tue, 12 Jul 2022 00:46:46 GMT  
		Size: 49.2 MB (49228928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d1ed6a27dab15e77b7afa9c8697a170f017a73ec9ea8f3f00d5f322e1d3ab`  
		Last Modified: Tue, 12 Jul 2022 02:43:49 GMT  
		Size: 7.7 MB (7720027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186afd5d5e89c602b988d31dd5210c9e3c19435f849f6cc4a6a22a2388e83cf`  
		Last Modified: Tue, 12 Jul 2022 02:43:46 GMT  
		Size: 9.8 MB (9768648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0df5326ac1fed63134e3c8159e5848b6b21984f5e3fcc471726138a3ad72a6`  
		Last Modified: Tue, 12 Jul 2022 21:33:32 GMT  
		Size: 1.7 KB (1657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6354ffc941f42e787a87e65c98641066c2adeab672dd2e105f4e774496dfd3`  
		Last Modified: Tue, 12 Jul 2022 21:33:33 GMT  
		Size: 896.3 KB (896337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a176f29b2f44c2cdb087ebd44351c964c95b7ec49e44eb5017d61b52fd090`  
		Last Modified: Tue, 12 Jul 2022 21:34:03 GMT  
		Size: 109.9 MB (109877904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8819733cfa7d8689336e48112a8efb0e0fe1d892e0aa110db3d146b5af370`  
		Last Modified: Tue, 12 Jul 2022 21:33:53 GMT  
		Size: 5.0 MB (4952627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efdb38ac112497a8690a1ae2787906dcf896385d128074300b125c53e9ade8a`  
		Last Modified: Tue, 12 Jul 2022 21:33:52 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8cdcefcb33b24e507e5709efc8bcdb7c3c75f5d3985f93a1cb99cc8220864c`  
		Last Modified: Tue, 12 Jul 2022 21:33:52 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d50757ee7568016db30fa8a1534a23987eee26efb6567f1493a661d38e6531c`  
		Last Modified: Tue, 12 Jul 2022 21:33:53 GMT  
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

## `influxdb:2.3`

```console
$ docker pull influxdb@sha256:c6c2e3b84913b4ab0fcd4512d85af5796bb090cb1fbbb69ca1bbee85229ef155
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.3` - linux; amd64

```console
$ docker pull influxdb@sha256:107d9264ecf117e3ffc7dfd92d1642efc99ec3631f608574e857ef421acaa9fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255109369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24266999a5d6dabef266905c8d2b5dd227dc5d2a7ad4d43688414c0f96dbd39`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:20 GMT
ADD file:d738977543f4afc4c3040c6fca3e3f15388ec3b7263a29a6aa83f9a4bf05fed1 in / 
# Tue, 12 Jul 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:49:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:49:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jul 2022 00:48:08 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 13 Jul 2022 00:48:08 GMT
ENV GOSU_VER=1.12
# Wed, 13 Jul 2022 00:48:12 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 13 Jul 2022 00:48:49 GMT
ENV INFLUXDB_VERSION=2.3.0
# Wed, 13 Jul 2022 00:48:58 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 13 Jul 2022 00:48:58 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 13 Jul 2022 00:49:01 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 13 Jul 2022 00:49:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 13 Jul 2022 00:49:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 13 Jul 2022 00:49:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 13 Jul 2022 00:49:02 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 13 Jul 2022 00:49:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jul 2022 00:49:02 GMT
CMD ["influxd"]
# Wed, 13 Jul 2022 00:49:02 GMT
EXPOSE 8086
# Wed, 13 Jul 2022 00:49:02 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 13 Jul 2022 00:49:02 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 13 Jul 2022 00:49:02 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 13 Jul 2022 00:49:03 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:80b89a2b88b24e7be7c8038e2cbff99ad4fd2f07ad914da4bab80dabaadf8a99`  
		Last Modified: Tue, 12 Jul 2022 01:24:55 GMT  
		Size: 50.4 MB (50440555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0405f798f5b335d83b02371187f3be0ce2092aa0c6b6178ff11290ee6a14c9`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 7.9 MB (7856888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab80b2b0494ab26b41941fb73a028292e2e5d2070c56b3488e890eda20e04641`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 10.0 MB (9998095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99c88ddeebad2b651c3edb1be60a716c899a4fcc58c8cff5c0c880d08a4afa9`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c19bb70c8cbec52a00e4bf3a3dd775454b5ddc47e2043117e196580d12eae8d`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 961.0 KB (960956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91464f3385c50c198633e39fc1158d4c9935d69a0136c402c5ea945abb80bbc`  
		Last Modified: Wed, 13 Jul 2022 00:50:48 GMT  
		Size: 180.5 MB (180478667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9499689b44d8d0f59a4dca1b557b64afa08293491123eb9e1f284752eaf6cca3`  
		Last Modified: Wed, 13 Jul 2022 00:50:35 GMT  
		Size: 5.4 MB (5366851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407603165b5b499688be3a09145270e5ba712c3fd8c95c4c940ed82729ee2d60`  
		Last Modified: Wed, 13 Jul 2022 00:50:34 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33debaf42eb6f3e0db6f41f956503c49322db9df4321a6a45501bf4fea222cd`  
		Last Modified: Wed, 13 Jul 2022 00:50:34 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902fce46e4e728f6fdd16ed9b9fe622b2623e08c2a61db95562615b5953a866`  
		Last Modified: Wed, 13 Jul 2022 00:50:34 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.3` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ffef41c242c6916ddb8d72fdb0570d344dbe39335e4e6fd9b893921628f2d3a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253366128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6362fd64c09bae094ddfd07494eb7a1eb1554681e343815e1176395ed7e9090c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:46 GMT
ADD file:ea39534c5e9a548d7938f6b0e2459383caaf3906f3cc5eafe8bf66053b19f2d5 in / 
# Tue, 12 Jul 2022 00:40:47 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:34:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 21:30:54 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 12 Jul 2022 21:30:55 GMT
ENV GOSU_VER=1.12
# Tue, 12 Jul 2022 21:30:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 12 Jul 2022 21:32:22 GMT
ENV INFLUXDB_VERSION=2.3.0
# Tue, 12 Jul 2022 21:32:34 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 12 Jul 2022 21:32:34 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Tue, 12 Jul 2022 21:32:37 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 12 Jul 2022 21:32:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 12 Jul 2022 21:32:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 12 Jul 2022 21:32:41 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 12 Jul 2022 21:32:42 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Tue, 12 Jul 2022 21:32:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jul 2022 21:32:43 GMT
CMD ["influxd"]
# Tue, 12 Jul 2022 21:32:44 GMT
EXPOSE 8086
# Tue, 12 Jul 2022 21:32:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 12 Jul 2022 21:32:46 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 12 Jul 2022 21:32:47 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 12 Jul 2022 21:32:48 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:891a1587d3644a8b4b6dab3726ef380a725a0e19bfbf0eac02a275f711985862`  
		Last Modified: Tue, 12 Jul 2022 00:46:46 GMT  
		Size: 49.2 MB (49228928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d1ed6a27dab15e77b7afa9c8697a170f017a73ec9ea8f3f00d5f322e1d3ab`  
		Last Modified: Tue, 12 Jul 2022 02:43:49 GMT  
		Size: 7.7 MB (7720027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186afd5d5e89c602b988d31dd5210c9e3c19435f849f6cc4a6a22a2388e83cf`  
		Last Modified: Tue, 12 Jul 2022 02:43:46 GMT  
		Size: 9.8 MB (9768648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0df5326ac1fed63134e3c8159e5848b6b21984f5e3fcc471726138a3ad72a6`  
		Last Modified: Tue, 12 Jul 2022 21:33:32 GMT  
		Size: 1.7 KB (1657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6354ffc941f42e787a87e65c98641066c2adeab672dd2e105f4e774496dfd3`  
		Last Modified: Tue, 12 Jul 2022 21:33:33 GMT  
		Size: 896.3 KB (896337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fcbacb5196e76298c72f9f64008a67987259f9709231150fdeea7b7fd12dd4e`  
		Last Modified: Tue, 12 Jul 2022 21:34:31 GMT  
		Size: 180.8 MB (180792446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ae52c693b92622571c468956d2078a30f684e134ce2879c552615dad709462`  
		Last Modified: Tue, 12 Jul 2022 21:34:17 GMT  
		Size: 5.0 MB (4952629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4278dea3bc40dcf8ff123886bdc4a23bf8e95259e2d3ec1c84b590cea3e9679e`  
		Last Modified: Tue, 12 Jul 2022 21:34:16 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77049a9c8a367ea2f8305ccf9fe2bf18f86ccb3da6059b2eec5b86bbba7f02c9`  
		Last Modified: Tue, 12 Jul 2022 21:34:16 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a727154dea679e4df502e93e277dacbe7037f7b24e121011cfe0e528c91059bc`  
		Last Modified: Tue, 12 Jul 2022 21:34:17 GMT  
		Size: 5.0 KB (5013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.3-alpine`

```console
$ docker pull influxdb@sha256:b21e01fd74eee0d318cf02118efb94ca5c3f8053f73459f3c119c11f8886fd62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.3-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:02f15da8fa163ebf27a18e9abd3f2b2d1fee45e233e7fb2d149d938cb009ba0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.5 MB (199468297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f58a0c9c632cdb66195942a7f620ee5ed2dc5bc5db483b1f63c20b30023ad15`
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
# Thu, 16 Jun 2022 22:20:31 GMT
ENV INFLUXDB_VERSION=2.3.0
# Thu, 16 Jun 2022 22:20:39 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 16 Jun 2022 22:20:39 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 16 Jun 2022 22:20:42 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 16 Jun 2022 22:20:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Jun 2022 22:20:43 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Jun 2022 22:20:43 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Jun 2022 22:20:43 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 16 Jun 2022 22:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Jun 2022 22:20:43 GMT
CMD ["influxd"]
# Thu, 16 Jun 2022 22:20:43 GMT
EXPOSE 8086
# Thu, 16 Jun 2022 22:20:43 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Jun 2022 22:20:44 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Jun 2022 22:20:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Jun 2022 22:20:44 GMT
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
	-	`sha256:c3a5beaff1353f4dc69c0a10bd65e7116a89188cc22e05d2f754dd3f73111c0d`  
		Last Modified: Thu, 16 Jun 2022 22:22:16 GMT  
		Size: 180.5 MB (180478679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325149cfb67924e4de205f483e9c2d03dfa7b477d1f7e63d6fcde2146a88e70a`  
		Last Modified: Thu, 16 Jun 2022 22:22:04 GMT  
		Size: 5.4 MB (5366873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b918e22717c1cb5d940f7a0d9fc54ae5f3908a124081a8d9596905c80341a2cc`  
		Last Modified: Thu, 16 Jun 2022 22:22:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa245e7165eba29536ea136a203182a2cb3e1e4317ae5db9e582a062495675e4`  
		Last Modified: Thu, 16 Jun 2022 22:22:03 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e5ae1d38fd0809723d5dc43ac11f9c1f200ac6fa5283e33fbca7dab640b923`  
		Last Modified: Thu, 16 Jun 2022 22:22:03 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:24f5488fd5aa896f3bc35dbc465c3b49f9b6d15a31395240b54b9cd3762347b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.0 MB (199037999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64d4259aa297df7d4d19d16adf08010b72d53a7ce5bcbe3e3373dfdad524a9fe`
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
# Thu, 16 Jun 2022 22:09:38 GMT
ENV INFLUXDB_VERSION=2.3.0
# Thu, 16 Jun 2022 22:09:47 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 16 Jun 2022 22:09:47 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 16 Jun 2022 22:09:50 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 16 Jun 2022 22:09:51 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Jun 2022 22:09:52 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Jun 2022 22:09:54 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Jun 2022 22:09:55 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 16 Jun 2022 22:09:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Jun 2022 22:09:56 GMT
CMD ["influxd"]
# Thu, 16 Jun 2022 22:09:57 GMT
EXPOSE 8086
# Thu, 16 Jun 2022 22:09:58 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Jun 2022 22:09:59 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Jun 2022 22:10:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Jun 2022 22:10:01 GMT
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
	-	`sha256:97c9820b7f7f53b34213d2f0aa4f2a26f67891b6e3e061177237035b1021725d`  
		Last Modified: Thu, 16 Jun 2022 22:11:34 GMT  
		Size: 180.8 MB (180792421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a8006c256ccb18b05dd77369f9e101bc086c7a512d874e375d5c9a13febe5e`  
		Last Modified: Thu, 16 Jun 2022 22:11:20 GMT  
		Size: 5.0 MB (4952646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccb26aa98552e698f543d5182c82ebb3d31f0d71e973a158749d6a274939259`  
		Last Modified: Thu, 16 Jun 2022 22:11:19 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181694003c21b466a912ba72a3e72ce95a926796c96945c4bbd20ef417d19ac3`  
		Last Modified: Thu, 16 Jun 2022 22:11:19 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d73c3913487d0d87a65bef6f026ab3d1104fe0a0f7638c837e970ddec9bae8`  
		Last Modified: Thu, 16 Jun 2022 22:11:19 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.3.0`

```console
$ docker pull influxdb@sha256:c6c2e3b84913b4ab0fcd4512d85af5796bb090cb1fbbb69ca1bbee85229ef155
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.3.0` - linux; amd64

```console
$ docker pull influxdb@sha256:107d9264ecf117e3ffc7dfd92d1642efc99ec3631f608574e857ef421acaa9fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255109369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24266999a5d6dabef266905c8d2b5dd227dc5d2a7ad4d43688414c0f96dbd39`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:20 GMT
ADD file:d738977543f4afc4c3040c6fca3e3f15388ec3b7263a29a6aa83f9a4bf05fed1 in / 
# Tue, 12 Jul 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:49:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:49:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jul 2022 00:48:08 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 13 Jul 2022 00:48:08 GMT
ENV GOSU_VER=1.12
# Wed, 13 Jul 2022 00:48:12 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 13 Jul 2022 00:48:49 GMT
ENV INFLUXDB_VERSION=2.3.0
# Wed, 13 Jul 2022 00:48:58 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 13 Jul 2022 00:48:58 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 13 Jul 2022 00:49:01 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 13 Jul 2022 00:49:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 13 Jul 2022 00:49:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 13 Jul 2022 00:49:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 13 Jul 2022 00:49:02 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 13 Jul 2022 00:49:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jul 2022 00:49:02 GMT
CMD ["influxd"]
# Wed, 13 Jul 2022 00:49:02 GMT
EXPOSE 8086
# Wed, 13 Jul 2022 00:49:02 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 13 Jul 2022 00:49:02 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 13 Jul 2022 00:49:02 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 13 Jul 2022 00:49:03 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:80b89a2b88b24e7be7c8038e2cbff99ad4fd2f07ad914da4bab80dabaadf8a99`  
		Last Modified: Tue, 12 Jul 2022 01:24:55 GMT  
		Size: 50.4 MB (50440555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0405f798f5b335d83b02371187f3be0ce2092aa0c6b6178ff11290ee6a14c9`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 7.9 MB (7856888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab80b2b0494ab26b41941fb73a028292e2e5d2070c56b3488e890eda20e04641`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 10.0 MB (9998095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99c88ddeebad2b651c3edb1be60a716c899a4fcc58c8cff5c0c880d08a4afa9`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c19bb70c8cbec52a00e4bf3a3dd775454b5ddc47e2043117e196580d12eae8d`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 961.0 KB (960956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91464f3385c50c198633e39fc1158d4c9935d69a0136c402c5ea945abb80bbc`  
		Last Modified: Wed, 13 Jul 2022 00:50:48 GMT  
		Size: 180.5 MB (180478667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9499689b44d8d0f59a4dca1b557b64afa08293491123eb9e1f284752eaf6cca3`  
		Last Modified: Wed, 13 Jul 2022 00:50:35 GMT  
		Size: 5.4 MB (5366851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407603165b5b499688be3a09145270e5ba712c3fd8c95c4c940ed82729ee2d60`  
		Last Modified: Wed, 13 Jul 2022 00:50:34 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33debaf42eb6f3e0db6f41f956503c49322db9df4321a6a45501bf4fea222cd`  
		Last Modified: Wed, 13 Jul 2022 00:50:34 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902fce46e4e728f6fdd16ed9b9fe622b2623e08c2a61db95562615b5953a866`  
		Last Modified: Wed, 13 Jul 2022 00:50:34 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.3.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ffef41c242c6916ddb8d72fdb0570d344dbe39335e4e6fd9b893921628f2d3a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253366128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6362fd64c09bae094ddfd07494eb7a1eb1554681e343815e1176395ed7e9090c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:46 GMT
ADD file:ea39534c5e9a548d7938f6b0e2459383caaf3906f3cc5eafe8bf66053b19f2d5 in / 
# Tue, 12 Jul 2022 00:40:47 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:34:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 21:30:54 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 12 Jul 2022 21:30:55 GMT
ENV GOSU_VER=1.12
# Tue, 12 Jul 2022 21:30:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 12 Jul 2022 21:32:22 GMT
ENV INFLUXDB_VERSION=2.3.0
# Tue, 12 Jul 2022 21:32:34 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 12 Jul 2022 21:32:34 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Tue, 12 Jul 2022 21:32:37 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 12 Jul 2022 21:32:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 12 Jul 2022 21:32:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 12 Jul 2022 21:32:41 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 12 Jul 2022 21:32:42 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Tue, 12 Jul 2022 21:32:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jul 2022 21:32:43 GMT
CMD ["influxd"]
# Tue, 12 Jul 2022 21:32:44 GMT
EXPOSE 8086
# Tue, 12 Jul 2022 21:32:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 12 Jul 2022 21:32:46 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 12 Jul 2022 21:32:47 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 12 Jul 2022 21:32:48 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:891a1587d3644a8b4b6dab3726ef380a725a0e19bfbf0eac02a275f711985862`  
		Last Modified: Tue, 12 Jul 2022 00:46:46 GMT  
		Size: 49.2 MB (49228928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d1ed6a27dab15e77b7afa9c8697a170f017a73ec9ea8f3f00d5f322e1d3ab`  
		Last Modified: Tue, 12 Jul 2022 02:43:49 GMT  
		Size: 7.7 MB (7720027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186afd5d5e89c602b988d31dd5210c9e3c19435f849f6cc4a6a22a2388e83cf`  
		Last Modified: Tue, 12 Jul 2022 02:43:46 GMT  
		Size: 9.8 MB (9768648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0df5326ac1fed63134e3c8159e5848b6b21984f5e3fcc471726138a3ad72a6`  
		Last Modified: Tue, 12 Jul 2022 21:33:32 GMT  
		Size: 1.7 KB (1657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6354ffc941f42e787a87e65c98641066c2adeab672dd2e105f4e774496dfd3`  
		Last Modified: Tue, 12 Jul 2022 21:33:33 GMT  
		Size: 896.3 KB (896337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fcbacb5196e76298c72f9f64008a67987259f9709231150fdeea7b7fd12dd4e`  
		Last Modified: Tue, 12 Jul 2022 21:34:31 GMT  
		Size: 180.8 MB (180792446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ae52c693b92622571c468956d2078a30f684e134ce2879c552615dad709462`  
		Last Modified: Tue, 12 Jul 2022 21:34:17 GMT  
		Size: 5.0 MB (4952629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4278dea3bc40dcf8ff123886bdc4a23bf8e95259e2d3ec1c84b590cea3e9679e`  
		Last Modified: Tue, 12 Jul 2022 21:34:16 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77049a9c8a367ea2f8305ccf9fe2bf18f86ccb3da6059b2eec5b86bbba7f02c9`  
		Last Modified: Tue, 12 Jul 2022 21:34:16 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a727154dea679e4df502e93e277dacbe7037f7b24e121011cfe0e528c91059bc`  
		Last Modified: Tue, 12 Jul 2022 21:34:17 GMT  
		Size: 5.0 KB (5013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.3.0-alpine`

```console
$ docker pull influxdb@sha256:b21e01fd74eee0d318cf02118efb94ca5c3f8053f73459f3c119c11f8886fd62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.3.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:02f15da8fa163ebf27a18e9abd3f2b2d1fee45e233e7fb2d149d938cb009ba0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.5 MB (199468297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f58a0c9c632cdb66195942a7f620ee5ed2dc5bc5db483b1f63c20b30023ad15`
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
# Thu, 16 Jun 2022 22:20:31 GMT
ENV INFLUXDB_VERSION=2.3.0
# Thu, 16 Jun 2022 22:20:39 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 16 Jun 2022 22:20:39 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 16 Jun 2022 22:20:42 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 16 Jun 2022 22:20:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Jun 2022 22:20:43 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Jun 2022 22:20:43 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Jun 2022 22:20:43 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 16 Jun 2022 22:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Jun 2022 22:20:43 GMT
CMD ["influxd"]
# Thu, 16 Jun 2022 22:20:43 GMT
EXPOSE 8086
# Thu, 16 Jun 2022 22:20:43 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Jun 2022 22:20:44 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Jun 2022 22:20:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Jun 2022 22:20:44 GMT
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
	-	`sha256:c3a5beaff1353f4dc69c0a10bd65e7116a89188cc22e05d2f754dd3f73111c0d`  
		Last Modified: Thu, 16 Jun 2022 22:22:16 GMT  
		Size: 180.5 MB (180478679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325149cfb67924e4de205f483e9c2d03dfa7b477d1f7e63d6fcde2146a88e70a`  
		Last Modified: Thu, 16 Jun 2022 22:22:04 GMT  
		Size: 5.4 MB (5366873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b918e22717c1cb5d940f7a0d9fc54ae5f3908a124081a8d9596905c80341a2cc`  
		Last Modified: Thu, 16 Jun 2022 22:22:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa245e7165eba29536ea136a203182a2cb3e1e4317ae5db9e582a062495675e4`  
		Last Modified: Thu, 16 Jun 2022 22:22:03 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e5ae1d38fd0809723d5dc43ac11f9c1f200ac6fa5283e33fbca7dab640b923`  
		Last Modified: Thu, 16 Jun 2022 22:22:03 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:24f5488fd5aa896f3bc35dbc465c3b49f9b6d15a31395240b54b9cd3762347b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.0 MB (199037999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64d4259aa297df7d4d19d16adf08010b72d53a7ce5bcbe3e3373dfdad524a9fe`
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
# Thu, 16 Jun 2022 22:09:38 GMT
ENV INFLUXDB_VERSION=2.3.0
# Thu, 16 Jun 2022 22:09:47 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 16 Jun 2022 22:09:47 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 16 Jun 2022 22:09:50 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 16 Jun 2022 22:09:51 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Jun 2022 22:09:52 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Jun 2022 22:09:54 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Jun 2022 22:09:55 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 16 Jun 2022 22:09:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Jun 2022 22:09:56 GMT
CMD ["influxd"]
# Thu, 16 Jun 2022 22:09:57 GMT
EXPOSE 8086
# Thu, 16 Jun 2022 22:09:58 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Jun 2022 22:09:59 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Jun 2022 22:10:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Jun 2022 22:10:01 GMT
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
	-	`sha256:97c9820b7f7f53b34213d2f0aa4f2a26f67891b6e3e061177237035b1021725d`  
		Last Modified: Thu, 16 Jun 2022 22:11:34 GMT  
		Size: 180.8 MB (180792421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a8006c256ccb18b05dd77369f9e101bc086c7a512d874e375d5c9a13febe5e`  
		Last Modified: Thu, 16 Jun 2022 22:11:20 GMT  
		Size: 5.0 MB (4952646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccb26aa98552e698f543d5182c82ebb3d31f0d71e973a158749d6a274939259`  
		Last Modified: Thu, 16 Jun 2022 22:11:19 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181694003c21b466a912ba72a3e72ce95a926796c96945c4bbd20ef417d19ac3`  
		Last Modified: Thu, 16 Jun 2022 22:11:19 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d73c3913487d0d87a65bef6f026ab3d1104fe0a0f7638c837e970ddec9bae8`  
		Last Modified: Thu, 16 Jun 2022 22:11:19 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:b21e01fd74eee0d318cf02118efb94ca5c3f8053f73459f3c119c11f8886fd62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:02f15da8fa163ebf27a18e9abd3f2b2d1fee45e233e7fb2d149d938cb009ba0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.5 MB (199468297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f58a0c9c632cdb66195942a7f620ee5ed2dc5bc5db483b1f63c20b30023ad15`
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
# Thu, 16 Jun 2022 22:20:31 GMT
ENV INFLUXDB_VERSION=2.3.0
# Thu, 16 Jun 2022 22:20:39 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 16 Jun 2022 22:20:39 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 16 Jun 2022 22:20:42 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 16 Jun 2022 22:20:43 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Jun 2022 22:20:43 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Jun 2022 22:20:43 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Jun 2022 22:20:43 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 16 Jun 2022 22:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Jun 2022 22:20:43 GMT
CMD ["influxd"]
# Thu, 16 Jun 2022 22:20:43 GMT
EXPOSE 8086
# Thu, 16 Jun 2022 22:20:43 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Jun 2022 22:20:44 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Jun 2022 22:20:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Jun 2022 22:20:44 GMT
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
	-	`sha256:c3a5beaff1353f4dc69c0a10bd65e7116a89188cc22e05d2f754dd3f73111c0d`  
		Last Modified: Thu, 16 Jun 2022 22:22:16 GMT  
		Size: 180.5 MB (180478679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325149cfb67924e4de205f483e9c2d03dfa7b477d1f7e63d6fcde2146a88e70a`  
		Last Modified: Thu, 16 Jun 2022 22:22:04 GMT  
		Size: 5.4 MB (5366873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b918e22717c1cb5d940f7a0d9fc54ae5f3908a124081a8d9596905c80341a2cc`  
		Last Modified: Thu, 16 Jun 2022 22:22:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa245e7165eba29536ea136a203182a2cb3e1e4317ae5db9e582a062495675e4`  
		Last Modified: Thu, 16 Jun 2022 22:22:03 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e5ae1d38fd0809723d5dc43ac11f9c1f200ac6fa5283e33fbca7dab640b923`  
		Last Modified: Thu, 16 Jun 2022 22:22:03 GMT  
		Size: 5.0 KB (5017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:24f5488fd5aa896f3bc35dbc465c3b49f9b6d15a31395240b54b9cd3762347b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.0 MB (199037999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64d4259aa297df7d4d19d16adf08010b72d53a7ce5bcbe3e3373dfdad524a9fe`
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
# Thu, 16 Jun 2022 22:09:38 GMT
ENV INFLUXDB_VERSION=2.3.0
# Thu, 16 Jun 2022 22:09:47 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Thu, 16 Jun 2022 22:09:47 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Thu, 16 Jun 2022 22:09:50 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Thu, 16 Jun 2022 22:09:51 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Thu, 16 Jun 2022 22:09:52 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Thu, 16 Jun 2022 22:09:54 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Thu, 16 Jun 2022 22:09:55 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Thu, 16 Jun 2022 22:09:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Jun 2022 22:09:56 GMT
CMD ["influxd"]
# Thu, 16 Jun 2022 22:09:57 GMT
EXPOSE 8086
# Thu, 16 Jun 2022 22:09:58 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Thu, 16 Jun 2022 22:09:59 GMT
ENV INFLUXD_INIT_PORT=9999
# Thu, 16 Jun 2022 22:10:00 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Thu, 16 Jun 2022 22:10:01 GMT
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
	-	`sha256:97c9820b7f7f53b34213d2f0aa4f2a26f67891b6e3e061177237035b1021725d`  
		Last Modified: Thu, 16 Jun 2022 22:11:34 GMT  
		Size: 180.8 MB (180792421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a8006c256ccb18b05dd77369f9e101bc086c7a512d874e375d5c9a13febe5e`  
		Last Modified: Thu, 16 Jun 2022 22:11:20 GMT  
		Size: 5.0 MB (4952646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccb26aa98552e698f543d5182c82ebb3d31f0d71e973a158749d6a274939259`  
		Last Modified: Thu, 16 Jun 2022 22:11:19 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181694003c21b466a912ba72a3e72ce95a926796c96945c4bbd20ef417d19ac3`  
		Last Modified: Thu, 16 Jun 2022 22:11:19 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d73c3913487d0d87a65bef6f026ab3d1104fe0a0f7638c837e970ddec9bae8`  
		Last Modified: Thu, 16 Jun 2022 22:11:19 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:fb64ca8970ce9f6b4d235de14124af0c998e3960436f5fd6429daa1084179b8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:bebc8358fd24a1888e3ad376a96896693beb7539ad66f8560908e735d9661603
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117789620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d217aae6287d1db96b3e3790861ee7c4d6606f2b7bb0321ea1fd5982f2f4ed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:17:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:18:14 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 23 Jun 2022 15:18:20 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 23 Jun 2022 15:18:21 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 23 Jun 2022 15:18:21 GMT
EXPOSE 8086
# Thu, 23 Jun 2022 15:18:21 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 15:18:21 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 23 Jun 2022 15:18:21 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 23 Jun 2022 15:18:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:18:21 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86e15a947f1f4c2ec5261546aba1007d9944f87c77bed2eb2cb9f38d91fe491`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950f7b7fdaff085645293a46684da21b15044d943489a4d2c277b4b26e680e9b`  
		Last Modified: Thu, 23 Jun 2022 15:20:56 GMT  
		Size: 56.7 MB (56709124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1872d73bcff1f595b2830cd35fc5f092d8c2a50d078b790877f9118613c8e1`  
		Last Modified: Thu, 23 Jun 2022 15:20:49 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d58f2fb0c6074e97aed0e4d9ddc3a70065731436d5c1d738acac3e66f6f62f`  
		Last Modified: Thu, 23 Jun 2022 15:20:49 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9a5e047ca0e0553d8afd2a4bd60baa41783dcdb113de5cb1c656091d7e0049`  
		Last Modified: Thu, 23 Jun 2022 15:20:49 GMT  
		Size: 1.3 KB (1280 bytes)  
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
$ docker pull influxdb@sha256:c6c2e3b84913b4ab0fcd4512d85af5796bb090cb1fbbb69ca1bbee85229ef155
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:107d9264ecf117e3ffc7dfd92d1642efc99ec3631f608574e857ef421acaa9fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255109369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24266999a5d6dabef266905c8d2b5dd227dc5d2a7ad4d43688414c0f96dbd39`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:20 GMT
ADD file:d738977543f4afc4c3040c6fca3e3f15388ec3b7263a29a6aa83f9a4bf05fed1 in / 
# Tue, 12 Jul 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:49:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:49:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jul 2022 00:48:08 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 13 Jul 2022 00:48:08 GMT
ENV GOSU_VER=1.12
# Wed, 13 Jul 2022 00:48:12 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Wed, 13 Jul 2022 00:48:49 GMT
ENV INFLUXDB_VERSION=2.3.0
# Wed, 13 Jul 2022 00:48:58 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 13 Jul 2022 00:48:58 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Wed, 13 Jul 2022 00:49:01 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 13 Jul 2022 00:49:02 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 13 Jul 2022 00:49:02 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 13 Jul 2022 00:49:02 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 13 Jul 2022 00:49:02 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Wed, 13 Jul 2022 00:49:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jul 2022 00:49:02 GMT
CMD ["influxd"]
# Wed, 13 Jul 2022 00:49:02 GMT
EXPOSE 8086
# Wed, 13 Jul 2022 00:49:02 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 13 Jul 2022 00:49:02 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 13 Jul 2022 00:49:02 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 13 Jul 2022 00:49:03 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:80b89a2b88b24e7be7c8038e2cbff99ad4fd2f07ad914da4bab80dabaadf8a99`  
		Last Modified: Tue, 12 Jul 2022 01:24:55 GMT  
		Size: 50.4 MB (50440555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0405f798f5b335d83b02371187f3be0ce2092aa0c6b6178ff11290ee6a14c9`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 7.9 MB (7856888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab80b2b0494ab26b41941fb73a028292e2e5d2070c56b3488e890eda20e04641`  
		Last Modified: Tue, 12 Jul 2022 02:56:14 GMT  
		Size: 10.0 MB (9998095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99c88ddeebad2b651c3edb1be60a716c899a4fcc58c8cff5c0c880d08a4afa9`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c19bb70c8cbec52a00e4bf3a3dd775454b5ddc47e2043117e196580d12eae8d`  
		Last Modified: Wed, 13 Jul 2022 00:49:58 GMT  
		Size: 961.0 KB (960956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91464f3385c50c198633e39fc1158d4c9935d69a0136c402c5ea945abb80bbc`  
		Last Modified: Wed, 13 Jul 2022 00:50:48 GMT  
		Size: 180.5 MB (180478667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9499689b44d8d0f59a4dca1b557b64afa08293491123eb9e1f284752eaf6cca3`  
		Last Modified: Wed, 13 Jul 2022 00:50:35 GMT  
		Size: 5.4 MB (5366851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407603165b5b499688be3a09145270e5ba712c3fd8c95c4c940ed82729ee2d60`  
		Last Modified: Wed, 13 Jul 2022 00:50:34 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33debaf42eb6f3e0db6f41f956503c49322db9df4321a6a45501bf4fea222cd`  
		Last Modified: Wed, 13 Jul 2022 00:50:34 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902fce46e4e728f6fdd16ed9b9fe622b2623e08c2a61db95562615b5953a866`  
		Last Modified: Wed, 13 Jul 2022 00:50:34 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ffef41c242c6916ddb8d72fdb0570d344dbe39335e4e6fd9b893921628f2d3a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253366128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6362fd64c09bae094ddfd07494eb7a1eb1554681e343815e1176395ed7e9090c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:46 GMT
ADD file:ea39534c5e9a548d7938f6b0e2459383caaf3906f3cc5eafe8bf66053b19f2d5 in / 
# Tue, 12 Jul 2022 00:40:47 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:34:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 21:30:54 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 12 Jul 2022 21:30:55 GMT
ENV GOSU_VER=1.12
# Tue, 12 Jul 2022 21:30:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)" &&     wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" &&     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" &&     export GNUPGHOME="$(mktemp -d)" &&     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 &&     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc &&     chmod +x /usr/local/bin/gosu &&     gosu --version &&     gosu nobody true
# Tue, 12 Jul 2022 21:32:22 GMT
ENV INFLUXDB_VERSION=2.3.0
# Tue, 12 Jul 2022 21:32:34 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2_linux_${ARCH}/influxd /usr/local/bin/influxd &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 12 Jul 2022 21:32:34 GMT
ENV INFLUX_CLI_VERSION=2.3.0
# Tue, 12 Jul 2022 21:32:37 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 12 Jul 2022 21:32:38 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 12 Jul 2022 21:32:39 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 12 Jul 2022 21:32:41 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 12 Jul 2022 21:32:42 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Tue, 12 Jul 2022 21:32:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jul 2022 21:32:43 GMT
CMD ["influxd"]
# Tue, 12 Jul 2022 21:32:44 GMT
EXPOSE 8086
# Tue, 12 Jul 2022 21:32:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 12 Jul 2022 21:32:46 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 12 Jul 2022 21:32:47 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 12 Jul 2022 21:32:48 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:891a1587d3644a8b4b6dab3726ef380a725a0e19bfbf0eac02a275f711985862`  
		Last Modified: Tue, 12 Jul 2022 00:46:46 GMT  
		Size: 49.2 MB (49228928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d1ed6a27dab15e77b7afa9c8697a170f017a73ec9ea8f3f00d5f322e1d3ab`  
		Last Modified: Tue, 12 Jul 2022 02:43:49 GMT  
		Size: 7.7 MB (7720027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186afd5d5e89c602b988d31dd5210c9e3c19435f849f6cc4a6a22a2388e83cf`  
		Last Modified: Tue, 12 Jul 2022 02:43:46 GMT  
		Size: 9.8 MB (9768648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0df5326ac1fed63134e3c8159e5848b6b21984f5e3fcc471726138a3ad72a6`  
		Last Modified: Tue, 12 Jul 2022 21:33:32 GMT  
		Size: 1.7 KB (1657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6354ffc941f42e787a87e65c98641066c2adeab672dd2e105f4e774496dfd3`  
		Last Modified: Tue, 12 Jul 2022 21:33:33 GMT  
		Size: 896.3 KB (896337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fcbacb5196e76298c72f9f64008a67987259f9709231150fdeea7b7fd12dd4e`  
		Last Modified: Tue, 12 Jul 2022 21:34:31 GMT  
		Size: 180.8 MB (180792446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ae52c693b92622571c468956d2078a30f684e134ce2879c552615dad709462`  
		Last Modified: Tue, 12 Jul 2022 21:34:17 GMT  
		Size: 5.0 MB (4952629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4278dea3bc40dcf8ff123886bdc4a23bf8e95259e2d3ec1c84b590cea3e9679e`  
		Last Modified: Tue, 12 Jul 2022 21:34:16 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77049a9c8a367ea2f8305ccf9fe2bf18f86ccb3da6059b2eec5b86bbba7f02c9`  
		Last Modified: Tue, 12 Jul 2022 21:34:16 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a727154dea679e4df502e93e277dacbe7037f7b24e121011cfe0e528c91059bc`  
		Last Modified: Tue, 12 Jul 2022 21:34:17 GMT  
		Size: 5.0 KB (5013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:22802a6c409c5cdd3bc054c2196b8320041e1be81dfa4683d21358cd832113d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:7ecfdafa61c3d2d3f057774038cf7c870861c9d1f094abb763bbccda889be0fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84496164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:095bfff223c443c0e87ec288f1462d1732302060b304b9799c4b17ae4447e1b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:10 GMT
ADD file:4c5e0bec5f780d9c6bfbafcb9e6ed641781dd7f7c2853a0c49d6613e9fef9516 in / 
# Thu, 23 Jun 2022 00:22:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:54:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:54:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 15:17:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 23 Jun 2022 15:18:14 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 23 Jun 2022 15:18:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 23 Jun 2022 15:18:30 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 23 Jun 2022 15:18:30 GMT
EXPOSE 8091
# Thu, 23 Jun 2022 15:18:30 GMT
VOLUME [/var/lib/influxdb]
# Thu, 23 Jun 2022 15:18:30 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 23 Jun 2022 15:18:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 15:18:30 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:8372a04f222be82bf67eb0010a59644b1e52f1246b3da9034edaa98f3d591cae`  
		Last Modified: Thu, 23 Jun 2022 00:29:36 GMT  
		Size: 45.4 MB (45430020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1728fee80d376293a9ef5fdcc0acd3f6398fc4159b12064ce4c1e66f67e7e9d`  
		Last Modified: Thu, 23 Jun 2022 01:02:01 GMT  
		Size: 11.3 MB (11302923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cf50aa0a4b80b39d1bf4be232d404da0b1ad38cdd3bb1a017b727947b5f4bb`  
		Last Modified: Thu, 23 Jun 2022 01:02:00 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86e15a947f1f4c2ec5261546aba1007d9944f87c77bed2eb2cb9f38d91fe491`  
		Last Modified: Thu, 23 Jun 2022 15:20:31 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7551c1766386d104f430be81f49cfaa95686138d88c7038f7e6cfd1e66f4c`  
		Last Modified: Thu, 23 Jun 2022 15:21:14 GMT  
		Size: 23.4 MB (23416877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535fe8a7786b0b29380c8643d4e5e61e5e5017afcfa08a3b8af6742f09dc3a68`  
		Last Modified: Thu, 23 Jun 2022 15:21:11 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa9e12f9123b3fb169ca58d9afa4152583f9f5531c26fa69ce35b5e7ec63667`  
		Last Modified: Thu, 23 Jun 2022 15:21:11 GMT  
		Size: 371.0 B  
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
