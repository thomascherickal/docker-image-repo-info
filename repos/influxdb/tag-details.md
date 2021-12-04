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
$ docker pull influxdb@sha256:9fd0539c4beda3b3fb5b9048653d7ea01af21eb14678a7a2edafa5a64a99c4a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7` - linux; amd64

```console
$ docker pull influxdb@sha256:259f405e896f24959510def763d50c74f28b6241d1a2c4ec906b757767a55595
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122315011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456adca50c37d73c85118c562b93b1537fc55d01be3275e028a9e730efbc1a03`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:14:05 GMT
ENV INFLUXDB_VERSION=1.7.11
# Fri, 03 Dec 2021 04:14:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 03 Dec 2021 04:14:14 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:14:14 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:14:14 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:14:14 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:14:15 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:14:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:14:15 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e37a81a7ff55764afc13aa71d037b3578bff0cf0526003b5dbf480ce3c60ea`  
		Last Modified: Fri, 03 Dec 2021 04:17:41 GMT  
		Size: 61.3 MB (61285098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3216a19437e44a8b0b9b8b84b501f24a5eddeee8c3c1f31940ee5f8a5e15ec`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96adcc23252368b160a38944aae82edfbbe622aba7248d22817c80ec76c631c`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18f29fd51eef19762924a48a31aa147dbf637debd58e42c643a2e22e12c0974`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:1ce5540af45251a6b89f9b410e84c63aefd83f4890c39ee996d1686f9c31cf17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113467660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29f70064d620f46dd382ba651ec41c8f510d839fb763ab5f504c403469cb94f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 09:10:39 GMT
ADD file:1f947e5a3f8b1da292340501298edf2b879183aea9e90531f21c2b22500e79ad in / 
# Thu, 02 Dec 2021 09:10:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:49:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Dec 2021 02:31:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 04 Dec 2021 02:31:19 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 04 Dec 2021 02:31:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 04 Dec 2021 02:31:34 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 04 Dec 2021 02:31:34 GMT
EXPOSE 8086
# Sat, 04 Dec 2021 02:31:35 GMT
VOLUME [/var/lib/influxdb]
# Sat, 04 Dec 2021 02:31:35 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 04 Dec 2021 02:31:36 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 04 Dec 2021 02:31:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Dec 2021 02:31:36 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:fdee104a33d14b2fdafeeaca15f0252d32280549d3cdc971244796c6e69ad0d3`  
		Last Modified: Thu, 02 Dec 2021 09:27:53 GMT  
		Size: 42.1 MB (42116754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44a93596b701db7b6e00e592b43547b3bbb7e984a3634dd91b34eb72c03ef1e`  
		Last Modified: Thu, 02 Dec 2021 12:08:46 GMT  
		Size: 10.0 MB (9956149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a002f84bb513d353d241296eda1ba0f01560a1ded46af2fe62c236c787a7559a`  
		Last Modified: Thu, 02 Dec 2021 12:08:43 GMT  
		Size: 3.9 MB (3921247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7512265925fd9b3295643dd954fe13e32b70794c509e55fe7f3c39a408ad3ec2`  
		Last Modified: Sat, 04 Dec 2021 02:32:41 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d91ccc1fc3e8c11ef443bc407ba0a16031376797b385e4a3a1359e84a66542`  
		Last Modified: Sat, 04 Dec 2021 02:33:10 GMT  
		Size: 57.5 MB (57468935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e347c344e882ab4f33501b268b94f07835bcb9ba7faff79f7a006aca65a3eb59`  
		Last Modified: Sat, 04 Dec 2021 02:32:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05082df7631e6b940f1b707d98fd269c32cb79cfbed3905dec2785854e228da8`  
		Last Modified: Sat, 04 Dec 2021 02:32:41 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e8c00b66ff3dd43aae1bbbc41647a04772ad7d647ad8287d78efed3cb3c798`  
		Last Modified: Sat, 04 Dec 2021 02:32:41 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:3b9408efbc60def781ca885fd6894e820e03fc8afdd2c285803c90625ff96a3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114473334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da6c02a6af37f6f108cec7e16495616a995529375d758514c479db19661aaf89`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 08:10:09 GMT
ADD file:7be59c7e3b187d010c0e8625e45324f421a21518258e6bd35bab6e0e86c9494c in / 
# Thu, 02 Dec 2021 08:10:10 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:57:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:47:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:47:28 GMT
ENV INFLUXDB_VERSION=1.7.11
# Fri, 03 Dec 2021 04:47:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 03 Dec 2021 04:47:36 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:47:36 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:47:37 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:47:39 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:47:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:47:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:47:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6965f119641a6f16b55da01b7c12884960366228a181268b0bf7d0b7d50b2336`  
		Last Modified: Thu, 02 Dec 2021 08:44:30 GMT  
		Size: 43.2 MB (43173684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e211a2e7bbb27084e1f8cd62281719dc9d90e3ddb76b862e471b1cde61512cb`  
		Last Modified: Thu, 02 Dec 2021 10:08:36 GMT  
		Size: 10.2 MB (10216757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca410b1e11dc0ad76bc18c383eafa45a44c94916e27e4f327bc75a9373a250ca`  
		Last Modified: Thu, 02 Dec 2021 10:08:34 GMT  
		Size: 3.9 MB (3873863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b42056f3d6099ac63c397725439faee3120acd8c334e07f81423af0461472e`  
		Last Modified: Fri, 03 Dec 2021 04:50:04 GMT  
		Size: 2.8 KB (2828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2016e40a54fa6f9bd61c47a1acd6bd78b9cdefb18420625f7b698aba3cbe20b9`  
		Last Modified: Fri, 03 Dec 2021 04:50:11 GMT  
		Size: 57.2 MB (57204486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9b752028715f4359e86d0013b891808085924c8a28b712021ada44751760cb`  
		Last Modified: Fri, 03 Dec 2021 04:50:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439b0477b2047db17487dad880a6b327c83a784bab051f3f1561740dff47c8ac`  
		Last Modified: Fri, 03 Dec 2021 04:50:04 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d2077bb7e6dafc404b2ffa1d1bc559941c13b9f262b88e36f84adf24c566de`  
		Last Modified: Fri, 03 Dec 2021 04:50:04 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:c135764c4b9066b80cbe32011ee2afa29b2f4a62919b244b76248b45604d26ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:fe9e4e64aa24f80640e60be53f70f0f8f30f0abe167c954b4e4bcd136ffcd48b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148978976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fdf17676851542b7e4923288cb4757c297163fd5ee0413d012d5c8bc3fa98b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:14:22 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Fri, 03 Dec 2021 04:14:33 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:14:33 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:14:33 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:14:34 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:14:34 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:14:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:14:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:14:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849c215c2217b301cd93253ad24ea33921f986b02c0b3e00f5da2bd433fd9a69`  
		Last Modified: Fri, 03 Dec 2021 04:18:03 GMT  
		Size: 87.9 MB (87949002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec36390bb5f09f2c1acd74a2e75b1d83318a102888cc1f1da2a2289e286ada8`  
		Last Modified: Fri, 03 Dec 2021 04:17:51 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab9b2ad2b10c6bd26599441350332e66151356df4575300a4f776c80dd1d4ba`  
		Last Modified: Fri, 03 Dec 2021 04:17:51 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891ec8d3660d1b00b87e5c2b15ecf4b0a82e7b87dc95224f4ea7763b62e78287`  
		Last Modified: Fri, 03 Dec 2021 04:17:52 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:584263ef784f3e925f420997af104e73ae544c142d0a2ee8ca952ecde8fa868f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:2201986c58cf211289a081d810873f20c2bfab06f7974c3c91e3de29ab8a3c12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84162340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fe91a869885376430184c6fa3d070c6868d6613d908349cc6fcb1b200bba10b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:14:22 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Fri, 03 Dec 2021 04:14:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:14:44 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 03 Dec 2021 04:14:44 GMT
EXPOSE 8091
# Fri, 03 Dec 2021 04:14:45 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:14:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:14:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:14:45 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dce2807a467616a038e10fea70284f51768f1c0957174bca5f61aba1bf2a9f8`  
		Last Modified: Fri, 03 Dec 2021 04:18:18 GMT  
		Size: 23.1 MB (23133574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed03e026f788ff6b999ccc5669124364e463e512216e536efb80fcce70274ce`  
		Last Modified: Fri, 03 Dec 2021 04:18:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf74e2f3ffbbd33c35022bd4507f4b107730bdd97c3797a38ec5c876fbdb242`  
		Last Modified: Fri, 03 Dec 2021 04:18:15 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:9fd0539c4beda3b3fb5b9048653d7ea01af21eb14678a7a2edafa5a64a99c4a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7.11` - linux; amd64

```console
$ docker pull influxdb@sha256:259f405e896f24959510def763d50c74f28b6241d1a2c4ec906b757767a55595
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122315011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456adca50c37d73c85118c562b93b1537fc55d01be3275e028a9e730efbc1a03`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:14:05 GMT
ENV INFLUXDB_VERSION=1.7.11
# Fri, 03 Dec 2021 04:14:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 03 Dec 2021 04:14:14 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:14:14 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:14:14 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:14:14 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:14:15 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:14:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:14:15 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e37a81a7ff55764afc13aa71d037b3578bff0cf0526003b5dbf480ce3c60ea`  
		Last Modified: Fri, 03 Dec 2021 04:17:41 GMT  
		Size: 61.3 MB (61285098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3216a19437e44a8b0b9b8b84b501f24a5eddeee8c3c1f31940ee5f8a5e15ec`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96adcc23252368b160a38944aae82edfbbe622aba7248d22817c80ec76c631c`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18f29fd51eef19762924a48a31aa147dbf637debd58e42c643a2e22e12c0974`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:1ce5540af45251a6b89f9b410e84c63aefd83f4890c39ee996d1686f9c31cf17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113467660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29f70064d620f46dd382ba651ec41c8f510d839fb763ab5f504c403469cb94f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 09:10:39 GMT
ADD file:1f947e5a3f8b1da292340501298edf2b879183aea9e90531f21c2b22500e79ad in / 
# Thu, 02 Dec 2021 09:10:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:49:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Dec 2021 02:31:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 04 Dec 2021 02:31:19 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 04 Dec 2021 02:31:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 04 Dec 2021 02:31:34 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 04 Dec 2021 02:31:34 GMT
EXPOSE 8086
# Sat, 04 Dec 2021 02:31:35 GMT
VOLUME [/var/lib/influxdb]
# Sat, 04 Dec 2021 02:31:35 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 04 Dec 2021 02:31:36 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 04 Dec 2021 02:31:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Dec 2021 02:31:36 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:fdee104a33d14b2fdafeeaca15f0252d32280549d3cdc971244796c6e69ad0d3`  
		Last Modified: Thu, 02 Dec 2021 09:27:53 GMT  
		Size: 42.1 MB (42116754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44a93596b701db7b6e00e592b43547b3bbb7e984a3634dd91b34eb72c03ef1e`  
		Last Modified: Thu, 02 Dec 2021 12:08:46 GMT  
		Size: 10.0 MB (9956149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a002f84bb513d353d241296eda1ba0f01560a1ded46af2fe62c236c787a7559a`  
		Last Modified: Thu, 02 Dec 2021 12:08:43 GMT  
		Size: 3.9 MB (3921247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7512265925fd9b3295643dd954fe13e32b70794c509e55fe7f3c39a408ad3ec2`  
		Last Modified: Sat, 04 Dec 2021 02:32:41 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d91ccc1fc3e8c11ef443bc407ba0a16031376797b385e4a3a1359e84a66542`  
		Last Modified: Sat, 04 Dec 2021 02:33:10 GMT  
		Size: 57.5 MB (57468935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e347c344e882ab4f33501b268b94f07835bcb9ba7faff79f7a006aca65a3eb59`  
		Last Modified: Sat, 04 Dec 2021 02:32:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05082df7631e6b940f1b707d98fd269c32cb79cfbed3905dec2785854e228da8`  
		Last Modified: Sat, 04 Dec 2021 02:32:41 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e8c00b66ff3dd43aae1bbbc41647a04772ad7d647ad8287d78efed3cb3c798`  
		Last Modified: Sat, 04 Dec 2021 02:32:41 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:3b9408efbc60def781ca885fd6894e820e03fc8afdd2c285803c90625ff96a3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114473334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da6c02a6af37f6f108cec7e16495616a995529375d758514c479db19661aaf89`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 08:10:09 GMT
ADD file:7be59c7e3b187d010c0e8625e45324f421a21518258e6bd35bab6e0e86c9494c in / 
# Thu, 02 Dec 2021 08:10:10 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:57:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:47:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:47:28 GMT
ENV INFLUXDB_VERSION=1.7.11
# Fri, 03 Dec 2021 04:47:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 03 Dec 2021 04:47:36 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:47:36 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:47:37 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:47:39 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:47:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:47:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:47:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6965f119641a6f16b55da01b7c12884960366228a181268b0bf7d0b7d50b2336`  
		Last Modified: Thu, 02 Dec 2021 08:44:30 GMT  
		Size: 43.2 MB (43173684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e211a2e7bbb27084e1f8cd62281719dc9d90e3ddb76b862e471b1cde61512cb`  
		Last Modified: Thu, 02 Dec 2021 10:08:36 GMT  
		Size: 10.2 MB (10216757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca410b1e11dc0ad76bc18c383eafa45a44c94916e27e4f327bc75a9373a250ca`  
		Last Modified: Thu, 02 Dec 2021 10:08:34 GMT  
		Size: 3.9 MB (3873863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b42056f3d6099ac63c397725439faee3120acd8c334e07f81423af0461472e`  
		Last Modified: Fri, 03 Dec 2021 04:50:04 GMT  
		Size: 2.8 KB (2828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2016e40a54fa6f9bd61c47a1acd6bd78b9cdefb18420625f7b698aba3cbe20b9`  
		Last Modified: Fri, 03 Dec 2021 04:50:11 GMT  
		Size: 57.2 MB (57204486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9b752028715f4359e86d0013b891808085924c8a28b712021ada44751760cb`  
		Last Modified: Fri, 03 Dec 2021 04:50:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439b0477b2047db17487dad880a6b327c83a784bab051f3f1561740dff47c8ac`  
		Last Modified: Fri, 03 Dec 2021 04:50:04 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d2077bb7e6dafc404b2ffa1d1bc559941c13b9f262b88e36f84adf24c566de`  
		Last Modified: Fri, 03 Dec 2021 04:50:04 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:c135764c4b9066b80cbe32011ee2afa29b2f4a62919b244b76248b45604d26ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:fe9e4e64aa24f80640e60be53f70f0f8f30f0abe167c954b4e4bcd136ffcd48b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148978976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fdf17676851542b7e4923288cb4757c297163fd5ee0413d012d5c8bc3fa98b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:14:22 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Fri, 03 Dec 2021 04:14:33 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:14:33 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:14:33 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:14:34 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:14:34 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:14:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:14:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:14:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849c215c2217b301cd93253ad24ea33921f986b02c0b3e00f5da2bd433fd9a69`  
		Last Modified: Fri, 03 Dec 2021 04:18:03 GMT  
		Size: 87.9 MB (87949002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec36390bb5f09f2c1acd74a2e75b1d83318a102888cc1f1da2a2289e286ada8`  
		Last Modified: Fri, 03 Dec 2021 04:17:51 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab9b2ad2b10c6bd26599441350332e66151356df4575300a4f776c80dd1d4ba`  
		Last Modified: Fri, 03 Dec 2021 04:17:51 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891ec8d3660d1b00b87e5c2b15ecf4b0a82e7b87dc95224f4ea7763b62e78287`  
		Last Modified: Fri, 03 Dec 2021 04:17:52 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:584263ef784f3e925f420997af104e73ae544c142d0a2ee8ca952ecde8fa868f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:2201986c58cf211289a081d810873f20c2bfab06f7974c3c91e3de29ab8a3c12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84162340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fe91a869885376430184c6fa3d070c6868d6613d908349cc6fcb1b200bba10b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:14:22 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Fri, 03 Dec 2021 04:14:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:14:44 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 03 Dec 2021 04:14:44 GMT
EXPOSE 8091
# Fri, 03 Dec 2021 04:14:45 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:14:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:14:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:14:45 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dce2807a467616a038e10fea70284f51768f1c0957174bca5f61aba1bf2a9f8`  
		Last Modified: Fri, 03 Dec 2021 04:18:18 GMT  
		Size: 23.1 MB (23133574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed03e026f788ff6b999ccc5669124364e463e512216e536efb80fcce70274ce`  
		Last Modified: Fri, 03 Dec 2021 04:18:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf74e2f3ffbbd33c35022bd4507f4b107730bdd97c3797a38ec5c876fbdb242`  
		Last Modified: Fri, 03 Dec 2021 04:18:15 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:49192399ceb736debe0202c3a1c5f8277e3ad53546c221779f4b61399a0bbee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:39cbab2f88a703d47b90645f64f585c4d9dea140309e045cd364dc9a341dbca4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115919392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a59ddecfe8fd96530b091dfccc9e23abdaf18b9389e258cb9753ea7059b13f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:14:50 GMT
ENV INFLUXDB_VERSION=1.8.10
# Fri, 03 Dec 2021 04:14:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 03 Dec 2021 04:14:56 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:14:56 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:14:56 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:14:56 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:14:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:14:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:14:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d272c6b4c091f2677bc94174cb715217c60c2346131cfd35607ecea81de080`  
		Last Modified: Fri, 03 Dec 2021 04:18:37 GMT  
		Size: 54.9 MB (54889479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199ff8c6aaebce00fd628792d5beb096ccb3c473641cc7ccf4bf4484535ec9a4`  
		Last Modified: Fri, 03 Dec 2021 04:18:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976ce52fa9d59ed0b81f6e6fb52151f2a99da8fa2789a9289f79ed80099f854`  
		Last Modified: Fri, 03 Dec 2021 04:18:29 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af89678e0336ac5e6e2c65046f6a7737c3131d934555ffe8365c0598ec61ee3d`  
		Last Modified: Fri, 03 Dec 2021 04:18:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:9b85c3a9381ff73dfda178f23a3ce55268f1742bd920e24ed876d63ca40a3fb9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107615555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37694b7723f827ed73be61288cd73c1728103682a5b938b62cc258928aa99be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 09:10:39 GMT
ADD file:1f947e5a3f8b1da292340501298edf2b879183aea9e90531f21c2b22500e79ad in / 
# Thu, 02 Dec 2021 09:10:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:49:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Dec 2021 02:31:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 04 Dec 2021 02:31:48 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sat, 04 Dec 2021 02:32:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 04 Dec 2021 02:32:07 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 04 Dec 2021 02:32:07 GMT
EXPOSE 8086
# Sat, 04 Dec 2021 02:32:07 GMT
VOLUME [/var/lib/influxdb]
# Sat, 04 Dec 2021 02:32:08 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 04 Dec 2021 02:32:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 04 Dec 2021 02:32:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Dec 2021 02:32:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:fdee104a33d14b2fdafeeaca15f0252d32280549d3cdc971244796c6e69ad0d3`  
		Last Modified: Thu, 02 Dec 2021 09:27:53 GMT  
		Size: 42.1 MB (42116754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44a93596b701db7b6e00e592b43547b3bbb7e984a3634dd91b34eb72c03ef1e`  
		Last Modified: Thu, 02 Dec 2021 12:08:46 GMT  
		Size: 10.0 MB (9956149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a002f84bb513d353d241296eda1ba0f01560a1ded46af2fe62c236c787a7559a`  
		Last Modified: Thu, 02 Dec 2021 12:08:43 GMT  
		Size: 3.9 MB (3921247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7512265925fd9b3295643dd954fe13e32b70794c509e55fe7f3c39a408ad3ec2`  
		Last Modified: Sat, 04 Dec 2021 02:32:41 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7be40161bd02715a1cafcfd975baa61c65f35eb3c55d2756ee7e04df387856`  
		Last Modified: Sat, 04 Dec 2021 02:33:50 GMT  
		Size: 51.6 MB (51616832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a2aa3343187e962c0528d9e414bd234d6d7200efcb8b6db3b50dab982845de`  
		Last Modified: Sat, 04 Dec 2021 02:33:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c704048419a0f6beb8ce2daa1174bea8c2d6a7e4e9ffbe310508c2d5d90a741`  
		Last Modified: Sat, 04 Dec 2021 02:33:23 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafd5465d5c4331510dd5b19ba77474a6a9ebfff1985423a71436850fbbc5507`  
		Last Modified: Sat, 04 Dec 2021 02:33:22 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:26f6484266779ab3a9a9a015ee82e2fb3348b986c3b76186d67cb33eb3f41749
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108502493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc9cc306d10cb2475ff5ab29c31753814a07feea28a006ad1a3e8fe99474c23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 08:10:09 GMT
ADD file:7be59c7e3b187d010c0e8625e45324f421a21518258e6bd35bab6e0e86c9494c in / 
# Thu, 02 Dec 2021 08:10:10 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:57:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:47:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:47:47 GMT
ENV INFLUXDB_VERSION=1.8.10
# Fri, 03 Dec 2021 04:47:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 03 Dec 2021 04:47:55 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:47:55 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:47:56 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:47:58 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:47:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:47:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:48:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6965f119641a6f16b55da01b7c12884960366228a181268b0bf7d0b7d50b2336`  
		Last Modified: Thu, 02 Dec 2021 08:44:30 GMT  
		Size: 43.2 MB (43173684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e211a2e7bbb27084e1f8cd62281719dc9d90e3ddb76b862e471b1cde61512cb`  
		Last Modified: Thu, 02 Dec 2021 10:08:36 GMT  
		Size: 10.2 MB (10216757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca410b1e11dc0ad76bc18c383eafa45a44c94916e27e4f327bc75a9373a250ca`  
		Last Modified: Thu, 02 Dec 2021 10:08:34 GMT  
		Size: 3.9 MB (3873863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b42056f3d6099ac63c397725439faee3120acd8c334e07f81423af0461472e`  
		Last Modified: Fri, 03 Dec 2021 04:50:04 GMT  
		Size: 2.8 KB (2828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d3998ef6831f4551cf36e5d1c4055cc65753365748f10331b423ebe2371ede`  
		Last Modified: Fri, 03 Dec 2021 04:50:29 GMT  
		Size: 51.2 MB (51233646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260f0db6084282000254725ef8b9b660eb0d980204d1a6e54d74fb4524cf8a25`  
		Last Modified: Fri, 03 Dec 2021 04:50:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16df3517c762360377f2b1439784f92ccc256ae21c0f1db21b6749799bb810e`  
		Last Modified: Fri, 03 Dec 2021 04:50:22 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa79dc942cedbe44370be245aa89a91d2c5bf383974924022b270f2ce76a0db`  
		Last Modified: Fri, 03 Dec 2021 04:50:22 GMT  
		Size: 1.3 KB (1280 bytes)  
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
$ docker pull influxdb@sha256:92f333040d0c2bb908acace09749f58fad16315bcd1feaab2cf02acc1abf6e0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:35963eb83419d50742a376de094a78f8a710a96622ba272f93fe3a2b802b383d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117738533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59f6e76ebb198651f581135910722ccc5f65d1d2bf7b31e2c2121681057d3cfc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:15:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Fri, 03 Dec 2021 04:15:09 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:15:09 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:15:10 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:15:10 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:15:10 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:15:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:15:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:15:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2090b310019ce97e7970604ff30ea6a152dbe8b0eaed9947c9d6db7408d139`  
		Last Modified: Fri, 03 Dec 2021 04:18:57 GMT  
		Size: 56.7 MB (56708560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19b008c9db370dc23bbbd8312dec6c3e409868dc2cb086d4528b5d17278b4fd`  
		Last Modified: Fri, 03 Dec 2021 04:18:50 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505eca482c8a4ca25c181824d56e9093680bb0bba4e87fbc5959260e46bdb88c`  
		Last Modified: Fri, 03 Dec 2021 04:18:49 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1310587db10fd45c1c9dbee91ad18ef7cd9f25d9dcad3161110c6dee1ae29f`  
		Last Modified: Fri, 03 Dec 2021 04:18:50 GMT  
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
$ docker pull influxdb@sha256:0ca5ceb1fdb6f66df576862dda11e64014d64654ff97b7548099f01308a5b782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:58b82d2d4f17694716bb7ca4c3cbb4e9eae0ab319a2b161afd3e8800b78b0d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84445105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ef285e9be66ff6fab01be62814bab2603b44639616578e1292f89c8dde35ac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:15:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Fri, 03 Dec 2021 04:15:19 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:15:20 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 03 Dec 2021 04:15:20 GMT
EXPOSE 8091
# Fri, 03 Dec 2021 04:15:20 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:15:21 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:15:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:15:21 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55629540dea7b7a486a85afaf3200eb077fdc749afb9b6d4f8d2e17d99367805`  
		Last Modified: Fri, 03 Dec 2021 04:19:15 GMT  
		Size: 23.4 MB (23416339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb75ec0d61146495eead82c8fc32161606e99fa030fbe345435c14aacc62633`  
		Last Modified: Fri, 03 Dec 2021 04:19:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a72762b74af5ed043fd0bc4f99b5ddf5bd63a028cf2b98e1c4376d39dea0349`  
		Last Modified: Fri, 03 Dec 2021 04:19:11 GMT  
		Size: 373.0 B  
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
$ docker pull influxdb@sha256:49192399ceb736debe0202c3a1c5f8277e3ad53546c221779f4b61399a0bbee1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:39cbab2f88a703d47b90645f64f585c4d9dea140309e045cd364dc9a341dbca4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115919392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a59ddecfe8fd96530b091dfccc9e23abdaf18b9389e258cb9753ea7059b13f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:14:50 GMT
ENV INFLUXDB_VERSION=1.8.10
# Fri, 03 Dec 2021 04:14:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 03 Dec 2021 04:14:56 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:14:56 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:14:56 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:14:56 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:14:57 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:14:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:14:57 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d272c6b4c091f2677bc94174cb715217c60c2346131cfd35607ecea81de080`  
		Last Modified: Fri, 03 Dec 2021 04:18:37 GMT  
		Size: 54.9 MB (54889479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199ff8c6aaebce00fd628792d5beb096ccb3c473641cc7ccf4bf4484535ec9a4`  
		Last Modified: Fri, 03 Dec 2021 04:18:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976ce52fa9d59ed0b81f6e6fb52151f2a99da8fa2789a9289f79ed80099f854`  
		Last Modified: Fri, 03 Dec 2021 04:18:29 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af89678e0336ac5e6e2c65046f6a7737c3131d934555ffe8365c0598ec61ee3d`  
		Last Modified: Fri, 03 Dec 2021 04:18:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:9b85c3a9381ff73dfda178f23a3ce55268f1742bd920e24ed876d63ca40a3fb9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107615555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37694b7723f827ed73be61288cd73c1728103682a5b938b62cc258928aa99be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 09:10:39 GMT
ADD file:1f947e5a3f8b1da292340501298edf2b879183aea9e90531f21c2b22500e79ad in / 
# Thu, 02 Dec 2021 09:10:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:49:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:49:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Dec 2021 02:31:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 04 Dec 2021 02:31:48 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sat, 04 Dec 2021 02:32:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 04 Dec 2021 02:32:07 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 04 Dec 2021 02:32:07 GMT
EXPOSE 8086
# Sat, 04 Dec 2021 02:32:07 GMT
VOLUME [/var/lib/influxdb]
# Sat, 04 Dec 2021 02:32:08 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 04 Dec 2021 02:32:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 04 Dec 2021 02:32:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Dec 2021 02:32:09 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:fdee104a33d14b2fdafeeaca15f0252d32280549d3cdc971244796c6e69ad0d3`  
		Last Modified: Thu, 02 Dec 2021 09:27:53 GMT  
		Size: 42.1 MB (42116754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44a93596b701db7b6e00e592b43547b3bbb7e984a3634dd91b34eb72c03ef1e`  
		Last Modified: Thu, 02 Dec 2021 12:08:46 GMT  
		Size: 10.0 MB (9956149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a002f84bb513d353d241296eda1ba0f01560a1ded46af2fe62c236c787a7559a`  
		Last Modified: Thu, 02 Dec 2021 12:08:43 GMT  
		Size: 3.9 MB (3921247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7512265925fd9b3295643dd954fe13e32b70794c509e55fe7f3c39a408ad3ec2`  
		Last Modified: Sat, 04 Dec 2021 02:32:41 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7be40161bd02715a1cafcfd975baa61c65f35eb3c55d2756ee7e04df387856`  
		Last Modified: Sat, 04 Dec 2021 02:33:50 GMT  
		Size: 51.6 MB (51616832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a2aa3343187e962c0528d9e414bd234d6d7200efcb8b6db3b50dab982845de`  
		Last Modified: Sat, 04 Dec 2021 02:33:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c704048419a0f6beb8ce2daa1174bea8c2d6a7e4e9ffbe310508c2d5d90a741`  
		Last Modified: Sat, 04 Dec 2021 02:33:23 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafd5465d5c4331510dd5b19ba77474a6a9ebfff1985423a71436850fbbc5507`  
		Last Modified: Sat, 04 Dec 2021 02:33:22 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:26f6484266779ab3a9a9a015ee82e2fb3348b986c3b76186d67cb33eb3f41749
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108502493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc9cc306d10cb2475ff5ab29c31753814a07feea28a006ad1a3e8fe99474c23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 08:10:09 GMT
ADD file:7be59c7e3b187d010c0e8625e45324f421a21518258e6bd35bab6e0e86c9494c in / 
# Thu, 02 Dec 2021 08:10:10 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:57:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:47:27 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:47:47 GMT
ENV INFLUXDB_VERSION=1.8.10
# Fri, 03 Dec 2021 04:47:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Fri, 03 Dec 2021 04:47:55 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:47:55 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:47:56 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:47:58 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:47:59 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:47:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:48:00 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6965f119641a6f16b55da01b7c12884960366228a181268b0bf7d0b7d50b2336`  
		Last Modified: Thu, 02 Dec 2021 08:44:30 GMT  
		Size: 43.2 MB (43173684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e211a2e7bbb27084e1f8cd62281719dc9d90e3ddb76b862e471b1cde61512cb`  
		Last Modified: Thu, 02 Dec 2021 10:08:36 GMT  
		Size: 10.2 MB (10216757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca410b1e11dc0ad76bc18c383eafa45a44c94916e27e4f327bc75a9373a250ca`  
		Last Modified: Thu, 02 Dec 2021 10:08:34 GMT  
		Size: 3.9 MB (3873863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b42056f3d6099ac63c397725439faee3120acd8c334e07f81423af0461472e`  
		Last Modified: Fri, 03 Dec 2021 04:50:04 GMT  
		Size: 2.8 KB (2828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d3998ef6831f4551cf36e5d1c4055cc65753365748f10331b423ebe2371ede`  
		Last Modified: Fri, 03 Dec 2021 04:50:29 GMT  
		Size: 51.2 MB (51233646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260f0db6084282000254725ef8b9b660eb0d980204d1a6e54d74fb4524cf8a25`  
		Last Modified: Fri, 03 Dec 2021 04:50:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16df3517c762360377f2b1439784f92ccc256ae21c0f1db21b6749799bb810e`  
		Last Modified: Fri, 03 Dec 2021 04:50:22 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa79dc942cedbe44370be245aa89a91d2c5bf383974924022b270f2ce76a0db`  
		Last Modified: Fri, 03 Dec 2021 04:50:22 GMT  
		Size: 1.3 KB (1280 bytes)  
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
$ docker pull influxdb@sha256:92f333040d0c2bb908acace09749f58fad16315bcd1feaab2cf02acc1abf6e0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:35963eb83419d50742a376de094a78f8a710a96622ba272f93fe3a2b802b383d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117738533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59f6e76ebb198651f581135910722ccc5f65d1d2bf7b31e2c2121681057d3cfc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:15:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Fri, 03 Dec 2021 04:15:09 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:15:09 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:15:10 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:15:10 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:15:10 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:15:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:15:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:15:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2090b310019ce97e7970604ff30ea6a152dbe8b0eaed9947c9d6db7408d139`  
		Last Modified: Fri, 03 Dec 2021 04:18:57 GMT  
		Size: 56.7 MB (56708560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19b008c9db370dc23bbbd8312dec6c3e409868dc2cb086d4528b5d17278b4fd`  
		Last Modified: Fri, 03 Dec 2021 04:18:50 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505eca482c8a4ca25c181824d56e9093680bb0bba4e87fbc5959260e46bdb88c`  
		Last Modified: Fri, 03 Dec 2021 04:18:49 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1310587db10fd45c1c9dbee91ad18ef7cd9f25d9dcad3161110c6dee1ae29f`  
		Last Modified: Fri, 03 Dec 2021 04:18:50 GMT  
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
$ docker pull influxdb@sha256:0ca5ceb1fdb6f66df576862dda11e64014d64654ff97b7548099f01308a5b782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:58b82d2d4f17694716bb7ca4c3cbb4e9eae0ab319a2b161afd3e8800b78b0d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84445105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ef285e9be66ff6fab01be62814bab2603b44639616578e1292f89c8dde35ac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:15:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Fri, 03 Dec 2021 04:15:19 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:15:20 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 03 Dec 2021 04:15:20 GMT
EXPOSE 8091
# Fri, 03 Dec 2021 04:15:20 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:15:21 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:15:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:15:21 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55629540dea7b7a486a85afaf3200eb077fdc749afb9b6d4f8d2e17d99367805`  
		Last Modified: Fri, 03 Dec 2021 04:19:15 GMT  
		Size: 23.4 MB (23416339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb75ec0d61146495eead82c8fc32161606e99fa030fbe345435c14aacc62633`  
		Last Modified: Fri, 03 Dec 2021 04:19:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a72762b74af5ed043fd0bc4f99b5ddf5bd63a028cf2b98e1c4376d39dea0349`  
		Last Modified: Fri, 03 Dec 2021 04:19:11 GMT  
		Size: 373.0 B  
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
$ docker pull influxdb@sha256:96716c30b8fcd81889261046156c7375173bcf7aaba473076fac2f1ee266263e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:823b71e5beec750bf48f1d2b978374a330f9da2c466ecdb5e56809ac0482c9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115569580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274dc8262418ca8a26c1114eb382e15921a995495e48558f0c5f51e4c79c8208`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:15:26 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Fri, 03 Dec 2021 04:15:34 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:15:34 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:15:34 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:15:35 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:15:35 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:15:35 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:15:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:15:36 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f173d1ca43d4f141edbcc8ed385bd1064cc09a7ad30a6b9feee59015b9ad10e4`  
		Last Modified: Fri, 03 Dec 2021 04:19:36 GMT  
		Size: 54.5 MB (54539607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b764ce66d083541d5df3da38911355f645e88ae8c83e67e520e946beca9f29`  
		Last Modified: Fri, 03 Dec 2021 04:19:29 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b154061280b15256231ba370c1f931cb164390a7734826cff279e73549eab6a`  
		Last Modified: Fri, 03 Dec 2021 04:19:29 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2556d20b43752ef17621c9c1311bfe30f0516e50e6c32647b8fd7263f08e52f2`  
		Last Modified: Fri, 03 Dec 2021 04:19:29 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:b061e01671e3376365a98ee9185f6bdd051b58f442554b5dd21e3afe45498b0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:8fa3a64f900dccd4658e4551a8f1bf2665fab005b769f4cc70a1809b276a6138
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86088955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cb9be51617f93227e93ffa889810e65bd09665efc119146348b300dbeb73644`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:15:26 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Fri, 03 Dec 2021 04:15:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:15:44 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 03 Dec 2021 04:15:44 GMT
EXPOSE 8091
# Fri, 03 Dec 2021 04:15:45 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:15:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:15:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:15:45 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2201d303bc22d2e2278cb1e24c524224971eb8609b18850f5797fd30664ca55f`  
		Last Modified: Fri, 03 Dec 2021 04:19:51 GMT  
		Size: 25.1 MB (25060188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e200a645e1d2f67a4a3a09448ce7ca85429eea326a7356723a961cccc7ba051b`  
		Last Modified: Fri, 03 Dec 2021 04:19:47 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffbd815f1b967b09b9d9eaf71abed7f583bf50a7de6f85f429d9fd622ac90f`  
		Last Modified: Fri, 03 Dec 2021 04:19:47 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:96716c30b8fcd81889261046156c7375173bcf7aaba473076fac2f1ee266263e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.5-data` - linux; amd64

```console
$ docker pull influxdb@sha256:823b71e5beec750bf48f1d2b978374a330f9da2c466ecdb5e56809ac0482c9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115569580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274dc8262418ca8a26c1114eb382e15921a995495e48558f0c5f51e4c79c8208`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:15:26 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Fri, 03 Dec 2021 04:15:34 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:15:34 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:15:34 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:15:35 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:15:35 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:15:35 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:15:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:15:36 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f173d1ca43d4f141edbcc8ed385bd1064cc09a7ad30a6b9feee59015b9ad10e4`  
		Last Modified: Fri, 03 Dec 2021 04:19:36 GMT  
		Size: 54.5 MB (54539607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b764ce66d083541d5df3da38911355f645e88ae8c83e67e520e946beca9f29`  
		Last Modified: Fri, 03 Dec 2021 04:19:29 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b154061280b15256231ba370c1f931cb164390a7734826cff279e73549eab6a`  
		Last Modified: Fri, 03 Dec 2021 04:19:29 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2556d20b43752ef17621c9c1311bfe30f0516e50e6c32647b8fd7263f08e52f2`  
		Last Modified: Fri, 03 Dec 2021 04:19:29 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:b061e01671e3376365a98ee9185f6bdd051b58f442554b5dd21e3afe45498b0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.5-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:8fa3a64f900dccd4658e4551a8f1bf2665fab005b769f4cc70a1809b276a6138
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86088955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cb9be51617f93227e93ffa889810e65bd09665efc119146348b300dbeb73644`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:15:26 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Fri, 03 Dec 2021 04:15:44 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:15:44 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 03 Dec 2021 04:15:44 GMT
EXPOSE 8091
# Fri, 03 Dec 2021 04:15:45 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:15:45 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:15:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:15:45 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2201d303bc22d2e2278cb1e24c524224971eb8609b18850f5797fd30664ca55f`  
		Last Modified: Fri, 03 Dec 2021 04:19:51 GMT  
		Size: 25.1 MB (25060188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e200a645e1d2f67a4a3a09448ce7ca85429eea326a7356723a961cccc7ba051b`  
		Last Modified: Fri, 03 Dec 2021 04:19:47 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffbd815f1b967b09b9d9eaf71abed7f583bf50a7de6f85f429d9fd622ac90f`  
		Last Modified: Fri, 03 Dec 2021 04:19:47 GMT  
		Size: 374.0 B  
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
$ docker pull influxdb@sha256:a530fc9aca9f4014c996429542b1dfcf74265239b02d66dfaf46092c3e2595ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:8abda459be419aaf0bf2c840ed5c2d85def5eecc29c23506ed2f03429ef75819
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172326431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ced164801874021cdf337d095e5dd35a7cab44c74e5ee1a31bd99c123ab9216`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:31 GMT
ADD file:f077e1a42fb919be2af67820782ceee3b46ffd13d7ab6949bea9921217d12813 in / 
# Thu, 02 Dec 2021 02:48:32 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:41:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:15:51 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 03 Dec 2021 04:15:51 GMT
ENV GOSU_VER=1.12
# Fri, 03 Dec 2021 04:15:55 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Fri, 03 Dec 2021 04:15:55 GMT
ENV INFLUXDB_VERSION=2.0.9
# Fri, 03 Dec 2021 04:16:04 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Fri, 03 Dec 2021 04:16:05 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 03 Dec 2021 04:16:05 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 03 Dec 2021 04:16:05 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 03 Dec 2021 04:16:05 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 03 Dec 2021 04:16:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:16:06 GMT
CMD ["influxd"]
# Fri, 03 Dec 2021 04:16:06 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:16:06 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 03 Dec 2021 04:16:07 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 03 Dec 2021 04:16:07 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 03 Dec 2021 04:16:07 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c4cc477c22ba7abce860198107408434dd7bd73ddbaf82f1e69ab941b9979405`  
		Last Modified: Thu, 02 Dec 2021 02:54:07 GMT  
		Size: 50.4 MB (50437113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077c54d048f1f1a1f28079caa54bf5d99803f937ffe5c1dc6e207698f70b4e74`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 7.8 MB (7833819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368544993b2deeeffdd19463cdf92ec4e39f83073de5de316f9f5c725ab403f`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 10.0 MB (9997240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046398de937b476bbd1dddbad558ac4c1920fab14866beef48912f8f2c298fa`  
		Last Modified: Fri, 03 Dec 2021 04:20:04 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df21b3d2252fff8be63abc8448901e25fc4884a5c908547c467ff4c1a69cb27`  
		Last Modified: Fri, 03 Dec 2021 04:20:02 GMT  
		Size: 961.0 KB (960957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8584c80132296e93e8eebc5ed623f751a203fbd0cb5d6fb9f655668b9630dd82`  
		Last Modified: Fri, 03 Dec 2021 04:20:11 GMT  
		Size: 103.1 MB (103090635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6da6d75a0ffe8b4f411eee868741bc1baa44abef4453262de5dea883d99d5d`  
		Last Modified: Fri, 03 Dec 2021 04:20:02 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb021560f7858f0127208912abae2557d2ffd3ff66dbd3f422516b05fdd81e8`  
		Last Modified: Fri, 03 Dec 2021 04:20:02 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3711bbacc13167eb4e6cd843c5ddd3dac8621d4937f6be2134d82bfc367e05`  
		Last Modified: Fri, 03 Dec 2021 04:20:02 GMT  
		Size: 4.3 KB (4325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f3e715294a3556340113519ae7d9f6b3268e3053dac8e632bbc3e2a9a3bb2b78
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174115186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0970b0bf56e24eeb05394df282616e340c1ae685a45a55175e1921c4aae0bd7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:20 GMT
ADD file:82c1819d8416d9d44564980e25e98a081f813bc2ee8ad2789114fe37e802848f in / 
# Thu, 02 Dec 2021 08:08:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:54:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:54:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:48:07 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 03 Dec 2021 04:48:08 GMT
ENV GOSU_VER=1.12
# Fri, 03 Dec 2021 04:48:17 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Fri, 03 Dec 2021 04:48:18 GMT
ENV INFLUXDB_VERSION=2.0.9
# Fri, 03 Dec 2021 04:48:30 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Fri, 03 Dec 2021 04:48:31 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 03 Dec 2021 04:48:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 03 Dec 2021 04:48:34 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 03 Dec 2021 04:48:35 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 03 Dec 2021 04:48:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:48:36 GMT
CMD ["influxd"]
# Fri, 03 Dec 2021 04:48:37 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:48:38 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 03 Dec 2021 04:48:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 03 Dec 2021 04:48:40 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 03 Dec 2021 04:48:41 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:39e4f823356a9e2dbba530f9d363b4d76beaff75a13bad788d38eebeae67e5b0`  
		Last Modified: Thu, 02 Dec 2021 08:41:08 GMT  
		Size: 49.2 MB (49223045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df66cf961d4016eccee4ce9bc5dc18dcd99e9f9963e66c4980a66e6492a421b2`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 7.7 MB (7695103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6c547e43b8b6afdfae413ba7a49c1120d0534fff63c4a242ef611d562a678c`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 9.8 MB (9767269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e453752afc1d0eeb18c400aa791f08f937a00ecdc6f38ebb18c2ee87a7ff5`  
		Last Modified: Fri, 03 Dec 2021 04:50:42 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4c33d24855b024e47dd55bf44ac4a8c685187c216da8db529dedc00602635`  
		Last Modified: Fri, 03 Dec 2021 04:50:40 GMT  
		Size: 896.4 KB (896361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a97405ad8522bdfb410cdbc6aac4c63560ba5ff199d147ab0fbce7a5e5e0da`  
		Last Modified: Fri, 03 Dec 2021 04:50:51 GMT  
		Size: 106.5 MB (106526971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9cf8cf19f09471b111e886dba122c8aa5a834f576dd3476106218569b92a1d`  
		Last Modified: Fri, 03 Dec 2021 04:50:40 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90288bc36b42645990ffa676ea1197a0fc8cd9d7922ea53108dca428b01f34c4`  
		Last Modified: Fri, 03 Dec 2021 04:50:40 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e3939b85fa46569ac3b6692407bb573cbd8afe317248821812e420a048e997`  
		Last Modified: Fri, 03 Dec 2021 04:50:40 GMT  
		Size: 4.3 KB (4325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0-alpine`

```console
$ docker pull influxdb@sha256:7045b772cd2a55ac402ddf1cc305bbbe0dc03d490390c14a8c5a32ec265716c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:0afdcd1798c8d6c602e89d68d2b6afcd26a366708d9b92cf02c9ec3d26e57b72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116735117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b42d591d50214a5345765f20ce86f57a4da86cde715cc16c2a0b7442dda75153`
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
# Fri, 19 Nov 2021 02:24:56 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 19 Nov 2021 02:24:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Nov 2021 02:24:56 GMT
CMD ["influxd"]
# Fri, 19 Nov 2021 02:24:57 GMT
EXPOSE 8086
# Fri, 19 Nov 2021 02:24:57 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 19 Nov 2021 02:24:57 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 19 Nov 2021 02:24:57 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 19 Nov 2021 02:24:58 GMT
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
	-	`sha256:c58e1d87b1e7395b9be1b16144e7b0a8a3298cbe01dc68dc6585a740ce076e7c`  
		Last Modified: Fri, 19 Nov 2021 02:26:19 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:06651d786bee0783fb295c430741a8e0ac33bae118fbdb24e93956e2f211135b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119835593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1586d2e5721c0dd6388674da773472c2fd99f4e84451a91e2ec8d5b8c0b510`
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
# Fri, 19 Nov 2021 01:46:14 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 19 Nov 2021 01:46:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Nov 2021 01:46:15 GMT
CMD ["influxd"]
# Fri, 19 Nov 2021 01:46:16 GMT
EXPOSE 8086
# Fri, 19 Nov 2021 01:46:17 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 19 Nov 2021 01:46:18 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 19 Nov 2021 01:46:19 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 19 Nov 2021 01:46:20 GMT
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
	-	`sha256:b6232be12aef54a87682eb985aa8448ca4e577351d82ee2f0e637087ab47f229`  
		Last Modified: Fri, 19 Nov 2021 01:47:38 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.9`

```console
$ docker pull influxdb@sha256:a530fc9aca9f4014c996429542b1dfcf74265239b02d66dfaf46092c3e2595ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9` - linux; amd64

```console
$ docker pull influxdb@sha256:8abda459be419aaf0bf2c840ed5c2d85def5eecc29c23506ed2f03429ef75819
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172326431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ced164801874021cdf337d095e5dd35a7cab44c74e5ee1a31bd99c123ab9216`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:31 GMT
ADD file:f077e1a42fb919be2af67820782ceee3b46ffd13d7ab6949bea9921217d12813 in / 
# Thu, 02 Dec 2021 02:48:32 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:41:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:15:51 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 03 Dec 2021 04:15:51 GMT
ENV GOSU_VER=1.12
# Fri, 03 Dec 2021 04:15:55 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Fri, 03 Dec 2021 04:15:55 GMT
ENV INFLUXDB_VERSION=2.0.9
# Fri, 03 Dec 2021 04:16:04 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Fri, 03 Dec 2021 04:16:05 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 03 Dec 2021 04:16:05 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 03 Dec 2021 04:16:05 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 03 Dec 2021 04:16:05 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 03 Dec 2021 04:16:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:16:06 GMT
CMD ["influxd"]
# Fri, 03 Dec 2021 04:16:06 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:16:06 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 03 Dec 2021 04:16:07 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 03 Dec 2021 04:16:07 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 03 Dec 2021 04:16:07 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c4cc477c22ba7abce860198107408434dd7bd73ddbaf82f1e69ab941b9979405`  
		Last Modified: Thu, 02 Dec 2021 02:54:07 GMT  
		Size: 50.4 MB (50437113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077c54d048f1f1a1f28079caa54bf5d99803f937ffe5c1dc6e207698f70b4e74`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 7.8 MB (7833819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368544993b2deeeffdd19463cdf92ec4e39f83073de5de316f9f5c725ab403f`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 10.0 MB (9997240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046398de937b476bbd1dddbad558ac4c1920fab14866beef48912f8f2c298fa`  
		Last Modified: Fri, 03 Dec 2021 04:20:04 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df21b3d2252fff8be63abc8448901e25fc4884a5c908547c467ff4c1a69cb27`  
		Last Modified: Fri, 03 Dec 2021 04:20:02 GMT  
		Size: 961.0 KB (960957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8584c80132296e93e8eebc5ed623f751a203fbd0cb5d6fb9f655668b9630dd82`  
		Last Modified: Fri, 03 Dec 2021 04:20:11 GMT  
		Size: 103.1 MB (103090635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6da6d75a0ffe8b4f411eee868741bc1baa44abef4453262de5dea883d99d5d`  
		Last Modified: Fri, 03 Dec 2021 04:20:02 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb021560f7858f0127208912abae2557d2ffd3ff66dbd3f422516b05fdd81e8`  
		Last Modified: Fri, 03 Dec 2021 04:20:02 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3711bbacc13167eb4e6cd843c5ddd3dac8621d4937f6be2134d82bfc367e05`  
		Last Modified: Fri, 03 Dec 2021 04:20:02 GMT  
		Size: 4.3 KB (4325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f3e715294a3556340113519ae7d9f6b3268e3053dac8e632bbc3e2a9a3bb2b78
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174115186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0970b0bf56e24eeb05394df282616e340c1ae685a45a55175e1921c4aae0bd7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:20 GMT
ADD file:82c1819d8416d9d44564980e25e98a081f813bc2ee8ad2789114fe37e802848f in / 
# Thu, 02 Dec 2021 08:08:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:54:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:54:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:48:07 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 03 Dec 2021 04:48:08 GMT
ENV GOSU_VER=1.12
# Fri, 03 Dec 2021 04:48:17 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Fri, 03 Dec 2021 04:48:18 GMT
ENV INFLUXDB_VERSION=2.0.9
# Fri, 03 Dec 2021 04:48:30 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Fri, 03 Dec 2021 04:48:31 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 03 Dec 2021 04:48:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 03 Dec 2021 04:48:34 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 03 Dec 2021 04:48:35 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 03 Dec 2021 04:48:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:48:36 GMT
CMD ["influxd"]
# Fri, 03 Dec 2021 04:48:37 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:48:38 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 03 Dec 2021 04:48:39 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 03 Dec 2021 04:48:40 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 03 Dec 2021 04:48:41 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:39e4f823356a9e2dbba530f9d363b4d76beaff75a13bad788d38eebeae67e5b0`  
		Last Modified: Thu, 02 Dec 2021 08:41:08 GMT  
		Size: 49.2 MB (49223045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df66cf961d4016eccee4ce9bc5dc18dcd99e9f9963e66c4980a66e6492a421b2`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 7.7 MB (7695103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6c547e43b8b6afdfae413ba7a49c1120d0534fff63c4a242ef611d562a678c`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 9.8 MB (9767269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e453752afc1d0eeb18c400aa791f08f937a00ecdc6f38ebb18c2ee87a7ff5`  
		Last Modified: Fri, 03 Dec 2021 04:50:42 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4c33d24855b024e47dd55bf44ac4a8c685187c216da8db529dedc00602635`  
		Last Modified: Fri, 03 Dec 2021 04:50:40 GMT  
		Size: 896.4 KB (896361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a97405ad8522bdfb410cdbc6aac4c63560ba5ff199d147ab0fbce7a5e5e0da`  
		Last Modified: Fri, 03 Dec 2021 04:50:51 GMT  
		Size: 106.5 MB (106526971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9cf8cf19f09471b111e886dba122c8aa5a834f576dd3476106218569b92a1d`  
		Last Modified: Fri, 03 Dec 2021 04:50:40 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90288bc36b42645990ffa676ea1197a0fc8cd9d7922ea53108dca428b01f34c4`  
		Last Modified: Fri, 03 Dec 2021 04:50:40 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e3939b85fa46569ac3b6692407bb573cbd8afe317248821812e420a048e997`  
		Last Modified: Fri, 03 Dec 2021 04:50:40 GMT  
		Size: 4.3 KB (4325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.9-alpine`

```console
$ docker pull influxdb@sha256:7045b772cd2a55ac402ddf1cc305bbbe0dc03d490390c14a8c5a32ec265716c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:0afdcd1798c8d6c602e89d68d2b6afcd26a366708d9b92cf02c9ec3d26e57b72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116735117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b42d591d50214a5345765f20ce86f57a4da86cde715cc16c2a0b7442dda75153`
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
# Fri, 19 Nov 2021 02:24:56 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 19 Nov 2021 02:24:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Nov 2021 02:24:56 GMT
CMD ["influxd"]
# Fri, 19 Nov 2021 02:24:57 GMT
EXPOSE 8086
# Fri, 19 Nov 2021 02:24:57 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 19 Nov 2021 02:24:57 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 19 Nov 2021 02:24:57 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 19 Nov 2021 02:24:58 GMT
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
	-	`sha256:c58e1d87b1e7395b9be1b16144e7b0a8a3298cbe01dc68dc6585a740ce076e7c`  
		Last Modified: Fri, 19 Nov 2021 02:26:19 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:06651d786bee0783fb295c430741a8e0ac33bae118fbdb24e93956e2f211135b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119835593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1586d2e5721c0dd6388674da773472c2fd99f4e84451a91e2ec8d5b8c0b510`
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
# Fri, 19 Nov 2021 01:46:14 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 19 Nov 2021 01:46:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Nov 2021 01:46:15 GMT
CMD ["influxd"]
# Fri, 19 Nov 2021 01:46:16 GMT
EXPOSE 8086
# Fri, 19 Nov 2021 01:46:17 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 19 Nov 2021 01:46:18 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 19 Nov 2021 01:46:19 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 19 Nov 2021 01:46:20 GMT
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
	-	`sha256:b6232be12aef54a87682eb985aa8448ca4e577351d82ee2f0e637087ab47f229`  
		Last Modified: Fri, 19 Nov 2021 01:47:38 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1`

```console
$ docker pull influxdb@sha256:6597ad58ab996d75e4f000e6295d2a2db8543644e329f009d0e3b7ceaaed3940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1` - linux; amd64

```console
$ docker pull influxdb@sha256:243f645d0e68cfd1d8a8a25cb505ba4614313fb3e04f3598fcbbd2ffe1ba0afc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182885073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a3e66c579fd83698cd7792b7a31f40b776f2be07bee7a73642502787e71cf2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:31 GMT
ADD file:f077e1a42fb919be2af67820782ceee3b46ffd13d7ab6949bea9921217d12813 in / 
# Thu, 02 Dec 2021 02:48:32 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:41:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:15:51 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 03 Dec 2021 04:15:51 GMT
ENV GOSU_VER=1.12
# Fri, 03 Dec 2021 04:15:55 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Fri, 03 Dec 2021 04:16:12 GMT
ENV INFLUXDB_VERSION=2.1.1
# Fri, 03 Dec 2021 04:16:25 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 03 Dec 2021 04:16:26 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Fri, 03 Dec 2021 04:16:31 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 03 Dec 2021 04:16:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 03 Dec 2021 04:16:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 03 Dec 2021 04:16:32 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 03 Dec 2021 04:16:33 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 03 Dec 2021 04:16:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:16:33 GMT
CMD ["influxd"]
# Fri, 03 Dec 2021 04:16:33 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:16:34 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 03 Dec 2021 04:16:34 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 03 Dec 2021 04:16:34 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 03 Dec 2021 04:16:34 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c4cc477c22ba7abce860198107408434dd7bd73ddbaf82f1e69ab941b9979405`  
		Last Modified: Thu, 02 Dec 2021 02:54:07 GMT  
		Size: 50.4 MB (50437113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077c54d048f1f1a1f28079caa54bf5d99803f937ffe5c1dc6e207698f70b4e74`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 7.8 MB (7833819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368544993b2deeeffdd19463cdf92ec4e39f83073de5de316f9f5c725ab403f`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 10.0 MB (9997240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046398de937b476bbd1dddbad558ac4c1920fab14866beef48912f8f2c298fa`  
		Last Modified: Fri, 03 Dec 2021 04:20:04 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df21b3d2252fff8be63abc8448901e25fc4884a5c908547c467ff4c1a69cb27`  
		Last Modified: Fri, 03 Dec 2021 04:20:02 GMT  
		Size: 961.0 KB (960957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23da490b8439fd90fb925e88dd05bb3f2baf355d643c9424b947f3c001f360f7`  
		Last Modified: Fri, 03 Dec 2021 04:20:31 GMT  
		Size: 108.3 MB (108324790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaafd74aa812957182e136339b85966d8f81b182941aba8676477f32ed4273c`  
		Last Modified: Fri, 03 Dec 2021 04:20:23 GMT  
		Size: 5.3 MB (5324489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adffecb8fd59efb0b2c62183c51351e3536471b84b7798b9cd214a22dcc55e66`  
		Last Modified: Fri, 03 Dec 2021 04:20:22 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41282bd9b235c778fb450ceb70a6588650efd451de12e9c2b42f2ea386995a7f`  
		Last Modified: Fri, 03 Dec 2021 04:20:22 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258ee0d08be6341996276bcba4089330840b5708a250224f4bec902ca39ae715`  
		Last Modified: Fri, 03 Dec 2021 04:20:22 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:92cb696238c0355c4c41436df43971d7f14e6952f528b0253cf2bab6beb801e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183386540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b807674ff0082f1f84c1a783b57406d1b8176ef84097d6beb956b916b5516d3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:20 GMT
ADD file:82c1819d8416d9d44564980e25e98a081f813bc2ee8ad2789114fe37e802848f in / 
# Thu, 02 Dec 2021 08:08:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:54:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:54:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:48:07 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 03 Dec 2021 04:48:08 GMT
ENV GOSU_VER=1.12
# Fri, 03 Dec 2021 04:48:17 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Fri, 03 Dec 2021 04:48:54 GMT
ENV INFLUXDB_VERSION=2.1.1
# Fri, 03 Dec 2021 04:49:09 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 03 Dec 2021 04:49:09 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Fri, 03 Dec 2021 04:49:14 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 03 Dec 2021 04:49:15 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 03 Dec 2021 04:49:15 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 03 Dec 2021 04:49:17 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 03 Dec 2021 04:49:18 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 03 Dec 2021 04:49:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:49:19 GMT
CMD ["influxd"]
# Fri, 03 Dec 2021 04:49:20 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:49:21 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 03 Dec 2021 04:49:22 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 03 Dec 2021 04:49:23 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 03 Dec 2021 04:49:24 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:39e4f823356a9e2dbba530f9d363b4d76beaff75a13bad788d38eebeae67e5b0`  
		Last Modified: Thu, 02 Dec 2021 08:41:08 GMT  
		Size: 49.2 MB (49223045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df66cf961d4016eccee4ce9bc5dc18dcd99e9f9963e66c4980a66e6492a421b2`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 7.7 MB (7695103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6c547e43b8b6afdfae413ba7a49c1120d0534fff63c4a242ef611d562a678c`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 9.8 MB (9767269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e453752afc1d0eeb18c400aa791f08f937a00ecdc6f38ebb18c2ee87a7ff5`  
		Last Modified: Fri, 03 Dec 2021 04:50:42 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4c33d24855b024e47dd55bf44ac4a8c685187c216da8db529dedc00602635`  
		Last Modified: Fri, 03 Dec 2021 04:50:40 GMT  
		Size: 896.4 KB (896361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8240edd1b1dfc75cb17498aaf77dc354d90f88872cd96f215d8a4d9487cd295f`  
		Last Modified: Fri, 03 Dec 2021 04:51:13 GMT  
		Size: 110.9 MB (110891610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d470fb0461896b3f8fc90d6e52aca4127540a50fe95665bd141a83b39e5c60e`  
		Last Modified: Fri, 03 Dec 2021 04:51:05 GMT  
		Size: 4.9 MB (4906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374b9f0297356c62d3be4a7c1a544a3f582bcffa3af49827c0ff51c0587188e`  
		Last Modified: Fri, 03 Dec 2021 04:51:04 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19627f99f85fbd769ed49c25523ea84a2dc4f82fbae5ed9d7eda8e233fec1dbc`  
		Last Modified: Fri, 03 Dec 2021 04:51:04 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792639683dfd3da7c9d7a1023bbd014f647e05e766c95d11430615194c905baa`  
		Last Modified: Fri, 03 Dec 2021 04:51:04 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1-alpine`

```console
$ docker pull influxdb@sha256:9ac49ef6120a7e643fe8d7ddb090eaf445b53cf3649a5ea842f5e2ba993641ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4846606e013a1fe8c99b5f891d56614dff89c5a5938cb8caf28faee4fc51fca1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127293789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fd4a87c67597c53f0a6dc4e77ffbb76dd2eb0f2f4ca7f0e93af9f1de04e21b6`
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
# Fri, 19 Nov 2021 02:25:04 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 19 Nov 2021 02:25:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Nov 2021 02:25:04 GMT
CMD ["influxd"]
# Fri, 19 Nov 2021 02:25:04 GMT
EXPOSE 8086
# Fri, 19 Nov 2021 02:25:05 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 19 Nov 2021 02:25:05 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 19 Nov 2021 02:25:05 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 19 Nov 2021 02:25:05 GMT
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
	-	`sha256:4b7574e9841a57f1749d68981ae64ff09b650a517c567d131e58218922327cd4`  
		Last Modified: Fri, 19 Nov 2021 02:26:43 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:90b06abdc30a1b74750e7c82c7c28265d3bc9ac9313c43cd59f75356b4a61e14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129106952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ace363ef6a1bcfe8772653cd7f68a3ded9e312988ded50f14c7677e948a5d8`
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
# Fri, 19 Nov 2021 01:46:39 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 19 Nov 2021 01:46:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Nov 2021 01:46:40 GMT
CMD ["influxd"]
# Fri, 19 Nov 2021 01:46:41 GMT
EXPOSE 8086
# Fri, 19 Nov 2021 01:46:42 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 19 Nov 2021 01:46:43 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 19 Nov 2021 01:46:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 19 Nov 2021 01:46:45 GMT
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
	-	`sha256:ef8780aa6d16fe2373309446670a390cd9fef4ff82c80d224b0b32b14576b759`  
		Last Modified: Fri, 19 Nov 2021 01:48:02 GMT  
		Size: 4.3 KB (4320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1.1`

```console
$ docker pull influxdb@sha256:6597ad58ab996d75e4f000e6295d2a2db8543644e329f009d0e3b7ceaaed3940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1` - linux; amd64

```console
$ docker pull influxdb@sha256:243f645d0e68cfd1d8a8a25cb505ba4614313fb3e04f3598fcbbd2ffe1ba0afc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182885073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a3e66c579fd83698cd7792b7a31f40b776f2be07bee7a73642502787e71cf2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:31 GMT
ADD file:f077e1a42fb919be2af67820782ceee3b46ffd13d7ab6949bea9921217d12813 in / 
# Thu, 02 Dec 2021 02:48:32 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:41:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:15:51 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 03 Dec 2021 04:15:51 GMT
ENV GOSU_VER=1.12
# Fri, 03 Dec 2021 04:15:55 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Fri, 03 Dec 2021 04:16:12 GMT
ENV INFLUXDB_VERSION=2.1.1
# Fri, 03 Dec 2021 04:16:25 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 03 Dec 2021 04:16:26 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Fri, 03 Dec 2021 04:16:31 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 03 Dec 2021 04:16:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 03 Dec 2021 04:16:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 03 Dec 2021 04:16:32 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 03 Dec 2021 04:16:33 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 03 Dec 2021 04:16:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:16:33 GMT
CMD ["influxd"]
# Fri, 03 Dec 2021 04:16:33 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:16:34 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 03 Dec 2021 04:16:34 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 03 Dec 2021 04:16:34 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 03 Dec 2021 04:16:34 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c4cc477c22ba7abce860198107408434dd7bd73ddbaf82f1e69ab941b9979405`  
		Last Modified: Thu, 02 Dec 2021 02:54:07 GMT  
		Size: 50.4 MB (50437113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077c54d048f1f1a1f28079caa54bf5d99803f937ffe5c1dc6e207698f70b4e74`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 7.8 MB (7833819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368544993b2deeeffdd19463cdf92ec4e39f83073de5de316f9f5c725ab403f`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 10.0 MB (9997240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046398de937b476bbd1dddbad558ac4c1920fab14866beef48912f8f2c298fa`  
		Last Modified: Fri, 03 Dec 2021 04:20:04 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df21b3d2252fff8be63abc8448901e25fc4884a5c908547c467ff4c1a69cb27`  
		Last Modified: Fri, 03 Dec 2021 04:20:02 GMT  
		Size: 961.0 KB (960957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23da490b8439fd90fb925e88dd05bb3f2baf355d643c9424b947f3c001f360f7`  
		Last Modified: Fri, 03 Dec 2021 04:20:31 GMT  
		Size: 108.3 MB (108324790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaafd74aa812957182e136339b85966d8f81b182941aba8676477f32ed4273c`  
		Last Modified: Fri, 03 Dec 2021 04:20:23 GMT  
		Size: 5.3 MB (5324489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adffecb8fd59efb0b2c62183c51351e3536471b84b7798b9cd214a22dcc55e66`  
		Last Modified: Fri, 03 Dec 2021 04:20:22 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41282bd9b235c778fb450ceb70a6588650efd451de12e9c2b42f2ea386995a7f`  
		Last Modified: Fri, 03 Dec 2021 04:20:22 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258ee0d08be6341996276bcba4089330840b5708a250224f4bec902ca39ae715`  
		Last Modified: Fri, 03 Dec 2021 04:20:22 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:92cb696238c0355c4c41436df43971d7f14e6952f528b0253cf2bab6beb801e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183386540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b807674ff0082f1f84c1a783b57406d1b8176ef84097d6beb956b916b5516d3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:20 GMT
ADD file:82c1819d8416d9d44564980e25e98a081f813bc2ee8ad2789114fe37e802848f in / 
# Thu, 02 Dec 2021 08:08:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:54:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:54:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:48:07 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 03 Dec 2021 04:48:08 GMT
ENV GOSU_VER=1.12
# Fri, 03 Dec 2021 04:48:17 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Fri, 03 Dec 2021 04:48:54 GMT
ENV INFLUXDB_VERSION=2.1.1
# Fri, 03 Dec 2021 04:49:09 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 03 Dec 2021 04:49:09 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Fri, 03 Dec 2021 04:49:14 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 03 Dec 2021 04:49:15 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 03 Dec 2021 04:49:15 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 03 Dec 2021 04:49:17 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 03 Dec 2021 04:49:18 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 03 Dec 2021 04:49:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:49:19 GMT
CMD ["influxd"]
# Fri, 03 Dec 2021 04:49:20 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:49:21 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 03 Dec 2021 04:49:22 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 03 Dec 2021 04:49:23 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 03 Dec 2021 04:49:24 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:39e4f823356a9e2dbba530f9d363b4d76beaff75a13bad788d38eebeae67e5b0`  
		Last Modified: Thu, 02 Dec 2021 08:41:08 GMT  
		Size: 49.2 MB (49223045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df66cf961d4016eccee4ce9bc5dc18dcd99e9f9963e66c4980a66e6492a421b2`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 7.7 MB (7695103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6c547e43b8b6afdfae413ba7a49c1120d0534fff63c4a242ef611d562a678c`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 9.8 MB (9767269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e453752afc1d0eeb18c400aa791f08f937a00ecdc6f38ebb18c2ee87a7ff5`  
		Last Modified: Fri, 03 Dec 2021 04:50:42 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4c33d24855b024e47dd55bf44ac4a8c685187c216da8db529dedc00602635`  
		Last Modified: Fri, 03 Dec 2021 04:50:40 GMT  
		Size: 896.4 KB (896361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8240edd1b1dfc75cb17498aaf77dc354d90f88872cd96f215d8a4d9487cd295f`  
		Last Modified: Fri, 03 Dec 2021 04:51:13 GMT  
		Size: 110.9 MB (110891610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d470fb0461896b3f8fc90d6e52aca4127540a50fe95665bd141a83b39e5c60e`  
		Last Modified: Fri, 03 Dec 2021 04:51:05 GMT  
		Size: 4.9 MB (4906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374b9f0297356c62d3be4a7c1a544a3f582bcffa3af49827c0ff51c0587188e`  
		Last Modified: Fri, 03 Dec 2021 04:51:04 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19627f99f85fbd769ed49c25523ea84a2dc4f82fbae5ed9d7eda8e233fec1dbc`  
		Last Modified: Fri, 03 Dec 2021 04:51:04 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792639683dfd3da7c9d7a1023bbd014f647e05e766c95d11430615194c905baa`  
		Last Modified: Fri, 03 Dec 2021 04:51:04 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1.1-alpine`

```console
$ docker pull influxdb@sha256:9ac49ef6120a7e643fe8d7ddb090eaf445b53cf3649a5ea842f5e2ba993641ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4846606e013a1fe8c99b5f891d56614dff89c5a5938cb8caf28faee4fc51fca1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127293789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fd4a87c67597c53f0a6dc4e77ffbb76dd2eb0f2f4ca7f0e93af9f1de04e21b6`
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
# Fri, 19 Nov 2021 02:25:04 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 19 Nov 2021 02:25:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Nov 2021 02:25:04 GMT
CMD ["influxd"]
# Fri, 19 Nov 2021 02:25:04 GMT
EXPOSE 8086
# Fri, 19 Nov 2021 02:25:05 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 19 Nov 2021 02:25:05 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 19 Nov 2021 02:25:05 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 19 Nov 2021 02:25:05 GMT
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
	-	`sha256:4b7574e9841a57f1749d68981ae64ff09b650a517c567d131e58218922327cd4`  
		Last Modified: Fri, 19 Nov 2021 02:26:43 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:90b06abdc30a1b74750e7c82c7c28265d3bc9ac9313c43cd59f75356b4a61e14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129106952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ace363ef6a1bcfe8772653cd7f68a3ded9e312988ded50f14c7677e948a5d8`
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
# Fri, 19 Nov 2021 01:46:39 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 19 Nov 2021 01:46:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Nov 2021 01:46:40 GMT
CMD ["influxd"]
# Fri, 19 Nov 2021 01:46:41 GMT
EXPOSE 8086
# Fri, 19 Nov 2021 01:46:42 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 19 Nov 2021 01:46:43 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 19 Nov 2021 01:46:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 19 Nov 2021 01:46:45 GMT
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
	-	`sha256:ef8780aa6d16fe2373309446670a390cd9fef4ff82c80d224b0b32b14576b759`  
		Last Modified: Fri, 19 Nov 2021 01:48:02 GMT  
		Size: 4.3 KB (4320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:9ac49ef6120a7e643fe8d7ddb090eaf445b53cf3649a5ea842f5e2ba993641ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4846606e013a1fe8c99b5f891d56614dff89c5a5938cb8caf28faee4fc51fca1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127293789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fd4a87c67597c53f0a6dc4e77ffbb76dd2eb0f2f4ca7f0e93af9f1de04e21b6`
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
# Fri, 19 Nov 2021 02:25:04 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 19 Nov 2021 02:25:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Nov 2021 02:25:04 GMT
CMD ["influxd"]
# Fri, 19 Nov 2021 02:25:04 GMT
EXPOSE 8086
# Fri, 19 Nov 2021 02:25:05 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 19 Nov 2021 02:25:05 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 19 Nov 2021 02:25:05 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 19 Nov 2021 02:25:05 GMT
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
	-	`sha256:4b7574e9841a57f1749d68981ae64ff09b650a517c567d131e58218922327cd4`  
		Last Modified: Fri, 19 Nov 2021 02:26:43 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:90b06abdc30a1b74750e7c82c7c28265d3bc9ac9313c43cd59f75356b4a61e14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129106952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ace363ef6a1bcfe8772653cd7f68a3ded9e312988ded50f14c7677e948a5d8`
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
# Fri, 19 Nov 2021 01:46:39 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 19 Nov 2021 01:46:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Nov 2021 01:46:40 GMT
CMD ["influxd"]
# Fri, 19 Nov 2021 01:46:41 GMT
EXPOSE 8086
# Fri, 19 Nov 2021 01:46:42 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 19 Nov 2021 01:46:43 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 19 Nov 2021 01:46:44 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 19 Nov 2021 01:46:45 GMT
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
	-	`sha256:ef8780aa6d16fe2373309446670a390cd9fef4ff82c80d224b0b32b14576b759`  
		Last Modified: Fri, 19 Nov 2021 01:48:02 GMT  
		Size: 4.3 KB (4320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:92f333040d0c2bb908acace09749f58fad16315bcd1feaab2cf02acc1abf6e0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:35963eb83419d50742a376de094a78f8a710a96622ba272f93fe3a2b802b383d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117738533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59f6e76ebb198651f581135910722ccc5f65d1d2bf7b31e2c2121681057d3cfc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:15:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Fri, 03 Dec 2021 04:15:09 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:15:09 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Fri, 03 Dec 2021 04:15:10 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:15:10 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:15:10 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:15:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Fri, 03 Dec 2021 04:15:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:15:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2090b310019ce97e7970604ff30ea6a152dbe8b0eaed9947c9d6db7408d139`  
		Last Modified: Fri, 03 Dec 2021 04:18:57 GMT  
		Size: 56.7 MB (56708560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19b008c9db370dc23bbbd8312dec6c3e409868dc2cb086d4528b5d17278b4fd`  
		Last Modified: Fri, 03 Dec 2021 04:18:50 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505eca482c8a4ca25c181824d56e9093680bb0bba4e87fbc5959260e46bdb88c`  
		Last Modified: Fri, 03 Dec 2021 04:18:49 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1310587db10fd45c1c9dbee91ad18ef7cd9f25d9dcad3161110c6dee1ae29f`  
		Last Modified: Fri, 03 Dec 2021 04:18:50 GMT  
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
$ docker pull influxdb@sha256:6597ad58ab996d75e4f000e6295d2a2db8543644e329f009d0e3b7ceaaed3940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:243f645d0e68cfd1d8a8a25cb505ba4614313fb3e04f3598fcbbd2ffe1ba0afc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182885073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a3e66c579fd83698cd7792b7a31f40b776f2be07bee7a73642502787e71cf2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:31 GMT
ADD file:f077e1a42fb919be2af67820782ceee3b46ffd13d7ab6949bea9921217d12813 in / 
# Thu, 02 Dec 2021 02:48:32 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:41:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:15:51 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 03 Dec 2021 04:15:51 GMT
ENV GOSU_VER=1.12
# Fri, 03 Dec 2021 04:15:55 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Fri, 03 Dec 2021 04:16:12 GMT
ENV INFLUXDB_VERSION=2.1.1
# Fri, 03 Dec 2021 04:16:25 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 03 Dec 2021 04:16:26 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Fri, 03 Dec 2021 04:16:31 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 03 Dec 2021 04:16:32 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 03 Dec 2021 04:16:32 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 03 Dec 2021 04:16:32 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 03 Dec 2021 04:16:33 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 03 Dec 2021 04:16:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:16:33 GMT
CMD ["influxd"]
# Fri, 03 Dec 2021 04:16:33 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:16:34 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 03 Dec 2021 04:16:34 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 03 Dec 2021 04:16:34 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 03 Dec 2021 04:16:34 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:c4cc477c22ba7abce860198107408434dd7bd73ddbaf82f1e69ab941b9979405`  
		Last Modified: Thu, 02 Dec 2021 02:54:07 GMT  
		Size: 50.4 MB (50437113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077c54d048f1f1a1f28079caa54bf5d99803f937ffe5c1dc6e207698f70b4e74`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 7.8 MB (7833819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368544993b2deeeffdd19463cdf92ec4e39f83073de5de316f9f5c725ab403f`  
		Last Modified: Thu, 02 Dec 2021 03:50:46 GMT  
		Size: 10.0 MB (9997240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9046398de937b476bbd1dddbad558ac4c1920fab14866beef48912f8f2c298fa`  
		Last Modified: Fri, 03 Dec 2021 04:20:04 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df21b3d2252fff8be63abc8448901e25fc4884a5c908547c467ff4c1a69cb27`  
		Last Modified: Fri, 03 Dec 2021 04:20:02 GMT  
		Size: 961.0 KB (960957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23da490b8439fd90fb925e88dd05bb3f2baf355d643c9424b947f3c001f360f7`  
		Last Modified: Fri, 03 Dec 2021 04:20:31 GMT  
		Size: 108.3 MB (108324790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaafd74aa812957182e136339b85966d8f81b182941aba8676477f32ed4273c`  
		Last Modified: Fri, 03 Dec 2021 04:20:23 GMT  
		Size: 5.3 MB (5324489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adffecb8fd59efb0b2c62183c51351e3536471b84b7798b9cd214a22dcc55e66`  
		Last Modified: Fri, 03 Dec 2021 04:20:22 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41282bd9b235c778fb450ceb70a6588650efd451de12e9c2b42f2ea386995a7f`  
		Last Modified: Fri, 03 Dec 2021 04:20:22 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258ee0d08be6341996276bcba4089330840b5708a250224f4bec902ca39ae715`  
		Last Modified: Fri, 03 Dec 2021 04:20:22 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:92cb696238c0355c4c41436df43971d7f14e6952f528b0253cf2bab6beb801e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183386540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b807674ff0082f1f84c1a783b57406d1b8176ef84097d6beb956b916b5516d3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:20 GMT
ADD file:82c1819d8416d9d44564980e25e98a081f813bc2ee8ad2789114fe37e802848f in / 
# Thu, 02 Dec 2021 08:08:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:54:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:54:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:48:07 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Fri, 03 Dec 2021 04:48:08 GMT
ENV GOSU_VER=1.12
# Fri, 03 Dec 2021 04:48:17 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Fri, 03 Dec 2021 04:48:54 GMT
ENV INFLUXDB_VERSION=2.1.1
# Fri, 03 Dec 2021 04:49:09 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Fri, 03 Dec 2021 04:49:09 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Fri, 03 Dec 2021 04:49:14 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Fri, 03 Dec 2021 04:49:15 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Fri, 03 Dec 2021 04:49:15 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Fri, 03 Dec 2021 04:49:17 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Fri, 03 Dec 2021 04:49:18 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Fri, 03 Dec 2021 04:49:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:49:19 GMT
CMD ["influxd"]
# Fri, 03 Dec 2021 04:49:20 GMT
EXPOSE 8086
# Fri, 03 Dec 2021 04:49:21 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Fri, 03 Dec 2021 04:49:22 GMT
ENV INFLUXD_INIT_PORT=9999
# Fri, 03 Dec 2021 04:49:23 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Fri, 03 Dec 2021 04:49:24 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:39e4f823356a9e2dbba530f9d363b4d76beaff75a13bad788d38eebeae67e5b0`  
		Last Modified: Thu, 02 Dec 2021 08:41:08 GMT  
		Size: 49.2 MB (49223045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df66cf961d4016eccee4ce9bc5dc18dcd99e9f9963e66c4980a66e6492a421b2`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 7.7 MB (7695103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6c547e43b8b6afdfae413ba7a49c1120d0534fff63c4a242ef611d562a678c`  
		Last Modified: Thu, 02 Dec 2021 10:03:39 GMT  
		Size: 9.8 MB (9767269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e453752afc1d0eeb18c400aa791f08f937a00ecdc6f38ebb18c2ee87a7ff5`  
		Last Modified: Fri, 03 Dec 2021 04:50:42 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4c33d24855b024e47dd55bf44ac4a8c685187c216da8db529dedc00602635`  
		Last Modified: Fri, 03 Dec 2021 04:50:40 GMT  
		Size: 896.4 KB (896361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8240edd1b1dfc75cb17498aaf77dc354d90f88872cd96f215d8a4d9487cd295f`  
		Last Modified: Fri, 03 Dec 2021 04:51:13 GMT  
		Size: 110.9 MB (110891610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d470fb0461896b3f8fc90d6e52aca4127540a50fe95665bd141a83b39e5c60e`  
		Last Modified: Fri, 03 Dec 2021 04:51:05 GMT  
		Size: 4.9 MB (4906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374b9f0297356c62d3be4a7c1a544a3f582bcffa3af49827c0ff51c0587188e`  
		Last Modified: Fri, 03 Dec 2021 04:51:04 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19627f99f85fbd769ed49c25523ea84a2dc4f82fbae5ed9d7eda8e233fec1dbc`  
		Last Modified: Fri, 03 Dec 2021 04:51:04 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792639683dfd3da7c9d7a1023bbd014f647e05e766c95d11430615194c905baa`  
		Last Modified: Fri, 03 Dec 2021 04:51:04 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:0ca5ceb1fdb6f66df576862dda11e64014d64654ff97b7548099f01308a5b782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:58b82d2d4f17694716bb7ca4c3cbb4e9eae0ab319a2b161afd3e8800b78b0d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84445105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ef285e9be66ff6fab01be62814bab2603b44639616578e1292f89c8dde35ac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Dec 2021 04:14:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 03 Dec 2021 04:15:02 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Fri, 03 Dec 2021 04:15:19 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Fri, 03 Dec 2021 04:15:20 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Fri, 03 Dec 2021 04:15:20 GMT
EXPOSE 8091
# Fri, 03 Dec 2021 04:15:20 GMT
VOLUME [/var/lib/influxdb]
# Fri, 03 Dec 2021 04:15:21 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Fri, 03 Dec 2021 04:15:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 04:15:21 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061a4d6f004f3e9cc9d459e874d04c28e3417428d31271aee2275b9aabc8c3f`  
		Last Modified: Fri, 03 Dec 2021 04:17:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55629540dea7b7a486a85afaf3200eb077fdc749afb9b6d4f8d2e17d99367805`  
		Last Modified: Fri, 03 Dec 2021 04:19:15 GMT  
		Size: 23.4 MB (23416339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb75ec0d61146495eead82c8fc32161606e99fa030fbe345435c14aacc62633`  
		Last Modified: Fri, 03 Dec 2021 04:19:12 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a72762b74af5ed043fd0bc4f99b5ddf5bd63a028cf2b98e1c4376d39dea0349`  
		Last Modified: Fri, 03 Dec 2021 04:19:11 GMT  
		Size: 373.0 B  
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
