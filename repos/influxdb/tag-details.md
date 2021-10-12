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
-	[`influxdb:1.9.4-data`](#influxdb194-data)
-	[`influxdb:1.9.4-data-alpine`](#influxdb194-data-alpine)
-	[`influxdb:1.9.4-meta`](#influxdb194-meta)
-	[`influxdb:1.9.4-meta-alpine`](#influxdb194-meta-alpine)
-	[`influxdb:2.0`](#influxdb20)
-	[`influxdb:2.0-alpine`](#influxdb20-alpine)
-	[`influxdb:2.0.9`](#influxdb209)
-	[`influxdb:2.0.9-alpine`](#influxdb209-alpine)
-	[`influxdb:alpine`](#influxdbalpine)
-	[`influxdb:data`](#influxdbdata)
-	[`influxdb:data-alpine`](#influxdbdata-alpine)
-	[`influxdb:latest`](#influxdblatest)
-	[`influxdb:meta`](#influxdbmeta)
-	[`influxdb:meta-alpine`](#influxdbmeta-alpine)

## `influxdb:1.7`

```console
$ docker pull influxdb@sha256:84b332cff4646d5c62e652efe63bcb0cc052e1064677554dbe471004f5eb468e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7` - linux; amd64

```console
$ docker pull influxdb@sha256:c5dba58e81b39093c1db5f9b955bb914d9e14c5acbe3dc5aea855866a70a2fc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122309611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed08bdb13e48afc4e0a0c95708f907999c718b522e1a7a608179f935c3503a58`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 29 Sep 2021 06:26:01 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 29 Sep 2021 06:26:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 29 Sep 2021 06:26:08 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 29 Sep 2021 06:26:09 GMT
EXPOSE 8086
# Wed, 29 Sep 2021 06:26:09 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Sep 2021 06:26:09 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 29 Sep 2021 06:26:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 29 Sep 2021 06:26:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Sep 2021 06:26:10 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2697d454d63fe1343a74cffe6c6a50e98e4fdbd77d748f9b9e99f15dad5f7a5d`  
		Last Modified: Wed, 29 Sep 2021 06:29:06 GMT  
		Size: 61.3 MB (61285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a885c579a71e29dcee9b19208bbdd892b12d7922f81ad7b1a398f6616d2d0154`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a06848cd68b336aaf9695490cd0fec19757a4a4888221627dcc55498717b1a`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417159661f380a08f716c03faeefefe8d61b6f9e3c50cf12016834c3c6c3379c`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:fc8b09ab0e41548d89d092fbdc83cf68cee741dee5778a50d176fb97aad805db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113469960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01b657964ffaa90402c69c9c77bdf1c1f12095565250d2fc437a112892e043b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 15:30:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 02 Oct 2021 15:30:30 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 02 Oct 2021 15:30:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 02 Oct 2021 15:30:46 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 02 Oct 2021 15:30:46 GMT
EXPOSE 8086
# Sat, 02 Oct 2021 15:30:46 GMT
VOLUME [/var/lib/influxdb]
# Sat, 02 Oct 2021 15:30:47 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 02 Oct 2021 15:30:48 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 02 Oct 2021 15:30:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Oct 2021 15:30:49 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b971858d80d06fe204d46d63285d784d8a83132df39eaae9a0c7b9dff178cd`  
		Last Modified: Sat, 02 Oct 2021 15:31:48 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f719262239b6cd02fb2bb4afa6a42fa26d4b24323fa17df1874231cad17e1b`  
		Last Modified: Sat, 02 Oct 2021 15:32:18 GMT  
		Size: 57.5 MB (57468927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adfe4701ef4ac089c34e7d10424c1c83b22ea31e6748ae7ad509ce3a96867b0`  
		Last Modified: Sat, 02 Oct 2021 15:31:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc1740c50955f47531c7c171ccf7cf7b4fc310eddf111a87e37174c11c33645`  
		Last Modified: Sat, 02 Oct 2021 15:31:48 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a420460c31ef96d15c6427276d2ef7ef0c8f646c0aeaabdc402d6d68f893a2fc`  
		Last Modified: Sat, 02 Oct 2021 15:31:48 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b68d9ec7f930342c0c3279cf0f1954fce36f4ca9995533820c5ea295d0860f52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114698759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1174198067fbe3b8613059e324b21c2880e1c6847b1cbb9ff3a23637593f37cb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 21:58:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 28 Sep 2021 21:58:03 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 28 Sep 2021 21:58:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 28 Sep 2021 21:58:09 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 28 Sep 2021 21:58:10 GMT
EXPOSE 8086
# Tue, 28 Sep 2021 21:58:10 GMT
VOLUME [/var/lib/influxdb]
# Tue, 28 Sep 2021 21:58:10 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 28 Sep 2021 21:58:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 28 Sep 2021 21:58:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Sep 2021 21:58:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df36ff09e1ede2cc321c3bc8e3bee61b25e75e77e64c51ad208867c48aa86e1`  
		Last Modified: Tue, 28 Sep 2021 21:59:20 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6831297732af2b9ffbb686ece5e0bc1bc30429d227278aabb18e1877a92dffde`  
		Last Modified: Tue, 28 Sep 2021 21:59:28 GMT  
		Size: 57.2 MB (57204315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58194e47f307000416139e21dd51a0d5c3a63c9a807c93e71ab6c6ea20d33206`  
		Last Modified: Tue, 28 Sep 2021 21:59:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d214d0cc85fd175aff59c96a62e5fded3b82ff5de21f0dc44619ece4e511582d`  
		Last Modified: Tue, 28 Sep 2021 21:59:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dae5b8f836d3627871250380642d631290ec7821f0b32821e30551be7757564`  
		Last Modified: Tue, 28 Sep 2021 21:59:20 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-alpine`

```console
$ docker pull influxdb@sha256:a3a735f1224bdaaacd0e7b3598b5d851a979fba83325320f707044d0ee6597be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f1cf3a101fabe43577eb3f841a744536618ea60c7b272d4dcb467f0bee1acb9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65315119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b16ffcff0af35d293d775f5e62350e1629004c6925b08718ffaa81472c66b3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Sep 2021 21:20:08 GMT
ENV INFLUXDB_VERSION=1.7.11
# Thu, 16 Sep 2021 21:20:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Sep 2021 21:20:26 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 16 Sep 2021 21:20:26 GMT
EXPOSE 8086
# Thu, 16 Sep 2021 21:20:26 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Sep 2021 21:20:27 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 16 Sep 2021 21:20:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Sep 2021 21:20:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Sep 2021 21:20:27 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7217af65c006384fcb34254a4a41da62f941eba652806e8ac68bcdfc9a39ee8d`  
		Last Modified: Thu, 16 Sep 2021 21:24:09 GMT  
		Size: 61.0 MB (61034604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1741713396b4f9a17a66ea91d0a143835a343686141da93f71c5ccd0b3d47b3c`  
		Last Modified: Thu, 16 Sep 2021 21:24:01 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b15d4407eb64e550ff5ea7d6fb522ed30a95b0de59812dce2b7a2d3d3585172`  
		Last Modified: Thu, 16 Sep 2021 21:24:01 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874fe04be8588a5a67c2c706fecb63324a081c8630ff2c4a91332fbf492a0099`  
		Last Modified: Thu, 16 Sep 2021 21:24:01 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data`

```console
$ docker pull influxdb@sha256:fa2c68b095ec1fbc4bd50a1ee9a82225d2f42093c6106397fda980f481824557
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:32fd0d105a2028a4f343a94ee95bc3065b8fe3ed25dd36f9485f133829d337b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148973561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:633bce8005c4cbe42b99e2859cf92b51ea8854041b27c4185513c5d8cf407bd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 29 Sep 2021 06:26:17 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 29 Sep 2021 06:26:27 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 29 Sep 2021 06:26:28 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 29 Sep 2021 06:26:28 GMT
EXPOSE 8086
# Wed, 29 Sep 2021 06:26:28 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Sep 2021 06:26:28 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 29 Sep 2021 06:26:28 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 29 Sep 2021 06:26:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Sep 2021 06:26:29 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf03cc7f4aa43a12ccdd748f7ece955f6628fcce22c72e86efb5d6d6285e0cd7`  
		Last Modified: Wed, 29 Sep 2021 06:29:28 GMT  
		Size: 87.9 MB (87948986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c79f2d9374dde99a3609ec16cf0f63fd4a4146cbfadc1a9f241de3e49cb1bf`  
		Last Modified: Wed, 29 Sep 2021 06:29:17 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc8d698d8a7e26afd319054795a8e68c2282fff2e303fb8ed57b130048aeb3b`  
		Last Modified: Wed, 29 Sep 2021 06:29:16 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd36178a6c8fe1d7e895e043df3f042119ca9a6f3652c3e1318015547f291648`  
		Last Modified: Wed, 29 Sep 2021 06:29:16 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data-alpine`

```console
$ docker pull influxdb@sha256:9afff27c8ad26a7d052f24e46562e4ad3a38c03b95fb1883c30dcc6b687f7455
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:6b5c1ad7cf6576ad51b9343a8f141ff5e4b6e28d3a5dac56d3038fa8885984e8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91921909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dbd1cc363975d43093319b9f49a41d15e6fdc04a75d8c91866cb4da41600007`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Sep 2021 21:20:34 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Thu, 16 Sep 2021 21:20:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Sep 2021 21:20:52 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Sep 2021 21:20:52 GMT
EXPOSE 8086
# Thu, 16 Sep 2021 21:20:52 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Sep 2021 21:20:52 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Sep 2021 21:20:53 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Sep 2021 21:20:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Sep 2021 21:20:53 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8730f15882b099e0e25e1505c55e5a52a02021e481bd930c7ce3c8edfe7003ea`  
		Last Modified: Thu, 16 Sep 2021 21:24:31 GMT  
		Size: 87.6 MB (87641336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8d443c8c6f55ad16ea25b42f853e309f2a350935ceea7c47dd1fe7047a01da`  
		Last Modified: Thu, 16 Sep 2021 21:24:20 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809c32c8a5350037bcca9b4e55877980f8f13ada36dbd53ae583b0e7de46abdb`  
		Last Modified: Thu, 16 Sep 2021 21:24:20 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f744e1c9bec438d7ab0a6e84b823960d5b86a30f530a11c4b04ce79e5ade43`  
		Last Modified: Thu, 16 Sep 2021 21:24:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta`

```console
$ docker pull influxdb@sha256:81e0b03e428b268d441f483bd648c9c6733c401b951e544a56683588820492fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:63a685b6a42ffd23c012f1198f90a634e9b2b2a29d294b7eb3cd47f2668d890c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84156922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d970d8dcdddd5de22e8ce608a118c3783debd78151ca2e94221a864e6b86471`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 29 Sep 2021 06:26:17 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 29 Sep 2021 06:26:39 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 29 Sep 2021 06:26:39 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 29 Sep 2021 06:26:40 GMT
EXPOSE 8091
# Wed, 29 Sep 2021 06:26:40 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Sep 2021 06:26:40 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 29 Sep 2021 06:26:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Sep 2021 06:26:40 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7494a6304bb1de16f217c389c108943b00965888cd2ddfd1eeeedd750f4440ba`  
		Last Modified: Wed, 29 Sep 2021 06:29:42 GMT  
		Size: 23.1 MB (23133552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eee0b8e4361bde1b3c5bdd815784ce925cdd2dd77db630f0d0fe6182c10e98`  
		Last Modified: Wed, 29 Sep 2021 06:29:38 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fae8ef72f9ca0f12e5baef24cb499773c7aaa1869d7a4504d2119ac7fecba57`  
		Last Modified: Wed, 29 Sep 2021 06:29:39 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta-alpine`

```console
$ docker pull influxdb@sha256:153c2f5e4506ce7327333805c6231cfabfcc3dfb1eeb8a091afeb2d9c9a4a944
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:67f3a0d1892e679633e4ad07e9fb2ef23205e510f3a8a62f7df52b0933e1a528
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27282868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:856f604842f4847ce4ea178bc068bf16df596b7eb298a8a23f8cea6c3e89cd42`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Sep 2021 21:20:34 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Thu, 16 Sep 2021 21:21:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Sep 2021 21:21:09 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Sep 2021 21:21:09 GMT
EXPOSE 8091
# Thu, 16 Sep 2021 21:21:10 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Sep 2021 21:21:10 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Sep 2021 21:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Sep 2021 21:21:10 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02a3bf95180b5791ca6424c745df8bd0f6d62f2347cd5e3ebed1d04510c1e36`  
		Last Modified: Thu, 16 Sep 2021 21:24:46 GMT  
		Size: 23.0 MB (23003501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd4a806b67a586afebab99e71b90abfd14982c1583e7d5d2acbf16a1a7f5ef9`  
		Last Modified: Thu, 16 Sep 2021 21:24:43 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545d1436c7f8f742e92125ba026915ae3baa87b871b34650e9492aa122cab75a`  
		Last Modified: Thu, 16 Sep 2021 21:24:43 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11`

```console
$ docker pull influxdb@sha256:84b332cff4646d5c62e652efe63bcb0cc052e1064677554dbe471004f5eb468e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7.11` - linux; amd64

```console
$ docker pull influxdb@sha256:c5dba58e81b39093c1db5f9b955bb914d9e14c5acbe3dc5aea855866a70a2fc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122309611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed08bdb13e48afc4e0a0c95708f907999c718b522e1a7a608179f935c3503a58`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 29 Sep 2021 06:26:01 GMT
ENV INFLUXDB_VERSION=1.7.11
# Wed, 29 Sep 2021 06:26:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Wed, 29 Sep 2021 06:26:08 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Wed, 29 Sep 2021 06:26:09 GMT
EXPOSE 8086
# Wed, 29 Sep 2021 06:26:09 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Sep 2021 06:26:09 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Wed, 29 Sep 2021 06:26:09 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 29 Sep 2021 06:26:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Sep 2021 06:26:10 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2697d454d63fe1343a74cffe6c6a50e98e4fdbd77d748f9b9e99f15dad5f7a5d`  
		Last Modified: Wed, 29 Sep 2021 06:29:06 GMT  
		Size: 61.3 MB (61285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a885c579a71e29dcee9b19208bbdd892b12d7922f81ad7b1a398f6616d2d0154`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a06848cd68b336aaf9695490cd0fec19757a4a4888221627dcc55498717b1a`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417159661f380a08f716c03faeefefe8d61b6f9e3c50cf12016834c3c6c3379c`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:fc8b09ab0e41548d89d092fbdc83cf68cee741dee5778a50d176fb97aad805db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113469960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01b657964ffaa90402c69c9c77bdf1c1f12095565250d2fc437a112892e043b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 15:30:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 02 Oct 2021 15:30:30 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 02 Oct 2021 15:30:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 02 Oct 2021 15:30:46 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 02 Oct 2021 15:30:46 GMT
EXPOSE 8086
# Sat, 02 Oct 2021 15:30:46 GMT
VOLUME [/var/lib/influxdb]
# Sat, 02 Oct 2021 15:30:47 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 02 Oct 2021 15:30:48 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 02 Oct 2021 15:30:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Oct 2021 15:30:49 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b971858d80d06fe204d46d63285d784d8a83132df39eaae9a0c7b9dff178cd`  
		Last Modified: Sat, 02 Oct 2021 15:31:48 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f719262239b6cd02fb2bb4afa6a42fa26d4b24323fa17df1874231cad17e1b`  
		Last Modified: Sat, 02 Oct 2021 15:32:18 GMT  
		Size: 57.5 MB (57468927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adfe4701ef4ac089c34e7d10424c1c83b22ea31e6748ae7ad509ce3a96867b0`  
		Last Modified: Sat, 02 Oct 2021 15:31:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc1740c50955f47531c7c171ccf7cf7b4fc310eddf111a87e37174c11c33645`  
		Last Modified: Sat, 02 Oct 2021 15:31:48 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a420460c31ef96d15c6427276d2ef7ef0c8f646c0aeaabdc402d6d68f893a2fc`  
		Last Modified: Sat, 02 Oct 2021 15:31:48 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b68d9ec7f930342c0c3279cf0f1954fce36f4ca9995533820c5ea295d0860f52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114698759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1174198067fbe3b8613059e324b21c2880e1c6847b1cbb9ff3a23637593f37cb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 21:58:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 28 Sep 2021 21:58:03 GMT
ENV INFLUXDB_VERSION=1.7.11
# Tue, 28 Sep 2021 21:58:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 28 Sep 2021 21:58:09 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 28 Sep 2021 21:58:10 GMT
EXPOSE 8086
# Tue, 28 Sep 2021 21:58:10 GMT
VOLUME [/var/lib/influxdb]
# Tue, 28 Sep 2021 21:58:10 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 28 Sep 2021 21:58:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 28 Sep 2021 21:58:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Sep 2021 21:58:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df36ff09e1ede2cc321c3bc8e3bee61b25e75e77e64c51ad208867c48aa86e1`  
		Last Modified: Tue, 28 Sep 2021 21:59:20 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6831297732af2b9ffbb686ece5e0bc1bc30429d227278aabb18e1877a92dffde`  
		Last Modified: Tue, 28 Sep 2021 21:59:28 GMT  
		Size: 57.2 MB (57204315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58194e47f307000416139e21dd51a0d5c3a63c9a807c93e71ab6c6ea20d33206`  
		Last Modified: Tue, 28 Sep 2021 21:59:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d214d0cc85fd175aff59c96a62e5fded3b82ff5de21f0dc44619ece4e511582d`  
		Last Modified: Tue, 28 Sep 2021 21:59:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dae5b8f836d3627871250380642d631290ec7821f0b32821e30551be7757564`  
		Last Modified: Tue, 28 Sep 2021 21:59:20 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-alpine`

```console
$ docker pull influxdb@sha256:a3a735f1224bdaaacd0e7b3598b5d851a979fba83325320f707044d0ee6597be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f1cf3a101fabe43577eb3f841a744536618ea60c7b272d4dcb467f0bee1acb9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65315119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b16ffcff0af35d293d775f5e62350e1629004c6925b08718ffaa81472c66b3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Sep 2021 21:20:08 GMT
ENV INFLUXDB_VERSION=1.7.11
# Thu, 16 Sep 2021 21:20:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Sep 2021 21:20:26 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Thu, 16 Sep 2021 21:20:26 GMT
EXPOSE 8086
# Thu, 16 Sep 2021 21:20:26 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Sep 2021 21:20:27 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Thu, 16 Sep 2021 21:20:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Sep 2021 21:20:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Sep 2021 21:20:27 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7217af65c006384fcb34254a4a41da62f941eba652806e8ac68bcdfc9a39ee8d`  
		Last Modified: Thu, 16 Sep 2021 21:24:09 GMT  
		Size: 61.0 MB (61034604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1741713396b4f9a17a66ea91d0a143835a343686141da93f71c5ccd0b3d47b3c`  
		Last Modified: Thu, 16 Sep 2021 21:24:01 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b15d4407eb64e550ff5ea7d6fb522ed30a95b0de59812dce2b7a2d3d3585172`  
		Last Modified: Thu, 16 Sep 2021 21:24:01 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874fe04be8588a5a67c2c706fecb63324a081c8630ff2c4a91332fbf492a0099`  
		Last Modified: Thu, 16 Sep 2021 21:24:01 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data`

```console
$ docker pull influxdb@sha256:fa2c68b095ec1fbc4bd50a1ee9a82225d2f42093c6106397fda980f481824557
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:32fd0d105a2028a4f343a94ee95bc3065b8fe3ed25dd36f9485f133829d337b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (148973561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:633bce8005c4cbe42b99e2859cf92b51ea8854041b27c4185513c5d8cf407bd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 29 Sep 2021 06:26:17 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 29 Sep 2021 06:26:27 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 29 Sep 2021 06:26:28 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 29 Sep 2021 06:26:28 GMT
EXPOSE 8086
# Wed, 29 Sep 2021 06:26:28 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Sep 2021 06:26:28 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 29 Sep 2021 06:26:28 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 29 Sep 2021 06:26:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Sep 2021 06:26:29 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf03cc7f4aa43a12ccdd748f7ece955f6628fcce22c72e86efb5d6d6285e0cd7`  
		Last Modified: Wed, 29 Sep 2021 06:29:28 GMT  
		Size: 87.9 MB (87948986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c79f2d9374dde99a3609ec16cf0f63fd4a4146cbfadc1a9f241de3e49cb1bf`  
		Last Modified: Wed, 29 Sep 2021 06:29:17 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc8d698d8a7e26afd319054795a8e68c2282fff2e303fb8ed57b130048aeb3b`  
		Last Modified: Wed, 29 Sep 2021 06:29:16 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd36178a6c8fe1d7e895e043df3f042119ca9a6f3652c3e1318015547f291648`  
		Last Modified: Wed, 29 Sep 2021 06:29:16 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data-alpine`

```console
$ docker pull influxdb@sha256:9afff27c8ad26a7d052f24e46562e4ad3a38c03b95fb1883c30dcc6b687f7455
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:6b5c1ad7cf6576ad51b9343a8f141ff5e4b6e28d3a5dac56d3038fa8885984e8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91921909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dbd1cc363975d43093319b9f49a41d15e6fdc04a75d8c91866cb4da41600007`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Sep 2021 21:20:34 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Thu, 16 Sep 2021 21:20:51 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Sep 2021 21:20:52 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Sep 2021 21:20:52 GMT
EXPOSE 8086
# Thu, 16 Sep 2021 21:20:52 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Sep 2021 21:20:52 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Sep 2021 21:20:53 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Sep 2021 21:20:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Sep 2021 21:20:53 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8730f15882b099e0e25e1505c55e5a52a02021e481bd930c7ce3c8edfe7003ea`  
		Last Modified: Thu, 16 Sep 2021 21:24:31 GMT  
		Size: 87.6 MB (87641336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8d443c8c6f55ad16ea25b42f853e309f2a350935ceea7c47dd1fe7047a01da`  
		Last Modified: Thu, 16 Sep 2021 21:24:20 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809c32c8a5350037bcca9b4e55877980f8f13ada36dbd53ae583b0e7de46abdb`  
		Last Modified: Thu, 16 Sep 2021 21:24:20 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f744e1c9bec438d7ab0a6e84b823960d5b86a30f530a11c4b04ce79e5ade43`  
		Last Modified: Thu, 16 Sep 2021 21:24:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta`

```console
$ docker pull influxdb@sha256:81e0b03e428b268d441f483bd648c9c6733c401b951e544a56683588820492fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:63a685b6a42ffd23c012f1198f90a634e9b2b2a29d294b7eb3cd47f2668d890c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84156922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d970d8dcdddd5de22e8ce608a118c3783debd78151ca2e94221a864e6b86471`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 29 Sep 2021 06:26:17 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Wed, 29 Sep 2021 06:26:39 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 29 Sep 2021 06:26:39 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 29 Sep 2021 06:26:40 GMT
EXPOSE 8091
# Wed, 29 Sep 2021 06:26:40 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Sep 2021 06:26:40 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 29 Sep 2021 06:26:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Sep 2021 06:26:40 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7494a6304bb1de16f217c389c108943b00965888cd2ddfd1eeeedd750f4440ba`  
		Last Modified: Wed, 29 Sep 2021 06:29:42 GMT  
		Size: 23.1 MB (23133552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eee0b8e4361bde1b3c5bdd815784ce925cdd2dd77db630f0d0fe6182c10e98`  
		Last Modified: Wed, 29 Sep 2021 06:29:38 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fae8ef72f9ca0f12e5baef24cb499773c7aaa1869d7a4504d2119ac7fecba57`  
		Last Modified: Wed, 29 Sep 2021 06:29:39 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta-alpine`

```console
$ docker pull influxdb@sha256:153c2f5e4506ce7327333805c6231cfabfcc3dfb1eeb8a091afeb2d9c9a4a944
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:67f3a0d1892e679633e4ad07e9fb2ef23205e510f3a8a62f7df52b0933e1a528
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27282868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:856f604842f4847ce4ea178bc068bf16df596b7eb298a8a23f8cea6c3e89cd42`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Sep 2021 21:20:34 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Thu, 16 Sep 2021 21:21:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Sep 2021 21:21:09 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Sep 2021 21:21:09 GMT
EXPOSE 8091
# Thu, 16 Sep 2021 21:21:10 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Sep 2021 21:21:10 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Sep 2021 21:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Sep 2021 21:21:10 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02a3bf95180b5791ca6424c745df8bd0f6d62f2347cd5e3ebed1d04510c1e36`  
		Last Modified: Thu, 16 Sep 2021 21:24:46 GMT  
		Size: 23.0 MB (23003501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd4a806b67a586afebab99e71b90abfd14982c1583e7d5d2acbf16a1a7f5ef9`  
		Last Modified: Thu, 16 Sep 2021 21:24:43 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545d1436c7f8f742e92125ba026915ae3baa87b871b34650e9492aa122cab75a`  
		Last Modified: Thu, 16 Sep 2021 21:24:43 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:b20a93f968abb071c040b999cf91e7a1628197338c82457b9eabca215ffb951d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:11906e523648c0ecfd715fd95461209271cdaa348e2b5cafd702875e2848ba49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115914028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf4f435ec85e0ffd46dcde4b0c905393950e8f992eee31bf53739e2640a3f6c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 11 Oct 2021 23:19:58 GMT
ENV INFLUXDB_VERSION=1.8.10
# Mon, 11 Oct 2021 23:20:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Mon, 11 Oct 2021 23:20:05 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:05 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:06 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:06 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:06 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e853ec0b4db1129f6cd70c2cf82dbacfdcf794465ade0e99a05a48632549311`  
		Last Modified: Mon, 11 Oct 2021 23:22:26 GMT  
		Size: 54.9 MB (54889512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4284fb25da07fd7dc1fc95522ca2d46aeff49f113c12732620232d136364d56`  
		Last Modified: Mon, 11 Oct 2021 23:22:19 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e28476118a92067c5f7d3228079310f8a279ab931dfa1c37eca3e090eafa5c`  
		Last Modified: Mon, 11 Oct 2021 23:22:18 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a0d8bc54100ca9ad29cc82bdb6029e53833288ffdc2a7a861f87131d281c6e`  
		Last Modified: Mon, 11 Oct 2021 23:22:18 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:8ead108522d403545a5d89ff77160dfb16a9ce8407e3ea138418a71ddb78b38c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107617859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2f84591f64a66c11a7423f63fb0042e9f299c8398ca3c40616831ba4ed0a06c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 15:30:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 12 Oct 2021 00:39:02 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 12 Oct 2021 00:39:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 12 Oct 2021 00:39:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 12 Oct 2021 00:39:17 GMT
EXPOSE 8086
# Tue, 12 Oct 2021 00:39:17 GMT
VOLUME [/var/lib/influxdb]
# Tue, 12 Oct 2021 00:39:18 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 12 Oct 2021 00:39:19 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 12 Oct 2021 00:39:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 00:39:19 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b971858d80d06fe204d46d63285d784d8a83132df39eaae9a0c7b9dff178cd`  
		Last Modified: Sat, 02 Oct 2021 15:31:48 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45116cd448979bf80e743f5b9643d61bb051ffb1fd9a5d7d1bf999ea6d8328a1`  
		Last Modified: Tue, 12 Oct 2021 00:40:20 GMT  
		Size: 51.6 MB (51616827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbfe6b6536214ca3f94afb0cde0d8f5b31c306cec5c97bfdb80706176f40b8c`  
		Last Modified: Tue, 12 Oct 2021 00:39:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa732ee042c0b81ac0285ab19b56a0e743945cf232ee6cd1598ffc038547e584`  
		Last Modified: Tue, 12 Oct 2021 00:39:53 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a979d8cbcec4658395ca5c58fdf5c7583441654a8fdbfc4ed2e35cbd242b50`  
		Last Modified: Tue, 12 Oct 2021 00:39:52 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:54fbf283e4693a7534a6c71fd4902577478da240152e8fee86c8d7e86e499597
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.7 MB (108728315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8693eca921ac41d14a583b82c6c78904f3d6e934a9aaeae1962ec759fbafa705`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 21:58:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 11 Oct 2021 23:39:35 GMT
ENV INFLUXDB_VERSION=1.8.10
# Mon, 11 Oct 2021 23:39:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Mon, 11 Oct 2021 23:39:40 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:39:41 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:39:41 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:39:41 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:39:41 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:39:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:39:42 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df36ff09e1ede2cc321c3bc8e3bee61b25e75e77e64c51ad208867c48aa86e1`  
		Last Modified: Tue, 28 Sep 2021 21:59:20 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f184b6531a16a931efaf5ac8bb6f40261651978bed1a09a8194795060310215b`  
		Last Modified: Mon, 11 Oct 2021 23:40:27 GMT  
		Size: 51.2 MB (51233870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22329aa77a5561878e10afe81c0f3540eed3ca803de06b5f0fb08f09371d6e4a`  
		Last Modified: Mon, 11 Oct 2021 23:40:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c359ea7e7322f06270ab8c4707441ccb8cb50abf6cba9f861f76ddca64b0a2f`  
		Last Modified: Mon, 11 Oct 2021 23:40:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12016972c965558f858af3592ac638037dc0d1fb8445240e38c56c913b8a5a1`  
		Last Modified: Mon, 11 Oct 2021 23:40:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:08b9e3840bf14c6766b1400750c8301700c36ef155c531778d104e095e95d1b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:a6be2a595ba851186623d09bb0489364eac55f13a0a397f7f2bc1b1b0c56b621
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58940318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a523b56f0b2b5dd896d10dc30ba3cb81a41a9658755b8f6da9b3e35af217cf63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 11 Oct 2021 23:20:09 GMT
ENV INFLUXDB_VERSION=1.8.10
# Mon, 11 Oct 2021 23:20:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 11 Oct 2021 23:20:22 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:22 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:22 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:23 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:23 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0d28ebb5fb88259e43852ee731dd9c6fad7344b353d52acf76bace2de78960`  
		Last Modified: Mon, 11 Oct 2021 23:22:44 GMT  
		Size: 54.7 MB (54659803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36610f60a90d0ab8bf62a1cdec2fb40bfcbc7a34988ae04e3bca96ac989c2be`  
		Last Modified: Mon, 11 Oct 2021 23:22:36 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f595c36e5893b42d753272276817a1c67d6f25a56df0b38eafff15c2f7d4572`  
		Last Modified: Mon, 11 Oct 2021 23:22:36 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08235009b8859fa7c0a2e24164737912abd3ef687e2dc46ebf130901dced1ec`  
		Last Modified: Mon, 11 Oct 2021 23:22:36 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:d04305dd8914c486e8ef3cbbcff811e54dc1738f4884be67bfcedcf4d15ae1f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:e7373d5b9b5c8427e7a920a37b66f0ab1576f3f9518ff1b837f60cc3027b79dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117733109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5698a773c4695af4f07c5c0048e86a2e902ec64cf473a5ccdec1af1a63d42b5b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 11 Oct 2021 23:20:26 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:20:32 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 11 Oct 2021 23:20:33 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:33 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:33 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:33 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:34 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe16c0b4bccccde6eb4a50c0557b13eaaba0dcc8c57e1214aa71f37724941f5`  
		Last Modified: Mon, 11 Oct 2021 23:23:02 GMT  
		Size: 56.7 MB (56708535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a832d21088fde43f8d6f8441268e6b19f9955d93fd2a4508973fe5cdd0a5558e`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793aaa7ad592f4bd291349c0afc6a3318bcd6f983d80f1909bbae21463cc3249`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6d48653c4e7352a26c96597a08281723742b610a46ec26a03b86beafe16e58`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:fe6ac4f357e16b19ff202f3bb26c46b2705b294984e1675f46bce753d0694ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b32206b0b89cd0b2366eed0298b2f983de3f64862bb38611b4b745b7b3353364
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60784165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7f3952479650ac95cd5661233633ca18ec9d5b6c6b4aa43b5a254c367b3249d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 11 Oct 2021 23:20:37 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:20:54 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 11 Oct 2021 23:20:54 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:54 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:54 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:55 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f617e688de2fe3e018e8342b0aef6fcb79cd667150730c3fe56cdca40f85c1af`  
		Last Modified: Mon, 11 Oct 2021 23:23:22 GMT  
		Size: 56.5 MB (56503592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4436b7c1c928d1ac0f25d7e757e21f63fa25ee52e086579e3c3c61f674235f`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305554dc9907f47dfe620e9ab5934f66e7476ecd500796b0c115e80eb000849`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc73aba05114206260f522c1fdfb34b05cdfa143b14829401f2d2ab1daa7728`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:530d76225e4c203094bc7a34beb12d6a8574226e7fe85740e868efa077967bc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:101461adc0a2bace3aad71d70d5fe5774ab9dd954f77d28fd99b20f85cc39c83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84439706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d297f315e2f7843b64053533294e8dac8ffb5ad92e27aac6fb69a62650efee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 11 Oct 2021 23:20:26 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:21:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 11 Oct 2021 23:21:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 11 Oct 2021 23:21:04 GMT
EXPOSE 8091
# Mon, 11 Oct 2021 23:21:04 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:21:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:21:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:21:05 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e082183c5d9aeb287229609fba070b3728d35f589916a7d63f8883a0be3897`  
		Last Modified: Mon, 11 Oct 2021 23:23:38 GMT  
		Size: 23.4 MB (23416335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea51a41f5937a5cbfa04ed5cffa168a7b436f3867b592648c41679a0797bd15`  
		Last Modified: Mon, 11 Oct 2021 23:23:35 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a8297136f94c38636787f47ea3f3182f47609d742a3a430279dc92c7d06c00`  
		Last Modified: Mon, 11 Oct 2021 23:23:35 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:c14412e9051e84e8d6bb2e73147dd79eb5381d2d47fdecd19524d20af54f1359
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:46bb24530636472e50b1b9ccf517430905a4e773437983218a6f57cc0c8c93ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27572254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a2535ab47162451d3c3d50f3236ace5eb8e52a9cfc616ff8af833f51de51875`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 11 Oct 2021 23:20:37 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:21:14 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 11 Oct 2021 23:21:15 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 11 Oct 2021 23:21:15 GMT
EXPOSE 8091
# Mon, 11 Oct 2021 23:21:15 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:21:15 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:21:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:21:16 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1969092b409f910536cd2ae2b8d930b0b3bd9a62c4edc0eb306ceaad9d8723`  
		Last Modified: Mon, 11 Oct 2021 23:23:53 GMT  
		Size: 23.3 MB (23292882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3a46cc6cbfd7f616c01f2861ef1b1905b452913950566d4470641bb31c871b`  
		Last Modified: Mon, 11 Oct 2021 23:23:50 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926287724a1fc5ec8210568eaf0f15438481e47e302691e6ff9921b200ff6f9e`  
		Last Modified: Mon, 11 Oct 2021 23:23:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10`

```console
$ docker pull influxdb@sha256:b20a93f968abb071c040b999cf91e7a1628197338c82457b9eabca215ffb951d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:11906e523648c0ecfd715fd95461209271cdaa348e2b5cafd702875e2848ba49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115914028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf4f435ec85e0ffd46dcde4b0c905393950e8f992eee31bf53739e2640a3f6c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 11 Oct 2021 23:19:58 GMT
ENV INFLUXDB_VERSION=1.8.10
# Mon, 11 Oct 2021 23:20:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Mon, 11 Oct 2021 23:20:05 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:05 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:06 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:06 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:06 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e853ec0b4db1129f6cd70c2cf82dbacfdcf794465ade0e99a05a48632549311`  
		Last Modified: Mon, 11 Oct 2021 23:22:26 GMT  
		Size: 54.9 MB (54889512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4284fb25da07fd7dc1fc95522ca2d46aeff49f113c12732620232d136364d56`  
		Last Modified: Mon, 11 Oct 2021 23:22:19 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e28476118a92067c5f7d3228079310f8a279ab931dfa1c37eca3e090eafa5c`  
		Last Modified: Mon, 11 Oct 2021 23:22:18 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a0d8bc54100ca9ad29cc82bdb6029e53833288ffdc2a7a861f87131d281c6e`  
		Last Modified: Mon, 11 Oct 2021 23:22:18 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:8ead108522d403545a5d89ff77160dfb16a9ce8407e3ea138418a71ddb78b38c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107617859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2f84591f64a66c11a7423f63fb0042e9f299c8398ca3c40616831ba4ed0a06c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 15:30:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 12 Oct 2021 00:39:02 GMT
ENV INFLUXDB_VERSION=1.8.10
# Tue, 12 Oct 2021 00:39:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Tue, 12 Oct 2021 00:39:17 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Tue, 12 Oct 2021 00:39:17 GMT
EXPOSE 8086
# Tue, 12 Oct 2021 00:39:17 GMT
VOLUME [/var/lib/influxdb]
# Tue, 12 Oct 2021 00:39:18 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Tue, 12 Oct 2021 00:39:19 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Tue, 12 Oct 2021 00:39:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 00:39:19 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b971858d80d06fe204d46d63285d784d8a83132df39eaae9a0c7b9dff178cd`  
		Last Modified: Sat, 02 Oct 2021 15:31:48 GMT  
		Size: 2.9 KB (2861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45116cd448979bf80e743f5b9643d61bb051ffb1fd9a5d7d1bf999ea6d8328a1`  
		Last Modified: Tue, 12 Oct 2021 00:40:20 GMT  
		Size: 51.6 MB (51616827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbfe6b6536214ca3f94afb0cde0d8f5b31c306cec5c97bfdb80706176f40b8c`  
		Last Modified: Tue, 12 Oct 2021 00:39:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa732ee042c0b81ac0285ab19b56a0e743945cf232ee6cd1598ffc038547e584`  
		Last Modified: Tue, 12 Oct 2021 00:39:53 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a979d8cbcec4658395ca5c58fdf5c7583441654a8fdbfc4ed2e35cbd242b50`  
		Last Modified: Tue, 12 Oct 2021 00:39:52 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:54fbf283e4693a7534a6c71fd4902577478da240152e8fee86c8d7e86e499597
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.7 MB (108728315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8693eca921ac41d14a583b82c6c78904f3d6e934a9aaeae1962ec759fbafa705`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 21:58:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 11 Oct 2021 23:39:35 GMT
ENV INFLUXDB_VERSION=1.8.10
# Mon, 11 Oct 2021 23:39:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Mon, 11 Oct 2021 23:39:40 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:39:41 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:39:41 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:39:41 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:39:41 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:39:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:39:42 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df36ff09e1ede2cc321c3bc8e3bee61b25e75e77e64c51ad208867c48aa86e1`  
		Last Modified: Tue, 28 Sep 2021 21:59:20 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f184b6531a16a931efaf5ac8bb6f40261651978bed1a09a8194795060310215b`  
		Last Modified: Mon, 11 Oct 2021 23:40:27 GMT  
		Size: 51.2 MB (51233870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22329aa77a5561878e10afe81c0f3540eed3ca803de06b5f0fb08f09371d6e4a`  
		Last Modified: Mon, 11 Oct 2021 23:40:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c359ea7e7322f06270ab8c4707441ccb8cb50abf6cba9f861f76ddca64b0a2f`  
		Last Modified: Mon, 11 Oct 2021 23:40:20 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12016972c965558f858af3592ac638037dc0d1fb8445240e38c56c913b8a5a1`  
		Last Modified: Mon, 11 Oct 2021 23:40:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-alpine`

```console
$ docker pull influxdb@sha256:08b9e3840bf14c6766b1400750c8301700c36ef155c531778d104e095e95d1b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:a6be2a595ba851186623d09bb0489364eac55f13a0a397f7f2bc1b1b0c56b621
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58940318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a523b56f0b2b5dd896d10dc30ba3cb81a41a9658755b8f6da9b3e35af217cf63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 11 Oct 2021 23:20:09 GMT
ENV INFLUXDB_VERSION=1.8.10
# Mon, 11 Oct 2021 23:20:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 11 Oct 2021 23:20:22 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:22 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:22 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:23 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:23 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0d28ebb5fb88259e43852ee731dd9c6fad7344b353d52acf76bace2de78960`  
		Last Modified: Mon, 11 Oct 2021 23:22:44 GMT  
		Size: 54.7 MB (54659803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36610f60a90d0ab8bf62a1cdec2fb40bfcbc7a34988ae04e3bca96ac989c2be`  
		Last Modified: Mon, 11 Oct 2021 23:22:36 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f595c36e5893b42d753272276817a1c67d6f25a56df0b38eafff15c2f7d4572`  
		Last Modified: Mon, 11 Oct 2021 23:22:36 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08235009b8859fa7c0a2e24164737912abd3ef687e2dc46ebf130901dced1ec`  
		Last Modified: Mon, 11 Oct 2021 23:22:36 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data`

```console
$ docker pull influxdb@sha256:d04305dd8914c486e8ef3cbbcff811e54dc1738f4884be67bfcedcf4d15ae1f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:e7373d5b9b5c8427e7a920a37b66f0ab1576f3f9518ff1b837f60cc3027b79dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117733109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5698a773c4695af4f07c5c0048e86a2e902ec64cf473a5ccdec1af1a63d42b5b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 11 Oct 2021 23:20:26 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:20:32 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 11 Oct 2021 23:20:33 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:33 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:33 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:33 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:34 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe16c0b4bccccde6eb4a50c0557b13eaaba0dcc8c57e1214aa71f37724941f5`  
		Last Modified: Mon, 11 Oct 2021 23:23:02 GMT  
		Size: 56.7 MB (56708535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a832d21088fde43f8d6f8441268e6b19f9955d93fd2a4508973fe5cdd0a5558e`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793aaa7ad592f4bd291349c0afc6a3318bcd6f983d80f1909bbae21463cc3249`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6d48653c4e7352a26c96597a08281723742b610a46ec26a03b86beafe16e58`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data-alpine`

```console
$ docker pull influxdb@sha256:fe6ac4f357e16b19ff202f3bb26c46b2705b294984e1675f46bce753d0694ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b32206b0b89cd0b2366eed0298b2f983de3f64862bb38611b4b745b7b3353364
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60784165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7f3952479650ac95cd5661233633ca18ec9d5b6c6b4aa43b5a254c367b3249d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 11 Oct 2021 23:20:37 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:20:54 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 11 Oct 2021 23:20:54 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:54 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:54 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:55 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f617e688de2fe3e018e8342b0aef6fcb79cd667150730c3fe56cdca40f85c1af`  
		Last Modified: Mon, 11 Oct 2021 23:23:22 GMT  
		Size: 56.5 MB (56503592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4436b7c1c928d1ac0f25d7e757e21f63fa25ee52e086579e3c3c61f674235f`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305554dc9907f47dfe620e9ab5934f66e7476ecd500796b0c115e80eb000849`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc73aba05114206260f522c1fdfb34b05cdfa143b14829401f2d2ab1daa7728`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta`

```console
$ docker pull influxdb@sha256:530d76225e4c203094bc7a34beb12d6a8574226e7fe85740e868efa077967bc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:101461adc0a2bace3aad71d70d5fe5774ab9dd954f77d28fd99b20f85cc39c83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84439706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d297f315e2f7843b64053533294e8dac8ffb5ad92e27aac6fb69a62650efee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 11 Oct 2021 23:20:26 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:21:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 11 Oct 2021 23:21:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 11 Oct 2021 23:21:04 GMT
EXPOSE 8091
# Mon, 11 Oct 2021 23:21:04 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:21:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:21:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:21:05 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e082183c5d9aeb287229609fba070b3728d35f589916a7d63f8883a0be3897`  
		Last Modified: Mon, 11 Oct 2021 23:23:38 GMT  
		Size: 23.4 MB (23416335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea51a41f5937a5cbfa04ed5cffa168a7b436f3867b592648c41679a0797bd15`  
		Last Modified: Mon, 11 Oct 2021 23:23:35 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a8297136f94c38636787f47ea3f3182f47609d742a3a430279dc92c7d06c00`  
		Last Modified: Mon, 11 Oct 2021 23:23:35 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta-alpine`

```console
$ docker pull influxdb@sha256:c14412e9051e84e8d6bb2e73147dd79eb5381d2d47fdecd19524d20af54f1359
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:46bb24530636472e50b1b9ccf517430905a4e773437983218a6f57cc0c8c93ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27572254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a2535ab47162451d3c3d50f3236ace5eb8e52a9cfc616ff8af833f51de51875`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 11 Oct 2021 23:20:37 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:21:14 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 11 Oct 2021 23:21:15 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 11 Oct 2021 23:21:15 GMT
EXPOSE 8091
# Mon, 11 Oct 2021 23:21:15 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:21:15 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:21:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:21:16 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1969092b409f910536cd2ae2b8d930b0b3bd9a62c4edc0eb306ceaad9d8723`  
		Last Modified: Mon, 11 Oct 2021 23:23:53 GMT  
		Size: 23.3 MB (23292882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3a46cc6cbfd7f616c01f2861ef1b1905b452913950566d4470641bb31c871b`  
		Last Modified: Mon, 11 Oct 2021 23:23:50 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926287724a1fc5ec8210568eaf0f15438481e47e302691e6ff9921b200ff6f9e`  
		Last Modified: Mon, 11 Oct 2021 23:23:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data`

```console
$ docker pull influxdb@sha256:ef2d9a7414e91ef240a01c13f2a7e5f4aac25b3575740a116b2ec2b01046e256
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:684589e45a2c8406fa01049c8c7de3041c63f8ffc7b9ce0c351473f72c5f1f2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.1 MB (118125718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e5e3d322d4fd5003a604abb72a95184e1c13a46184d56b404f1040a376373bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 29 Sep 2021 06:27:25 GMT
ENV INFLUXDB_VERSION=1.9.4-c1.9.4
# Wed, 29 Sep 2021 06:27:32 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 29 Sep 2021 06:27:32 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 29 Sep 2021 06:27:32 GMT
EXPOSE 8086
# Wed, 29 Sep 2021 06:27:32 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Sep 2021 06:27:33 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 29 Sep 2021 06:27:33 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 29 Sep 2021 06:27:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Sep 2021 06:27:33 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287acdcd984a8abc7f55d2c6849d6e552efed56e8057d515113ce994dde0495e`  
		Last Modified: Wed, 29 Sep 2021 06:30:57 GMT  
		Size: 57.1 MB (57101143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db57ee45eaf193f701a697d2d9ea5dc719987e75bd46e4e772ab26598da52af6`  
		Last Modified: Wed, 29 Sep 2021 06:30:49 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500f458fedea419ff37f377fa5734ed903fa748603bcbb56782de2272da003bc`  
		Last Modified: Wed, 29 Sep 2021 06:30:49 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dcde6bb7f54070a5c9b34d6a8fc286bb5ed5379afefc7f7c74de5cd7965ce`  
		Last Modified: Wed, 29 Sep 2021 06:30:49 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:a34baf98120c2ef84b03164e8fdc8aa9fd335aa9f3260ec62596139868444b4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:07438a91e2dd67caebdbebcfa712642a50f8220283eccacc35c257ec2d9dd910
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61345926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d4606079b88e37eba3997519af44ddcdc64b5eeac729e482c12ecd0651f1078`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Sep 2021 21:22:17 GMT
ENV INFLUXDB_VERSION=1.9.4-c1.9.4
# Thu, 16 Sep 2021 21:22:28 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Sep 2021 21:22:29 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Sep 2021 21:22:29 GMT
EXPOSE 8086
# Thu, 16 Sep 2021 21:22:29 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Sep 2021 21:22:29 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Sep 2021 21:22:29 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Sep 2021 21:22:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Sep 2021 21:22:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e483791956c063225a7f78d89c2e24a9c4a7fc628be75ac2630d08ed4c8595`  
		Last Modified: Thu, 16 Sep 2021 21:26:21 GMT  
		Size: 57.1 MB (57065353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09024cd60230c187523ab1176edd39580d042622c96f2259972c2b8490bc2ad9`  
		Last Modified: Thu, 16 Sep 2021 21:26:14 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3b7813434a80d1f507722d9ce878ef15ba2fa333b4ad2fb1a59b66e33ce84`  
		Last Modified: Thu, 16 Sep 2021 21:26:13 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d0eb7f2cefaca6763a22984bfacf8c9aac352835da7a12299d5f1486f2d5a1`  
		Last Modified: Thu, 16 Sep 2021 21:26:13 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:d95665ecfeb5e0406809f2c45d279be2c1b8bdb4d2380c6b8b6d5b5781894396
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:35f2eb6784b966aa9bee0aa0065f689d22d2cd45321f58d2f6730f9996b6c9bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86086987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8407220020dee3914acc4c196823d1f14c58c9b1906b6fd01215f4118eca32ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 29 Sep 2021 06:27:25 GMT
ENV INFLUXDB_VERSION=1.9.4-c1.9.4
# Wed, 29 Sep 2021 06:27:43 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 29 Sep 2021 06:27:43 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 29 Sep 2021 06:27:43 GMT
EXPOSE 8091
# Wed, 29 Sep 2021 06:27:44 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Sep 2021 06:27:44 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 29 Sep 2021 06:27:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Sep 2021 06:27:44 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f90f72f634e267126a2f5995732a437923c46ee68180bb74c0e44b2c051520`  
		Last Modified: Wed, 29 Sep 2021 06:31:12 GMT  
		Size: 25.1 MB (25063618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b493f3a4b0d44f6a8af14278cdc7bb3c6d84e21e092c702b23223e63973d60`  
		Last Modified: Wed, 29 Sep 2021 06:31:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645949cd24564153c84dd25a7e0c0a74b7211880598ea8fcf5fce5cd868efbe6`  
		Last Modified: Wed, 29 Sep 2021 06:31:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:29c95c0454874e19ba9f8eb910620f6632dfd93606813d9379cc458de7477765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b5c93dfd5aae4eb55fc61d1e61a228b0e1754d242afe02288b9e27455d103c82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29311146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10d07081494f2e0f23d25526eca425b8e07d7f8f46925b89538d6f88bbd700a3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Sep 2021 21:22:17 GMT
ENV INFLUXDB_VERSION=1.9.4-c1.9.4
# Thu, 16 Sep 2021 21:22:47 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     (rm -rf /root/.gnupg || true) &&     rm -rf *.tar.gz* /usr/src &&     apk del .build-deps
# Thu, 16 Sep 2021 21:22:48 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Sep 2021 21:22:48 GMT
EXPOSE 8091
# Thu, 16 Sep 2021 21:22:48 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Sep 2021 21:22:48 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Sep 2021 21:22:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Sep 2021 21:22:49 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f516c2c4fd35cbca3a7989edeb51cc3aae6af6cf4013085bc33cc0aead1715`  
		Last Modified: Thu, 16 Sep 2021 21:26:48 GMT  
		Size: 25.0 MB (25031774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35216cbce08b0a487c56ce52005d737c062a120c9c9ede036c444e83d77a67bc`  
		Last Modified: Thu, 16 Sep 2021 21:26:45 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568f78441909aad1474e20c1e02928f27925bf3cf9e6fc17318eb2c42d2a117a`  
		Last Modified: Thu, 16 Sep 2021 21:26:45 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.4-data`

```console
$ docker pull influxdb@sha256:ef2d9a7414e91ef240a01c13f2a7e5f4aac25b3575740a116b2ec2b01046e256
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.4-data` - linux; amd64

```console
$ docker pull influxdb@sha256:684589e45a2c8406fa01049c8c7de3041c63f8ffc7b9ce0c351473f72c5f1f2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.1 MB (118125718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e5e3d322d4fd5003a604abb72a95184e1c13a46184d56b404f1040a376373bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 29 Sep 2021 06:27:25 GMT
ENV INFLUXDB_VERSION=1.9.4-c1.9.4
# Wed, 29 Sep 2021 06:27:32 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 29 Sep 2021 06:27:32 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 29 Sep 2021 06:27:32 GMT
EXPOSE 8086
# Wed, 29 Sep 2021 06:27:32 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Sep 2021 06:27:33 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 29 Sep 2021 06:27:33 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 29 Sep 2021 06:27:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Sep 2021 06:27:33 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287acdcd984a8abc7f55d2c6849d6e552efed56e8057d515113ce994dde0495e`  
		Last Modified: Wed, 29 Sep 2021 06:30:57 GMT  
		Size: 57.1 MB (57101143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db57ee45eaf193f701a697d2d9ea5dc719987e75bd46e4e772ab26598da52af6`  
		Last Modified: Wed, 29 Sep 2021 06:30:49 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500f458fedea419ff37f377fa5734ed903fa748603bcbb56782de2272da003bc`  
		Last Modified: Wed, 29 Sep 2021 06:30:49 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dcde6bb7f54070a5c9b34d6a8fc286bb5ed5379afefc7f7c74de5cd7965ce`  
		Last Modified: Wed, 29 Sep 2021 06:30:49 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.4-data-alpine`

```console
$ docker pull influxdb@sha256:a34baf98120c2ef84b03164e8fdc8aa9fd335aa9f3260ec62596139868444b4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.4-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:07438a91e2dd67caebdbebcfa712642a50f8220283eccacc35c257ec2d9dd910
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61345926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d4606079b88e37eba3997519af44ddcdc64b5eeac729e482c12ecd0651f1078`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Sep 2021 21:22:17 GMT
ENV INFLUXDB_VERSION=1.9.4-c1.9.4
# Thu, 16 Sep 2021 21:22:28 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Sep 2021 21:22:29 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Sep 2021 21:22:29 GMT
EXPOSE 8086
# Thu, 16 Sep 2021 21:22:29 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Sep 2021 21:22:29 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Sep 2021 21:22:29 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Sep 2021 21:22:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Sep 2021 21:22:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e483791956c063225a7f78d89c2e24a9c4a7fc628be75ac2630d08ed4c8595`  
		Last Modified: Thu, 16 Sep 2021 21:26:21 GMT  
		Size: 57.1 MB (57065353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09024cd60230c187523ab1176edd39580d042622c96f2259972c2b8490bc2ad9`  
		Last Modified: Thu, 16 Sep 2021 21:26:14 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3b7813434a80d1f507722d9ce878ef15ba2fa333b4ad2fb1a59b66e33ce84`  
		Last Modified: Thu, 16 Sep 2021 21:26:13 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d0eb7f2cefaca6763a22984bfacf8c9aac352835da7a12299d5f1486f2d5a1`  
		Last Modified: Thu, 16 Sep 2021 21:26:13 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.4-meta`

```console
$ docker pull influxdb@sha256:d95665ecfeb5e0406809f2c45d279be2c1b8bdb4d2380c6b8b6d5b5781894396
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.4-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:35f2eb6784b966aa9bee0aa0065f689d22d2cd45321f58d2f6730f9996b6c9bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86086987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8407220020dee3914acc4c196823d1f14c58c9b1906b6fd01215f4118eca32ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 29 Sep 2021 06:27:25 GMT
ENV INFLUXDB_VERSION=1.9.4-c1.9.4
# Wed, 29 Sep 2021 06:27:43 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 29 Sep 2021 06:27:43 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 29 Sep 2021 06:27:43 GMT
EXPOSE 8091
# Wed, 29 Sep 2021 06:27:44 GMT
VOLUME [/var/lib/influxdb]
# Wed, 29 Sep 2021 06:27:44 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 29 Sep 2021 06:27:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Sep 2021 06:27:44 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f90f72f634e267126a2f5995732a437923c46ee68180bb74c0e44b2c051520`  
		Last Modified: Wed, 29 Sep 2021 06:31:12 GMT  
		Size: 25.1 MB (25063618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b493f3a4b0d44f6a8af14278cdc7bb3c6d84e21e092c702b23223e63973d60`  
		Last Modified: Wed, 29 Sep 2021 06:31:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645949cd24564153c84dd25a7e0c0a74b7211880598ea8fcf5fce5cd868efbe6`  
		Last Modified: Wed, 29 Sep 2021 06:31:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.4-meta-alpine`

```console
$ docker pull influxdb@sha256:29c95c0454874e19ba9f8eb910620f6632dfd93606813d9379cc458de7477765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.4-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b5c93dfd5aae4eb55fc61d1e61a228b0e1754d242afe02288b9e27455d103c82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29311146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10d07081494f2e0f23d25526eca425b8e07d7f8f46925b89538d6f88bbd700a3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Sep 2021 21:22:17 GMT
ENV INFLUXDB_VERSION=1.9.4-c1.9.4
# Thu, 16 Sep 2021 21:22:47 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     (rm -rf /root/.gnupg || true) &&     rm -rf *.tar.gz* /usr/src &&     apk del .build-deps
# Thu, 16 Sep 2021 21:22:48 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 16 Sep 2021 21:22:48 GMT
EXPOSE 8091
# Thu, 16 Sep 2021 21:22:48 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Sep 2021 21:22:48 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 16 Sep 2021 21:22:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Sep 2021 21:22:49 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f516c2c4fd35cbca3a7989edeb51cc3aae6af6cf4013085bc33cc0aead1715`  
		Last Modified: Thu, 16 Sep 2021 21:26:48 GMT  
		Size: 25.0 MB (25031774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35216cbce08b0a487c56ce52005d737c062a120c9c9ede036c444e83d77a67bc`  
		Last Modified: Thu, 16 Sep 2021 21:26:45 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568f78441909aad1474e20c1e02928f27925bf3cf9e6fc17318eb2c42d2a117a`  
		Last Modified: Thu, 16 Sep 2021 21:26:45 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0`

```console
$ docker pull influxdb@sha256:d20893f055bb937d2071a40f1fe4b8b9cdcc6376763d5d1d1e9ca54f1bff8aab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:194407d7191e84a6c69f9edc16e1493179241bf1600d366d4975229fee3e038f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172325295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25e63af069cd6e36536b6451ce0675104e5a5ec4c5e7fd176297e185bf37a686`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:27:51 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 29 Sep 2021 06:27:51 GMT
ENV GOSU_VER=1.12
# Wed, 29 Sep 2021 06:27:55 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Tue, 05 Oct 2021 17:39:16 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 17:39:26 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 17:39:27 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 17:39:28 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 17:39:28 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 17:39:28 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 17:39:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 17:39:29 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 17:39:29 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 17:39:29 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 17:39:29 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 17:39:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 17:39:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c929756af316d40810a0b10a60961acc9de8d603ed050710a7e894689a1e17a`  
		Last Modified: Wed, 29 Sep 2021 06:31:25 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186926ca7015fa3f6b798752ddfc1a42db9763e43500bc8e5de9fff7b92522d`  
		Last Modified: Wed, 29 Sep 2021 06:31:22 GMT  
		Size: 961.0 KB (960989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe55f2d8f25daf887add134b4dea1131e5920cd052ab48276ac168b61024a75b`  
		Last Modified: Tue, 05 Oct 2021 17:40:58 GMT  
		Size: 103.1 MB (103090642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79ed64c23c171a2a780be71df757f8d1c8be1392c4fd5f408bc130bfeb2aae`  
		Last Modified: Tue, 05 Oct 2021 17:40:49 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad642110b70ade9dce6fb304dfaae9419b9ecaf713be4e2088a683d3f79bb10`  
		Last Modified: Tue, 05 Oct 2021 17:40:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086844e7c60e63f32c18b42782910fbb25b11cfb88365b78838a8835cc0cabfe`  
		Last Modified: Tue, 05 Oct 2021 17:40:49 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4e56d7ae7e306c8d54463b43bd0cc0603a97295a5987309dd6b8d576ddaa083e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174332651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048ac864884959d98cc21955b72b2005681becdabbbc0b9a386ebf1b665d4155`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 21:58:31 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 28 Sep 2021 21:58:31 GMT
ENV GOSU_VER=1.12
# Tue, 28 Sep 2021 21:58:34 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Tue, 05 Oct 2021 00:39:59 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 00:40:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 00:40:12 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 00:40:12 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 00:40:12 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 00:40:12 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 00:40:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 00:40:13 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 00:40:13 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 00:40:13 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 00:40:13 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 00:40:13 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 00:40:14 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fbdf4c46d6c97c0f3af3092d2060290dad9a1fd542b91c4e8790cad0c7381d`  
		Last Modified: Tue, 28 Sep 2021 22:00:03 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a8253f6adc5ce3b687e412c769d37cdd7576a45eb3a86e8950210ab1d4d427`  
		Last Modified: Tue, 28 Sep 2021 22:00:00 GMT  
		Size: 896.4 KB (896379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f6e5daeeb4f0987916be588e5df6b582e80a7d588af38c081c9fd0ff753afb`  
		Last Modified: Tue, 05 Oct 2021 00:41:16 GMT  
		Size: 106.5 MB (106527052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2dd575eea52432344d4ed259dc5512ae195bd265cad024ed206aad92977438`  
		Last Modified: Tue, 05 Oct 2021 00:41:04 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072eea4819167ce610a410f2c1add4ecc36c5b4ebb5b2aed99ca18ee0ab6f295`  
		Last Modified: Tue, 05 Oct 2021 00:41:04 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3a246b2dc644132f7b437f032890b29f733117925801c763a1813eac8a65c3`  
		Last Modified: Tue, 05 Oct 2021 00:41:04 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0-alpine`

```console
$ docker pull influxdb@sha256:ce37728563dce6b9e50cebb5414a20fd21d8600be1fe7808c87f6be0a0865c45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:71a5533b39fe9ce2e8918b4043ed42283a97319c75dce557e027b320a312185e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116662545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6516a90d7f6a2627ebfa5a7442ed3783fdbc8bd8df49d53a461dc26a552556f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:22:57 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Thu, 16 Sep 2021 21:22:58 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Sep 2021 21:22:59 GMT
ENV GOSU_VER=1.12
# Thu, 16 Sep 2021 21:23:02 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Oct 2021 17:39:35 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 17:39:44 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 17:39:45 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 17:39:46 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 17:39:46 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 17:39:46 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 17:39:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 17:39:47 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 17:39:47 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 17:39:47 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 17:39:47 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 17:39:47 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 17:39:48 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a33a59ed40857217bfaf7d10edd52beb9edde5c53c10d498d0669e63b715ac5`  
		Last Modified: Thu, 16 Sep 2021 21:27:04 GMT  
		Size: 9.8 MB (9790585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9fc214535bef0c112afb12ae496eb70400d1712fe645063ac16c1eb085db5a`  
		Last Modified: Thu, 16 Sep 2021 21:27:02 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65b0c7df0242d67c9b06c22c38d15b7eb040bb0279805206c68d9b0ffbbe39f`  
		Last Modified: Thu, 16 Sep 2021 21:27:00 GMT  
		Size: 960.6 KB (960613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4ec960b3bdf651c06b863304ab0f9c5c40db445b5007b05c5875dd3698fbeb`  
		Last Modified: Tue, 05 Oct 2021 17:41:21 GMT  
		Size: 103.1 MB (103090620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bd0f832d6524244dfa496041ada3a242527dc99e75c96c17bcc41e7d714d5`  
		Last Modified: Tue, 05 Oct 2021 17:41:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3f4fdbfefb0d562c1075811f8f1fc725308e3d820a69a9746a5dc7d68018f9`  
		Last Modified: Tue, 05 Oct 2021 17:41:12 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cceff34f66aa4eda9c20102442b3eccb02d107982a23949b67a9ce6d9706cd1`  
		Last Modified: Tue, 05 Oct 2021 17:41:11 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4eff9c4401cf313bbff884b0894c08f28f0a1dda9ba41e960de21b442bc36c72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119769630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3116b8dd718d977a7a9fe690e83ed4ae538b09d91647af810a3447b972a056e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:40:11 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:40:13 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Thu, 16 Sep 2021 21:40:13 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Sep 2021 21:40:14 GMT
ENV GOSU_VER=1.12
# Thu, 16 Sep 2021 21:40:17 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Oct 2021 00:40:20 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 00:40:27 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 00:40:28 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 00:40:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 00:40:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 00:40:29 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 00:40:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 00:40:29 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 00:40:30 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 00:40:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 00:40:30 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 00:40:30 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 00:40:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b541109e4b3da396713d17fef9d204f410648de5e7aafb0955dd468349522061`  
		Last Modified: Thu, 16 Sep 2021 21:41:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6165774c176fed7302917ad69bad74db8a9b1ae83d7785bb5efe9d28cab259`  
		Last Modified: Thu, 16 Sep 2021 21:41:16 GMT  
		Size: 9.6 MB (9628384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7356f991ea5090b4db00141e333e6e26c8efcc0e6e28a8ddc1d5edbb564dbc88`  
		Last Modified: Thu, 16 Sep 2021 21:41:15 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f59de30cf5b00bbee31abfc65870f8f139c6eb52ce076c05c465b00d4252d6`  
		Last Modified: Thu, 16 Sep 2021 21:41:13 GMT  
		Size: 896.1 KB (896107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c227536956cbd4b8a8e9b1e1a299bb1d5ef142e61c637a47d8537e4eb3d2a03`  
		Last Modified: Tue, 05 Oct 2021 00:41:42 GMT  
		Size: 106.5 MB (106527026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85f75e2a7bec5bac92fdf9bdf75da2069cb7205021f0e5fd3031a6975a24867`  
		Last Modified: Tue, 05 Oct 2021 00:41:30 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3a7c437379d37cc991f0389dfe6cfcf768e98b68db1be13cbc25a60196ccc7`  
		Last Modified: Tue, 05 Oct 2021 00:41:30 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6e731d3161a3f2537d051469bba818c02a9be7c02222844b138f9ea176f165`  
		Last Modified: Tue, 05 Oct 2021 00:41:30 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.9`

```console
$ docker pull influxdb@sha256:d20893f055bb937d2071a40f1fe4b8b9cdcc6376763d5d1d1e9ca54f1bff8aab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9` - linux; amd64

```console
$ docker pull influxdb@sha256:194407d7191e84a6c69f9edc16e1493179241bf1600d366d4975229fee3e038f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172325295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25e63af069cd6e36536b6451ce0675104e5a5ec4c5e7fd176297e185bf37a686`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:27:51 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 29 Sep 2021 06:27:51 GMT
ENV GOSU_VER=1.12
# Wed, 29 Sep 2021 06:27:55 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Tue, 05 Oct 2021 17:39:16 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 17:39:26 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 17:39:27 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 17:39:28 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 17:39:28 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 17:39:28 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 17:39:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 17:39:29 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 17:39:29 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 17:39:29 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 17:39:29 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 17:39:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 17:39:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c929756af316d40810a0b10a60961acc9de8d603ed050710a7e894689a1e17a`  
		Last Modified: Wed, 29 Sep 2021 06:31:25 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186926ca7015fa3f6b798752ddfc1a42db9763e43500bc8e5de9fff7b92522d`  
		Last Modified: Wed, 29 Sep 2021 06:31:22 GMT  
		Size: 961.0 KB (960989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe55f2d8f25daf887add134b4dea1131e5920cd052ab48276ac168b61024a75b`  
		Last Modified: Tue, 05 Oct 2021 17:40:58 GMT  
		Size: 103.1 MB (103090642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79ed64c23c171a2a780be71df757f8d1c8be1392c4fd5f408bc130bfeb2aae`  
		Last Modified: Tue, 05 Oct 2021 17:40:49 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad642110b70ade9dce6fb304dfaae9419b9ecaf713be4e2088a683d3f79bb10`  
		Last Modified: Tue, 05 Oct 2021 17:40:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086844e7c60e63f32c18b42782910fbb25b11cfb88365b78838a8835cc0cabfe`  
		Last Modified: Tue, 05 Oct 2021 17:40:49 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4e56d7ae7e306c8d54463b43bd0cc0603a97295a5987309dd6b8d576ddaa083e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174332651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048ac864884959d98cc21955b72b2005681becdabbbc0b9a386ebf1b665d4155`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 21:58:31 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 28 Sep 2021 21:58:31 GMT
ENV GOSU_VER=1.12
# Tue, 28 Sep 2021 21:58:34 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Tue, 05 Oct 2021 00:39:59 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 00:40:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 00:40:12 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 00:40:12 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 00:40:12 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 00:40:12 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 00:40:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 00:40:13 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 00:40:13 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 00:40:13 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 00:40:13 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 00:40:13 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 00:40:14 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fbdf4c46d6c97c0f3af3092d2060290dad9a1fd542b91c4e8790cad0c7381d`  
		Last Modified: Tue, 28 Sep 2021 22:00:03 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a8253f6adc5ce3b687e412c769d37cdd7576a45eb3a86e8950210ab1d4d427`  
		Last Modified: Tue, 28 Sep 2021 22:00:00 GMT  
		Size: 896.4 KB (896379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f6e5daeeb4f0987916be588e5df6b582e80a7d588af38c081c9fd0ff753afb`  
		Last Modified: Tue, 05 Oct 2021 00:41:16 GMT  
		Size: 106.5 MB (106527052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2dd575eea52432344d4ed259dc5512ae195bd265cad024ed206aad92977438`  
		Last Modified: Tue, 05 Oct 2021 00:41:04 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072eea4819167ce610a410f2c1add4ecc36c5b4ebb5b2aed99ca18ee0ab6f295`  
		Last Modified: Tue, 05 Oct 2021 00:41:04 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3a246b2dc644132f7b437f032890b29f733117925801c763a1813eac8a65c3`  
		Last Modified: Tue, 05 Oct 2021 00:41:04 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.9-alpine`

```console
$ docker pull influxdb@sha256:ce37728563dce6b9e50cebb5414a20fd21d8600be1fe7808c87f6be0a0865c45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:71a5533b39fe9ce2e8918b4043ed42283a97319c75dce557e027b320a312185e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116662545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6516a90d7f6a2627ebfa5a7442ed3783fdbc8bd8df49d53a461dc26a552556f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:22:57 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Thu, 16 Sep 2021 21:22:58 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Sep 2021 21:22:59 GMT
ENV GOSU_VER=1.12
# Thu, 16 Sep 2021 21:23:02 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Oct 2021 17:39:35 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 17:39:44 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 17:39:45 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 17:39:46 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 17:39:46 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 17:39:46 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 17:39:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 17:39:47 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 17:39:47 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 17:39:47 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 17:39:47 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 17:39:47 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 17:39:48 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a33a59ed40857217bfaf7d10edd52beb9edde5c53c10d498d0669e63b715ac5`  
		Last Modified: Thu, 16 Sep 2021 21:27:04 GMT  
		Size: 9.8 MB (9790585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9fc214535bef0c112afb12ae496eb70400d1712fe645063ac16c1eb085db5a`  
		Last Modified: Thu, 16 Sep 2021 21:27:02 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65b0c7df0242d67c9b06c22c38d15b7eb040bb0279805206c68d9b0ffbbe39f`  
		Last Modified: Thu, 16 Sep 2021 21:27:00 GMT  
		Size: 960.6 KB (960613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4ec960b3bdf651c06b863304ab0f9c5c40db445b5007b05c5875dd3698fbeb`  
		Last Modified: Tue, 05 Oct 2021 17:41:21 GMT  
		Size: 103.1 MB (103090620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bd0f832d6524244dfa496041ada3a242527dc99e75c96c17bcc41e7d714d5`  
		Last Modified: Tue, 05 Oct 2021 17:41:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3f4fdbfefb0d562c1075811f8f1fc725308e3d820a69a9746a5dc7d68018f9`  
		Last Modified: Tue, 05 Oct 2021 17:41:12 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cceff34f66aa4eda9c20102442b3eccb02d107982a23949b67a9ce6d9706cd1`  
		Last Modified: Tue, 05 Oct 2021 17:41:11 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4eff9c4401cf313bbff884b0894c08f28f0a1dda9ba41e960de21b442bc36c72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119769630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3116b8dd718d977a7a9fe690e83ed4ae538b09d91647af810a3447b972a056e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:40:11 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:40:13 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Thu, 16 Sep 2021 21:40:13 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Sep 2021 21:40:14 GMT
ENV GOSU_VER=1.12
# Thu, 16 Sep 2021 21:40:17 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Oct 2021 00:40:20 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 00:40:27 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 00:40:28 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 00:40:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 00:40:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 00:40:29 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 00:40:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 00:40:29 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 00:40:30 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 00:40:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 00:40:30 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 00:40:30 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 00:40:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b541109e4b3da396713d17fef9d204f410648de5e7aafb0955dd468349522061`  
		Last Modified: Thu, 16 Sep 2021 21:41:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6165774c176fed7302917ad69bad74db8a9b1ae83d7785bb5efe9d28cab259`  
		Last Modified: Thu, 16 Sep 2021 21:41:16 GMT  
		Size: 9.6 MB (9628384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7356f991ea5090b4db00141e333e6e26c8efcc0e6e28a8ddc1d5edbb564dbc88`  
		Last Modified: Thu, 16 Sep 2021 21:41:15 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f59de30cf5b00bbee31abfc65870f8f139c6eb52ce076c05c465b00d4252d6`  
		Last Modified: Thu, 16 Sep 2021 21:41:13 GMT  
		Size: 896.1 KB (896107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c227536956cbd4b8a8e9b1e1a299bb1d5ef142e61c637a47d8537e4eb3d2a03`  
		Last Modified: Tue, 05 Oct 2021 00:41:42 GMT  
		Size: 106.5 MB (106527026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85f75e2a7bec5bac92fdf9bdf75da2069cb7205021f0e5fd3031a6975a24867`  
		Last Modified: Tue, 05 Oct 2021 00:41:30 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3a7c437379d37cc991f0389dfe6cfcf768e98b68db1be13cbc25a60196ccc7`  
		Last Modified: Tue, 05 Oct 2021 00:41:30 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6e731d3161a3f2537d051469bba818c02a9be7c02222844b138f9ea176f165`  
		Last Modified: Tue, 05 Oct 2021 00:41:30 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:ce37728563dce6b9e50cebb5414a20fd21d8600be1fe7808c87f6be0a0865c45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:71a5533b39fe9ce2e8918b4043ed42283a97319c75dce557e027b320a312185e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116662545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6516a90d7f6a2627ebfa5a7442ed3783fdbc8bd8df49d53a461dc26a552556f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:22:57 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Thu, 16 Sep 2021 21:22:58 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Sep 2021 21:22:59 GMT
ENV GOSU_VER=1.12
# Thu, 16 Sep 2021 21:23:02 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Oct 2021 17:39:35 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 17:39:44 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 17:39:45 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 17:39:46 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 17:39:46 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 17:39:46 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 17:39:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 17:39:47 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 17:39:47 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 17:39:47 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 17:39:47 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 17:39:47 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 17:39:48 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a33a59ed40857217bfaf7d10edd52beb9edde5c53c10d498d0669e63b715ac5`  
		Last Modified: Thu, 16 Sep 2021 21:27:04 GMT  
		Size: 9.8 MB (9790585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9fc214535bef0c112afb12ae496eb70400d1712fe645063ac16c1eb085db5a`  
		Last Modified: Thu, 16 Sep 2021 21:27:02 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65b0c7df0242d67c9b06c22c38d15b7eb040bb0279805206c68d9b0ffbbe39f`  
		Last Modified: Thu, 16 Sep 2021 21:27:00 GMT  
		Size: 960.6 KB (960613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4ec960b3bdf651c06b863304ab0f9c5c40db445b5007b05c5875dd3698fbeb`  
		Last Modified: Tue, 05 Oct 2021 17:41:21 GMT  
		Size: 103.1 MB (103090620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bd0f832d6524244dfa496041ada3a242527dc99e75c96c17bcc41e7d714d5`  
		Last Modified: Tue, 05 Oct 2021 17:41:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3f4fdbfefb0d562c1075811f8f1fc725308e3d820a69a9746a5dc7d68018f9`  
		Last Modified: Tue, 05 Oct 2021 17:41:12 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cceff34f66aa4eda9c20102442b3eccb02d107982a23949b67a9ce6d9706cd1`  
		Last Modified: Tue, 05 Oct 2021 17:41:11 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4eff9c4401cf313bbff884b0894c08f28f0a1dda9ba41e960de21b442bc36c72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119769630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3116b8dd718d977a7a9fe690e83ed4ae538b09d91647af810a3447b972a056e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:40:11 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:40:13 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Thu, 16 Sep 2021 21:40:13 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Thu, 16 Sep 2021 21:40:14 GMT
ENV GOSU_VER=1.12
# Thu, 16 Sep 2021 21:40:17 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Oct 2021 00:40:20 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 00:40:27 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 00:40:28 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 00:40:29 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 00:40:29 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 00:40:29 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 00:40:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 00:40:29 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 00:40:30 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 00:40:30 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 00:40:30 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 00:40:30 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 00:40:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b541109e4b3da396713d17fef9d204f410648de5e7aafb0955dd468349522061`  
		Last Modified: Thu, 16 Sep 2021 21:41:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6165774c176fed7302917ad69bad74db8a9b1ae83d7785bb5efe9d28cab259`  
		Last Modified: Thu, 16 Sep 2021 21:41:16 GMT  
		Size: 9.6 MB (9628384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7356f991ea5090b4db00141e333e6e26c8efcc0e6e28a8ddc1d5edbb564dbc88`  
		Last Modified: Thu, 16 Sep 2021 21:41:15 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f59de30cf5b00bbee31abfc65870f8f139c6eb52ce076c05c465b00d4252d6`  
		Last Modified: Thu, 16 Sep 2021 21:41:13 GMT  
		Size: 896.1 KB (896107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c227536956cbd4b8a8e9b1e1a299bb1d5ef142e61c637a47d8537e4eb3d2a03`  
		Last Modified: Tue, 05 Oct 2021 00:41:42 GMT  
		Size: 106.5 MB (106527026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85f75e2a7bec5bac92fdf9bdf75da2069cb7205021f0e5fd3031a6975a24867`  
		Last Modified: Tue, 05 Oct 2021 00:41:30 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3a7c437379d37cc991f0389dfe6cfcf768e98b68db1be13cbc25a60196ccc7`  
		Last Modified: Tue, 05 Oct 2021 00:41:30 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6e731d3161a3f2537d051469bba818c02a9be7c02222844b138f9ea176f165`  
		Last Modified: Tue, 05 Oct 2021 00:41:30 GMT  
		Size: 4.3 KB (4326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:d04305dd8914c486e8ef3cbbcff811e54dc1738f4884be67bfcedcf4d15ae1f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:e7373d5b9b5c8427e7a920a37b66f0ab1576f3f9518ff1b837f60cc3027b79dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117733109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5698a773c4695af4f07c5c0048e86a2e902ec64cf473a5ccdec1af1a63d42b5b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 11 Oct 2021 23:20:26 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:20:32 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 11 Oct 2021 23:20:33 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:33 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:33 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:33 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:34 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe16c0b4bccccde6eb4a50c0557b13eaaba0dcc8c57e1214aa71f37724941f5`  
		Last Modified: Mon, 11 Oct 2021 23:23:02 GMT  
		Size: 56.7 MB (56708535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a832d21088fde43f8d6f8441268e6b19f9955d93fd2a4508973fe5cdd0a5558e`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793aaa7ad592f4bd291349c0afc6a3318bcd6f983d80f1909bbae21463cc3249`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6d48653c4e7352a26c96597a08281723742b610a46ec26a03b86beafe16e58`  
		Last Modified: Mon, 11 Oct 2021 23:22:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:fe6ac4f357e16b19ff202f3bb26c46b2705b294984e1675f46bce753d0694ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b32206b0b89cd0b2366eed0298b2f983de3f64862bb38611b4b745b7b3353364
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60784165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7f3952479650ac95cd5661233633ca18ec9d5b6c6b4aa43b5a254c367b3249d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 11 Oct 2021 23:20:37 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:20:54 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 11 Oct 2021 23:20:54 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:54 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:54 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:55 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f617e688de2fe3e018e8342b0aef6fcb79cd667150730c3fe56cdca40f85c1af`  
		Last Modified: Mon, 11 Oct 2021 23:23:22 GMT  
		Size: 56.5 MB (56503592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4436b7c1c928d1ac0f25d7e757e21f63fa25ee52e086579e3c3c61f674235f`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305554dc9907f47dfe620e9ab5934f66e7476ecd500796b0c115e80eb000849`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc73aba05114206260f522c1fdfb34b05cdfa143b14829401f2d2ab1daa7728`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:d20893f055bb937d2071a40f1fe4b8b9cdcc6376763d5d1d1e9ca54f1bff8aab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:194407d7191e84a6c69f9edc16e1493179241bf1600d366d4975229fee3e038f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172325295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25e63af069cd6e36536b6451ce0675104e5a5ec4c5e7fd176297e185bf37a686`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:27:51 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Wed, 29 Sep 2021 06:27:51 GMT
ENV GOSU_VER=1.12
# Wed, 29 Sep 2021 06:27:55 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Tue, 05 Oct 2021 17:39:16 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 17:39:26 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 17:39:27 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 17:39:28 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 17:39:28 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 17:39:28 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 17:39:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 17:39:29 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 17:39:29 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 17:39:29 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 17:39:29 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 17:39:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 17:39:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c929756af316d40810a0b10a60961acc9de8d603ed050710a7e894689a1e17a`  
		Last Modified: Wed, 29 Sep 2021 06:31:25 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186926ca7015fa3f6b798752ddfc1a42db9763e43500bc8e5de9fff7b92522d`  
		Last Modified: Wed, 29 Sep 2021 06:31:22 GMT  
		Size: 961.0 KB (960989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe55f2d8f25daf887add134b4dea1131e5920cd052ab48276ac168b61024a75b`  
		Last Modified: Tue, 05 Oct 2021 17:40:58 GMT  
		Size: 103.1 MB (103090642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c79ed64c23c171a2a780be71df757f8d1c8be1392c4fd5f408bc130bfeb2aae`  
		Last Modified: Tue, 05 Oct 2021 17:40:49 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad642110b70ade9dce6fb304dfaae9419b9ecaf713be4e2088a683d3f79bb10`  
		Last Modified: Tue, 05 Oct 2021 17:40:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086844e7c60e63f32c18b42782910fbb25b11cfb88365b78838a8835cc0cabfe`  
		Last Modified: Tue, 05 Oct 2021 17:40:49 GMT  
		Size: 4.3 KB (4323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4e56d7ae7e306c8d54463b43bd0cc0603a97295a5987309dd6b8d576ddaa083e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174332651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048ac864884959d98cc21955b72b2005681becdabbbc0b9a386ebf1b665d4155`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 21:58:31 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 28 Sep 2021 21:58:31 GMT
ENV GOSU_VER=1.12
# Tue, 28 Sep 2021 21:58:34 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Tue, 05 Oct 2021 00:39:59 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 05 Oct 2021 00:40:11 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 05 Oct 2021 00:40:12 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 05 Oct 2021 00:40:12 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 05 Oct 2021 00:40:12 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 05 Oct 2021 00:40:12 GMT
COPY file:d7feb20b951141d711981be8e82cc1301ac374a4bdcd763025f350ecad4e1f75 in /entrypoint.sh 
# Tue, 05 Oct 2021 00:40:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Oct 2021 00:40:13 GMT
CMD ["influxd"]
# Tue, 05 Oct 2021 00:40:13 GMT
EXPOSE 8086
# Tue, 05 Oct 2021 00:40:13 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 05 Oct 2021 00:40:13 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 05 Oct 2021 00:40:13 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 05 Oct 2021 00:40:14 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fbdf4c46d6c97c0f3af3092d2060290dad9a1fd542b91c4e8790cad0c7381d`  
		Last Modified: Tue, 28 Sep 2021 22:00:03 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a8253f6adc5ce3b687e412c769d37cdd7576a45eb3a86e8950210ab1d4d427`  
		Last Modified: Tue, 28 Sep 2021 22:00:00 GMT  
		Size: 896.4 KB (896379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f6e5daeeb4f0987916be588e5df6b582e80a7d588af38c081c9fd0ff753afb`  
		Last Modified: Tue, 05 Oct 2021 00:41:16 GMT  
		Size: 106.5 MB (106527052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2dd575eea52432344d4ed259dc5512ae195bd265cad024ed206aad92977438`  
		Last Modified: Tue, 05 Oct 2021 00:41:04 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072eea4819167ce610a410f2c1add4ecc36c5b4ebb5b2aed99ca18ee0ab6f295`  
		Last Modified: Tue, 05 Oct 2021 00:41:04 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3a246b2dc644132f7b437f032890b29f733117925801c763a1813eac8a65c3`  
		Last Modified: Tue, 05 Oct 2021 00:41:04 GMT  
		Size: 4.3 KB (4324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:530d76225e4c203094bc7a34beb12d6a8574226e7fe85740e868efa077967bc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:101461adc0a2bace3aad71d70d5fe5774ab9dd954f77d28fd99b20f85cc39c83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84439706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d297f315e2f7843b64053533294e8dac8ffb5ad92e27aac6fb69a62650efee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 11 Oct 2021 23:20:26 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:21:04 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Mon, 11 Oct 2021 23:21:04 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 11 Oct 2021 23:21:04 GMT
EXPOSE 8091
# Mon, 11 Oct 2021 23:21:04 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:21:05 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:21:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:21:05 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7664c6d90947b8b4ab65e0ebad116c3c01dbc88442f8c45245e5fe0c22431ca`  
		Last Modified: Wed, 29 Sep 2021 06:28:57 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e082183c5d9aeb287229609fba070b3728d35f589916a7d63f8883a0be3897`  
		Last Modified: Mon, 11 Oct 2021 23:23:38 GMT  
		Size: 23.4 MB (23416335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea51a41f5937a5cbfa04ed5cffa168a7b436f3867b592648c41679a0797bd15`  
		Last Modified: Mon, 11 Oct 2021 23:23:35 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a8297136f94c38636787f47ea3f3182f47609d742a3a430279dc92c7d06c00`  
		Last Modified: Mon, 11 Oct 2021 23:23:35 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:c14412e9051e84e8d6bb2e73147dd79eb5381d2d47fdecd19524d20af54f1359
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:46bb24530636472e50b1b9ccf517430905a4e773437983218a6f57cc0c8c93ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27572254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a2535ab47162451d3c3d50f3236ace5eb8e52a9cfc616ff8af833f51de51875`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 11 Oct 2021 23:20:37 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:21:14 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 11 Oct 2021 23:21:15 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Mon, 11 Oct 2021 23:21:15 GMT
EXPOSE 8091
# Mon, 11 Oct 2021 23:21:15 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:21:15 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:21:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:21:16 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1969092b409f910536cd2ae2b8d930b0b3bd9a62c4edc0eb306ceaad9d8723`  
		Last Modified: Mon, 11 Oct 2021 23:23:53 GMT  
		Size: 23.3 MB (23292882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3a46cc6cbfd7f616c01f2861ef1b1905b452913950566d4470641bb31c871b`  
		Last Modified: Mon, 11 Oct 2021 23:23:50 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926287724a1fc5ec8210568eaf0f15438481e47e302691e6ff9921b200ff6f9e`  
		Last Modified: Mon, 11 Oct 2021 23:23:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
