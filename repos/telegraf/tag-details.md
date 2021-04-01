<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.16`](#telegraf116)
-	[`telegraf:1.16-alpine`](#telegraf116-alpine)
-	[`telegraf:1.16.3`](#telegraf1163)
-	[`telegraf:1.16.3-alpine`](#telegraf1163-alpine)
-	[`telegraf:1.17`](#telegraf117)
-	[`telegraf:1.17-alpine`](#telegraf117-alpine)
-	[`telegraf:1.17.3`](#telegraf1173)
-	[`telegraf:1.17.3-alpine`](#telegraf1173-alpine)
-	[`telegraf:1.18`](#telegraf118)
-	[`telegraf:1.18-alpine`](#telegraf118-alpine)
-	[`telegraf:1.18.0`](#telegraf1180)
-	[`telegraf:1.18.0-alpine`](#telegraf1180-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.16`

```console
$ docker pull telegraf@sha256:75636c2a636a73edb4cf9fa1f5b3a45b71de556b49a7849954c1c9ef56c166b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.16` - linux; amd64

```console
$ docker pull telegraf@sha256:4265e834819a7722d69406b8edee898e1347c91b676ada0b10e3246e83411a1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (108037527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d413dbae156ee9045a1bf028dbe816de0bb8f9149084d188e08d6aa8fda0f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:46:31 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:46:37 GMT
ENV TELEGRAF_VERSION=1.16.3
# Wed, 31 Mar 2021 22:46:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:46:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:46:44 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:46:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:46:45 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f1e8117dbb1c6a57603cb4f321a861a08105a81bcc6b01b0ec2b78c8523a5`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 7.8 MB (7832608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2faf66abec3dce9f54d6722ff592fce6dd4fb58a0d0b72282936c6598a3b3`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 10.0 MB (9997208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86207fc29d89bea4c2d79d45aa28f8dab5408d1b5646e6279d640cd8a2e857d5`  
		Last Modified: Wed, 31 Mar 2021 22:48:16 GMT  
		Size: 17.4 MB (17414524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e93c7da54121b4ac3d6cafa7058eeb1a43da87a6f99e3cea4038f2be1390a4`  
		Last Modified: Wed, 31 Mar 2021 22:48:11 GMT  
		Size: 2.9 KB (2909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b2a00ec649043f0c7b3a2c71f606a141e2009b7d7c3c3c1bba94153156ac03`  
		Last Modified: Wed, 31 Mar 2021 22:48:15 GMT  
		Size: 22.4 MB (22357252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44c1d68d6258792028d04412d7c35e2c80638c17080d54e690c03edf36fce1f`  
		Last Modified: Wed, 31 Mar 2021 22:48:10 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.16` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:fca4ccb4da37ab64d708f2d0013c7e96b27a34fccf378ea13b12141122e38097
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99435381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2599185adc5abea0cfb1806fb9cd6134031c80c74efeedeb61db618397494502`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:08 GMT
ADD file:bd48b3fec0eec547919c9e90c2055f1d879c78e4eb7d92598bf55c0f83c44836 in / 
# Tue, 30 Mar 2021 23:08:12 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:22:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:26:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:26:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:26:36 GMT
ENV TELEGRAF_VERSION=1.16.3
# Wed, 31 Mar 2021 22:26:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:26:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:26:45 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:26:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:26:46 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0bf0c5f21d801f530938b2464483aaad40947de697c29cedece44096ead1522c`  
		Last Modified: Tue, 30 Mar 2021 23:15:55 GMT  
		Size: 45.9 MB (45915428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8c35c4e8e932b85e0233ff1c20dcdd8bc13a0238128bcfcde181c0b04b037`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 7.1 MB (7123902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d88df2bbeddb232fbd4bf0ffd8efd62285f56f8eb6e2007c1a89ecfdc0f3ad`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 9.3 MB (9343731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a109f5c8c61633040e902da4a22004cdff8af3da4aec748c629a645ce3ae66a1`  
		Last Modified: Wed, 31 Mar 2021 22:27:50 GMT  
		Size: 16.2 MB (16159155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ab9c2159ba9b5e101028955dc796186a890dbc8bf5f65893e5ae7fea81840d`  
		Last Modified: Wed, 31 Mar 2021 22:27:39 GMT  
		Size: 2.9 KB (2910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76be1d2e687b918df1c130729ab862292bb4fcb21206f001f2fce2df439ba06`  
		Last Modified: Wed, 31 Mar 2021 22:27:47 GMT  
		Size: 20.9 MB (20890071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cf0485d23d4f6b5592b015174f3854eea4392f05b869824c72ffaffb583ea`  
		Last Modified: Wed, 31 Mar 2021 22:27:39 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.16` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:2f90775ef09e76dff604814fcd0fc90af8f892490dd67e0ce974f1b6e1ca0a1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104671759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb24938ea2c991e3e39fec538d12a77309d0c219bde13d62e535e8a4a8dfd62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:51:32 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 23:51:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 23:51:38 GMT
ENV TELEGRAF_VERSION=1.16.3
# Wed, 31 Mar 2021 23:51:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 23:51:45 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 23:51:46 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 23:51:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 23:51:48 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ccb2b90ef28919d82b935e6918055d100dffe73773e1b39b27c9389f0b1ef8`  
		Last Modified: Wed, 31 Mar 2021 23:53:17 GMT  
		Size: 17.3 MB (17269621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cbdac78f11712418529367b951f71d2d3634210107f88af2a92072b463ba6b`  
		Last Modified: Wed, 31 Mar 2021 23:53:09 GMT  
		Size: 2.9 KB (2896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539c67f81ca6d044fd05c8feae45e98257412d97b10168922f01e32665fa5c3`  
		Last Modified: Wed, 31 Mar 2021 23:53:18 GMT  
		Size: 20.5 MB (20494328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcceb0e52ad6a8b577fcf79f6f3c3751d2ded3557632d3edb3b40e6342da363c`  
		Last Modified: Wed, 31 Mar 2021 23:53:09 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.16-alpine`

```console
$ docker pull telegraf@sha256:bafffff80f705dc77b3ddffdc085018edc8ca29fe6036b8dc55ce2cbdeac20c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.16-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4b97547cb91d8b2f9d9b84ed744303e723033bb267e43334385e41451b1ef9bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28315034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5ae49b672a1396eee003f7937a976d58212ca2aec493fefa226f012b0bc9fd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:46:56 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Wed, 31 Mar 2021 22:46:56 GMT
ENV TELEGRAF_VERSION=1.16.3
# Wed, 31 Mar 2021 22:47:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 31 Mar 2021 22:47:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:05 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38a141eb441d0521693dd710eb5a2a3ceae66767667e8820f152011f8f8a1de`  
		Last Modified: Wed, 31 Mar 2021 22:12:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3d7ca742af0ce468e2012708013276fbd53bc83cbfbc6067bee7576dfc77fd`  
		Last Modified: Wed, 31 Mar 2021 22:48:32 GMT  
		Size: 3.3 MB (3300612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b24b2ef2e945c093a864cee98065bb150dcf6fb3f625d1b8a0e5747387e6113`  
		Last Modified: Wed, 31 Mar 2021 22:48:38 GMT  
		Size: 22.2 MB (22214370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e62aa81482401d0acc5589d9a8cb6d47c2eaa7eeb1c6e43750365771c0c8fb5`  
		Last Modified: Wed, 31 Mar 2021 22:48:28 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.16.3`

```console
$ docker pull telegraf@sha256:75636c2a636a73edb4cf9fa1f5b3a45b71de556b49a7849954c1c9ef56c166b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.16.3` - linux; amd64

```console
$ docker pull telegraf@sha256:4265e834819a7722d69406b8edee898e1347c91b676ada0b10e3246e83411a1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (108037527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d413dbae156ee9045a1bf028dbe816de0bb8f9149084d188e08d6aa8fda0f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:46:31 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:46:37 GMT
ENV TELEGRAF_VERSION=1.16.3
# Wed, 31 Mar 2021 22:46:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:46:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:46:44 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:46:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:46:45 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f1e8117dbb1c6a57603cb4f321a861a08105a81bcc6b01b0ec2b78c8523a5`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 7.8 MB (7832608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2faf66abec3dce9f54d6722ff592fce6dd4fb58a0d0b72282936c6598a3b3`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 10.0 MB (9997208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86207fc29d89bea4c2d79d45aa28f8dab5408d1b5646e6279d640cd8a2e857d5`  
		Last Modified: Wed, 31 Mar 2021 22:48:16 GMT  
		Size: 17.4 MB (17414524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e93c7da54121b4ac3d6cafa7058eeb1a43da87a6f99e3cea4038f2be1390a4`  
		Last Modified: Wed, 31 Mar 2021 22:48:11 GMT  
		Size: 2.9 KB (2909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b2a00ec649043f0c7b3a2c71f606a141e2009b7d7c3c3c1bba94153156ac03`  
		Last Modified: Wed, 31 Mar 2021 22:48:15 GMT  
		Size: 22.4 MB (22357252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44c1d68d6258792028d04412d7c35e2c80638c17080d54e690c03edf36fce1f`  
		Last Modified: Wed, 31 Mar 2021 22:48:10 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.16.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:fca4ccb4da37ab64d708f2d0013c7e96b27a34fccf378ea13b12141122e38097
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99435381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2599185adc5abea0cfb1806fb9cd6134031c80c74efeedeb61db618397494502`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:08 GMT
ADD file:bd48b3fec0eec547919c9e90c2055f1d879c78e4eb7d92598bf55c0f83c44836 in / 
# Tue, 30 Mar 2021 23:08:12 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:22:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:26:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:26:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:26:36 GMT
ENV TELEGRAF_VERSION=1.16.3
# Wed, 31 Mar 2021 22:26:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:26:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:26:45 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:26:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:26:46 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0bf0c5f21d801f530938b2464483aaad40947de697c29cedece44096ead1522c`  
		Last Modified: Tue, 30 Mar 2021 23:15:55 GMT  
		Size: 45.9 MB (45915428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8c35c4e8e932b85e0233ff1c20dcdd8bc13a0238128bcfcde181c0b04b037`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 7.1 MB (7123902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d88df2bbeddb232fbd4bf0ffd8efd62285f56f8eb6e2007c1a89ecfdc0f3ad`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 9.3 MB (9343731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a109f5c8c61633040e902da4a22004cdff8af3da4aec748c629a645ce3ae66a1`  
		Last Modified: Wed, 31 Mar 2021 22:27:50 GMT  
		Size: 16.2 MB (16159155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ab9c2159ba9b5e101028955dc796186a890dbc8bf5f65893e5ae7fea81840d`  
		Last Modified: Wed, 31 Mar 2021 22:27:39 GMT  
		Size: 2.9 KB (2910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76be1d2e687b918df1c130729ab862292bb4fcb21206f001f2fce2df439ba06`  
		Last Modified: Wed, 31 Mar 2021 22:27:47 GMT  
		Size: 20.9 MB (20890071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cf0485d23d4f6b5592b015174f3854eea4392f05b869824c72ffaffb583ea`  
		Last Modified: Wed, 31 Mar 2021 22:27:39 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.16.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:2f90775ef09e76dff604814fcd0fc90af8f892490dd67e0ce974f1b6e1ca0a1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104671759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb24938ea2c991e3e39fec538d12a77309d0c219bde13d62e535e8a4a8dfd62`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:51:32 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 23:51:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 23:51:38 GMT
ENV TELEGRAF_VERSION=1.16.3
# Wed, 31 Mar 2021 23:51:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 23:51:45 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 23:51:46 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 23:51:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 23:51:48 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ccb2b90ef28919d82b935e6918055d100dffe73773e1b39b27c9389f0b1ef8`  
		Last Modified: Wed, 31 Mar 2021 23:53:17 GMT  
		Size: 17.3 MB (17269621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cbdac78f11712418529367b951f71d2d3634210107f88af2a92072b463ba6b`  
		Last Modified: Wed, 31 Mar 2021 23:53:09 GMT  
		Size: 2.9 KB (2896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539c67f81ca6d044fd05c8feae45e98257412d97b10168922f01e32665fa5c3`  
		Last Modified: Wed, 31 Mar 2021 23:53:18 GMT  
		Size: 20.5 MB (20494328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcceb0e52ad6a8b577fcf79f6f3c3751d2ded3557632d3edb3b40e6342da363c`  
		Last Modified: Wed, 31 Mar 2021 23:53:09 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.16.3-alpine`

```console
$ docker pull telegraf@sha256:bafffff80f705dc77b3ddffdc085018edc8ca29fe6036b8dc55ce2cbdeac20c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.16.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4b97547cb91d8b2f9d9b84ed744303e723033bb267e43334385e41451b1ef9bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28315034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5ae49b672a1396eee003f7937a976d58212ca2aec493fefa226f012b0bc9fd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:46:56 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Wed, 31 Mar 2021 22:46:56 GMT
ENV TELEGRAF_VERSION=1.16.3
# Wed, 31 Mar 2021 22:47:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 31 Mar 2021 22:47:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:05 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38a141eb441d0521693dd710eb5a2a3ceae66767667e8820f152011f8f8a1de`  
		Last Modified: Wed, 31 Mar 2021 22:12:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3d7ca742af0ce468e2012708013276fbd53bc83cbfbc6067bee7576dfc77fd`  
		Last Modified: Wed, 31 Mar 2021 22:48:32 GMT  
		Size: 3.3 MB (3300612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b24b2ef2e945c093a864cee98065bb150dcf6fb3f625d1b8a0e5747387e6113`  
		Last Modified: Wed, 31 Mar 2021 22:48:38 GMT  
		Size: 22.2 MB (22214370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e62aa81482401d0acc5589d9a8cb6d47c2eaa7eeb1c6e43750365771c0c8fb5`  
		Last Modified: Wed, 31 Mar 2021 22:48:28 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.17`

```console
$ docker pull telegraf@sha256:2ba1409c13b9828c0c2a3472fb62f14d8986275ffc9d4fa602914a2ceb5869a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.17` - linux; amd64

```console
$ docker pull telegraf@sha256:aeb3d24820f7fae0b7a13fcbfeed5fa0b0c0ef85c49d1e196bb691e1aabf36bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.6 MB (108639189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b78eeab63bfad65e92e345c688e27185b78fecb8ae22973f9423da5d016ae34`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:46:31 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:47:10 GMT
ENV TELEGRAF_VERSION=1.17.3
# Wed, 31 Mar 2021 22:47:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:47:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:16 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f1e8117dbb1c6a57603cb4f321a861a08105a81bcc6b01b0ec2b78c8523a5`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 7.8 MB (7832608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2faf66abec3dce9f54d6722ff592fce6dd4fb58a0d0b72282936c6598a3b3`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 10.0 MB (9997208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86207fc29d89bea4c2d79d45aa28f8dab5408d1b5646e6279d640cd8a2e857d5`  
		Last Modified: Wed, 31 Mar 2021 22:48:16 GMT  
		Size: 17.4 MB (17414524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e93c7da54121b4ac3d6cafa7058eeb1a43da87a6f99e3cea4038f2be1390a4`  
		Last Modified: Wed, 31 Mar 2021 22:48:11 GMT  
		Size: 2.9 KB (2909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e802bfc9d38fa3434e9124075184b3ae13d9341db17ce2747fc704d271d3148c`  
		Last Modified: Wed, 31 Mar 2021 22:48:55 GMT  
		Size: 23.0 MB (22958913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4fccc5df3152b22dbbef534ef88325b73d78274445d0ec9b398a570f383593`  
		Last Modified: Wed, 31 Mar 2021 22:48:50 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:4032c45661291e5ea299216abbde37079f8e20e6399a7304152940e5ad2cc4f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.0 MB (100003943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25120e31c568da2ed2c2a098c3fc64422a8677e4e6e9917812080da5d2b785d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:08 GMT
ADD file:bd48b3fec0eec547919c9e90c2055f1d879c78e4eb7d92598bf55c0f83c44836 in / 
# Tue, 30 Mar 2021 23:08:12 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:22:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:26:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:26:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:26:56 GMT
ENV TELEGRAF_VERSION=1.17.3
# Wed, 31 Mar 2021 22:27:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:27:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:27:04 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:27:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:27:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0bf0c5f21d801f530938b2464483aaad40947de697c29cedece44096ead1522c`  
		Last Modified: Tue, 30 Mar 2021 23:15:55 GMT  
		Size: 45.9 MB (45915428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8c35c4e8e932b85e0233ff1c20dcdd8bc13a0238128bcfcde181c0b04b037`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 7.1 MB (7123902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d88df2bbeddb232fbd4bf0ffd8efd62285f56f8eb6e2007c1a89ecfdc0f3ad`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 9.3 MB (9343731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a109f5c8c61633040e902da4a22004cdff8af3da4aec748c629a645ce3ae66a1`  
		Last Modified: Wed, 31 Mar 2021 22:27:50 GMT  
		Size: 16.2 MB (16159155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ab9c2159ba9b5e101028955dc796186a890dbc8bf5f65893e5ae7fea81840d`  
		Last Modified: Wed, 31 Mar 2021 22:27:39 GMT  
		Size: 2.9 KB (2910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3db5f4fae44ec3bd6465a080c7dd23b43096c529fc7e839aab22d6d3768c4c`  
		Last Modified: Wed, 31 Mar 2021 22:28:06 GMT  
		Size: 21.5 MB (21458631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20e2982d8ce5a1ace5424745386aa84d70bae681b3d238ff975e02cbcfb625d`  
		Last Modified: Wed, 31 Mar 2021 22:27:59 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ef252195e7af7b249b821f1aa75cf82400c360aa33bc74d602b2bbcf4c57ad58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105229176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c94a81c60855059ce0d52f7224e0cd9017b75f93a3343ea423463a4cefa67c87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:51:32 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 23:51:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 23:52:01 GMT
ENV TELEGRAF_VERSION=1.17.3
# Wed, 31 Mar 2021 23:52:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 23:52:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 23:52:09 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 23:52:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 23:52:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ccb2b90ef28919d82b935e6918055d100dffe73773e1b39b27c9389f0b1ef8`  
		Last Modified: Wed, 31 Mar 2021 23:53:17 GMT  
		Size: 17.3 MB (17269621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cbdac78f11712418529367b951f71d2d3634210107f88af2a92072b463ba6b`  
		Last Modified: Wed, 31 Mar 2021 23:53:09 GMT  
		Size: 2.9 KB (2896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618ae38d583fdc5dad41f64c2c582cdfaf7f81ac31940f7e73d72038caa9770f`  
		Last Modified: Wed, 31 Mar 2021 23:53:36 GMT  
		Size: 21.1 MB (21051746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45081dfdf226939f968b1ac129bfd8089ebfd61de803bb67bc597657d88199cb`  
		Last Modified: Wed, 31 Mar 2021 23:53:29 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.17-alpine`

```console
$ docker pull telegraf@sha256:e5cc20de430b19e5cf2531e8898e06211294064ac9d7a8a69d7e73ec3827f343
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.17-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:0c45633c35118bbe3cb87ffaa0c9dec06416ee4ff41b7a8d35ffbe2bf335ef69
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28921560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:108daa767dcdeb9e7c67fcef201a04fe0b608f3ad13b6063543e075e1bef514e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:46:56 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Wed, 31 Mar 2021 22:47:22 GMT
ENV TELEGRAF_VERSION=1.17.3
# Wed, 31 Mar 2021 22:47:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 31 Mar 2021 22:47:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:30 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38a141eb441d0521693dd710eb5a2a3ceae66767667e8820f152011f8f8a1de`  
		Last Modified: Wed, 31 Mar 2021 22:12:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3d7ca742af0ce468e2012708013276fbd53bc83cbfbc6067bee7576dfc77fd`  
		Last Modified: Wed, 31 Mar 2021 22:48:32 GMT  
		Size: 3.3 MB (3300612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d91d88132675be9b65b0d93277ac84b4b02ebaec36a901faf284f9926353be`  
		Last Modified: Wed, 31 Mar 2021 22:49:10 GMT  
		Size: 22.8 MB (22820900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5acc6235f76ad9d31e59cbea5a553dd404f4856299d178c28db76f1f66c3b3`  
		Last Modified: Wed, 31 Mar 2021 22:49:05 GMT  
		Size: 181.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.17.3`

```console
$ docker pull telegraf@sha256:2ba1409c13b9828c0c2a3472fb62f14d8986275ffc9d4fa602914a2ceb5869a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.17.3` - linux; amd64

```console
$ docker pull telegraf@sha256:aeb3d24820f7fae0b7a13fcbfeed5fa0b0c0ef85c49d1e196bb691e1aabf36bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.6 MB (108639189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b78eeab63bfad65e92e345c688e27185b78fecb8ae22973f9423da5d016ae34`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:46:31 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:47:10 GMT
ENV TELEGRAF_VERSION=1.17.3
# Wed, 31 Mar 2021 22:47:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:47:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:16 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f1e8117dbb1c6a57603cb4f321a861a08105a81bcc6b01b0ec2b78c8523a5`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 7.8 MB (7832608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2faf66abec3dce9f54d6722ff592fce6dd4fb58a0d0b72282936c6598a3b3`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 10.0 MB (9997208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86207fc29d89bea4c2d79d45aa28f8dab5408d1b5646e6279d640cd8a2e857d5`  
		Last Modified: Wed, 31 Mar 2021 22:48:16 GMT  
		Size: 17.4 MB (17414524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e93c7da54121b4ac3d6cafa7058eeb1a43da87a6f99e3cea4038f2be1390a4`  
		Last Modified: Wed, 31 Mar 2021 22:48:11 GMT  
		Size: 2.9 KB (2909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e802bfc9d38fa3434e9124075184b3ae13d9341db17ce2747fc704d271d3148c`  
		Last Modified: Wed, 31 Mar 2021 22:48:55 GMT  
		Size: 23.0 MB (22958913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4fccc5df3152b22dbbef534ef88325b73d78274445d0ec9b398a570f383593`  
		Last Modified: Wed, 31 Mar 2021 22:48:50 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:4032c45661291e5ea299216abbde37079f8e20e6399a7304152940e5ad2cc4f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.0 MB (100003943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25120e31c568da2ed2c2a098c3fc64422a8677e4e6e9917812080da5d2b785d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:08 GMT
ADD file:bd48b3fec0eec547919c9e90c2055f1d879c78e4eb7d92598bf55c0f83c44836 in / 
# Tue, 30 Mar 2021 23:08:12 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:22:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:26:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:26:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:26:56 GMT
ENV TELEGRAF_VERSION=1.17.3
# Wed, 31 Mar 2021 22:27:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:27:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:27:04 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:27:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:27:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0bf0c5f21d801f530938b2464483aaad40947de697c29cedece44096ead1522c`  
		Last Modified: Tue, 30 Mar 2021 23:15:55 GMT  
		Size: 45.9 MB (45915428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8c35c4e8e932b85e0233ff1c20dcdd8bc13a0238128bcfcde181c0b04b037`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 7.1 MB (7123902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d88df2bbeddb232fbd4bf0ffd8efd62285f56f8eb6e2007c1a89ecfdc0f3ad`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 9.3 MB (9343731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a109f5c8c61633040e902da4a22004cdff8af3da4aec748c629a645ce3ae66a1`  
		Last Modified: Wed, 31 Mar 2021 22:27:50 GMT  
		Size: 16.2 MB (16159155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ab9c2159ba9b5e101028955dc796186a890dbc8bf5f65893e5ae7fea81840d`  
		Last Modified: Wed, 31 Mar 2021 22:27:39 GMT  
		Size: 2.9 KB (2910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3db5f4fae44ec3bd6465a080c7dd23b43096c529fc7e839aab22d6d3768c4c`  
		Last Modified: Wed, 31 Mar 2021 22:28:06 GMT  
		Size: 21.5 MB (21458631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20e2982d8ce5a1ace5424745386aa84d70bae681b3d238ff975e02cbcfb625d`  
		Last Modified: Wed, 31 Mar 2021 22:27:59 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ef252195e7af7b249b821f1aa75cf82400c360aa33bc74d602b2bbcf4c57ad58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105229176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c94a81c60855059ce0d52f7224e0cd9017b75f93a3343ea423463a4cefa67c87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:51:32 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 23:51:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 23:52:01 GMT
ENV TELEGRAF_VERSION=1.17.3
# Wed, 31 Mar 2021 23:52:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 23:52:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 23:52:09 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 23:52:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 23:52:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ccb2b90ef28919d82b935e6918055d100dffe73773e1b39b27c9389f0b1ef8`  
		Last Modified: Wed, 31 Mar 2021 23:53:17 GMT  
		Size: 17.3 MB (17269621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cbdac78f11712418529367b951f71d2d3634210107f88af2a92072b463ba6b`  
		Last Modified: Wed, 31 Mar 2021 23:53:09 GMT  
		Size: 2.9 KB (2896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618ae38d583fdc5dad41f64c2c582cdfaf7f81ac31940f7e73d72038caa9770f`  
		Last Modified: Wed, 31 Mar 2021 23:53:36 GMT  
		Size: 21.1 MB (21051746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45081dfdf226939f968b1ac129bfd8089ebfd61de803bb67bc597657d88199cb`  
		Last Modified: Wed, 31 Mar 2021 23:53:29 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.17.3-alpine`

```console
$ docker pull telegraf@sha256:e5cc20de430b19e5cf2531e8898e06211294064ac9d7a8a69d7e73ec3827f343
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.17.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:0c45633c35118bbe3cb87ffaa0c9dec06416ee4ff41b7a8d35ffbe2bf335ef69
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28921560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:108daa767dcdeb9e7c67fcef201a04fe0b608f3ad13b6063543e075e1bef514e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:46:56 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Wed, 31 Mar 2021 22:47:22 GMT
ENV TELEGRAF_VERSION=1.17.3
# Wed, 31 Mar 2021 22:47:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 31 Mar 2021 22:47:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:30 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38a141eb441d0521693dd710eb5a2a3ceae66767667e8820f152011f8f8a1de`  
		Last Modified: Wed, 31 Mar 2021 22:12:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3d7ca742af0ce468e2012708013276fbd53bc83cbfbc6067bee7576dfc77fd`  
		Last Modified: Wed, 31 Mar 2021 22:48:32 GMT  
		Size: 3.3 MB (3300612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d91d88132675be9b65b0d93277ac84b4b02ebaec36a901faf284f9926353be`  
		Last Modified: Wed, 31 Mar 2021 22:49:10 GMT  
		Size: 22.8 MB (22820900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5acc6235f76ad9d31e59cbea5a553dd404f4856299d178c28db76f1f66c3b3`  
		Last Modified: Wed, 31 Mar 2021 22:49:05 GMT  
		Size: 181.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.18`

```console
$ docker pull telegraf@sha256:dc1205055a2d5f697a8e9b2fb17bbaf863d1e6b4c9919e9a9b92b0015ed6375e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.18` - linux; amd64

```console
$ docker pull telegraf@sha256:79d82b7fe8bdd243a0b4973f4a309a2507ea8212ed5a184fa07bb9109bf783e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111376378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c8543d57198b96c057599d9ef49df31bcde9c04d47679f9cc783240d67cc26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:46:31 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:47:36 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 22:47:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:47:40 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:41 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:41 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f1e8117dbb1c6a57603cb4f321a861a08105a81bcc6b01b0ec2b78c8523a5`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 7.8 MB (7832608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2faf66abec3dce9f54d6722ff592fce6dd4fb58a0d0b72282936c6598a3b3`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 10.0 MB (9997208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86207fc29d89bea4c2d79d45aa28f8dab5408d1b5646e6279d640cd8a2e857d5`  
		Last Modified: Wed, 31 Mar 2021 22:48:16 GMT  
		Size: 17.4 MB (17414524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e93c7da54121b4ac3d6cafa7058eeb1a43da87a6f99e3cea4038f2be1390a4`  
		Last Modified: Wed, 31 Mar 2021 22:48:11 GMT  
		Size: 2.9 KB (2909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d134f601eecb12eddb78ab2697eed9ca5318d2b239825f91c887dfbccc55e7f4`  
		Last Modified: Wed, 31 Mar 2021 22:49:26 GMT  
		Size: 25.7 MB (25696103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a57192cc13951fa7bb4e8420e970ddb6dc834082db60de2abc8be869b65cb03`  
		Last Modified: Wed, 31 Mar 2021 22:49:20 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:462f8196eda90ca6a23411655c8e57d912a6f2f729c3fdd5143cc31b0bd38486
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102315612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0c9a48fb0ef31b83b59fca66951f7c416979f9b9ef109163371f57543a7d19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:08 GMT
ADD file:bd48b3fec0eec547919c9e90c2055f1d879c78e4eb7d92598bf55c0f83c44836 in / 
# Tue, 30 Mar 2021 23:08:12 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:22:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:26:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:26:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:27:12 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 22:27:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:27:20 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:27:21 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:27:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:27:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0bf0c5f21d801f530938b2464483aaad40947de697c29cedece44096ead1522c`  
		Last Modified: Tue, 30 Mar 2021 23:15:55 GMT  
		Size: 45.9 MB (45915428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8c35c4e8e932b85e0233ff1c20dcdd8bc13a0238128bcfcde181c0b04b037`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 7.1 MB (7123902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d88df2bbeddb232fbd4bf0ffd8efd62285f56f8eb6e2007c1a89ecfdc0f3ad`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 9.3 MB (9343731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a109f5c8c61633040e902da4a22004cdff8af3da4aec748c629a645ce3ae66a1`  
		Last Modified: Wed, 31 Mar 2021 22:27:50 GMT  
		Size: 16.2 MB (16159155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ab9c2159ba9b5e101028955dc796186a890dbc8bf5f65893e5ae7fea81840d`  
		Last Modified: Wed, 31 Mar 2021 22:27:39 GMT  
		Size: 2.9 KB (2910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb40734448f3dc24bb11668cd23e00fb7c4aa30d45182526e716c8c19596099`  
		Last Modified: Wed, 31 Mar 2021 22:28:26 GMT  
		Size: 23.8 MB (23770303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e04e52c28276e26a588d2443589289d7172009cbf136a89d689479dbb98d071`  
		Last Modified: Wed, 31 Mar 2021 22:28:13 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:1a5b7024f29935bdec90cb2c89c440992b0046f20b5252d61c57615e07c4db75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.5 MB (107499137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:541bcc63db768011f1b05584cb490204585425aa5fbe86caa13b78d9e08c4f4a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:51:32 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 23:51:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 23:52:18 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 23:52:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 23:52:30 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 23:52:32 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 23:52:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 23:52:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ccb2b90ef28919d82b935e6918055d100dffe73773e1b39b27c9389f0b1ef8`  
		Last Modified: Wed, 31 Mar 2021 23:53:17 GMT  
		Size: 17.3 MB (17269621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cbdac78f11712418529367b951f71d2d3634210107f88af2a92072b463ba6b`  
		Last Modified: Wed, 31 Mar 2021 23:53:09 GMT  
		Size: 2.9 KB (2896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e643f0eee42e05f5fb23f0502c492dbaa0db4fb76f24af2af21ac1b14ca413`  
		Last Modified: Wed, 31 Mar 2021 23:53:56 GMT  
		Size: 23.3 MB (23321706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e6f9f8cd013e43adb97a48b71323fcd5a78e391eb95df0a3ab21ea2f4bc7bd`  
		Last Modified: Wed, 31 Mar 2021 23:53:46 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.18-alpine`

```console
$ docker pull telegraf@sha256:36b91f1582e5135cf7b364254c58f5b1089279c9aada634da80be47cc89a96df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.18-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7e38484d276e49516ca195d478859650659d0057d2fdfdd34a4c139167db8a1d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31650834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e24cbd9987bbf706e6ce8bdb7a9bfc02622bb77af5e2ebfccbfc500b83909a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:46:56 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Wed, 31 Mar 2021 22:47:44 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 22:47:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 31 Mar 2021 22:47:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:49 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:49 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38a141eb441d0521693dd710eb5a2a3ceae66767667e8820f152011f8f8a1de`  
		Last Modified: Wed, 31 Mar 2021 22:12:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3d7ca742af0ce468e2012708013276fbd53bc83cbfbc6067bee7576dfc77fd`  
		Last Modified: Wed, 31 Mar 2021 22:48:32 GMT  
		Size: 3.3 MB (3300612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3416fc49face30e14e2ca552ea8a524ab14963560a5ee9f61b4decba732d7868`  
		Last Modified: Wed, 31 Mar 2021 22:49:45 GMT  
		Size: 25.6 MB (25550173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322d29285336a8ea82c427137430dce78b0018e178ee228df76215f4e6536815`  
		Last Modified: Wed, 31 Mar 2021 22:49:39 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.18.0`

```console
$ docker pull telegraf@sha256:dc1205055a2d5f697a8e9b2fb17bbaf863d1e6b4c9919e9a9b92b0015ed6375e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.18.0` - linux; amd64

```console
$ docker pull telegraf@sha256:79d82b7fe8bdd243a0b4973f4a309a2507ea8212ed5a184fa07bb9109bf783e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111376378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c8543d57198b96c057599d9ef49df31bcde9c04d47679f9cc783240d67cc26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:46:31 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:47:36 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 22:47:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:47:40 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:41 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:41 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f1e8117dbb1c6a57603cb4f321a861a08105a81bcc6b01b0ec2b78c8523a5`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 7.8 MB (7832608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2faf66abec3dce9f54d6722ff592fce6dd4fb58a0d0b72282936c6598a3b3`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 10.0 MB (9997208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86207fc29d89bea4c2d79d45aa28f8dab5408d1b5646e6279d640cd8a2e857d5`  
		Last Modified: Wed, 31 Mar 2021 22:48:16 GMT  
		Size: 17.4 MB (17414524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e93c7da54121b4ac3d6cafa7058eeb1a43da87a6f99e3cea4038f2be1390a4`  
		Last Modified: Wed, 31 Mar 2021 22:48:11 GMT  
		Size: 2.9 KB (2909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d134f601eecb12eddb78ab2697eed9ca5318d2b239825f91c887dfbccc55e7f4`  
		Last Modified: Wed, 31 Mar 2021 22:49:26 GMT  
		Size: 25.7 MB (25696103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a57192cc13951fa7bb4e8420e970ddb6dc834082db60de2abc8be869b65cb03`  
		Last Modified: Wed, 31 Mar 2021 22:49:20 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18.0` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:462f8196eda90ca6a23411655c8e57d912a6f2f729c3fdd5143cc31b0bd38486
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102315612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0c9a48fb0ef31b83b59fca66951f7c416979f9b9ef109163371f57543a7d19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:08 GMT
ADD file:bd48b3fec0eec547919c9e90c2055f1d879c78e4eb7d92598bf55c0f83c44836 in / 
# Tue, 30 Mar 2021 23:08:12 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:22:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:26:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:26:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:27:12 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 22:27:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:27:20 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:27:21 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:27:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:27:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0bf0c5f21d801f530938b2464483aaad40947de697c29cedece44096ead1522c`  
		Last Modified: Tue, 30 Mar 2021 23:15:55 GMT  
		Size: 45.9 MB (45915428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8c35c4e8e932b85e0233ff1c20dcdd8bc13a0238128bcfcde181c0b04b037`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 7.1 MB (7123902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d88df2bbeddb232fbd4bf0ffd8efd62285f56f8eb6e2007c1a89ecfdc0f3ad`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 9.3 MB (9343731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a109f5c8c61633040e902da4a22004cdff8af3da4aec748c629a645ce3ae66a1`  
		Last Modified: Wed, 31 Mar 2021 22:27:50 GMT  
		Size: 16.2 MB (16159155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ab9c2159ba9b5e101028955dc796186a890dbc8bf5f65893e5ae7fea81840d`  
		Last Modified: Wed, 31 Mar 2021 22:27:39 GMT  
		Size: 2.9 KB (2910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb40734448f3dc24bb11668cd23e00fb7c4aa30d45182526e716c8c19596099`  
		Last Modified: Wed, 31 Mar 2021 22:28:26 GMT  
		Size: 23.8 MB (23770303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e04e52c28276e26a588d2443589289d7172009cbf136a89d689479dbb98d071`  
		Last Modified: Wed, 31 Mar 2021 22:28:13 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18.0` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:1a5b7024f29935bdec90cb2c89c440992b0046f20b5252d61c57615e07c4db75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.5 MB (107499137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:541bcc63db768011f1b05584cb490204585425aa5fbe86caa13b78d9e08c4f4a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:51:32 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 23:51:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 23:52:18 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 23:52:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 23:52:30 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 23:52:32 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 23:52:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 23:52:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ccb2b90ef28919d82b935e6918055d100dffe73773e1b39b27c9389f0b1ef8`  
		Last Modified: Wed, 31 Mar 2021 23:53:17 GMT  
		Size: 17.3 MB (17269621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cbdac78f11712418529367b951f71d2d3634210107f88af2a92072b463ba6b`  
		Last Modified: Wed, 31 Mar 2021 23:53:09 GMT  
		Size: 2.9 KB (2896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e643f0eee42e05f5fb23f0502c492dbaa0db4fb76f24af2af21ac1b14ca413`  
		Last Modified: Wed, 31 Mar 2021 23:53:56 GMT  
		Size: 23.3 MB (23321706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e6f9f8cd013e43adb97a48b71323fcd5a78e391eb95df0a3ab21ea2f4bc7bd`  
		Last Modified: Wed, 31 Mar 2021 23:53:46 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.18.0-alpine`

```console
$ docker pull telegraf@sha256:36b91f1582e5135cf7b364254c58f5b1089279c9aada634da80be47cc89a96df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.18.0-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7e38484d276e49516ca195d478859650659d0057d2fdfdd34a4c139167db8a1d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31650834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e24cbd9987bbf706e6ce8bdb7a9bfc02622bb77af5e2ebfccbfc500b83909a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:46:56 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Wed, 31 Mar 2021 22:47:44 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 22:47:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 31 Mar 2021 22:47:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:49 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:49 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38a141eb441d0521693dd710eb5a2a3ceae66767667e8820f152011f8f8a1de`  
		Last Modified: Wed, 31 Mar 2021 22:12:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3d7ca742af0ce468e2012708013276fbd53bc83cbfbc6067bee7576dfc77fd`  
		Last Modified: Wed, 31 Mar 2021 22:48:32 GMT  
		Size: 3.3 MB (3300612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3416fc49face30e14e2ca552ea8a524ab14963560a5ee9f61b4decba732d7868`  
		Last Modified: Wed, 31 Mar 2021 22:49:45 GMT  
		Size: 25.6 MB (25550173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322d29285336a8ea82c427137430dce78b0018e178ee228df76215f4e6536815`  
		Last Modified: Wed, 31 Mar 2021 22:49:39 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:36b91f1582e5135cf7b364254c58f5b1089279c9aada634da80be47cc89a96df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7e38484d276e49516ca195d478859650659d0057d2fdfdd34a4c139167db8a1d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31650834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e24cbd9987bbf706e6ce8bdb7a9bfc02622bb77af5e2ebfccbfc500b83909a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:46:56 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Wed, 31 Mar 2021 22:47:44 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 22:47:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 31 Mar 2021 22:47:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:49 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:49 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38a141eb441d0521693dd710eb5a2a3ceae66767667e8820f152011f8f8a1de`  
		Last Modified: Wed, 31 Mar 2021 22:12:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3d7ca742af0ce468e2012708013276fbd53bc83cbfbc6067bee7576dfc77fd`  
		Last Modified: Wed, 31 Mar 2021 22:48:32 GMT  
		Size: 3.3 MB (3300612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3416fc49face30e14e2ca552ea8a524ab14963560a5ee9f61b4decba732d7868`  
		Last Modified: Wed, 31 Mar 2021 22:49:45 GMT  
		Size: 25.6 MB (25550173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322d29285336a8ea82c427137430dce78b0018e178ee228df76215f4e6536815`  
		Last Modified: Wed, 31 Mar 2021 22:49:39 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:dc1205055a2d5f697a8e9b2fb17bbaf863d1e6b4c9919e9a9b92b0015ed6375e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:79d82b7fe8bdd243a0b4973f4a309a2507ea8212ed5a184fa07bb9109bf783e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111376378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c8543d57198b96c057599d9ef49df31bcde9c04d47679f9cc783240d67cc26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:46:31 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:47:36 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 22:47:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:47:40 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:47:41 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:47:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:47:41 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f1e8117dbb1c6a57603cb4f321a861a08105a81bcc6b01b0ec2b78c8523a5`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 7.8 MB (7832608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2faf66abec3dce9f54d6722ff592fce6dd4fb58a0d0b72282936c6598a3b3`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 10.0 MB (9997208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86207fc29d89bea4c2d79d45aa28f8dab5408d1b5646e6279d640cd8a2e857d5`  
		Last Modified: Wed, 31 Mar 2021 22:48:16 GMT  
		Size: 17.4 MB (17414524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e93c7da54121b4ac3d6cafa7058eeb1a43da87a6f99e3cea4038f2be1390a4`  
		Last Modified: Wed, 31 Mar 2021 22:48:11 GMT  
		Size: 2.9 KB (2909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d134f601eecb12eddb78ab2697eed9ca5318d2b239825f91c887dfbccc55e7f4`  
		Last Modified: Wed, 31 Mar 2021 22:49:26 GMT  
		Size: 25.7 MB (25696103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a57192cc13951fa7bb4e8420e970ddb6dc834082db60de2abc8be869b65cb03`  
		Last Modified: Wed, 31 Mar 2021 22:49:20 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:462f8196eda90ca6a23411655c8e57d912a6f2f729c3fdd5143cc31b0bd38486
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102315612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0c9a48fb0ef31b83b59fca66951f7c416979f9b9ef109163371f57543a7d19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:08 GMT
ADD file:bd48b3fec0eec547919c9e90c2055f1d879c78e4eb7d92598bf55c0f83c44836 in / 
# Tue, 30 Mar 2021 23:08:12 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:22:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:26:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 22:26:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:27:12 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 22:27:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 22:27:20 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 22:27:21 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 22:27:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:27:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0bf0c5f21d801f530938b2464483aaad40947de697c29cedece44096ead1522c`  
		Last Modified: Tue, 30 Mar 2021 23:15:55 GMT  
		Size: 45.9 MB (45915428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8c35c4e8e932b85e0233ff1c20dcdd8bc13a0238128bcfcde181c0b04b037`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 7.1 MB (7123902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d88df2bbeddb232fbd4bf0ffd8efd62285f56f8eb6e2007c1a89ecfdc0f3ad`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 9.3 MB (9343731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a109f5c8c61633040e902da4a22004cdff8af3da4aec748c629a645ce3ae66a1`  
		Last Modified: Wed, 31 Mar 2021 22:27:50 GMT  
		Size: 16.2 MB (16159155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ab9c2159ba9b5e101028955dc796186a890dbc8bf5f65893e5ae7fea81840d`  
		Last Modified: Wed, 31 Mar 2021 22:27:39 GMT  
		Size: 2.9 KB (2910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb40734448f3dc24bb11668cd23e00fb7c4aa30d45182526e716c8c19596099`  
		Last Modified: Wed, 31 Mar 2021 22:28:26 GMT  
		Size: 23.8 MB (23770303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e04e52c28276e26a588d2443589289d7172009cbf136a89d689479dbb98d071`  
		Last Modified: Wed, 31 Mar 2021 22:28:13 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:1a5b7024f29935bdec90cb2c89c440992b0046f20b5252d61c57615e07c4db75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.5 MB (107499137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:541bcc63db768011f1b05584cb490204585425aa5fbe86caa13b78d9e08c4f4a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:51:32 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 23:51:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 23:52:18 GMT
ENV TELEGRAF_VERSION=1.18.0
# Wed, 31 Mar 2021 23:52:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 31 Mar 2021 23:52:30 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 31 Mar 2021 23:52:32 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 31 Mar 2021 23:52:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 23:52:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ccb2b90ef28919d82b935e6918055d100dffe73773e1b39b27c9389f0b1ef8`  
		Last Modified: Wed, 31 Mar 2021 23:53:17 GMT  
		Size: 17.3 MB (17269621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cbdac78f11712418529367b951f71d2d3634210107f88af2a92072b463ba6b`  
		Last Modified: Wed, 31 Mar 2021 23:53:09 GMT  
		Size: 2.9 KB (2896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e643f0eee42e05f5fb23f0502c492dbaa0db4fb76f24af2af21ac1b14ca413`  
		Last Modified: Wed, 31 Mar 2021 23:53:56 GMT  
		Size: 23.3 MB (23321706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e6f9f8cd013e43adb97a48b71323fcd5a78e391eb95df0a3ab21ea2f4bc7bd`  
		Last Modified: Wed, 31 Mar 2021 23:53:46 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
