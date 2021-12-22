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
$ docker pull influxdb@sha256:295ec9e1768f95e705f093358c22768e5c9ce8e93648135b8c54de57dd95fab9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7` - linux; amd64

```console
$ docker pull influxdb@sha256:3d9aaf0250ed780fd9f0d2c9e2734fcac44a67e329c2a264608f14f294dbdb10
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122315331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1201b89d591b6cf0c0909938473968819b1c0416d638dc1f1dde4dd48f1713b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:09:49 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 22 Dec 2021 09:09:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 22 Dec 2021 09:09:57 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 22 Dec 2021 09:09:57 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:09:58 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:09:58 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:09:58 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 22 Dec 2021 09:09:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:09:59 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b422bc2afb059c410a56e9d9f1ee349c35c2a9f1db6af7b1e4dd9f2bac3a97`  
		Last Modified: Wed, 22 Dec 2021 09:13:21 GMT  
		Size: 61.3 MB (61285104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e31d3b90e0160c98a3b006a6a0ecf091485465280891c3739fe04a1018ab5ea`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633945671cf8f82cb283b60bad23bfdfd4fd435cdb1743be9937f588216877d7`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4e80f7e6efff80f70133bb8c31da3090c33d432a3fdc5f6736b01b4c7bfd95`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
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
$ docker pull influxdb@sha256:8021750e887f8e70a29e6a0cb22e41194930fcde1ca8a85efd3650e31c7e965a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114473770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ea1a958229c30c596736f2d9a757f845a119d1b31fe18e7cc74bfa782c8af0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:24 GMT
ADD file:a938be6f1e00e8fe4e0dde6657fcab5db99de34969d54368106a9334f67c1533 in / 
# Tue, 21 Dec 2021 01:44:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:16:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:37:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Dec 2021 19:37:11 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 21 Dec 2021 19:37:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 21 Dec 2021 19:37:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 21 Dec 2021 19:37:17 GMT
EXPOSE 8086
# Tue, 21 Dec 2021 19:37:18 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Dec 2021 19:37:20 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 21 Dec 2021 19:37:21 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Dec 2021 19:37:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:37:22 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d097540eada98ef0bee6e7283ee6a0fbe163c439c3543706a7fbf2f0158fd907`  
		Last Modified: Tue, 21 Dec 2021 01:52:36 GMT  
		Size: 43.2 MB (43173780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cc8f4026ffff85190545c2b0228f223f2fdbf2c94740c8bc8b6ec6acc7e5cf`  
		Last Modified: Tue, 21 Dec 2021 02:26:14 GMT  
		Size: 10.2 MB (10217083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ec2ba0d61fd5c0766a70b7db0bd27e7f6e86fbd1511504e8a5c8d0af26411`  
		Last Modified: Tue, 21 Dec 2021 02:26:13 GMT  
		Size: 3.9 MB (3873882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11925d104b31de38ae0aac03785e451a5c540804d69c7a4b53744dbf0c57712d`  
		Last Modified: Tue, 21 Dec 2021 19:39:43 GMT  
		Size: 2.8 KB (2828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf591ceb499923bee4997adb3ba7cf56d6abd76c8fb8fb3b347480280506f9bb`  
		Last Modified: Tue, 21 Dec 2021 19:39:51 GMT  
		Size: 57.2 MB (57204481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4865a5bc42178c447e42f46420ccf2d2307c789015cd5583691671e0205aab7`  
		Last Modified: Tue, 21 Dec 2021 19:39:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d527e746a8440df9867962c22c01ea7cc375cfc87f0a61a1ee87acc1dc7c16dc`  
		Last Modified: Tue, 21 Dec 2021 19:39:43 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef7b3e034db039537bf2808d4f825654d317d18ee759d7cce501e2db7792283`  
		Last Modified: Tue, 21 Dec 2021 19:39:43 GMT  
		Size: 1.3 KB (1279 bytes)  
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
$ docker pull influxdb@sha256:7063cc2ce5228b4fb6745eed10ef7f38868d48b32156a4e95bde77dfd77f3176
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:aa4b36ecbd15bdea3fdcdb687d6f91394a0c994b3f7687e50b9132b575fbdbe6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148979301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6ad20bbd5aebada6b7d93dfe8b1d9e8319d1569a76dad580f11272187769aa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:03 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 22 Dec 2021 09:10:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:10:12 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 22 Dec 2021 09:10:13 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:10:13 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:10:13 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:10:13 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 22 Dec 2021 09:10:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:10:14 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d4bff0a092481ea40a88a761281c4ebb1969c16471961dde36324a9deb7793`  
		Last Modified: Wed, 22 Dec 2021 09:13:43 GMT  
		Size: 87.9 MB (87949015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac94ae4ab13dc164c00129863fd49e8f70c9ea08cc9ecfa652de90b27c4a7d26`  
		Last Modified: Wed, 22 Dec 2021 09:13:32 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796dd1dc0cad83a7a3993574203f1e5466468aaf2975ea6d63c662b97235e79e`  
		Last Modified: Wed, 22 Dec 2021 09:13:32 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc2d4c0b6b20c859cd7ced0e6876e8808de683e630122976a07ea870c41f2cf`  
		Last Modified: Wed, 22 Dec 2021 09:13:32 GMT  
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
$ docker pull influxdb@sha256:beba51226ae345fffd41cf5b43b93b845f669a5061db176abec22b857be2e25e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:b53fc5aa5d74fac8fd0e40102065418ff68f43392dc228eb3aa6d4f665fa770a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84162647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a1ed51582b5e7558f2c8eaa9dc1a7013272d441e5cea5f7d0dd68d66ab9c66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:03 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 22 Dec 2021 09:10:22 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:10:23 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 22 Dec 2021 09:10:23 GMT
EXPOSE 8091
# Wed, 22 Dec 2021 09:10:23 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:10:23 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:10:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:10:24 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94685fdcf7d6404f0bc4bf76a01f42ab7c62b5306b9974480e6712db1f7f9fc7`  
		Last Modified: Wed, 22 Dec 2021 09:13:57 GMT  
		Size: 23.1 MB (23133569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac08c4d01df7ff777754168f5e0d50b4c9c86734a1d9238b1ac631785aa65a52`  
		Last Modified: Wed, 22 Dec 2021 09:13:54 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc46114f7b45051dcad166ebc2f5f5b47ac2f05dee7d8e5b50eb2aa105607bc`  
		Last Modified: Wed, 22 Dec 2021 09:13:54 GMT  
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
$ docker pull influxdb@sha256:295ec9e1768f95e705f093358c22768e5c9ce8e93648135b8c54de57dd95fab9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7.11` - linux; amd64

```console
$ docker pull influxdb@sha256:3d9aaf0250ed780fd9f0d2c9e2734fcac44a67e329c2a264608f14f294dbdb10
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122315331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1201b89d591b6cf0c0909938473968819b1c0416d638dc1f1dde4dd48f1713b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:09:49 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 22 Dec 2021 09:09:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 22 Dec 2021 09:09:57 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 22 Dec 2021 09:09:57 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:09:58 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:09:58 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:09:58 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 22 Dec 2021 09:09:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:09:59 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b422bc2afb059c410a56e9d9f1ee349c35c2a9f1db6af7b1e4dd9f2bac3a97`  
		Last Modified: Wed, 22 Dec 2021 09:13:21 GMT  
		Size: 61.3 MB (61285104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e31d3b90e0160c98a3b006a6a0ecf091485465280891c3739fe04a1018ab5ea`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633945671cf8f82cb283b60bad23bfdfd4fd435cdb1743be9937f588216877d7`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4e80f7e6efff80f70133bb8c31da3090c33d432a3fdc5f6736b01b4c7bfd95`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
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
$ docker pull influxdb@sha256:8021750e887f8e70a29e6a0cb22e41194930fcde1ca8a85efd3650e31c7e965a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114473770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ea1a958229c30c596736f2d9a757f845a119d1b31fe18e7cc74bfa782c8af0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:24 GMT
ADD file:a938be6f1e00e8fe4e0dde6657fcab5db99de34969d54368106a9334f67c1533 in / 
# Tue, 21 Dec 2021 01:44:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:16:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:37:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Dec 2021 19:37:11 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 21 Dec 2021 19:37:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 21 Dec 2021 19:37:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 21 Dec 2021 19:37:17 GMT
EXPOSE 8086
# Tue, 21 Dec 2021 19:37:18 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Dec 2021 19:37:20 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 21 Dec 2021 19:37:21 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Dec 2021 19:37:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:37:22 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d097540eada98ef0bee6e7283ee6a0fbe163c439c3543706a7fbf2f0158fd907`  
		Last Modified: Tue, 21 Dec 2021 01:52:36 GMT  
		Size: 43.2 MB (43173780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cc8f4026ffff85190545c2b0228f223f2fdbf2c94740c8bc8b6ec6acc7e5cf`  
		Last Modified: Tue, 21 Dec 2021 02:26:14 GMT  
		Size: 10.2 MB (10217083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ec2ba0d61fd5c0766a70b7db0bd27e7f6e86fbd1511504e8a5c8d0af26411`  
		Last Modified: Tue, 21 Dec 2021 02:26:13 GMT  
		Size: 3.9 MB (3873882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11925d104b31de38ae0aac03785e451a5c540804d69c7a4b53744dbf0c57712d`  
		Last Modified: Tue, 21 Dec 2021 19:39:43 GMT  
		Size: 2.8 KB (2828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf591ceb499923bee4997adb3ba7cf56d6abd76c8fb8fb3b347480280506f9bb`  
		Last Modified: Tue, 21 Dec 2021 19:39:51 GMT  
		Size: 57.2 MB (57204481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4865a5bc42178c447e42f46420ccf2d2307c789015cd5583691671e0205aab7`  
		Last Modified: Tue, 21 Dec 2021 19:39:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d527e746a8440df9867962c22c01ea7cc375cfc87f0a61a1ee87acc1dc7c16dc`  
		Last Modified: Tue, 21 Dec 2021 19:39:43 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef7b3e034db039537bf2808d4f825654d317d18ee759d7cce501e2db7792283`  
		Last Modified: Tue, 21 Dec 2021 19:39:43 GMT  
		Size: 1.3 KB (1279 bytes)  
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
$ docker pull influxdb@sha256:7063cc2ce5228b4fb6745eed10ef7f38868d48b32156a4e95bde77dfd77f3176
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:aa4b36ecbd15bdea3fdcdb687d6f91394a0c994b3f7687e50b9132b575fbdbe6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148979301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6ad20bbd5aebada6b7d93dfe8b1d9e8319d1569a76dad580f11272187769aa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:03 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 22 Dec 2021 09:10:11 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:10:12 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 22 Dec 2021 09:10:13 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:10:13 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:10:13 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:10:13 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 22 Dec 2021 09:10:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:10:14 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d4bff0a092481ea40a88a761281c4ebb1969c16471961dde36324a9deb7793`  
		Last Modified: Wed, 22 Dec 2021 09:13:43 GMT  
		Size: 87.9 MB (87949015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac94ae4ab13dc164c00129863fd49e8f70c9ea08cc9ecfa652de90b27c4a7d26`  
		Last Modified: Wed, 22 Dec 2021 09:13:32 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796dd1dc0cad83a7a3993574203f1e5466468aaf2975ea6d63c662b97235e79e`  
		Last Modified: Wed, 22 Dec 2021 09:13:32 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc2d4c0b6b20c859cd7ced0e6876e8808de683e630122976a07ea870c41f2cf`  
		Last Modified: Wed, 22 Dec 2021 09:13:32 GMT  
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
$ docker pull influxdb@sha256:beba51226ae345fffd41cf5b43b93b845f669a5061db176abec22b857be2e25e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:b53fc5aa5d74fac8fd0e40102065418ff68f43392dc228eb3aa6d4f665fa770a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84162647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a1ed51582b5e7558f2c8eaa9dc1a7013272d441e5cea5f7d0dd68d66ab9c66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:03 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 22 Dec 2021 09:10:22 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:10:23 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 22 Dec 2021 09:10:23 GMT
EXPOSE 8091
# Wed, 22 Dec 2021 09:10:23 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:10:23 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:10:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:10:24 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94685fdcf7d6404f0bc4bf76a01f42ab7c62b5306b9974480e6712db1f7f9fc7`  
		Last Modified: Wed, 22 Dec 2021 09:13:57 GMT  
		Size: 23.1 MB (23133569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac08c4d01df7ff777754168f5e0d50b4c9c86734a1d9238b1ac631785aa65a52`  
		Last Modified: Wed, 22 Dec 2021 09:13:54 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc46114f7b45051dcad166ebc2f5f5b47ac2f05dee7d8e5b50eb2aa105607bc`  
		Last Modified: Wed, 22 Dec 2021 09:13:54 GMT  
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
$ docker pull influxdb@sha256:ecab71531ababda454811676e320e1d4536582462a450a291e578bbcd9d00556
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:fe1dafde09cc435ec20a7e8eb9143c73cee02af1310fb390fc913cd7c2170c74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115919701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e20d1d5e2cbd233465da5b626f8a106e38b2db49fe278432feeb374657b587b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:28 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 22 Dec 2021 09:10:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 22 Dec 2021 09:10:34 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 22 Dec 2021 09:10:34 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:10:34 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:10:34 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:10:35 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 22 Dec 2021 09:10:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:10:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c155df9ce9e06969e0bbc7a563ee6b819c2aac4da44b8e2d5027fa8050cce8`  
		Last Modified: Wed, 22 Dec 2021 09:14:16 GMT  
		Size: 54.9 MB (54889473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e62ec82f21c773f44b8eee334d67170d4807c331dca4569789ddd3b63890a5`  
		Last Modified: Wed, 22 Dec 2021 09:14:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f986a4f4c3faf9504ab968b7b2aaa4f794d51b67adf37649ab6f9b5fb86d6e`  
		Last Modified: Wed, 22 Dec 2021 09:14:08 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b16c4f86cfa26da2e2090fe6dff52e7b850e0f9129f43ca601b001bf8d68379`  
		Last Modified: Wed, 22 Dec 2021 09:14:08 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:523fe48a78770ed0c478cfc28740c384242a8a43a5a1e4d02ec10b5f015ca8c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108502945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b81631f547c54808b646e14ef19a5dd41db2c2098b8af88f2cf5d946e068d6d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:24 GMT
ADD file:a938be6f1e00e8fe4e0dde6657fcab5db99de34969d54368106a9334f67c1533 in / 
# Tue, 21 Dec 2021 01:44:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:16:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:37:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Dec 2021 19:37:29 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 21 Dec 2021 19:37:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 21 Dec 2021 19:37:36 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 21 Dec 2021 19:37:36 GMT
EXPOSE 8086
# Tue, 21 Dec 2021 19:37:37 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Dec 2021 19:37:39 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 21 Dec 2021 19:37:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Dec 2021 19:37:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:37:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d097540eada98ef0bee6e7283ee6a0fbe163c439c3543706a7fbf2f0158fd907`  
		Last Modified: Tue, 21 Dec 2021 01:52:36 GMT  
		Size: 43.2 MB (43173780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cc8f4026ffff85190545c2b0228f223f2fdbf2c94740c8bc8b6ec6acc7e5cf`  
		Last Modified: Tue, 21 Dec 2021 02:26:14 GMT  
		Size: 10.2 MB (10217083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ec2ba0d61fd5c0766a70b7db0bd27e7f6e86fbd1511504e8a5c8d0af26411`  
		Last Modified: Tue, 21 Dec 2021 02:26:13 GMT  
		Size: 3.9 MB (3873882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11925d104b31de38ae0aac03785e451a5c540804d69c7a4b53744dbf0c57712d`  
		Last Modified: Tue, 21 Dec 2021 19:39:43 GMT  
		Size: 2.8 KB (2828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87528bf9e2e260d23a5e570e233c591a788767280b43cf93a617838ee997d43`  
		Last Modified: Tue, 21 Dec 2021 19:40:08 GMT  
		Size: 51.2 MB (51233654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4cd1b43a7cc78eb8ece336d24462817ef9fe9d59e9d739595f383c23e0a40`  
		Last Modified: Tue, 21 Dec 2021 19:40:02 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf14f3f46fff17f5d224ae599a02769bc8e4742f6d078569f8a7c57a24c6264f`  
		Last Modified: Tue, 21 Dec 2021 19:40:02 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c190c20e820d458d917d5063e3139f051db5edba862c0773a22199661378aa`  
		Last Modified: Tue, 21 Dec 2021 19:40:02 GMT  
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
$ docker pull influxdb@sha256:c4b004dfec2d89e2ac43ca06ad688f3c26b1d4a3d83b121e39e811b2134a748b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:c1f8810e888df0d116f6b263296e04262e2a52ccc47b48b7078b1db4c0816ba0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117738825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f0c63c2806747f33ac32ceb11d51db71207af8c6bb9836622dfb4146413689`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:40 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 22 Dec 2021 09:10:47 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:10:48 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 22 Dec 2021 09:10:48 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:10:48 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:10:49 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:10:49 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 22 Dec 2021 09:10:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:10:49 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5457901e9b1eb23a9cdc111b2c41ef1de5367a2c51e2b554177c6d569ab481f4`  
		Last Modified: Wed, 22 Dec 2021 09:14:35 GMT  
		Size: 56.7 MB (56708538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914cd714492a90286dcb4c534acea2fde1185d474c3207e16b7862a0e2ca3904`  
		Last Modified: Wed, 22 Dec 2021 09:14:27 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f5e1e401c027f60cfad33af07a2b520e912d951e62f3a5bea3a953bdaa7747`  
		Last Modified: Wed, 22 Dec 2021 09:14:27 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bdc72aedcbc9d8397b983e48069f129a54af1024d8478fbeeae6390ab98d7d`  
		Last Modified: Wed, 22 Dec 2021 09:14:27 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:95634380d6086158376d63eea5a484fe860bbed32b5cb486d7c7714bb150ea52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:c43499819b4d18d8bca5e6a79493bb9a2d457c17a966c1caf8e4e6e3a5b788e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84445428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117517c5b51f7a004429ede7f729d2b0bc1b70f69267a3205e7a0878bc5cb9d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:40 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 22 Dec 2021 09:10:59 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:10:59 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 22 Dec 2021 09:10:59 GMT
EXPOSE 8091
# Wed, 22 Dec 2021 09:11:00 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:11:00 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:11:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:11:01 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eafc7507bd49fb322c1bc7a8b8659ee8f30848b9ecd489b8a47635aad6729ab`  
		Last Modified: Wed, 22 Dec 2021 09:14:52 GMT  
		Size: 23.4 MB (23416348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8847c33bf111eff87c8df062ec12534444aa6baf07719d87104bed2958b9ad9b`  
		Last Modified: Wed, 22 Dec 2021 09:14:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0b4877617ddd1c214745691c4dd0f0d248166dc32390676fa78ac99753cc41`  
		Last Modified: Wed, 22 Dec 2021 09:14:49 GMT  
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
$ docker pull influxdb@sha256:ecab71531ababda454811676e320e1d4536582462a450a291e578bbcd9d00556
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:fe1dafde09cc435ec20a7e8eb9143c73cee02af1310fb390fc913cd7c2170c74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115919701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e20d1d5e2cbd233465da5b626f8a106e38b2db49fe278432feeb374657b587b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:28 GMT
ENV INFLUXDB_VERSION=1.8.10
# Wed, 22 Dec 2021 09:10:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 22 Dec 2021 09:10:34 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 22 Dec 2021 09:10:34 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:10:34 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:10:34 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:10:35 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 22 Dec 2021 09:10:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:10:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c155df9ce9e06969e0bbc7a563ee6b819c2aac4da44b8e2d5027fa8050cce8`  
		Last Modified: Wed, 22 Dec 2021 09:14:16 GMT  
		Size: 54.9 MB (54889473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e62ec82f21c773f44b8eee334d67170d4807c331dca4569789ddd3b63890a5`  
		Last Modified: Wed, 22 Dec 2021 09:14:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f986a4f4c3faf9504ab968b7b2aaa4f794d51b67adf37649ab6f9b5fb86d6e`  
		Last Modified: Wed, 22 Dec 2021 09:14:08 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b16c4f86cfa26da2e2090fe6dff52e7b850e0f9129f43ca601b001bf8d68379`  
		Last Modified: Wed, 22 Dec 2021 09:14:08 GMT  
		Size: 1.3 KB (1281 bytes)  
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
$ docker pull influxdb@sha256:523fe48a78770ed0c478cfc28740c384242a8a43a5a1e4d02ec10b5f015ca8c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108502945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b81631f547c54808b646e14ef19a5dd41db2c2098b8af88f2cf5d946e068d6d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:24 GMT
ADD file:a938be6f1e00e8fe4e0dde6657fcab5db99de34969d54368106a9334f67c1533 in / 
# Tue, 21 Dec 2021 01:44:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:16:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:37:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Dec 2021 19:37:29 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 21 Dec 2021 19:37:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 21 Dec 2021 19:37:36 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 21 Dec 2021 19:37:36 GMT
EXPOSE 8086
# Tue, 21 Dec 2021 19:37:37 GMT
VOLUME [/var/lib/influxdb]
# Tue, 21 Dec 2021 19:37:39 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 21 Dec 2021 19:37:40 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 21 Dec 2021 19:37:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:37:41 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d097540eada98ef0bee6e7283ee6a0fbe163c439c3543706a7fbf2f0158fd907`  
		Last Modified: Tue, 21 Dec 2021 01:52:36 GMT  
		Size: 43.2 MB (43173780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cc8f4026ffff85190545c2b0228f223f2fdbf2c94740c8bc8b6ec6acc7e5cf`  
		Last Modified: Tue, 21 Dec 2021 02:26:14 GMT  
		Size: 10.2 MB (10217083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ec2ba0d61fd5c0766a70b7db0bd27e7f6e86fbd1511504e8a5c8d0af26411`  
		Last Modified: Tue, 21 Dec 2021 02:26:13 GMT  
		Size: 3.9 MB (3873882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11925d104b31de38ae0aac03785e451a5c540804d69c7a4b53744dbf0c57712d`  
		Last Modified: Tue, 21 Dec 2021 19:39:43 GMT  
		Size: 2.8 KB (2828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87528bf9e2e260d23a5e570e233c591a788767280b43cf93a617838ee997d43`  
		Last Modified: Tue, 21 Dec 2021 19:40:08 GMT  
		Size: 51.2 MB (51233654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4cd1b43a7cc78eb8ece336d24462817ef9fe9d59e9d739595f383c23e0a40`  
		Last Modified: Tue, 21 Dec 2021 19:40:02 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf14f3f46fff17f5d224ae599a02769bc8e4742f6d078569f8a7c57a24c6264f`  
		Last Modified: Tue, 21 Dec 2021 19:40:02 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c190c20e820d458d917d5063e3139f051db5edba862c0773a22199661378aa`  
		Last Modified: Tue, 21 Dec 2021 19:40:02 GMT  
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
$ docker pull influxdb@sha256:c4b004dfec2d89e2ac43ca06ad688f3c26b1d4a3d83b121e39e811b2134a748b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:c1f8810e888df0d116f6b263296e04262e2a52ccc47b48b7078b1db4c0816ba0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117738825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f0c63c2806747f33ac32ceb11d51db71207af8c6bb9836622dfb4146413689`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:40 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 22 Dec 2021 09:10:47 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:10:48 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 22 Dec 2021 09:10:48 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:10:48 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:10:49 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:10:49 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 22 Dec 2021 09:10:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:10:49 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5457901e9b1eb23a9cdc111b2c41ef1de5367a2c51e2b554177c6d569ab481f4`  
		Last Modified: Wed, 22 Dec 2021 09:14:35 GMT  
		Size: 56.7 MB (56708538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914cd714492a90286dcb4c534acea2fde1185d474c3207e16b7862a0e2ca3904`  
		Last Modified: Wed, 22 Dec 2021 09:14:27 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f5e1e401c027f60cfad33af07a2b520e912d951e62f3a5bea3a953bdaa7747`  
		Last Modified: Wed, 22 Dec 2021 09:14:27 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bdc72aedcbc9d8397b983e48069f129a54af1024d8478fbeeae6390ab98d7d`  
		Last Modified: Wed, 22 Dec 2021 09:14:27 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:95634380d6086158376d63eea5a484fe860bbed32b5cb486d7c7714bb150ea52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:c43499819b4d18d8bca5e6a79493bb9a2d457c17a966c1caf8e4e6e3a5b788e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84445428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117517c5b51f7a004429ede7f729d2b0bc1b70f69267a3205e7a0878bc5cb9d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:40 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 22 Dec 2021 09:10:59 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:10:59 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 22 Dec 2021 09:10:59 GMT
EXPOSE 8091
# Wed, 22 Dec 2021 09:11:00 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:11:00 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:11:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:11:01 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eafc7507bd49fb322c1bc7a8b8659ee8f30848b9ecd489b8a47635aad6729ab`  
		Last Modified: Wed, 22 Dec 2021 09:14:52 GMT  
		Size: 23.4 MB (23416348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8847c33bf111eff87c8df062ec12534444aa6baf07719d87104bed2958b9ad9b`  
		Last Modified: Wed, 22 Dec 2021 09:14:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0b4877617ddd1c214745691c4dd0f0d248166dc32390676fa78ac99753cc41`  
		Last Modified: Wed, 22 Dec 2021 09:14:49 GMT  
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
$ docker pull influxdb@sha256:39138852cb7b31f3a2371b62b70f54666e5047c62b39ccd0463a110f68aa2d78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:ecf762d76115372d8d6b10456b6294b4a3db95ffada68f9c9d6de5b356da1fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115569885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af081c88c8433618d7d917d7ba914d2548e4ef9e45c8f40f9147ca466fcb1af8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:11:06 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Wed, 22 Dec 2021 09:11:13 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:11:13 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 22 Dec 2021 09:11:13 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:11:14 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:11:14 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:11:14 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 22 Dec 2021 09:11:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:11:15 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a594cd9d8021ed8021a82d68a850f19a3df9863fd1163116657a7b17e8f742fe`  
		Last Modified: Wed, 22 Dec 2021 09:15:14 GMT  
		Size: 54.5 MB (54539601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23e0b5d4c4b72be1daa4ad053b68faaddda27f694e82163d69fffe4f8e0f5e8`  
		Last Modified: Wed, 22 Dec 2021 09:15:06 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f583723852e4ab41011bcdb3f2b0c225eaf81db201e4b6f018fcd732f6f7772`  
		Last Modified: Wed, 22 Dec 2021 09:15:06 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc91a14f9984f678427dbe43f595bdde106fbd52eafe5fd9b4c7b303f814693b`  
		Last Modified: Wed, 22 Dec 2021 09:15:06 GMT  
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
$ docker pull influxdb@sha256:8dc9f715c2457d2f0123fc10305a69770cb1d7a3c7563026c41c76e41f804f95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:7fb559674b0e796a4f6fafaba9123c379aba2bde1facceb536e3027458893bb3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86089264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2602f6437a076680403bb825010302b238e7996763f91a19fed5811cf890396e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:11:06 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Wed, 22 Dec 2021 09:11:25 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:11:25 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 22 Dec 2021 09:11:25 GMT
EXPOSE 8091
# Wed, 22 Dec 2021 09:11:26 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:11:26 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:11:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:11:27 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58a31d513d5f86d6df8781f5a30d48fed69eef5a8f228c7e6682127b042433e`  
		Last Modified: Wed, 22 Dec 2021 09:15:28 GMT  
		Size: 25.1 MB (25060183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb7719311e06c5115282757f74f7810a8769ba81c285c3d7e3bde2d2aea191f`  
		Last Modified: Wed, 22 Dec 2021 09:15:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf60081b791de43bee57e3efd7946ccfb2323a713bbcc6a2ba1a13217d8af61a`  
		Last Modified: Wed, 22 Dec 2021 09:15:24 GMT  
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
$ docker pull influxdb@sha256:39138852cb7b31f3a2371b62b70f54666e5047c62b39ccd0463a110f68aa2d78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.5-data` - linux; amd64

```console
$ docker pull influxdb@sha256:ecf762d76115372d8d6b10456b6294b4a3db95ffada68f9c9d6de5b356da1fe0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115569885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af081c88c8433618d7d917d7ba914d2548e4ef9e45c8f40f9147ca466fcb1af8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:11:06 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Wed, 22 Dec 2021 09:11:13 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:11:13 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 22 Dec 2021 09:11:13 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:11:14 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:11:14 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:11:14 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 22 Dec 2021 09:11:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:11:15 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a594cd9d8021ed8021a82d68a850f19a3df9863fd1163116657a7b17e8f742fe`  
		Last Modified: Wed, 22 Dec 2021 09:15:14 GMT  
		Size: 54.5 MB (54539601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23e0b5d4c4b72be1daa4ad053b68faaddda27f694e82163d69fffe4f8e0f5e8`  
		Last Modified: Wed, 22 Dec 2021 09:15:06 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f583723852e4ab41011bcdb3f2b0c225eaf81db201e4b6f018fcd732f6f7772`  
		Last Modified: Wed, 22 Dec 2021 09:15:06 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc91a14f9984f678427dbe43f595bdde106fbd52eafe5fd9b4c7b303f814693b`  
		Last Modified: Wed, 22 Dec 2021 09:15:06 GMT  
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
$ docker pull influxdb@sha256:8dc9f715c2457d2f0123fc10305a69770cb1d7a3c7563026c41c76e41f804f95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.5-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:7fb559674b0e796a4f6fafaba9123c379aba2bde1facceb536e3027458893bb3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86089264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2602f6437a076680403bb825010302b238e7996763f91a19fed5811cf890396e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:11:06 GMT
ENV INFLUXDB_VERSION=1.9.5-c1.9.5
# Wed, 22 Dec 2021 09:11:25 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:11:25 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 22 Dec 2021 09:11:25 GMT
EXPOSE 8091
# Wed, 22 Dec 2021 09:11:26 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:11:26 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:11:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:11:27 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58a31d513d5f86d6df8781f5a30d48fed69eef5a8f228c7e6682127b042433e`  
		Last Modified: Wed, 22 Dec 2021 09:15:28 GMT  
		Size: 25.1 MB (25060183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb7719311e06c5115282757f74f7810a8769ba81c285c3d7e3bde2d2aea191f`  
		Last Modified: Wed, 22 Dec 2021 09:15:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf60081b791de43bee57e3efd7946ccfb2323a713bbcc6a2ba1a13217d8af61a`  
		Last Modified: Wed, 22 Dec 2021 09:15:24 GMT  
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
$ docker pull influxdb@sha256:a04a623d052b81287d3c3466c30e47cc79ae9071e1b985cba2e74c92d7161ecc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:40fe447e96f10f3475ab34a6905c7a41be76504dfcd55d9f314e5d8c50e09fda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172326470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f568b26cd9d4d67341c15b40a836eb88295f4cf62115ef6165d0447829086d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:53:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:11:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 22 Dec 2021 09:11:32 GMT
ENV GOSU_VER=1.12
# Wed, 22 Dec 2021 09:11:36 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 22 Dec 2021 09:11:37 GMT
ENV INFLUXDB_VERSION=2.0.9
# Wed, 22 Dec 2021 09:11:45 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 22 Dec 2021 09:11:47 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 22 Dec 2021 09:11:47 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 22 Dec 2021 09:11:47 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 22 Dec 2021 09:11:48 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Wed, 22 Dec 2021 09:11:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:11:48 GMT
CMD ["influxd"]
# Wed, 22 Dec 2021 09:11:49 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:11:49 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 22 Dec 2021 09:11:49 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 22 Dec 2021 09:11:49 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 22 Dec 2021 09:11:50 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6013b3e77fe6fd3dcf46a05f8e5b3afa9fbca7ba0161c62e56beb4058334dec`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 7.8 MB (7833863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbced17b6899896c8e4016d62c885d737fe667acace2733e17c64bb974232887`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 10.0 MB (9997172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e540b687b165a61dbe3c24deeb951b27015a89191ed58f2353ff9c3ca738e4`  
		Last Modified: Wed, 22 Dec 2021 09:15:41 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80bad39181a3a0496fad89f84733fbce3d48ea22d2042df767b1577b85823c1`  
		Last Modified: Wed, 22 Dec 2021 09:15:38 GMT  
		Size: 961.0 KB (960950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7f92d3102365755c75be0d4fc4aef0cc0c4d5c5d01e9d2138043e58c46f96`  
		Last Modified: Wed, 22 Dec 2021 09:15:48 GMT  
		Size: 103.1 MB (103090678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2c295b9c41402b3a78064db173ac66d8bf871c5e6dc29a4ddd2b0c5521dd01`  
		Last Modified: Wed, 22 Dec 2021 09:15:38 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a402e463955a76b7b7440e49e6209db16b07f5eaf98915a791f3ae3825d541`  
		Last Modified: Wed, 22 Dec 2021 09:15:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930124f4445a6c63bbcf6c38220e174f703e89447504b0a5dab9ba96a2bdf350`  
		Last Modified: Wed, 22 Dec 2021 09:15:38 GMT  
		Size: 4.3 KB (4327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:011da12beee5c0320d444f2f09e35fc6d4632eeecf0755154019aa272ad3e777
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174115221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6836bcb74a838354daba15487bdb2c5faf2f5ddbfcddccb3a2267e761a56f68b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:34 GMT
ADD file:73bd5e773b257a6ea5d29845b2b112ebce468878a9467e7c0fe61c69994bb47f in / 
# Tue, 21 Dec 2021 01:42:35 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:37:47 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 21 Dec 2021 19:37:48 GMT
ENV GOSU_VER=1.12
# Tue, 21 Dec 2021 19:37:51 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Tue, 21 Dec 2021 19:37:52 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 21 Dec 2021 19:38:05 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 21 Dec 2021 19:38:05 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 21 Dec 2021 19:38:06 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 21 Dec 2021 19:38:08 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 21 Dec 2021 19:38:09 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Tue, 21 Dec 2021 19:38:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:38:10 GMT
CMD ["influxd"]
# Tue, 21 Dec 2021 19:38:11 GMT
EXPOSE 8086
# Tue, 21 Dec 2021 19:38:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 21 Dec 2021 19:38:13 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 21 Dec 2021 19:38:14 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 21 Dec 2021 19:38:15 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:741eb94195433e00f9799629cc66740c97d607d6f3ed207e5738995897c52959`  
		Last Modified: Tue, 21 Dec 2021 01:49:16 GMT  
		Size: 49.2 MB (49223144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098cf33298807975a4d84f59f6689e0bf729b62fca9b7320adb80ebeaabc578`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 7.7 MB (7695163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0317c7db28bd6855b787608d1f4236185907b452f6f545a9954be870828af6`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 9.8 MB (9767165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3dc621fee881f5259b87c37890e99872b5ca801decf25ee25deb63642e0e0f`  
		Last Modified: Tue, 21 Dec 2021 19:40:21 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33deb2bc314db76efb83776d7fa99a3201cc307ed7670baed4c9feb6dd613a0`  
		Last Modified: Tue, 21 Dec 2021 19:40:19 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0839712adc551ace47b291c905a198935c1033aeb0d2a88a30270d50e214a7`  
		Last Modified: Tue, 21 Dec 2021 19:40:30 GMT  
		Size: 106.5 MB (106526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0dfe4ae502bc43880b05d7aa2c94fd4e533e7e5e519dd0f7a5eede208d666d`  
		Last Modified: Tue, 21 Dec 2021 19:40:19 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86128ec2dbbd550d4ff145d46b2d07a928d7780cd567c4ab969b517b7d551423`  
		Last Modified: Tue, 21 Dec 2021 19:40:19 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6dba0bdca1586ee1085d366f1d8916256980b61408c8778940bb44eaf7db5d`  
		Last Modified: Tue, 21 Dec 2021 19:40:19 GMT  
		Size: 4.3 KB (4327 bytes)  
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
$ docker pull influxdb@sha256:a04a623d052b81287d3c3466c30e47cc79ae9071e1b985cba2e74c92d7161ecc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9` - linux; amd64

```console
$ docker pull influxdb@sha256:40fe447e96f10f3475ab34a6905c7a41be76504dfcd55d9f314e5d8c50e09fda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172326470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f568b26cd9d4d67341c15b40a836eb88295f4cf62115ef6165d0447829086d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:53:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:11:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 22 Dec 2021 09:11:32 GMT
ENV GOSU_VER=1.12
# Wed, 22 Dec 2021 09:11:36 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 22 Dec 2021 09:11:37 GMT
ENV INFLUXDB_VERSION=2.0.9
# Wed, 22 Dec 2021 09:11:45 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Wed, 22 Dec 2021 09:11:47 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 22 Dec 2021 09:11:47 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 22 Dec 2021 09:11:47 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 22 Dec 2021 09:11:48 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Wed, 22 Dec 2021 09:11:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:11:48 GMT
CMD ["influxd"]
# Wed, 22 Dec 2021 09:11:49 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:11:49 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 22 Dec 2021 09:11:49 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 22 Dec 2021 09:11:49 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 22 Dec 2021 09:11:50 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6013b3e77fe6fd3dcf46a05f8e5b3afa9fbca7ba0161c62e56beb4058334dec`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 7.8 MB (7833863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbced17b6899896c8e4016d62c885d737fe667acace2733e17c64bb974232887`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 10.0 MB (9997172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e540b687b165a61dbe3c24deeb951b27015a89191ed58f2353ff9c3ca738e4`  
		Last Modified: Wed, 22 Dec 2021 09:15:41 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80bad39181a3a0496fad89f84733fbce3d48ea22d2042df767b1577b85823c1`  
		Last Modified: Wed, 22 Dec 2021 09:15:38 GMT  
		Size: 961.0 KB (960950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d7f92d3102365755c75be0d4fc4aef0cc0c4d5c5d01e9d2138043e58c46f96`  
		Last Modified: Wed, 22 Dec 2021 09:15:48 GMT  
		Size: 103.1 MB (103090678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2c295b9c41402b3a78064db173ac66d8bf871c5e6dc29a4ddd2b0c5521dd01`  
		Last Modified: Wed, 22 Dec 2021 09:15:38 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a402e463955a76b7b7440e49e6209db16b07f5eaf98915a791f3ae3825d541`  
		Last Modified: Wed, 22 Dec 2021 09:15:38 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930124f4445a6c63bbcf6c38220e174f703e89447504b0a5dab9ba96a2bdf350`  
		Last Modified: Wed, 22 Dec 2021 09:15:38 GMT  
		Size: 4.3 KB (4327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:011da12beee5c0320d444f2f09e35fc6d4632eeecf0755154019aa272ad3e777
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174115221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6836bcb74a838354daba15487bdb2c5faf2f5ddbfcddccb3a2267e761a56f68b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:34 GMT
ADD file:73bd5e773b257a6ea5d29845b2b112ebce468878a9467e7c0fe61c69994bb47f in / 
# Tue, 21 Dec 2021 01:42:35 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:37:47 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 21 Dec 2021 19:37:48 GMT
ENV GOSU_VER=1.12
# Tue, 21 Dec 2021 19:37:51 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Tue, 21 Dec 2021 19:37:52 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 21 Dec 2021 19:38:05 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 21 Dec 2021 19:38:05 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 21 Dec 2021 19:38:06 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 21 Dec 2021 19:38:08 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 21 Dec 2021 19:38:09 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Tue, 21 Dec 2021 19:38:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:38:10 GMT
CMD ["influxd"]
# Tue, 21 Dec 2021 19:38:11 GMT
EXPOSE 8086
# Tue, 21 Dec 2021 19:38:12 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 21 Dec 2021 19:38:13 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 21 Dec 2021 19:38:14 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 21 Dec 2021 19:38:15 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:741eb94195433e00f9799629cc66740c97d607d6f3ed207e5738995897c52959`  
		Last Modified: Tue, 21 Dec 2021 01:49:16 GMT  
		Size: 49.2 MB (49223144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098cf33298807975a4d84f59f6689e0bf729b62fca9b7320adb80ebeaabc578`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 7.7 MB (7695163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0317c7db28bd6855b787608d1f4236185907b452f6f545a9954be870828af6`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 9.8 MB (9767165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3dc621fee881f5259b87c37890e99872b5ca801decf25ee25deb63642e0e0f`  
		Last Modified: Tue, 21 Dec 2021 19:40:21 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33deb2bc314db76efb83776d7fa99a3201cc307ed7670baed4c9feb6dd613a0`  
		Last Modified: Tue, 21 Dec 2021 19:40:19 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0839712adc551ace47b291c905a198935c1033aeb0d2a88a30270d50e214a7`  
		Last Modified: Tue, 21 Dec 2021 19:40:30 GMT  
		Size: 106.5 MB (106526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0dfe4ae502bc43880b05d7aa2c94fd4e533e7e5e519dd0f7a5eede208d666d`  
		Last Modified: Tue, 21 Dec 2021 19:40:19 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86128ec2dbbd550d4ff145d46b2d07a928d7780cd567c4ab969b517b7d551423`  
		Last Modified: Tue, 21 Dec 2021 19:40:19 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6dba0bdca1586ee1085d366f1d8916256980b61408c8778940bb44eaf7db5d`  
		Last Modified: Tue, 21 Dec 2021 19:40:19 GMT  
		Size: 4.3 KB (4327 bytes)  
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
$ docker pull influxdb@sha256:1a48c5c4b957b795cdf381bcf91e0d7de9edea2d9be984afbd6e4922e2e24484
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1` - linux; amd64

```console
$ docker pull influxdb@sha256:33379201246b7db4e2438a007eb09459c280bbf669e3a32d0beb2aedce73cfa7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182885090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5a04237d8e1be82d950136533137c5396aeb11c0b7063f6fcb1148041327b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:53:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:11:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 22 Dec 2021 09:11:32 GMT
ENV GOSU_VER=1.12
# Wed, 22 Dec 2021 09:11:36 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 22 Dec 2021 09:11:56 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 22 Dec 2021 09:12:04 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 22 Dec 2021 09:12:05 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 22 Dec 2021 09:12:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 22 Dec 2021 09:12:12 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 22 Dec 2021 09:12:12 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 22 Dec 2021 09:12:12 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 22 Dec 2021 09:12:13 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Wed, 22 Dec 2021 09:12:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:12:13 GMT
CMD ["influxd"]
# Wed, 22 Dec 2021 09:12:13 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:12:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 22 Dec 2021 09:12:14 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 22 Dec 2021 09:12:14 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 22 Dec 2021 09:12:14 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6013b3e77fe6fd3dcf46a05f8e5b3afa9fbca7ba0161c62e56beb4058334dec`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 7.8 MB (7833863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbced17b6899896c8e4016d62c885d737fe667acace2733e17c64bb974232887`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 10.0 MB (9997172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e540b687b165a61dbe3c24deeb951b27015a89191ed58f2353ff9c3ca738e4`  
		Last Modified: Wed, 22 Dec 2021 09:15:41 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80bad39181a3a0496fad89f84733fbce3d48ea22d2042df767b1577b85823c1`  
		Last Modified: Wed, 22 Dec 2021 09:15:38 GMT  
		Size: 961.0 KB (960950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f68ff56df29dddbb2c3c44330303e1a6cf84cffaa1d016b1830853737156a20`  
		Last Modified: Wed, 22 Dec 2021 09:16:09 GMT  
		Size: 108.3 MB (108324813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3136e30866a95c4740cd1c6b7a9593db8a56dd65b59685c661071daac659bb5`  
		Last Modified: Wed, 22 Dec 2021 09:16:00 GMT  
		Size: 5.3 MB (5324488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf057a88c2bad73c9651f4854c3bf55927a6050ae238600dac7acfb12153f3c2`  
		Last Modified: Wed, 22 Dec 2021 09:16:00 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea3b1950251ce2b88984d312df1c27fe94f52a7f5b6940cda6a2853074fd6ee`  
		Last Modified: Wed, 22 Dec 2021 09:15:59 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a6ad39ca1fdd88ee3ebe92f3f2b2bef3c1f947ff8aad69518e38459003374a`  
		Last Modified: Wed, 22 Dec 2021 09:15:59 GMT  
		Size: 4.3 KB (4327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f2d9eb59611928bb8557164e214d63fc90a9cb2f429c2e165269f52272448d5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183386562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8876e4350725bd7a64f0e66729d63f75fb22d4c8bf9519d7cb8f0e58d9b65d73`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:34 GMT
ADD file:73bd5e773b257a6ea5d29845b2b112ebce468878a9467e7c0fe61c69994bb47f in / 
# Tue, 21 Dec 2021 01:42:35 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:37:47 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 21 Dec 2021 19:37:48 GMT
ENV GOSU_VER=1.12
# Tue, 21 Dec 2021 19:37:51 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Tue, 21 Dec 2021 19:38:27 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 21 Dec 2021 19:38:44 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 21 Dec 2021 19:38:44 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 21 Dec 2021 19:38:53 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 21 Dec 2021 19:38:54 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 21 Dec 2021 19:38:55 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 21 Dec 2021 19:38:57 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 21 Dec 2021 19:38:58 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Tue, 21 Dec 2021 19:38:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:38:59 GMT
CMD ["influxd"]
# Tue, 21 Dec 2021 19:39:00 GMT
EXPOSE 8086
# Tue, 21 Dec 2021 19:39:01 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 21 Dec 2021 19:39:02 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 21 Dec 2021 19:39:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 21 Dec 2021 19:39:04 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:741eb94195433e00f9799629cc66740c97d607d6f3ed207e5738995897c52959`  
		Last Modified: Tue, 21 Dec 2021 01:49:16 GMT  
		Size: 49.2 MB (49223144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098cf33298807975a4d84f59f6689e0bf729b62fca9b7320adb80ebeaabc578`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 7.7 MB (7695163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0317c7db28bd6855b787608d1f4236185907b452f6f545a9954be870828af6`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 9.8 MB (9767165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3dc621fee881f5259b87c37890e99872b5ca801decf25ee25deb63642e0e0f`  
		Last Modified: Tue, 21 Dec 2021 19:40:21 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33deb2bc314db76efb83776d7fa99a3201cc307ed7670baed4c9feb6dd613a0`  
		Last Modified: Tue, 21 Dec 2021 19:40:19 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032e939eae958fd2dc4e0072e2433c7e96828de34f77c82f8cbde854a6ae071a`  
		Last Modified: Tue, 21 Dec 2021 19:40:52 GMT  
		Size: 110.9 MB (110891599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c272f1cdfc02cf2f1925154f01ad800a15a6a34af46a02f6685a13abe7bcb81`  
		Last Modified: Tue, 21 Dec 2021 19:40:44 GMT  
		Size: 4.9 MB (4906722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062a34156c9a0c6708828558dda9a70ff6b296ead850475be3b50d773ea7fb54`  
		Last Modified: Tue, 21 Dec 2021 19:40:43 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4b6281d9904c30acb7a4b521b262746053d22f712978ff899236dfd07b4886`  
		Last Modified: Tue, 21 Dec 2021 19:40:43 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9218f9b24364e4e47a9471f48d2c4c9549eaff0575097bb10e99a95dc68d80f`  
		Last Modified: Tue, 21 Dec 2021 19:40:43 GMT  
		Size: 4.3 KB (4327 bytes)  
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
$ docker pull influxdb@sha256:1a48c5c4b957b795cdf381bcf91e0d7de9edea2d9be984afbd6e4922e2e24484
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1` - linux; amd64

```console
$ docker pull influxdb@sha256:33379201246b7db4e2438a007eb09459c280bbf669e3a32d0beb2aedce73cfa7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182885090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5a04237d8e1be82d950136533137c5396aeb11c0b7063f6fcb1148041327b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:53:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:11:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 22 Dec 2021 09:11:32 GMT
ENV GOSU_VER=1.12
# Wed, 22 Dec 2021 09:11:36 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 22 Dec 2021 09:11:56 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 22 Dec 2021 09:12:04 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 22 Dec 2021 09:12:05 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 22 Dec 2021 09:12:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 22 Dec 2021 09:12:12 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 22 Dec 2021 09:12:12 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 22 Dec 2021 09:12:12 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 22 Dec 2021 09:12:13 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Wed, 22 Dec 2021 09:12:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:12:13 GMT
CMD ["influxd"]
# Wed, 22 Dec 2021 09:12:13 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:12:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 22 Dec 2021 09:12:14 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 22 Dec 2021 09:12:14 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 22 Dec 2021 09:12:14 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6013b3e77fe6fd3dcf46a05f8e5b3afa9fbca7ba0161c62e56beb4058334dec`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 7.8 MB (7833863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbced17b6899896c8e4016d62c885d737fe667acace2733e17c64bb974232887`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 10.0 MB (9997172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e540b687b165a61dbe3c24deeb951b27015a89191ed58f2353ff9c3ca738e4`  
		Last Modified: Wed, 22 Dec 2021 09:15:41 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80bad39181a3a0496fad89f84733fbce3d48ea22d2042df767b1577b85823c1`  
		Last Modified: Wed, 22 Dec 2021 09:15:38 GMT  
		Size: 961.0 KB (960950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f68ff56df29dddbb2c3c44330303e1a6cf84cffaa1d016b1830853737156a20`  
		Last Modified: Wed, 22 Dec 2021 09:16:09 GMT  
		Size: 108.3 MB (108324813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3136e30866a95c4740cd1c6b7a9593db8a56dd65b59685c661071daac659bb5`  
		Last Modified: Wed, 22 Dec 2021 09:16:00 GMT  
		Size: 5.3 MB (5324488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf057a88c2bad73c9651f4854c3bf55927a6050ae238600dac7acfb12153f3c2`  
		Last Modified: Wed, 22 Dec 2021 09:16:00 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea3b1950251ce2b88984d312df1c27fe94f52a7f5b6940cda6a2853074fd6ee`  
		Last Modified: Wed, 22 Dec 2021 09:15:59 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a6ad39ca1fdd88ee3ebe92f3f2b2bef3c1f947ff8aad69518e38459003374a`  
		Last Modified: Wed, 22 Dec 2021 09:15:59 GMT  
		Size: 4.3 KB (4327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f2d9eb59611928bb8557164e214d63fc90a9cb2f429c2e165269f52272448d5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183386562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8876e4350725bd7a64f0e66729d63f75fb22d4c8bf9519d7cb8f0e58d9b65d73`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:34 GMT
ADD file:73bd5e773b257a6ea5d29845b2b112ebce468878a9467e7c0fe61c69994bb47f in / 
# Tue, 21 Dec 2021 01:42:35 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:37:47 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 21 Dec 2021 19:37:48 GMT
ENV GOSU_VER=1.12
# Tue, 21 Dec 2021 19:37:51 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Tue, 21 Dec 2021 19:38:27 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 21 Dec 2021 19:38:44 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 21 Dec 2021 19:38:44 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 21 Dec 2021 19:38:53 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 21 Dec 2021 19:38:54 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 21 Dec 2021 19:38:55 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 21 Dec 2021 19:38:57 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 21 Dec 2021 19:38:58 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Tue, 21 Dec 2021 19:38:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:38:59 GMT
CMD ["influxd"]
# Tue, 21 Dec 2021 19:39:00 GMT
EXPOSE 8086
# Tue, 21 Dec 2021 19:39:01 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 21 Dec 2021 19:39:02 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 21 Dec 2021 19:39:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 21 Dec 2021 19:39:04 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:741eb94195433e00f9799629cc66740c97d607d6f3ed207e5738995897c52959`  
		Last Modified: Tue, 21 Dec 2021 01:49:16 GMT  
		Size: 49.2 MB (49223144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098cf33298807975a4d84f59f6689e0bf729b62fca9b7320adb80ebeaabc578`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 7.7 MB (7695163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0317c7db28bd6855b787608d1f4236185907b452f6f545a9954be870828af6`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 9.8 MB (9767165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3dc621fee881f5259b87c37890e99872b5ca801decf25ee25deb63642e0e0f`  
		Last Modified: Tue, 21 Dec 2021 19:40:21 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33deb2bc314db76efb83776d7fa99a3201cc307ed7670baed4c9feb6dd613a0`  
		Last Modified: Tue, 21 Dec 2021 19:40:19 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032e939eae958fd2dc4e0072e2433c7e96828de34f77c82f8cbde854a6ae071a`  
		Last Modified: Tue, 21 Dec 2021 19:40:52 GMT  
		Size: 110.9 MB (110891599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c272f1cdfc02cf2f1925154f01ad800a15a6a34af46a02f6685a13abe7bcb81`  
		Last Modified: Tue, 21 Dec 2021 19:40:44 GMT  
		Size: 4.9 MB (4906722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062a34156c9a0c6708828558dda9a70ff6b296ead850475be3b50d773ea7fb54`  
		Last Modified: Tue, 21 Dec 2021 19:40:43 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4b6281d9904c30acb7a4b521b262746053d22f712978ff899236dfd07b4886`  
		Last Modified: Tue, 21 Dec 2021 19:40:43 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9218f9b24364e4e47a9471f48d2c4c9549eaff0575097bb10e99a95dc68d80f`  
		Last Modified: Tue, 21 Dec 2021 19:40:43 GMT  
		Size: 4.3 KB (4327 bytes)  
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
$ docker pull influxdb@sha256:c4b004dfec2d89e2ac43ca06ad688f3c26b1d4a3d83b121e39e811b2134a748b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:c1f8810e888df0d116f6b263296e04262e2a52ccc47b48b7078b1db4c0816ba0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117738825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f0c63c2806747f33ac32ceb11d51db71207af8c6bb9836622dfb4146413689`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:40 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 22 Dec 2021 09:10:47 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:10:48 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 22 Dec 2021 09:10:48 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:10:48 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:10:49 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:10:49 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 22 Dec 2021 09:10:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:10:49 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5457901e9b1eb23a9cdc111b2c41ef1de5367a2c51e2b554177c6d569ab481f4`  
		Last Modified: Wed, 22 Dec 2021 09:14:35 GMT  
		Size: 56.7 MB (56708538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914cd714492a90286dcb4c534acea2fde1185d474c3207e16b7862a0e2ca3904`  
		Last Modified: Wed, 22 Dec 2021 09:14:27 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f5e1e401c027f60cfad33af07a2b520e912d951e62f3a5bea3a953bdaa7747`  
		Last Modified: Wed, 22 Dec 2021 09:14:27 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bdc72aedcbc9d8397b983e48069f129a54af1024d8478fbeeae6390ab98d7d`  
		Last Modified: Wed, 22 Dec 2021 09:14:27 GMT  
		Size: 1.3 KB (1282 bytes)  
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
$ docker pull influxdb@sha256:1a48c5c4b957b795cdf381bcf91e0d7de9edea2d9be984afbd6e4922e2e24484
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:33379201246b7db4e2438a007eb09459c280bbf669e3a32d0beb2aedce73cfa7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182885090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5a04237d8e1be82d950136533137c5396aeb11c0b7063f6fcb1148041327b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:53:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:11:32 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 22 Dec 2021 09:11:32 GMT
ENV GOSU_VER=1.12
# Wed, 22 Dec 2021 09:11:36 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Wed, 22 Dec 2021 09:11:56 GMT
ENV INFLUXDB_VERSION=2.1.1
# Wed, 22 Dec 2021 09:12:04 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Wed, 22 Dec 2021 09:12:05 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Wed, 22 Dec 2021 09:12:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Wed, 22 Dec 2021 09:12:12 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Wed, 22 Dec 2021 09:12:12 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Wed, 22 Dec 2021 09:12:12 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Wed, 22 Dec 2021 09:12:13 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Wed, 22 Dec 2021 09:12:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:12:13 GMT
CMD ["influxd"]
# Wed, 22 Dec 2021 09:12:13 GMT
EXPOSE 8086
# Wed, 22 Dec 2021 09:12:14 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Wed, 22 Dec 2021 09:12:14 GMT
ENV INFLUXD_INIT_PORT=9999
# Wed, 22 Dec 2021 09:12:14 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Wed, 22 Dec 2021 09:12:14 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6013b3e77fe6fd3dcf46a05f8e5b3afa9fbca7ba0161c62e56beb4058334dec`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 7.8 MB (7833863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbced17b6899896c8e4016d62c885d737fe667acace2733e17c64bb974232887`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 10.0 MB (9997172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e540b687b165a61dbe3c24deeb951b27015a89191ed58f2353ff9c3ca738e4`  
		Last Modified: Wed, 22 Dec 2021 09:15:41 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80bad39181a3a0496fad89f84733fbce3d48ea22d2042df767b1577b85823c1`  
		Last Modified: Wed, 22 Dec 2021 09:15:38 GMT  
		Size: 961.0 KB (960950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f68ff56df29dddbb2c3c44330303e1a6cf84cffaa1d016b1830853737156a20`  
		Last Modified: Wed, 22 Dec 2021 09:16:09 GMT  
		Size: 108.3 MB (108324813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3136e30866a95c4740cd1c6b7a9593db8a56dd65b59685c661071daac659bb5`  
		Last Modified: Wed, 22 Dec 2021 09:16:00 GMT  
		Size: 5.3 MB (5324488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf057a88c2bad73c9651f4854c3bf55927a6050ae238600dac7acfb12153f3c2`  
		Last Modified: Wed, 22 Dec 2021 09:16:00 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea3b1950251ce2b88984d312df1c27fe94f52a7f5b6940cda6a2853074fd6ee`  
		Last Modified: Wed, 22 Dec 2021 09:15:59 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a6ad39ca1fdd88ee3ebe92f3f2b2bef3c1f947ff8aad69518e38459003374a`  
		Last Modified: Wed, 22 Dec 2021 09:15:59 GMT  
		Size: 4.3 KB (4327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:f2d9eb59611928bb8557164e214d63fc90a9cb2f429c2e165269f52272448d5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183386562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8876e4350725bd7a64f0e66729d63f75fb22d4c8bf9519d7cb8f0e58d9b65d73`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:34 GMT
ADD file:73bd5e773b257a6ea5d29845b2b112ebce468878a9467e7c0fe61c69994bb47f in / 
# Tue, 21 Dec 2021 01:42:35 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:37:47 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 21 Dec 2021 19:37:48 GMT
ENV GOSU_VER=1.12
# Tue, 21 Dec 2021 19:37:51 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Tue, 21 Dec 2021 19:38:27 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 21 Dec 2021 19:38:44 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 21 Dec 2021 19:38:44 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 21 Dec 2021 19:38:53 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 21 Dec 2021 19:38:54 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 21 Dec 2021 19:38:55 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 21 Dec 2021 19:38:57 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 21 Dec 2021 19:38:58 GMT
COPY file:eb5abb8e3cc7d06174d5d4f90530232d892794f95ab3288feff92a49f909192f in /entrypoint.sh 
# Tue, 21 Dec 2021 19:38:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Dec 2021 19:38:59 GMT
CMD ["influxd"]
# Tue, 21 Dec 2021 19:39:00 GMT
EXPOSE 8086
# Tue, 21 Dec 2021 19:39:01 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 21 Dec 2021 19:39:02 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 21 Dec 2021 19:39:03 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 21 Dec 2021 19:39:04 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:741eb94195433e00f9799629cc66740c97d607d6f3ed207e5738995897c52959`  
		Last Modified: Tue, 21 Dec 2021 01:49:16 GMT  
		Size: 49.2 MB (49223144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098cf33298807975a4d84f59f6689e0bf729b62fca9b7320adb80ebeaabc578`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 7.7 MB (7695163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0317c7db28bd6855b787608d1f4236185907b452f6f545a9954be870828af6`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 9.8 MB (9767165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3dc621fee881f5259b87c37890e99872b5ca801decf25ee25deb63642e0e0f`  
		Last Modified: Tue, 21 Dec 2021 19:40:21 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33deb2bc314db76efb83776d7fa99a3201cc307ed7670baed4c9feb6dd613a0`  
		Last Modified: Tue, 21 Dec 2021 19:40:19 GMT  
		Size: 896.3 KB (896336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032e939eae958fd2dc4e0072e2433c7e96828de34f77c82f8cbde854a6ae071a`  
		Last Modified: Tue, 21 Dec 2021 19:40:52 GMT  
		Size: 110.9 MB (110891599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c272f1cdfc02cf2f1925154f01ad800a15a6a34af46a02f6685a13abe7bcb81`  
		Last Modified: Tue, 21 Dec 2021 19:40:44 GMT  
		Size: 4.9 MB (4906722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062a34156c9a0c6708828558dda9a70ff6b296ead850475be3b50d773ea7fb54`  
		Last Modified: Tue, 21 Dec 2021 19:40:43 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4b6281d9904c30acb7a4b521b262746053d22f712978ff899236dfd07b4886`  
		Last Modified: Tue, 21 Dec 2021 19:40:43 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9218f9b24364e4e47a9471f48d2c4c9549eaff0575097bb10e99a95dc68d80f`  
		Last Modified: Tue, 21 Dec 2021 19:40:43 GMT  
		Size: 4.3 KB (4327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:95634380d6086158376d63eea5a484fe860bbed32b5cb486d7c7714bb150ea52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:c43499819b4d18d8bca5e6a79493bb9a2d457c17a966c1caf8e4e6e3a5b788e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84445428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117517c5b51f7a004429ede7f729d2b0bc1b70f69267a3205e7a0878bc5cb9d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:31 GMT
ADD file:4937a62e9e92f367221357a58d7438d1f76546bf3669281431633aebcfd7839d in / 
# Tue, 21 Dec 2021 01:24:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:56:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 09:09:49 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 09:10:40 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 22 Dec 2021 09:10:59 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 22 Dec 2021 09:10:59 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 22 Dec 2021 09:10:59 GMT
EXPOSE 8091
# Wed, 22 Dec 2021 09:11:00 GMT
VOLUME [/var/lib/influxdb]
# Wed, 22 Dec 2021 09:11:00 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 22 Dec 2021 09:11:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 09:11:01 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:6a56b4def9c45045931a9cf99e9365b558347ae41ec8bfb104a7787e1c3129b0`  
		Last Modified: Tue, 21 Dec 2021 01:31:13 GMT  
		Size: 45.4 MB (45381404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a7240797a1605f51c11e7c8f49754a8a78c89616dec348fa937886702d115`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 11.3 MB (11301861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb8704bdb1f04110dfee1bc6e00f421a37681ff4f136c12337f31c1ccd62bb`  
		Last Modified: Tue, 21 Dec 2021 02:04:58 GMT  
		Size: 4.3 MB (4342385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0dd837ecaa07c6ca38834d78380269abc5acfa13cf70844e7cab915c36c493`  
		Last Modified: Wed, 22 Dec 2021 09:13:12 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eafc7507bd49fb322c1bc7a8b8659ee8f30848b9ecd489b8a47635aad6729ab`  
		Last Modified: Wed, 22 Dec 2021 09:14:52 GMT  
		Size: 23.4 MB (23416348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8847c33bf111eff87c8df062ec12534444aa6baf07719d87104bed2958b9ad9b`  
		Last Modified: Wed, 22 Dec 2021 09:14:49 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0b4877617ddd1c214745691c4dd0f0d248166dc32390676fa78ac99753cc41`  
		Last Modified: Wed, 22 Dec 2021 09:14:49 GMT  
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
