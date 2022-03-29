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
-	[`influxdb:1.9.6-data`](#influxdb196-data)
-	[`influxdb:1.9.6-data-alpine`](#influxdb196-data-alpine)
-	[`influxdb:1.9.6-meta`](#influxdb196-meta)
-	[`influxdb:1.9.6-meta-alpine`](#influxdb196-meta-alpine)
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
$ docker pull influxdb@sha256:c6d17cbd35cd147140505798e87f7f42fa375a17880ac126497147e23201ba03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7` - linux; amd64

```console
$ docker pull influxdb@sha256:c55e49d95a60b470ba401d6a96741ea6dfdc29fca6f579b2e975a4a34582211c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122363909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4e988acce0ffd129d0a56d537c926f3c009f3288fa0ee0c28931cd6171b5ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:48:00 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 19 Mar 2022 08:48:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 19 Mar 2022 08:48:07 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:48:07 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:48:07 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:48:07 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:48:07 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:48:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:48:07 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b8c85f9a7c7e62ff5b15877dd9c3edf3b1572f7e71aec1b08f4e83e2ef2610`  
		Last Modified: Sat, 19 Mar 2022 08:57:53 GMT  
		Size: 61.3 MB (61285875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe22cacce7f61602a5b5d3df4621e00faca8be5205bb568b8d07ac70ab3c8b1`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1347b49f4a6773b2d72a0ba1ef37c97d615b1688cb9d391a014a452c8f07e2`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0299f6b0a0ab15796154543959e115e3a63d2986ea8ccee10eac950c270eea`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:069bd61d81f0ef2d7f5af1f14b145c726fa7347cadf60edc112887502aecafcd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113504070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd92dd0f9b7d79a1eed394d7b7a63bf43c1748b61d8f4da162085f5e77e1f803`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 09:36:25 GMT
ADD file:e869f7223f16639eccabff7b2c6a85a7e6b075d0933c31f2fecae79c1c26d5be in / 
# Thu, 17 Mar 2022 09:36:26 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 20 Mar 2022 17:38:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 20 Mar 2022 17:38:38 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sun, 20 Mar 2022 17:38:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sun, 20 Mar 2022 17:38:52 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sun, 20 Mar 2022 17:38:53 GMT
EXPOSE 8086
# Sun, 20 Mar 2022 17:38:53 GMT
VOLUME [/var/lib/influxdb]
# Sun, 20 Mar 2022 17:38:54 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sun, 20 Mar 2022 17:38:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 20 Mar 2022 17:38:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 20 Mar 2022 17:38:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a9f775cd9058b832779f6c0dd1ca0fbb1417961dd87ca3ba6200f41aa283371b`  
		Last Modified: Thu, 17 Mar 2022 09:53:00 GMT  
		Size: 42.2 MB (42151366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c76f62b4a80636807fcffcd72fa68808c0faab499371e9e49ea3805cb8de8`  
		Last Modified: Sat, 19 Mar 2022 03:37:42 GMT  
		Size: 10.0 MB (9956816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe67020a39019149bd81805e6b89528643f4464d33964fe8bd1c39ed3c68dfd`  
		Last Modified: Sat, 19 Mar 2022 03:37:39 GMT  
		Size: 3.9 MB (3921814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dabf083c89b4d5b61d293c482bbff189bed8dfdba4ced2a3eb85a1ee237b61`  
		Last Modified: Sun, 20 Mar 2022 17:39:53 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dfca2cf831bf60d2b97d2938ac859247efbb96bb2a960f1141037f26a4c68a`  
		Last Modified: Sun, 20 Mar 2022 17:40:24 GMT  
		Size: 57.5 MB (57469503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9c740677876b1ab6a1ce25bd545099f0461b4452bca1d65321ee5e0012e01`  
		Last Modified: Sun, 20 Mar 2022 17:39:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09983857e81734debea688a64193486cbd25e3cc0c953263d6e4699ebd9c1365`  
		Last Modified: Sun, 20 Mar 2022 17:39:53 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a5baf65aefa3c81d0e3dc250c0e65f7223a9e5ad819dd3b3c0e40f5a8ca384`  
		Last Modified: Sun, 20 Mar 2022 17:39:53 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b123e277ecead2b16123e21ae54705442f7530860e6e90cb9fc797a4079ae235
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114514874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e20ac026d60d748729c16ddf5a4815f22ce679c4604ce8a0e8dd545753501ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:02 GMT
ADD file:eb07f8b0889bb0b4499fbba08599cdf04f3efaafdec453e96fa4175723f4fec1 in / 
# Thu, 17 Mar 2022 03:24:03 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:09:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 04:09:58 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 19 Mar 2022 04:10:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 19 Mar 2022 04:10:06 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 04:10:06 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 04:10:07 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 04:10:09 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 04:10:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 04:10:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:10:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0d6ecff05d590b97ebc357d19bd439c17d4142359ceceb25dda468284e978583`  
		Last Modified: Thu, 17 Mar 2022 03:32:27 GMT  
		Size: 43.2 MB (43213043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf8187d7f23f7722584cf9a7359b8e6859ca891c112d0398819cecdac7fa008`  
		Last Modified: Thu, 17 Mar 2022 22:24:30 GMT  
		Size: 10.2 MB (10217652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9ad8247187d77aea7d1a40486c48551a68a63e2b6be93a43c47cc27d726beb`  
		Last Modified: Thu, 17 Mar 2022 22:24:29 GMT  
		Size: 3.9 MB (3874519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35351da126f53a65477046cd67ef9c3e5dfd0897c6e735d167f5df8ce3adf9f5`  
		Last Modified: Sat, 19 Mar 2022 04:12:25 GMT  
		Size: 2.8 KB (2824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bfa83b8bfc9aad3fcee8614be308820a5af31316b3bccf2063246adabb8b37`  
		Last Modified: Sat, 19 Mar 2022 04:12:33 GMT  
		Size: 57.2 MB (57205117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714ce8acca608065e143772f4da5a516a702d652397f3eadf0741a5d45772fac`  
		Last Modified: Sat, 19 Mar 2022 04:12:25 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1416e1173a8f0ad401b7708c2b040ac39dbb8d03d994aa696a2acb88d550d44`  
		Last Modified: Sat, 19 Mar 2022 04:12:25 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf5e3ba5f032e96003cb05a3fcdc76ca31537900b07fdaf9db58464fbcaf3b9`  
		Last Modified: Sat, 19 Mar 2022 04:12:25 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-alpine`

```console
$ docker pull influxdb@sha256:17df73614ac561229d94073c87bfbc790be0615c375c5281ef964ef96d462469
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:a3dafb37366a7533561a2bbbdbaa47cb4b569e6e7feb4264c4842d703e0010c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65327591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe2b09dec88ac7e0bea7e69d6f93adc148038ae0799fec272ed54420618503`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:48:11 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 19 Mar 2022 08:49:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:49:05 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:49:05 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:49:06 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:49:06 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:49:06 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:49:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:49:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6455a31641f738dbcbb40f8d09d3898261e17b9f803e6735d1a96dd0f5691c`  
		Last Modified: Sat, 19 Mar 2022 08:58:10 GMT  
		Size: 61.0 MB (61034507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0c6bc63d0e746e1c692736de3ab75fa0985082c13cd31de2b3452c12a805de`  
		Last Modified: Sat, 19 Mar 2022 08:58:02 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8be17136db2382a835a69c2ce05c2e40dd194335c117b75cb28073a6607b88`  
		Last Modified: Sat, 19 Mar 2022 08:58:02 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883757d7fdc33b921dc17c22daadab0f6bf88415c24269494a240cc49f049bcd`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data`

```console
$ docker pull influxdb@sha256:507374d0e908b584688c52dce6544e0520944be5745d7a5479741d57a62e1e9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-data` - linux; amd64

```console
$ docker pull influxdb@sha256:47c06c25a5fdc5ee580872aa27bd136aca18242d12845df18ee61ac27ac59cf3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (149027692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d1f8fcc2466c5ee7310496e9701730c47c9ea7e75354a6831564e67c7d93e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:49:18 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 19 Mar 2022 08:49:27 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:49:27 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:49:27 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:49:27 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:49:27 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:49:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:49:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:49:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b42564246e81cc81844d8386fcca8681f8d97f100c4b8fbd586dfcf9f13fc0`  
		Last Modified: Sat, 19 Mar 2022 08:58:31 GMT  
		Size: 87.9 MB (87949599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0c45aaea6c8ec10a7949e398d0d9ca6855f9af34f90977df8c88efdc8f425f`  
		Last Modified: Sat, 19 Mar 2022 08:58:20 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca226e02e2407dce227ea358b4f5f424e0efd611d0f4af9b50e5fa10f25276d1`  
		Last Modified: Sat, 19 Mar 2022 08:58:19 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96c6f3aa11cfd437713892e8b2ef1dfe4ec4652ad9ac9915005b2d9a1ebc219`  
		Last Modified: Sat, 19 Mar 2022 08:58:19 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-data-alpine`

```console
$ docker pull influxdb@sha256:8bbfd60e328f095ef57a815f734c28e0cdbdd432120f1aa47d9a70562c016ff3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f451151c1e0c0e42fd17adf36910ccf39558f1ed5b892517bf475e6592cd1dc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91933934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e067cde8425de742a3bfd72b4a1b6e688f3d258da4b41b7438d886c74ae55361`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:49:30 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 19 Mar 2022 08:50:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:50:17 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:50:17 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:50:17 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:50:17 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:50:17 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:50:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:50:17 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55582a1d5c37a8718465ff82f1de765282286aee86a1b1f2b07c3eb782c3a0`  
		Last Modified: Sat, 19 Mar 2022 08:58:51 GMT  
		Size: 87.6 MB (87640792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195fb0bc74b3dca96271b128a97bcce4b5d4d1601a8a7de14910a06c1d29dca0`  
		Last Modified: Sat, 19 Mar 2022 08:58:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205dd80208a2ee71917bc034b1b5e25ed189eb17ade11f5eb359a724330628f1`  
		Last Modified: Sat, 19 Mar 2022 08:58:41 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b6ff983d87bf4581e54792e71fb862ab238f5bd888a9a866d4f7bbb7649e21`  
		Last Modified: Sat, 19 Mar 2022 08:58:40 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta`

```console
$ docker pull influxdb@sha256:931825278815c8b6c6c61c9681418fcf39f866820e89076c8e59140f4e09890e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:1e7b2293e04a3c6b2337d79235ace2f207fa654ffe56dfce1997d124e58c7609
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84211162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e1222e454a4b6ff1477cd12aa1439f47b75f559cba7b8b5b5c8a93441a508f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:49:18 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 19 Mar 2022 08:50:31 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:50:31 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:50:31 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:50:31 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:50:31 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:50:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:50:31 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e29f1bc2d40f8af063c58ac0d19b03d2d81a85f0841c40c87be7a97031f69f`  
		Last Modified: Sat, 19 Mar 2022 08:59:04 GMT  
		Size: 23.1 MB (23134274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f93fd36a6c647c23d655dcf3a0f232ca13f6bceba2f449eb5893e4b49bb918d`  
		Last Modified: Sat, 19 Mar 2022 08:59:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2b1752d0da3c4986b19a9c9b3f8d9f2fc6a9d885de4112ef3a20cd59d6f47a`  
		Last Modified: Sat, 19 Mar 2022 08:59:01 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7-meta-alpine`

```console
$ docker pull influxdb@sha256:27be7ea6cef851c877ab0b7e7d137c141ad4d605b5a2d3d93217790ffef836b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:7a3f994d57a2f2ce2acf37cf958f6e96f07456fac65c7799efa18c07afa5ab9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27295490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1cdff24d08c6cdde65beb5b53d51a6ea9328f732985e4429f2c493474ce030b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:49:30 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 19 Mar 2022 08:51:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:51:14 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:51:14 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:51:14 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:51:15 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:51:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:51:15 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17af8ab5af2fa32987b86a594dddeb85019de439627c830beba632db363c473`  
		Last Modified: Sat, 19 Mar 2022 08:59:16 GMT  
		Size: 23.0 MB (23003551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46d4b983e272a019b1c2d2bbf053d138f8b53a0ff4add67e6455636f80a5bd3`  
		Last Modified: Sat, 19 Mar 2022 08:59:13 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19be00089aad3e208f7e1f0660e15b1dc27d88a4cde0c28a707820f0deaba33`  
		Last Modified: Sat, 19 Mar 2022 08:59:13 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11`

```console
$ docker pull influxdb@sha256:c6d17cbd35cd147140505798e87f7f42fa375a17880ac126497147e23201ba03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.7.11` - linux; amd64

```console
$ docker pull influxdb@sha256:c55e49d95a60b470ba401d6a96741ea6dfdc29fca6f579b2e975a4a34582211c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122363909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4e988acce0ffd129d0a56d537c926f3c009f3288fa0ee0c28931cd6171b5ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:48:00 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 19 Mar 2022 08:48:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 19 Mar 2022 08:48:07 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:48:07 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:48:07 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:48:07 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:48:07 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:48:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:48:07 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b8c85f9a7c7e62ff5b15877dd9c3edf3b1572f7e71aec1b08f4e83e2ef2610`  
		Last Modified: Sat, 19 Mar 2022 08:57:53 GMT  
		Size: 61.3 MB (61285875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe22cacce7f61602a5b5d3df4621e00faca8be5205bb568b8d07ac70ab3c8b1`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1347b49f4a6773b2d72a0ba1ef37c97d615b1688cb9d391a014a452c8f07e2`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0299f6b0a0ab15796154543959e115e3a63d2986ea8ccee10eac950c270eea`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:069bd61d81f0ef2d7f5af1f14b145c726fa7347cadf60edc112887502aecafcd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113504070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd92dd0f9b7d79a1eed394d7b7a63bf43c1748b61d8f4da162085f5e77e1f803`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 09:36:25 GMT
ADD file:e869f7223f16639eccabff7b2c6a85a7e6b075d0933c31f2fecae79c1c26d5be in / 
# Thu, 17 Mar 2022 09:36:26 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 20 Mar 2022 17:38:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 20 Mar 2022 17:38:38 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sun, 20 Mar 2022 17:38:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sun, 20 Mar 2022 17:38:52 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sun, 20 Mar 2022 17:38:53 GMT
EXPOSE 8086
# Sun, 20 Mar 2022 17:38:53 GMT
VOLUME [/var/lib/influxdb]
# Sun, 20 Mar 2022 17:38:54 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sun, 20 Mar 2022 17:38:54 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 20 Mar 2022 17:38:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 20 Mar 2022 17:38:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a9f775cd9058b832779f6c0dd1ca0fbb1417961dd87ca3ba6200f41aa283371b`  
		Last Modified: Thu, 17 Mar 2022 09:53:00 GMT  
		Size: 42.2 MB (42151366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c76f62b4a80636807fcffcd72fa68808c0faab499371e9e49ea3805cb8de8`  
		Last Modified: Sat, 19 Mar 2022 03:37:42 GMT  
		Size: 10.0 MB (9956816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe67020a39019149bd81805e6b89528643f4464d33964fe8bd1c39ed3c68dfd`  
		Last Modified: Sat, 19 Mar 2022 03:37:39 GMT  
		Size: 3.9 MB (3921814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dabf083c89b4d5b61d293c482bbff189bed8dfdba4ced2a3eb85a1ee237b61`  
		Last Modified: Sun, 20 Mar 2022 17:39:53 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dfca2cf831bf60d2b97d2938ac859247efbb96bb2a960f1141037f26a4c68a`  
		Last Modified: Sun, 20 Mar 2022 17:40:24 GMT  
		Size: 57.5 MB (57469503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be9c740677876b1ab6a1ce25bd545099f0461b4452bca1d65321ee5e0012e01`  
		Last Modified: Sun, 20 Mar 2022 17:39:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09983857e81734debea688a64193486cbd25e3cc0c953263d6e4699ebd9c1365`  
		Last Modified: Sun, 20 Mar 2022 17:39:53 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a5baf65aefa3c81d0e3dc250c0e65f7223a9e5ad819dd3b3c0e40f5a8ca384`  
		Last Modified: Sun, 20 Mar 2022 17:39:53 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.7.11` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:b123e277ecead2b16123e21ae54705442f7530860e6e90cb9fc797a4079ae235
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114514874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e20ac026d60d748729c16ddf5a4815f22ce679c4604ce8a0e8dd545753501ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:02 GMT
ADD file:eb07f8b0889bb0b4499fbba08599cdf04f3efaafdec453e96fa4175723f4fec1 in / 
# Thu, 17 Mar 2022 03:24:03 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:09:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 04:09:58 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 19 Mar 2022 04:10:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 19 Mar 2022 04:10:06 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 04:10:06 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 04:10:07 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 04:10:09 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 04:10:10 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 04:10:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:10:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0d6ecff05d590b97ebc357d19bd439c17d4142359ceceb25dda468284e978583`  
		Last Modified: Thu, 17 Mar 2022 03:32:27 GMT  
		Size: 43.2 MB (43213043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf8187d7f23f7722584cf9a7359b8e6859ca891c112d0398819cecdac7fa008`  
		Last Modified: Thu, 17 Mar 2022 22:24:30 GMT  
		Size: 10.2 MB (10217652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9ad8247187d77aea7d1a40486c48551a68a63e2b6be93a43c47cc27d726beb`  
		Last Modified: Thu, 17 Mar 2022 22:24:29 GMT  
		Size: 3.9 MB (3874519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35351da126f53a65477046cd67ef9c3e5dfd0897c6e735d167f5df8ce3adf9f5`  
		Last Modified: Sat, 19 Mar 2022 04:12:25 GMT  
		Size: 2.8 KB (2824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bfa83b8bfc9aad3fcee8614be308820a5af31316b3bccf2063246adabb8b37`  
		Last Modified: Sat, 19 Mar 2022 04:12:33 GMT  
		Size: 57.2 MB (57205117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714ce8acca608065e143772f4da5a516a702d652397f3eadf0741a5d45772fac`  
		Last Modified: Sat, 19 Mar 2022 04:12:25 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1416e1173a8f0ad401b7708c2b040ac39dbb8d03d994aa696a2acb88d550d44`  
		Last Modified: Sat, 19 Mar 2022 04:12:25 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf5e3ba5f032e96003cb05a3fcdc76ca31537900b07fdaf9db58464fbcaf3b9`  
		Last Modified: Sat, 19 Mar 2022 04:12:25 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-alpine`

```console
$ docker pull influxdb@sha256:17df73614ac561229d94073c87bfbc790be0615c375c5281ef964ef96d462469
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:a3dafb37366a7533561a2bbbdbaa47cb4b569e6e7feb4264c4842d703e0010c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65327591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3fe2b09dec88ac7e0bea7e69d6f93adc148038ae0799fec272ed54420618503`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:48:11 GMT
ENV INFLUXDB_VERSION=1.7.11
# Sat, 19 Mar 2022 08:49:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:49:05 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:49:05 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:49:06 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:49:06 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:49:06 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:49:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:49:06 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6455a31641f738dbcbb40f8d09d3898261e17b9f803e6735d1a96dd0f5691c`  
		Last Modified: Sat, 19 Mar 2022 08:58:10 GMT  
		Size: 61.0 MB (61034507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0c6bc63d0e746e1c692736de3ab75fa0985082c13cd31de2b3452c12a805de`  
		Last Modified: Sat, 19 Mar 2022 08:58:02 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8be17136db2382a835a69c2ce05c2e40dd194335c117b75cb28073a6607b88`  
		Last Modified: Sat, 19 Mar 2022 08:58:02 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883757d7fdc33b921dc17c22daadab0f6bf88415c24269494a240cc49f049bcd`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data`

```console
$ docker pull influxdb@sha256:507374d0e908b584688c52dce6544e0520944be5745d7a5479741d57a62e1e9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-data` - linux; amd64

```console
$ docker pull influxdb@sha256:47c06c25a5fdc5ee580872aa27bd136aca18242d12845df18ee61ac27ac59cf3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (149027692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d1f8fcc2466c5ee7310496e9701730c47c9ea7e75354a6831564e67c7d93e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:49:18 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 19 Mar 2022 08:49:27 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:49:27 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:49:27 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:49:27 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:49:27 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:49:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:49:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:49:28 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b42564246e81cc81844d8386fcca8681f8d97f100c4b8fbd586dfcf9f13fc0`  
		Last Modified: Sat, 19 Mar 2022 08:58:31 GMT  
		Size: 87.9 MB (87949599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0c45aaea6c8ec10a7949e398d0d9ca6855f9af34f90977df8c88efdc8f425f`  
		Last Modified: Sat, 19 Mar 2022 08:58:20 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca226e02e2407dce227ea358b4f5f424e0efd611d0f4af9b50e5fa10f25276d1`  
		Last Modified: Sat, 19 Mar 2022 08:58:19 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96c6f3aa11cfd437713892e8b2ef1dfe4ec4652ad9ac9915005b2d9a1ebc219`  
		Last Modified: Sat, 19 Mar 2022 08:58:19 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-data-alpine`

```console
$ docker pull influxdb@sha256:8bbfd60e328f095ef57a815f734c28e0cdbdd432120f1aa47d9a70562c016ff3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f451151c1e0c0e42fd17adf36910ccf39558f1ed5b892517bf475e6592cd1dc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91933934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e067cde8425de742a3bfd72b4a1b6e688f3d258da4b41b7438d886c74ae55361`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:49:30 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 19 Mar 2022 08:50:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:50:17 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:50:17 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:50:17 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:50:17 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:50:17 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:50:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:50:17 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55582a1d5c37a8718465ff82f1de765282286aee86a1b1f2b07c3eb782c3a0`  
		Last Modified: Sat, 19 Mar 2022 08:58:51 GMT  
		Size: 87.6 MB (87640792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195fb0bc74b3dca96271b128a97bcce4b5d4d1601a8a7de14910a06c1d29dca0`  
		Last Modified: Sat, 19 Mar 2022 08:58:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205dd80208a2ee71917bc034b1b5e25ed189eb17ade11f5eb359a724330628f1`  
		Last Modified: Sat, 19 Mar 2022 08:58:41 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b6ff983d87bf4581e54792e71fb862ab238f5bd888a9a866d4f7bbb7649e21`  
		Last Modified: Sat, 19 Mar 2022 08:58:40 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta`

```console
$ docker pull influxdb@sha256:931825278815c8b6c6c61c9681418fcf39f866820e89076c8e59140f4e09890e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:1e7b2293e04a3c6b2337d79235ace2f207fa654ffe56dfce1997d124e58c7609
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84211162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e1222e454a4b6ff1477cd12aa1439f47b75f559cba7b8b5b5c8a93441a508f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:49:18 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 19 Mar 2022 08:50:31 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:50:31 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:50:31 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:50:31 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:50:31 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:50:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:50:31 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e29f1bc2d40f8af063c58ac0d19b03d2d81a85f0841c40c87be7a97031f69f`  
		Last Modified: Sat, 19 Mar 2022 08:59:04 GMT  
		Size: 23.1 MB (23134274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f93fd36a6c647c23d655dcf3a0f232ca13f6bceba2f449eb5893e4b49bb918d`  
		Last Modified: Sat, 19 Mar 2022 08:59:01 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2b1752d0da3c4986b19a9c9b3f8d9f2fc6a9d885de4112ef3a20cd59d6f47a`  
		Last Modified: Sat, 19 Mar 2022 08:59:01 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.7.11-meta-alpine`

```console
$ docker pull influxdb@sha256:27be7ea6cef851c877ab0b7e7d137c141ad4d605b5a2d3d93217790ffef836b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.7.11-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:7a3f994d57a2f2ce2acf37cf958f6e96f07456fac65c7799efa18c07afa5ab9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27295490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1cdff24d08c6cdde65beb5b53d51a6ea9328f732985e4429f2c493474ce030b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:49:30 GMT
ENV INFLUXDB_VERSION=1.7.11-c1.7.11
# Sat, 19 Mar 2022 08:51:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:51:14 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:51:14 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:51:14 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:51:15 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:51:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:51:15 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17af8ab5af2fa32987b86a594dddeb85019de439627c830beba632db363c473`  
		Last Modified: Sat, 19 Mar 2022 08:59:16 GMT  
		Size: 23.0 MB (23003551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46d4b983e272a019b1c2d2bbf053d138f8b53a0ff4add67e6455636f80a5bd3`  
		Last Modified: Sat, 19 Mar 2022 08:59:13 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19be00089aad3e208f7e1f0660e15b1dc27d88a4cde0c28a707820f0deaba33`  
		Last Modified: Sat, 19 Mar 2022 08:59:13 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8`

```console
$ docker pull influxdb@sha256:e1ffb5ec80549a930bdcf24035ee452da0780f030487fb50481820940c620a40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8` - linux; amd64

```console
$ docker pull influxdb@sha256:f2417b3494ae3a0a427ffd17b35882c5a840a1f731377c680d650561eb97c2e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115968184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a92f4c2e0cfc6545f25744d2545fbf753fff2438236759dab9e41ced77cc82c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:51:22 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sat, 19 Mar 2022 08:51:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 19 Mar 2022 08:51:27 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:51:27 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:51:27 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:51:27 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:51:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:51:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:51:27 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4811b21b97565307f8c2c42fc869ca5061f629ee6cb627e4611703ab3225eea`  
		Last Modified: Sat, 19 Mar 2022 08:59:36 GMT  
		Size: 54.9 MB (54890151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db13646b10fd1fb8bcbd14e396b02039095c9965945279b4d4eef4c138e5d36e`  
		Last Modified: Sat, 19 Mar 2022 08:59:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5c296ff9834cfa097ed81df55628ba51029570f21a7b694316a836295380e0`  
		Last Modified: Sat, 19 Mar 2022 08:59:29 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3178c3dd38039ee33aa8902299097560371d94d06e9fb606b12c942b0f3d9506`  
		Last Modified: Sat, 19 Mar 2022 08:59:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:42c2d969737adabfa9e9cef4dd217270f9cfb97f29d41361066a15762b182faa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107651964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01be217e9dea728fb4bcfad6a8fe368c299761168a4555da6397b4e11d024eeb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 09:36:25 GMT
ADD file:e869f7223f16639eccabff7b2c6a85a7e6b075d0933c31f2fecae79c1c26d5be in / 
# Thu, 17 Mar 2022 09:36:26 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 20 Mar 2022 17:38:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 20 Mar 2022 17:39:07 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sun, 20 Mar 2022 17:39:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sun, 20 Mar 2022 17:39:20 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sun, 20 Mar 2022 17:39:21 GMT
EXPOSE 8086
# Sun, 20 Mar 2022 17:39:21 GMT
VOLUME [/var/lib/influxdb]
# Sun, 20 Mar 2022 17:39:22 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sun, 20 Mar 2022 17:39:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 20 Mar 2022 17:39:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 20 Mar 2022 17:39:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a9f775cd9058b832779f6c0dd1ca0fbb1417961dd87ca3ba6200f41aa283371b`  
		Last Modified: Thu, 17 Mar 2022 09:53:00 GMT  
		Size: 42.2 MB (42151366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c76f62b4a80636807fcffcd72fa68808c0faab499371e9e49ea3805cb8de8`  
		Last Modified: Sat, 19 Mar 2022 03:37:42 GMT  
		Size: 10.0 MB (9956816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe67020a39019149bd81805e6b89528643f4464d33964fe8bd1c39ed3c68dfd`  
		Last Modified: Sat, 19 Mar 2022 03:37:39 GMT  
		Size: 3.9 MB (3921814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dabf083c89b4d5b61d293c482bbff189bed8dfdba4ced2a3eb85a1ee237b61`  
		Last Modified: Sun, 20 Mar 2022 17:39:53 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56b940c1e9e2377291092f96b90d3d6baebf7a7a5b5e3c9aa61027f44957aa`  
		Last Modified: Sun, 20 Mar 2022 17:41:03 GMT  
		Size: 51.6 MB (51617401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b229066ab98468dc3100a4ad4992dc41f3a2b21e8e51b3de41f319491ad92de`  
		Last Modified: Sun, 20 Mar 2022 17:40:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41298bb0edb20b21c1a3ed42b80bed690cf420b93a9a3fc42b7f8fc1a8ee77fa`  
		Last Modified: Sun, 20 Mar 2022 17:40:36 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71729132b21a6611ce18e480b3ac7544e35ede9d70ca8bca70d358d88dbed17`  
		Last Modified: Sun, 20 Mar 2022 17:40:36 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:796ce62651622aadd094a0cd0b4fd28bb5812efa1916caa25cff0e5137ec227d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108544067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d21eb812a7668d39f93f4e51910f1270249b03b9a3aac15a0e311b0fa1663e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:02 GMT
ADD file:eb07f8b0889bb0b4499fbba08599cdf04f3efaafdec453e96fa4175723f4fec1 in / 
# Thu, 17 Mar 2022 03:24:03 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:09:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 04:10:24 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sat, 19 Mar 2022 04:10:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 19 Mar 2022 04:10:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 04:10:30 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 04:10:31 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 04:10:33 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 04:10:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 04:10:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:10:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0d6ecff05d590b97ebc357d19bd439c17d4142359ceceb25dda468284e978583`  
		Last Modified: Thu, 17 Mar 2022 03:32:27 GMT  
		Size: 43.2 MB (43213043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf8187d7f23f7722584cf9a7359b8e6859ca891c112d0398819cecdac7fa008`  
		Last Modified: Thu, 17 Mar 2022 22:24:30 GMT  
		Size: 10.2 MB (10217652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9ad8247187d77aea7d1a40486c48551a68a63e2b6be93a43c47cc27d726beb`  
		Last Modified: Thu, 17 Mar 2022 22:24:29 GMT  
		Size: 3.9 MB (3874519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35351da126f53a65477046cd67ef9c3e5dfd0897c6e735d167f5df8ce3adf9f5`  
		Last Modified: Sat, 19 Mar 2022 04:12:25 GMT  
		Size: 2.8 KB (2824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b799927fec87191cf721322b3055d26d93d3100dd67c7aa2d015ab21401624`  
		Last Modified: Sat, 19 Mar 2022 04:12:53 GMT  
		Size: 51.2 MB (51234310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5953a5bfd76286b1e27bb25914c2f807f4ac55e43af95fa28734378b31943e8`  
		Last Modified: Sat, 19 Mar 2022 04:12:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce049e3149d4f3619d183ae514d3c9cbdb73a105a25150930191459ebb46a935`  
		Last Modified: Sat, 19 Mar 2022 04:12:45 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1999ab0b268b2a0faa0287e03df3ebd6813dd0375d603146aff9c850e7517`  
		Last Modified: Sat, 19 Mar 2022 04:12:45 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-alpine`

```console
$ docker pull influxdb@sha256:71515740ee6364f962cc5f38b564b086ef3e9fd47071f65934fdd2980dfc3e6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:399536a2083884b305405f9dcd41c3e39331f805fdda87d4c331da86f1675d3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58952663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aff85dfe21a8daa7e34a634592e74d0b49326ee44109440047e6cbcf50e4b9d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:51:30 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sat, 19 Mar 2022 08:52:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:52:15 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:52:15 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:52:15 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:52:15 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:52:16 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:52:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:52:16 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881070f84f6b09f6403e878b5c62226c519b34aa93d62671dc1525e5809ec5dd`  
		Last Modified: Sat, 19 Mar 2022 08:59:53 GMT  
		Size: 54.7 MB (54659579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4a3f466a34eaa8cb2baecd8891bb1339da5f67ca0f3f89c39a2ebd5efaf876`  
		Last Modified: Sat, 19 Mar 2022 08:59:45 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64fc0cfbe868b2aad8d972fc4874512d68a73bac9406f43616ea3f54031d436`  
		Last Modified: Sat, 19 Mar 2022 08:59:45 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f8ca533a4bcfe50ab55ef34b918dd5fbd70d2d29ed531b739ff33d0872db3`  
		Last Modified: Sat, 19 Mar 2022 08:59:45 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data`

```console
$ docker pull influxdb@sha256:4adfd68bca455c5c804ad58e4198991d2174de8ac9f3d09a5506d2313132ec5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data` - linux; amd64

```console
$ docker pull influxdb@sha256:ba9a258ea5df77d3788b60655ff7034525f0ae60edf607007e23b459eaf101df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117787247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc9a2aea6ebfb56517ef166d9738e75f6e72019dcf6a8740c32f5f5ae94c9b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:52:18 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:52:24 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:52:24 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:52:24 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:52:24 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:52:24 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:52:24 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:52:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:52:24 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550eb93b184ae327ebbe4e87ba6c3f6b72123e2ff51cdbf8b894e380c0bc9f78`  
		Last Modified: Sat, 19 Mar 2022 09:00:10 GMT  
		Size: 56.7 MB (56709155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcd6f8e29a97d8f8e9fc790faefe89969811575bef2e745063df15e584f9922`  
		Last Modified: Sat, 19 Mar 2022 09:00:03 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2694323f619607cd2e22f8fcc0558fd67d95225a567dc9ee7a5869d3acf190`  
		Last Modified: Sat, 19 Mar 2022 09:00:03 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08d6800f658e5286060c2cec18f42454d14f14f9f9ef709eae90f1cf4494f45`  
		Last Modified: Sat, 19 Mar 2022 09:00:03 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-data-alpine`

```console
$ docker pull influxdb@sha256:7102c7ea58d0a3729140ab83049d423e0f137c7948e69ced1f82becf4e452bc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ce0834c6c67f4955122723fd09db4e983cd013adedff43e74c05146581a0175b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60796867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e69c05e78ef8c082da94810348cb501b5d32f210cf04d092989b17e2a0e8acff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:52:27 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:53:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:53:11 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:53:11 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:53:11 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:53:11 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:53:11 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:53:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:53:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1352e4303694301bbf45526ed2c20f6e2fbe7e6434cd8fe0e79bc9869ffe7b35`  
		Last Modified: Sat, 19 Mar 2022 09:00:30 GMT  
		Size: 56.5 MB (56503726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905d7114896f9e29bd5019dcbe803a2b817d827c3828e375485cc5dc2c35e00b`  
		Last Modified: Sat, 19 Mar 2022 09:00:23 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfa2ebc20c8b652b37aad6032d184c6f2b2925f1c872c8dea5e718e32045032`  
		Last Modified: Sat, 19 Mar 2022 09:00:23 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b410d84e27dad55d0faab8229945215a48627443e6e6824328fe6672acb911b1`  
		Last Modified: Sat, 19 Mar 2022 09:00:23 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta`

```console
$ docker pull influxdb@sha256:d0240f21f89ae3d7cec4acd7f8cd750f44d0dd00e0ba18f508969130dff47471
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:b76d35eb1b56e57f22a38b623f452c15770822e38f9f309b870fd15588757801
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84493855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:081ce2abdbb8d32f017e6fa5582fd9bd760c9f9004f91ab420a02940519e09e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:52:18 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:53:19 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:53:19 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:53:19 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:53:19 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:53:19 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:53:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:53:19 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4992723de53d8c0fbf3427d7d82e32278cdc6fb974adf1f202d282f2803846b3`  
		Last Modified: Sat, 19 Mar 2022 09:00:46 GMT  
		Size: 23.4 MB (23416969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f938aaece62656aeed448d46875c5090e41b32f0dc6292cef7ad512a7a6f67`  
		Last Modified: Sat, 19 Mar 2022 09:00:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38110311c491242933400eb982b1c811e8ceef8cc16a07d8396623de246a369`  
		Last Modified: Sat, 19 Mar 2022 09:00:42 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8-meta-alpine`

```console
$ docker pull influxdb@sha256:f9ebef848c77b595c77ee0eaf6ab978b8dc69468ef104b3f9b7fa4a88ae10092
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:866f5587dba36266786414c65d3b322628296778c30561297a69b84070f2e5e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27584917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83b8b4d5495d637ee6649737dda3c65582ed6d18009f548712d8a1fbc65488`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:52:27 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:54:02 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:54:02 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:54:02 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:54:02 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:54:02 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:54:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:54:02 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0043723f2d668517ea2dd3c7f050fc58c203aef11bc2f8a374f2f98397286d5`  
		Last Modified: Sat, 19 Mar 2022 09:01:01 GMT  
		Size: 23.3 MB (23292980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005777352236f2ef3b11e4ba9451d590459f4f8d684f356cece973ba5782c54a`  
		Last Modified: Sat, 19 Mar 2022 09:00:58 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5c86b33a986181c1f1bb66954a31888f6ed2907d490db462a2da4a8a28060`  
		Last Modified: Sat, 19 Mar 2022 09:00:58 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10`

```console
$ docker pull influxdb@sha256:e1ffb5ec80549a930bdcf24035ee452da0780f030487fb50481820940c620a40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `influxdb:1.8.10` - linux; amd64

```console
$ docker pull influxdb@sha256:f2417b3494ae3a0a427ffd17b35882c5a840a1f731377c680d650561eb97c2e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115968184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a92f4c2e0cfc6545f25744d2545fbf753fff2438236759dab9e41ced77cc82c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:51:22 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sat, 19 Mar 2022 08:51:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 19 Mar 2022 08:51:27 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:51:27 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:51:27 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:51:27 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:51:27 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:51:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:51:27 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4811b21b97565307f8c2c42fc869ca5061f629ee6cb627e4611703ab3225eea`  
		Last Modified: Sat, 19 Mar 2022 08:59:36 GMT  
		Size: 54.9 MB (54890151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db13646b10fd1fb8bcbd14e396b02039095c9965945279b4d4eef4c138e5d36e`  
		Last Modified: Sat, 19 Mar 2022 08:59:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5c296ff9834cfa097ed81df55628ba51029570f21a7b694316a836295380e0`  
		Last Modified: Sat, 19 Mar 2022 08:59:29 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3178c3dd38039ee33aa8902299097560371d94d06e9fb606b12c942b0f3d9506`  
		Last Modified: Sat, 19 Mar 2022 08:59:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm variant v7

```console
$ docker pull influxdb@sha256:42c2d969737adabfa9e9cef4dd217270f9cfb97f29d41361066a15762b182faa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107651964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01be217e9dea728fb4bcfad6a8fe368c299761168a4555da6397b4e11d024eeb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 09:36:25 GMT
ADD file:e869f7223f16639eccabff7b2c6a85a7e6b075d0933c31f2fecae79c1c26d5be in / 
# Thu, 17 Mar 2022 09:36:26 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 20 Mar 2022 17:38:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 20 Mar 2022 17:39:07 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sun, 20 Mar 2022 17:39:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sun, 20 Mar 2022 17:39:20 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sun, 20 Mar 2022 17:39:21 GMT
EXPOSE 8086
# Sun, 20 Mar 2022 17:39:21 GMT
VOLUME [/var/lib/influxdb]
# Sun, 20 Mar 2022 17:39:22 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sun, 20 Mar 2022 17:39:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sun, 20 Mar 2022 17:39:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 20 Mar 2022 17:39:23 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a9f775cd9058b832779f6c0dd1ca0fbb1417961dd87ca3ba6200f41aa283371b`  
		Last Modified: Thu, 17 Mar 2022 09:53:00 GMT  
		Size: 42.2 MB (42151366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c76f62b4a80636807fcffcd72fa68808c0faab499371e9e49ea3805cb8de8`  
		Last Modified: Sat, 19 Mar 2022 03:37:42 GMT  
		Size: 10.0 MB (9956816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe67020a39019149bd81805e6b89528643f4464d33964fe8bd1c39ed3c68dfd`  
		Last Modified: Sat, 19 Mar 2022 03:37:39 GMT  
		Size: 3.9 MB (3921814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dabf083c89b4d5b61d293c482bbff189bed8dfdba4ced2a3eb85a1ee237b61`  
		Last Modified: Sun, 20 Mar 2022 17:39:53 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56b940c1e9e2377291092f96b90d3d6baebf7a7a5b5e3c9aa61027f44957aa`  
		Last Modified: Sun, 20 Mar 2022 17:41:03 GMT  
		Size: 51.6 MB (51617401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b229066ab98468dc3100a4ad4992dc41f3a2b21e8e51b3de41f319491ad92de`  
		Last Modified: Sun, 20 Mar 2022 17:40:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41298bb0edb20b21c1a3ed42b80bed690cf420b93a9a3fc42b7f8fc1a8ee77fa`  
		Last Modified: Sun, 20 Mar 2022 17:40:36 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71729132b21a6611ce18e480b3ac7544e35ede9d70ca8bca70d358d88dbed17`  
		Last Modified: Sun, 20 Mar 2022 17:40:36 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:1.8.10` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:796ce62651622aadd094a0cd0b4fd28bb5812efa1916caa25cff0e5137ec227d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108544067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d21eb812a7668d39f93f4e51910f1270249b03b9a3aac15a0e311b0fa1663e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:02 GMT
ADD file:eb07f8b0889bb0b4499fbba08599cdf04f3efaafdec453e96fa4175723f4fec1 in / 
# Thu, 17 Mar 2022 03:24:03 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:09:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 04:10:24 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sat, 19 Mar 2022 04:10:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     gpg --batch --verify influxdb_${INFLUXDB_VERSION}_${ARCH}.deb.asc influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     dpkg -i influxdb_${INFLUXDB_VERSION}_${ARCH}.deb &&     rm -f influxdb_${INFLUXDB_VERSION}_${ARCH}.deb*
# Sat, 19 Mar 2022 04:10:30 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 04:10:30 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 04:10:31 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 04:10:33 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 04:10:34 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 04:10:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:10:35 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:0d6ecff05d590b97ebc357d19bd439c17d4142359ceceb25dda468284e978583`  
		Last Modified: Thu, 17 Mar 2022 03:32:27 GMT  
		Size: 43.2 MB (43213043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf8187d7f23f7722584cf9a7359b8e6859ca891c112d0398819cecdac7fa008`  
		Last Modified: Thu, 17 Mar 2022 22:24:30 GMT  
		Size: 10.2 MB (10217652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9ad8247187d77aea7d1a40486c48551a68a63e2b6be93a43c47cc27d726beb`  
		Last Modified: Thu, 17 Mar 2022 22:24:29 GMT  
		Size: 3.9 MB (3874519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35351da126f53a65477046cd67ef9c3e5dfd0897c6e735d167f5df8ce3adf9f5`  
		Last Modified: Sat, 19 Mar 2022 04:12:25 GMT  
		Size: 2.8 KB (2824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b799927fec87191cf721322b3055d26d93d3100dd67c7aa2d015ab21401624`  
		Last Modified: Sat, 19 Mar 2022 04:12:53 GMT  
		Size: 51.2 MB (51234310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5953a5bfd76286b1e27bb25914c2f807f4ac55e43af95fa28734378b31943e8`  
		Last Modified: Sat, 19 Mar 2022 04:12:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce049e3149d4f3619d183ae514d3c9cbdb73a105a25150930191459ebb46a935`  
		Last Modified: Sat, 19 Mar 2022 04:12:45 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c1999ab0b268b2a0faa0287e03df3ebd6813dd0375d603146aff9c850e7517`  
		Last Modified: Sat, 19 Mar 2022 04:12:45 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-alpine`

```console
$ docker pull influxdb@sha256:71515740ee6364f962cc5f38b564b086ef3e9fd47071f65934fdd2980dfc3e6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:399536a2083884b305405f9dcd41c3e39331f805fdda87d4c331da86f1675d3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58952663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aff85dfe21a8daa7e34a634592e74d0b49326ee44109440047e6cbcf50e4b9d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:51:30 GMT
ENV INFLUXDB_VERSION=1.8.10
# Sat, 19 Mar 2022 08:52:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:52:15 GMT
COPY file:3d8a606d61e1fc0042cf34d036eda4550a18d140c47376dacc02d96ee6f2dd8b in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:52:15 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:52:15 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:52:15 GMT
COPY file:61c4af7a0e637328374ec46266ed6dde40adf7d14ac6c5081100924991beb7f3 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:52:16 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:52:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:52:16 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881070f84f6b09f6403e878b5c62226c519b34aa93d62671dc1525e5809ec5dd`  
		Last Modified: Sat, 19 Mar 2022 08:59:53 GMT  
		Size: 54.7 MB (54659579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4a3f466a34eaa8cb2baecd8891bb1339da5f67ca0f3f89c39a2ebd5efaf876`  
		Last Modified: Sat, 19 Mar 2022 08:59:45 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64fc0cfbe868b2aad8d972fc4874512d68a73bac9406f43616ea3f54031d436`  
		Last Modified: Sat, 19 Mar 2022 08:59:45 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f8ca533a4bcfe50ab55ef34b918dd5fbd70d2d29ed531b739ff33d0872db3`  
		Last Modified: Sat, 19 Mar 2022 08:59:45 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data`

```console
$ docker pull influxdb@sha256:4adfd68bca455c5c804ad58e4198991d2174de8ac9f3d09a5506d2313132ec5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data` - linux; amd64

```console
$ docker pull influxdb@sha256:ba9a258ea5df77d3788b60655ff7034525f0ae60edf607007e23b459eaf101df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117787247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc9a2aea6ebfb56517ef166d9738e75f6e72019dcf6a8740c32f5f5ae94c9b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:52:18 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:52:24 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:52:24 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:52:24 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:52:24 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:52:24 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:52:24 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:52:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:52:24 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550eb93b184ae327ebbe4e87ba6c3f6b72123e2ff51cdbf8b894e380c0bc9f78`  
		Last Modified: Sat, 19 Mar 2022 09:00:10 GMT  
		Size: 56.7 MB (56709155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcd6f8e29a97d8f8e9fc790faefe89969811575bef2e745063df15e584f9922`  
		Last Modified: Sat, 19 Mar 2022 09:00:03 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2694323f619607cd2e22f8fcc0558fd67d95225a567dc9ee7a5869d3acf190`  
		Last Modified: Sat, 19 Mar 2022 09:00:03 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08d6800f658e5286060c2cec18f42454d14f14f9f9ef709eae90f1cf4494f45`  
		Last Modified: Sat, 19 Mar 2022 09:00:03 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-data-alpine`

```console
$ docker pull influxdb@sha256:7102c7ea58d0a3729140ab83049d423e0f137c7948e69ced1f82becf4e452bc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ce0834c6c67f4955122723fd09db4e983cd013adedff43e74c05146581a0175b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60796867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e69c05e78ef8c082da94810348cb501b5d32f210cf04d092989b17e2a0e8acff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:52:27 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:53:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:53:11 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:53:11 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:53:11 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:53:11 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:53:11 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:53:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:53:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1352e4303694301bbf45526ed2c20f6e2fbe7e6434cd8fe0e79bc9869ffe7b35`  
		Last Modified: Sat, 19 Mar 2022 09:00:30 GMT  
		Size: 56.5 MB (56503726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905d7114896f9e29bd5019dcbe803a2b817d827c3828e375485cc5dc2c35e00b`  
		Last Modified: Sat, 19 Mar 2022 09:00:23 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfa2ebc20c8b652b37aad6032d184c6f2b2925f1c872c8dea5e718e32045032`  
		Last Modified: Sat, 19 Mar 2022 09:00:23 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b410d84e27dad55d0faab8229945215a48627443e6e6824328fe6672acb911b1`  
		Last Modified: Sat, 19 Mar 2022 09:00:23 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta`

```console
$ docker pull influxdb@sha256:d0240f21f89ae3d7cec4acd7f8cd750f44d0dd00e0ba18f508969130dff47471
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:b76d35eb1b56e57f22a38b623f452c15770822e38f9f309b870fd15588757801
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84493855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:081ce2abdbb8d32f017e6fa5582fd9bd760c9f9004f91ab420a02940519e09e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:52:18 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:53:19 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:53:19 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:53:19 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:53:19 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:53:19 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:53:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:53:19 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4992723de53d8c0fbf3427d7d82e32278cdc6fb974adf1f202d282f2803846b3`  
		Last Modified: Sat, 19 Mar 2022 09:00:46 GMT  
		Size: 23.4 MB (23416969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f938aaece62656aeed448d46875c5090e41b32f0dc6292cef7ad512a7a6f67`  
		Last Modified: Sat, 19 Mar 2022 09:00:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38110311c491242933400eb982b1c811e8ceef8cc16a07d8396623de246a369`  
		Last Modified: Sat, 19 Mar 2022 09:00:42 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.8.10-meta-alpine`

```console
$ docker pull influxdb@sha256:f9ebef848c77b595c77ee0eaf6ab978b8dc69468ef104b3f9b7fa4a88ae10092
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.8.10-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:866f5587dba36266786414c65d3b322628296778c30561297a69b84070f2e5e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27584917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83b8b4d5495d637ee6649737dda3c65582ed6d18009f548712d8a1fbc65488`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:52:27 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:54:02 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:54:02 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:54:02 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:54:02 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:54:02 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:54:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:54:02 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0043723f2d668517ea2dd3c7f050fc58c203aef11bc2f8a374f2f98397286d5`  
		Last Modified: Sat, 19 Mar 2022 09:01:01 GMT  
		Size: 23.3 MB (23292980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005777352236f2ef3b11e4ba9451d590459f4f8d684f356cece973ba5782c54a`  
		Last Modified: Sat, 19 Mar 2022 09:00:58 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5c86b33a986181c1f1bb66954a31888f6ed2907d490db462a2da4a8a28060`  
		Last Modified: Sat, 19 Mar 2022 09:00:58 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data`

```console
$ docker pull influxdb@sha256:94d71fea9a38337ddb83c7b2a81912e2d26cfcba5072921a9548bb64bcb14850
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data` - linux; amd64

```console
$ docker pull influxdb@sha256:46b9a6038de6827c570212c89ac6311b4b965fa8902b46395d6dff69e6a11b9a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88682297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b84247fd9a6273356e45f474fabc973ea1892f7bda7746fd3f3691e7141e295`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:54:10 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Sat, 19 Mar 2022 08:54:14 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:54:14 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:54:14 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:54:14 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:54:14 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:54:14 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:54:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:54:14 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b94258c3005958c0db6dca10eefc1225c937044d4969eba095823c2bacd2d84`  
		Last Modified: Sat, 19 Mar 2022 09:01:17 GMT  
		Size: 27.6 MB (27604205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d18ee2ab93508a7461f0f67d23554cd711038e88f9853be805f194ab22e7fe`  
		Last Modified: Sat, 19 Mar 2022 09:01:13 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df35ebdf1c292402b53b91907b468b570ee03550b8d967e706255c41f0ad74`  
		Last Modified: Sat, 19 Mar 2022 09:01:12 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6527928b019d3389c223dc712f7c093fb2c276f448975c4713ff940a845d2a82`  
		Last Modified: Sat, 19 Mar 2022 09:01:13 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-data-alpine`

```console
$ docker pull influxdb@sha256:3f18662a79f534c4708fdcc07f848d2ce4fd2a993d58ff2134cbedb91811aa52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:bcaf46716c19f46d17d77a4f4261d740bb3d3519731dd17718fc714d3ca951f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.9 MB (31860511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2864b8e92d9da464aed802772bbd7f4f9b800c6590be96e45cd7e5ffcb9002c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:54:17 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Sat, 19 Mar 2022 08:55:00 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:55:00 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:55:00 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:55:00 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:55:00 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:55:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:55:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:55:01 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ca9388042f655859d60f03b6fca4817aae91cd9c3e3cfcdbc5f70d5f349d4b`  
		Last Modified: Sat, 19 Mar 2022 09:01:31 GMT  
		Size: 27.6 MB (27567369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933ef16f7ec3d15024bcce88e50d8f9d48109e9ba0801b8cdd8274222033cae`  
		Last Modified: Sat, 19 Mar 2022 09:01:26 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f27dc2d1d34eff4e8ab7693fba7c59528e90d96037bc823e93182e700c9d48`  
		Last Modified: Sat, 19 Mar 2022 09:01:26 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a99a6053b6fe095eb3a39ed537e6123f6ed92bbcb1bc688d4f6387529b02f3`  
		Last Modified: Sat, 19 Mar 2022 09:01:26 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta`

```console
$ docker pull influxdb@sha256:8e4f3879f7e95dfdc728bb1b2fa453858511e75ec273bc0bb30d98d044a4bf7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:3ddb298d5268e92daca50646d1d3f48276e0a722107523c6861c4fd295f3f34d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71516514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1004a49985422b9254b7a595d7f5fa2923a212679bdeaafa030e2633bd9ae50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:54:10 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Sat, 19 Mar 2022 08:55:07 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:55:07 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:55:07 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:55:07 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:55:08 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:55:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:55:08 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5762d4b1c4fcd3d7cd5a930b3b6b5e5ba97d62df1beca3779b4be779621d94`  
		Last Modified: Sat, 19 Mar 2022 09:01:42 GMT  
		Size: 10.4 MB (10439628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8b1bf791d9423d240fd6f0ffdf287a2ca00bce5037696729ac3f34ba394fb2`  
		Last Modified: Sat, 19 Mar 2022 09:01:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0779104db49646162d86066d3a59c3c612e924a4715d9760a5d929c449ce6d7f`  
		Last Modified: Sat, 19 Mar 2022 09:01:41 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9-meta-alpine`

```console
$ docker pull influxdb@sha256:4d032021e8f004a32f2e0dee870b902741a267b21ab5fe34bbbd6784f8788bf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:c0e57b0bdbf6ac342d47d3642cf8d453e04f7af72d383bf686c8b60de011a410
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14701585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a4daa79e38ff933b58be09502ee92b0e34e44e91ae7c24018f63fe0b2d02a4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:54:17 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Sat, 19 Mar 2022 08:55:49 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     (rm -rf /root/.gnupg || true) &&     rm -rf *.tar.gz* /usr/src &&     apk del .build-deps
# Sat, 19 Mar 2022 08:55:49 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:55:49 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:55:49 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:55:49 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:55:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:55:50 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061e7b61a00a5f47389afd926ef5fa18a9655efbc43d4b271d68b8d6d7f75ccb`  
		Last Modified: Sat, 19 Mar 2022 09:01:54 GMT  
		Size: 10.4 MB (10409646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc091de58d009f9378517e3927b085a434a1c45f57df72cc453b9e445c1921d`  
		Last Modified: Sat, 19 Mar 2022 09:01:52 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710df9fe2fedd01f3e61a0ab3da34a0e55a145bf8a7f97b116d2cd5b08467ea0`  
		Last Modified: Sat, 19 Mar 2022 09:01:52 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.6-data`

```console
$ docker pull influxdb@sha256:94d71fea9a38337ddb83c7b2a81912e2d26cfcba5072921a9548bb64bcb14850
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.6-data` - linux; amd64

```console
$ docker pull influxdb@sha256:46b9a6038de6827c570212c89ac6311b4b965fa8902b46395d6dff69e6a11b9a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88682297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b84247fd9a6273356e45f474fabc973ea1892f7bda7746fd3f3691e7141e295`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:54:10 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Sat, 19 Mar 2022 08:54:14 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:54:14 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:54:14 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:54:14 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:54:14 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:54:14 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:54:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:54:14 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b94258c3005958c0db6dca10eefc1225c937044d4969eba095823c2bacd2d84`  
		Last Modified: Sat, 19 Mar 2022 09:01:17 GMT  
		Size: 27.6 MB (27604205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d18ee2ab93508a7461f0f67d23554cd711038e88f9853be805f194ab22e7fe`  
		Last Modified: Sat, 19 Mar 2022 09:01:13 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df35ebdf1c292402b53b91907b468b570ee03550b8d967e706255c41f0ad74`  
		Last Modified: Sat, 19 Mar 2022 09:01:12 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6527928b019d3389c223dc712f7c093fb2c276f448975c4713ff940a845d2a82`  
		Last Modified: Sat, 19 Mar 2022 09:01:13 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.6-data-alpine`

```console
$ docker pull influxdb@sha256:3f18662a79f534c4708fdcc07f848d2ce4fd2a993d58ff2134cbedb91811aa52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.6-data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:bcaf46716c19f46d17d77a4f4261d740bb3d3519731dd17718fc714d3ca951f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.9 MB (31860511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2864b8e92d9da464aed802772bbd7f4f9b800c6590be96e45cd7e5ffcb9002c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:54:17 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Sat, 19 Mar 2022 08:55:00 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:55:00 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:55:00 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:55:00 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:55:00 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:55:00 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:55:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:55:01 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ca9388042f655859d60f03b6fca4817aae91cd9c3e3cfcdbc5f70d5f349d4b`  
		Last Modified: Sat, 19 Mar 2022 09:01:31 GMT  
		Size: 27.6 MB (27567369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933ef16f7ec3d15024bcce88e50d8f9d48109e9ba0801b8cdd8274222033cae`  
		Last Modified: Sat, 19 Mar 2022 09:01:26 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f27dc2d1d34eff4e8ab7693fba7c59528e90d96037bc823e93182e700c9d48`  
		Last Modified: Sat, 19 Mar 2022 09:01:26 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a99a6053b6fe095eb3a39ed537e6123f6ed92bbcb1bc688d4f6387529b02f3`  
		Last Modified: Sat, 19 Mar 2022 09:01:26 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.6-meta`

```console
$ docker pull influxdb@sha256:8e4f3879f7e95dfdc728bb1b2fa453858511e75ec273bc0bb30d98d044a4bf7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.6-meta` - linux; amd64

```console
$ docker pull influxdb@sha256:3ddb298d5268e92daca50646d1d3f48276e0a722107523c6861c4fd295f3f34d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71516514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1004a49985422b9254b7a595d7f5fa2923a212679bdeaafa030e2633bd9ae50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:54:10 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Sat, 19 Mar 2022 08:55:07 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:55:07 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:55:07 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:55:07 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:55:08 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:55:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:55:08 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5762d4b1c4fcd3d7cd5a930b3b6b5e5ba97d62df1beca3779b4be779621d94`  
		Last Modified: Sat, 19 Mar 2022 09:01:42 GMT  
		Size: 10.4 MB (10439628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8b1bf791d9423d240fd6f0ffdf287a2ca00bce5037696729ac3f34ba394fb2`  
		Last Modified: Sat, 19 Mar 2022 09:01:41 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0779104db49646162d86066d3a59c3c612e924a4715d9760a5d929c449ce6d7f`  
		Last Modified: Sat, 19 Mar 2022 09:01:41 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:1.9.6-meta-alpine`

```console
$ docker pull influxdb@sha256:4d032021e8f004a32f2e0dee870b902741a267b21ab5fe34bbbd6784f8788bf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:1.9.6-meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:c0e57b0bdbf6ac342d47d3642cf8d453e04f7af72d383bf686c8b60de011a410
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14701585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a4daa79e38ff933b58be09502ee92b0e34e44e91ae7c24018f63fe0b2d02a4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:54:17 GMT
ENV INFLUXDB_VERSION=1.9.6-c1.9.6
# Sat, 19 Mar 2022 08:55:49 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     (rm -rf /root/.gnupg || true) &&     rm -rf *.tar.gz* /usr/src &&     apk del .build-deps
# Sat, 19 Mar 2022 08:55:49 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:55:49 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:55:49 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:55:49 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:55:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:55:50 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061e7b61a00a5f47389afd926ef5fa18a9655efbc43d4b271d68b8d6d7f75ccb`  
		Last Modified: Sat, 19 Mar 2022 09:01:54 GMT  
		Size: 10.4 MB (10409646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc091de58d009f9378517e3927b085a434a1c45f57df72cc453b9e445c1921d`  
		Last Modified: Sat, 19 Mar 2022 09:01:52 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710df9fe2fedd01f3e61a0ab3da34a0e55a145bf8a7f97b116d2cd5b08467ea0`  
		Last Modified: Sat, 19 Mar 2022 09:01:52 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0`

```console
$ docker pull influxdb@sha256:e62f3150c097d314bbcafbb43e7e0f3f4b17437a2fd543abd0547d892da90015
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0` - linux; amd64

```console
$ docker pull influxdb@sha256:f37dc742c07ac120a5827ef5234198990139da413865ebbb4a7c1c8eebf93c44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172327590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e840a1532004fe955929db97589372fc135932120d2701833c4a506b4b56ff3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:10 GMT
ADD file:28eba36c2d43c343d9dfd5ace80db0043e1f92aa3afb4aa95d6cbb54d7e6efef in / 
# Thu, 17 Mar 2022 04:04:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:32:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:55:58 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 08:55:58 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 08:56:03 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 19 Mar 2022 08:56:03 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sat, 19 Mar 2022 08:56:13 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 19 Mar 2022 08:56:14 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 08:56:14 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 08:56:14 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 08:56:14 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Sat, 19 Mar 2022 08:56:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:56:15 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 08:56:15 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:56:15 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 08:56:15 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 08:56:15 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 08:56:15 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:7d66b83ec869a899bc8364af9c9eb0f1a5ba6907f699ef52f3182e19e2598924`  
		Last Modified: Thu, 17 Mar 2022 04:10:29 GMT  
		Size: 50.4 MB (50437294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88439e7b50a5f3923f67f432b6863c1e11adf4e45bf9740515d2cc01fd8e155`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 7.8 MB (7834140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22360a9558f73f04bb5e4dbe6dbe1584cb913040ae66388a8db66fc2ed131002`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 10.0 MB (9997260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9d2c016e5c17deb8126e44153c5ba641cfc920a91ed6a5e11a669c544e02fe`  
		Last Modified: Sat, 19 Mar 2022 09:02:05 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f676b1914da4ce851ebca49deca0e782ff75c061dd08f73c41961196b6ac03f8`  
		Last Modified: Sat, 19 Mar 2022 09:02:03 GMT  
		Size: 961.0 KB (960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97d4965368692440c0b44be160ea4a27269759eeed85f7c8cc3583d82b39dfe`  
		Last Modified: Sat, 19 Mar 2022 09:02:12 GMT  
		Size: 103.1 MB (103090643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9d4d8a019ccb1f483ddd6e35352f75ffb818fc990f29bb3b9412d03881f60`  
		Last Modified: Sat, 19 Mar 2022 09:02:03 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961d5f0bcd831f9f2725540c8e9cbfff56ad5efccf4d1421d42cf474a6b0bddb`  
		Last Modified: Sat, 19 Mar 2022 09:02:03 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdc326aabd35b9f012701568d2ed919a0ac4b813e668f4ed61d2fa8990e17b4`  
		Last Modified: Sat, 19 Mar 2022 09:02:04 GMT  
		Size: 4.9 KB (4947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4bd072ab7a7da49880598d2e9a1b0311f4cc19485fd86e6e8b85403b71747b51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174115929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896fad7ca913853eacb2117fc3316a79dbcc12551ecadf1a4ca92749218b1805`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:08 GMT
ADD file:37cabd1fec04269c22fc158f62ce5bc655934f2e58fb1ff3a1e366a33ba9bc18 in / 
# Thu, 17 Mar 2022 03:22:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:12:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:12:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:10:41 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 04:10:42 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 04:10:46 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 19 Mar 2022 04:10:47 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sat, 19 Mar 2022 04:10:56 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 19 Mar 2022 04:10:56 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 04:10:57 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 04:10:59 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 04:11:00 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Sat, 19 Mar 2022 04:11:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:11:01 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 04:11:02 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 04:11:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 04:11:04 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 04:11:05 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 04:11:06 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3996f04b7c6c17d8b25c04c7287353b896b4a0b10ab440f47d00573a7d5c3e17`  
		Last Modified: Thu, 17 Mar 2022 03:28:59 GMT  
		Size: 49.2 MB (49222993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80907b498681187ef4aa817ec6f39ba351e376afbb4fcf4415841ab9015cfc59`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 7.7 MB (7695349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8327dc7899c1a628cf11f95bb594fca3c86e45d1f4f0eb73d2ba9058eba5927`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 9.8 MB (9767203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444eeb277652a3ac4ff0d84540a509c644cdf53587304b3cf527e6f63ad3af4d`  
		Last Modified: Sat, 19 Mar 2022 04:13:06 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d0fc7c44655b4f54d98daf50549faa19be0ae99d7b70b04906ca9262d4d8e`  
		Last Modified: Sat, 19 Mar 2022 04:13:04 GMT  
		Size: 896.3 KB (896338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fee7999fd5b6cfa65c80b615dc573cf82b53bc621a189790095b41ffa551360`  
		Last Modified: Sat, 19 Mar 2022 04:13:16 GMT  
		Size: 106.5 MB (106527000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12acf972ee57d29dcd2663f68617dd5d5ee7a2f631463a238bee74708e3ac0f6`  
		Last Modified: Sat, 19 Mar 2022 04:13:04 GMT  
		Size: 206.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13493a164cfa865e3261baa2c00b8ffd39d59f3aa8802213637d764b48413a3d`  
		Last Modified: Sat, 19 Mar 2022 04:13:04 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ebfa65fd7c9f4e00c660e39072e6363e5a2b19e266a7d1d04e066756265c4`  
		Last Modified: Sat, 19 Mar 2022 04:13:05 GMT  
		Size: 4.9 KB (4945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0-alpine`

```console
$ docker pull influxdb@sha256:65cb6b95b90ad7817236f3e19d77cea5a2d35634284303b0717d93c913ba75f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:39acd601bd3a55e57f1a575d0ad693356b0ba273fbc6b03ac76672811eb373a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116710683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6085d3cb127f08f7fa810c45e9d405b749fc091356a81cce148bb0a14953dd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 19 Mar 2022 08:56:20 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 08:56:20 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 08:56:23 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 08:56:23 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sat, 19 Mar 2022 08:56:29 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 19 Mar 2022 08:56:30 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 08:56:30 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 08:56:30 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 08:56:30 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Sat, 19 Mar 2022 08:56:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:56:30 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 08:56:30 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:56:31 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 08:56:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 08:56:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 08:56:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d7448b2ddd8d77f4ff33830a3b6999154e9ad8524d87d2c68bd0b4d3b4a388`  
		Last Modified: Sat, 19 Mar 2022 09:02:26 GMT  
		Size: 9.8 MB (9836358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2c7a943976e02f6571ee342a1aa333db1e733ea9ba13bc2a9d4347c69c1b09`  
		Last Modified: Sat, 19 Mar 2022 09:02:24 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe0c4b4cfa9b6fe3d275579024680036078029c8c0e7c805cc5672657336a12`  
		Last Modified: Sat, 19 Mar 2022 09:02:22 GMT  
		Size: 960.6 KB (960606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c447ab1833ff93a4ef6f1600bf7b53a9e961678af9f70c4289b1322698270ed`  
		Last Modified: Sat, 19 Mar 2022 09:02:31 GMT  
		Size: 103.1 MB (103090645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e18a2c75ba6918bda5480fd332c722fa6b2714b314320e031700258657c9825`  
		Last Modified: Sat, 19 Mar 2022 09:02:22 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ab63825da6f6595aec229f99e06997a0cdc3bc41fbd2fda626bf665afeccab`  
		Last Modified: Sat, 19 Mar 2022 09:02:22 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c51eaad5f4944305ae2eaa5cb5d2ffff497a57e4ecefa6f6bdb3673d769ab0`  
		Last Modified: Sat, 19 Mar 2022 09:02:22 GMT  
		Size: 4.9 KB (4946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:dda981f6f49da91ccbf99d17fd1ad10ec11c261b1b684a73aa2c86c45d9a5377
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119819806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a027902951a09dccb50b6f82e4897f14bd9179124de2eb90c517c3d85e5396bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:55:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 29 Mar 2022 11:55:21 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 29 Mar 2022 11:55:22 GMT
ENV GOSU_VER=1.12
# Tue, 29 Mar 2022 11:55:26 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 11:55:27 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 29 Mar 2022 11:55:40 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 29 Mar 2022 11:55:41 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 29 Mar 2022 11:55:42 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 29 Mar 2022 11:55:44 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 29 Mar 2022 11:55:45 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Tue, 29 Mar 2022 11:55:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:55:46 GMT
CMD ["influxd"]
# Tue, 29 Mar 2022 11:55:47 GMT
EXPOSE 8086
# Tue, 29 Mar 2022 11:55:48 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 29 Mar 2022 11:55:49 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 29 Mar 2022 11:55:50 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 29 Mar 2022 11:55:51 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d05fbec0985dd4e2437413ad065a5e9de75bd6c2b3d8ddf507f114b646ae286`  
		Last Modified: Tue, 29 Mar 2022 11:57:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1d1662bf96050f7b6919306a6d549c24ffdd1b8c572aeb04f46aaed1f1261b`  
		Last Modified: Tue, 29 Mar 2022 11:57:14 GMT  
		Size: 9.7 MB (9672483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f2be565408f265515dccdc66af14c3289ea56a405f7ddc1377cb21ee637b7`  
		Last Modified: Tue, 29 Mar 2022 11:57:12 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e0a53cc77406effa83102261ce01a8855c9bd7c7ed944976b69bb337a8dda7`  
		Last Modified: Tue, 29 Mar 2022 11:57:10 GMT  
		Size: 896.1 KB (896076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dac3e9348b0d2266c4ba73b58002c390560eb7ea10e62fdf8df626b62c2b8d5`  
		Last Modified: Tue, 29 Mar 2022 11:57:21 GMT  
		Size: 106.5 MB (106526971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3356f6d8a9bba2b1e98bbfb1f8673356d980faaf9056b4858ad410f28323f534`  
		Last Modified: Tue, 29 Mar 2022 11:57:10 GMT  
		Size: 207.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214c9f61b85c8b804e0949dcfe0cc4897a7bc9c3258d4e6cb9c053660342fc3`  
		Last Modified: Tue, 29 Mar 2022 11:57:10 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc1166df3f370637b58fb18236949d2eb77fb8c068d5c877e8c98857efbf017`  
		Last Modified: Tue, 29 Mar 2022 11:57:10 GMT  
		Size: 4.9 KB (4948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.9`

```console
$ docker pull influxdb@sha256:e62f3150c097d314bbcafbb43e7e0f3f4b17437a2fd543abd0547d892da90015
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9` - linux; amd64

```console
$ docker pull influxdb@sha256:f37dc742c07ac120a5827ef5234198990139da413865ebbb4a7c1c8eebf93c44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172327590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e840a1532004fe955929db97589372fc135932120d2701833c4a506b4b56ff3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:10 GMT
ADD file:28eba36c2d43c343d9dfd5ace80db0043e1f92aa3afb4aa95d6cbb54d7e6efef in / 
# Thu, 17 Mar 2022 04:04:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:32:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:55:58 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 08:55:58 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 08:56:03 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 19 Mar 2022 08:56:03 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sat, 19 Mar 2022 08:56:13 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 19 Mar 2022 08:56:14 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 08:56:14 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 08:56:14 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 08:56:14 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Sat, 19 Mar 2022 08:56:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:56:15 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 08:56:15 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:56:15 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 08:56:15 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 08:56:15 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 08:56:15 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:7d66b83ec869a899bc8364af9c9eb0f1a5ba6907f699ef52f3182e19e2598924`  
		Last Modified: Thu, 17 Mar 2022 04:10:29 GMT  
		Size: 50.4 MB (50437294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88439e7b50a5f3923f67f432b6863c1e11adf4e45bf9740515d2cc01fd8e155`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 7.8 MB (7834140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22360a9558f73f04bb5e4dbe6dbe1584cb913040ae66388a8db66fc2ed131002`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 10.0 MB (9997260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9d2c016e5c17deb8126e44153c5ba641cfc920a91ed6a5e11a669c544e02fe`  
		Last Modified: Sat, 19 Mar 2022 09:02:05 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f676b1914da4ce851ebca49deca0e782ff75c061dd08f73c41961196b6ac03f8`  
		Last Modified: Sat, 19 Mar 2022 09:02:03 GMT  
		Size: 961.0 KB (960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97d4965368692440c0b44be160ea4a27269759eeed85f7c8cc3583d82b39dfe`  
		Last Modified: Sat, 19 Mar 2022 09:02:12 GMT  
		Size: 103.1 MB (103090643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9d4d8a019ccb1f483ddd6e35352f75ffb818fc990f29bb3b9412d03881f60`  
		Last Modified: Sat, 19 Mar 2022 09:02:03 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961d5f0bcd831f9f2725540c8e9cbfff56ad5efccf4d1421d42cf474a6b0bddb`  
		Last Modified: Sat, 19 Mar 2022 09:02:03 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdc326aabd35b9f012701568d2ed919a0ac4b813e668f4ed61d2fa8990e17b4`  
		Last Modified: Sat, 19 Mar 2022 09:02:04 GMT  
		Size: 4.9 KB (4947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:4bd072ab7a7da49880598d2e9a1b0311f4cc19485fd86e6e8b85403b71747b51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174115929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896fad7ca913853eacb2117fc3316a79dbcc12551ecadf1a4ca92749218b1805`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:08 GMT
ADD file:37cabd1fec04269c22fc158f62ce5bc655934f2e58fb1ff3a1e366a33ba9bc18 in / 
# Thu, 17 Mar 2022 03:22:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:12:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:12:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:10:41 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 04:10:42 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 04:10:46 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 19 Mar 2022 04:10:47 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sat, 19 Mar 2022 04:10:56 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 19 Mar 2022 04:10:56 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 04:10:57 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 04:10:59 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 04:11:00 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Sat, 19 Mar 2022 04:11:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:11:01 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 04:11:02 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 04:11:03 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 04:11:04 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 04:11:05 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 04:11:06 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3996f04b7c6c17d8b25c04c7287353b896b4a0b10ab440f47d00573a7d5c3e17`  
		Last Modified: Thu, 17 Mar 2022 03:28:59 GMT  
		Size: 49.2 MB (49222993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80907b498681187ef4aa817ec6f39ba351e376afbb4fcf4415841ab9015cfc59`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 7.7 MB (7695349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8327dc7899c1a628cf11f95bb594fca3c86e45d1f4f0eb73d2ba9058eba5927`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 9.8 MB (9767203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444eeb277652a3ac4ff0d84540a509c644cdf53587304b3cf527e6f63ad3af4d`  
		Last Modified: Sat, 19 Mar 2022 04:13:06 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d0fc7c44655b4f54d98daf50549faa19be0ae99d7b70b04906ca9262d4d8e`  
		Last Modified: Sat, 19 Mar 2022 04:13:04 GMT  
		Size: 896.3 KB (896338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fee7999fd5b6cfa65c80b615dc573cf82b53bc621a189790095b41ffa551360`  
		Last Modified: Sat, 19 Mar 2022 04:13:16 GMT  
		Size: 106.5 MB (106527000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12acf972ee57d29dcd2663f68617dd5d5ee7a2f631463a238bee74708e3ac0f6`  
		Last Modified: Sat, 19 Mar 2022 04:13:04 GMT  
		Size: 206.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13493a164cfa865e3261baa2c00b8ffd39d59f3aa8802213637d764b48413a3d`  
		Last Modified: Sat, 19 Mar 2022 04:13:04 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ebfa65fd7c9f4e00c660e39072e6363e5a2b19e266a7d1d04e066756265c4`  
		Last Modified: Sat, 19 Mar 2022 04:13:05 GMT  
		Size: 4.9 KB (4945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.0.9-alpine`

```console
$ docker pull influxdb@sha256:65cb6b95b90ad7817236f3e19d77cea5a2d35634284303b0717d93c913ba75f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.0.9-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:39acd601bd3a55e57f1a575d0ad693356b0ba273fbc6b03ac76672811eb373a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116710683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6085d3cb127f08f7fa810c45e9d405b749fc091356a81cce148bb0a14953dd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 19 Mar 2022 08:56:20 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 08:56:20 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 08:56:23 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 08:56:23 GMT
ENV INFLUXDB_VERSION=2.0.9
# Sat, 19 Mar 2022 08:56:29 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Sat, 19 Mar 2022 08:56:30 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 08:56:30 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 08:56:30 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 08:56:30 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Sat, 19 Mar 2022 08:56:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:56:30 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 08:56:30 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:56:31 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 08:56:31 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 08:56:31 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 08:56:31 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d7448b2ddd8d77f4ff33830a3b6999154e9ad8524d87d2c68bd0b4d3b4a388`  
		Last Modified: Sat, 19 Mar 2022 09:02:26 GMT  
		Size: 9.8 MB (9836358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2c7a943976e02f6571ee342a1aa333db1e733ea9ba13bc2a9d4347c69c1b09`  
		Last Modified: Sat, 19 Mar 2022 09:02:24 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe0c4b4cfa9b6fe3d275579024680036078029c8c0e7c805cc5672657336a12`  
		Last Modified: Sat, 19 Mar 2022 09:02:22 GMT  
		Size: 960.6 KB (960606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c447ab1833ff93a4ef6f1600bf7b53a9e961678af9f70c4289b1322698270ed`  
		Last Modified: Sat, 19 Mar 2022 09:02:31 GMT  
		Size: 103.1 MB (103090645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e18a2c75ba6918bda5480fd332c722fa6b2714b314320e031700258657c9825`  
		Last Modified: Sat, 19 Mar 2022 09:02:22 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ab63825da6f6595aec229f99e06997a0cdc3bc41fbd2fda626bf665afeccab`  
		Last Modified: Sat, 19 Mar 2022 09:02:22 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c51eaad5f4944305ae2eaa5cb5d2ffff497a57e4ecefa6f6bdb3673d769ab0`  
		Last Modified: Sat, 19 Mar 2022 09:02:22 GMT  
		Size: 4.9 KB (4946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.0.9-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:dda981f6f49da91ccbf99d17fd1ad10ec11c261b1b684a73aa2c86c45d9a5377
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119819806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a027902951a09dccb50b6f82e4897f14bd9179124de2eb90c517c3d85e5396bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:55:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 29 Mar 2022 11:55:21 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 29 Mar 2022 11:55:22 GMT
ENV GOSU_VER=1.12
# Tue, 29 Mar 2022 11:55:26 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 11:55:27 GMT
ENV INFLUXDB_VERSION=2.0.9
# Tue, 29 Mar 2022 11:55:40 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influx* /usr/local/bin/ &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version &&     influx version
# Tue, 29 Mar 2022 11:55:41 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 29 Mar 2022 11:55:42 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 29 Mar 2022 11:55:44 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 29 Mar 2022 11:55:45 GMT
COPY file:f5ca019f6dbd57be875676710efe0403265acecd892fdd8af6f1b2af0b5129bb in /entrypoint.sh 
# Tue, 29 Mar 2022 11:55:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:55:46 GMT
CMD ["influxd"]
# Tue, 29 Mar 2022 11:55:47 GMT
EXPOSE 8086
# Tue, 29 Mar 2022 11:55:48 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 29 Mar 2022 11:55:49 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 29 Mar 2022 11:55:50 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 29 Mar 2022 11:55:51 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d05fbec0985dd4e2437413ad065a5e9de75bd6c2b3d8ddf507f114b646ae286`  
		Last Modified: Tue, 29 Mar 2022 11:57:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1d1662bf96050f7b6919306a6d549c24ffdd1b8c572aeb04f46aaed1f1261b`  
		Last Modified: Tue, 29 Mar 2022 11:57:14 GMT  
		Size: 9.7 MB (9672483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f2be565408f265515dccdc66af14c3289ea56a405f7ddc1377cb21ee637b7`  
		Last Modified: Tue, 29 Mar 2022 11:57:12 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e0a53cc77406effa83102261ce01a8855c9bd7c7ed944976b69bb337a8dda7`  
		Last Modified: Tue, 29 Mar 2022 11:57:10 GMT  
		Size: 896.1 KB (896076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dac3e9348b0d2266c4ba73b58002c390560eb7ea10e62fdf8df626b62c2b8d5`  
		Last Modified: Tue, 29 Mar 2022 11:57:21 GMT  
		Size: 106.5 MB (106526971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3356f6d8a9bba2b1e98bbfb1f8673356d980faaf9056b4858ad410f28323f534`  
		Last Modified: Tue, 29 Mar 2022 11:57:10 GMT  
		Size: 207.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214c9f61b85c8b804e0949dcfe0cc4897a7bc9c3258d4e6cb9c053660342fc3`  
		Last Modified: Tue, 29 Mar 2022 11:57:10 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc1166df3f370637b58fb18236949d2eb77fb8c068d5c877e8c98857efbf017`  
		Last Modified: Tue, 29 Mar 2022 11:57:10 GMT  
		Size: 4.9 KB (4948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1`

```console
$ docker pull influxdb@sha256:799aace0d410205ee8f37041acc6072ca4d5fff643119727a140d213f8ae44c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1` - linux; amd64

```console
$ docker pull influxdb@sha256:a29e5df3e1cca465176376e64ee2e6ed0120f10ab04b330b5324faa22eed6daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182886325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d67ab18943c7df0b5d0da16348608c3aa8eb6a5d54d21ac2a3c236a74927189`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:10 GMT
ADD file:28eba36c2d43c343d9dfd5ace80db0043e1f92aa3afb4aa95d6cbb54d7e6efef in / 
# Thu, 17 Mar 2022 04:04:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:32:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:55:58 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 08:55:58 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 08:56:03 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 19 Mar 2022 08:56:34 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 19 Mar 2022 08:56:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 19 Mar 2022 08:56:40 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 19 Mar 2022 08:56:44 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 19 Mar 2022 08:56:45 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 08:56:45 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 08:56:45 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 08:56:45 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:56:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:56:45 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 08:56:45 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:56:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 08:56:45 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 08:56:46 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 08:56:46 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:7d66b83ec869a899bc8364af9c9eb0f1a5ba6907f699ef52f3182e19e2598924`  
		Last Modified: Thu, 17 Mar 2022 04:10:29 GMT  
		Size: 50.4 MB (50437294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88439e7b50a5f3923f67f432b6863c1e11adf4e45bf9740515d2cc01fd8e155`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 7.8 MB (7834140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22360a9558f73f04bb5e4dbe6dbe1584cb913040ae66388a8db66fc2ed131002`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 10.0 MB (9997260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9d2c016e5c17deb8126e44153c5ba641cfc920a91ed6a5e11a669c544e02fe`  
		Last Modified: Sat, 19 Mar 2022 09:02:05 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f676b1914da4ce851ebca49deca0e782ff75c061dd08f73c41961196b6ac03f8`  
		Last Modified: Sat, 19 Mar 2022 09:02:03 GMT  
		Size: 961.0 KB (960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fec6e1b6230576c5a7ba164c88e323a9c9a31a35b2b1dc32a469aa3e0836106`  
		Last Modified: Sat, 19 Mar 2022 09:02:48 GMT  
		Size: 108.3 MB (108324841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d103a21252e57304f7629ada34a8fa20a029aa543d776fb2441ed008a32da6b2`  
		Last Modified: Sat, 19 Mar 2022 09:02:41 GMT  
		Size: 5.3 MB (5324471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c306a07eeb6fd70d1ff7c64b17285949364b8134a40c1d1ef7bb4f07e8631f0e`  
		Last Modified: Sat, 19 Mar 2022 09:02:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c1726c8842101f5068807f0e578eb641c94902a76ac0955589c3ccef36b32d`  
		Last Modified: Sat, 19 Mar 2022 09:02:40 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588dc4b1425218e636903757e933d54958e5166579505d6a00fe9d72712dc46`  
		Last Modified: Sat, 19 Mar 2022 09:02:40 GMT  
		Size: 5.0 KB (5012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:1de096d85e07563fde58e70656b71785f95932cc934b2f76e2b07d5192a4d840
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183387337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa46e52834181a5c7409d6cf0496f7a8bf7f54a936ad2eb29c8adc606f3a4621`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:08 GMT
ADD file:37cabd1fec04269c22fc158f62ce5bc655934f2e58fb1ff3a1e366a33ba9bc18 in / 
# Thu, 17 Mar 2022 03:22:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:12:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:12:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:10:41 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 04:10:42 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 04:10:46 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 19 Mar 2022 04:11:16 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 19 Mar 2022 04:11:29 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 19 Mar 2022 04:11:29 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 19 Mar 2022 04:11:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 19 Mar 2022 04:11:34 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 04:11:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 04:11:37 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 04:11:38 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sat, 19 Mar 2022 04:11:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:11:39 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 04:11:40 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 04:11:41 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 04:11:42 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 04:11:43 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 04:11:44 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3996f04b7c6c17d8b25c04c7287353b896b4a0b10ab440f47d00573a7d5c3e17`  
		Last Modified: Thu, 17 Mar 2022 03:28:59 GMT  
		Size: 49.2 MB (49222993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80907b498681187ef4aa817ec6f39ba351e376afbb4fcf4415841ab9015cfc59`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 7.7 MB (7695349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8327dc7899c1a628cf11f95bb594fca3c86e45d1f4f0eb73d2ba9058eba5927`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 9.8 MB (9767203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444eeb277652a3ac4ff0d84540a509c644cdf53587304b3cf527e6f63ad3af4d`  
		Last Modified: Sat, 19 Mar 2022 04:13:06 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d0fc7c44655b4f54d98daf50549faa19be0ae99d7b70b04906ca9262d4d8e`  
		Last Modified: Sat, 19 Mar 2022 04:13:04 GMT  
		Size: 896.3 KB (896338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ac9bfc5c9efe3c16232111ecb45ddbce1a26a960c87244ca416a1a08566426`  
		Last Modified: Sat, 19 Mar 2022 04:13:38 GMT  
		Size: 110.9 MB (110891609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c2245c9f8827d2cae66e3c93ac8a5e69bfe5a533d4cb5f342ec87219ae468`  
		Last Modified: Sat, 19 Mar 2022 04:13:29 GMT  
		Size: 4.9 MB (4906725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eb5f55c031ecf1698fa52d24bcc7293768ec4b8354a9fcb027d7df82bcd29c`  
		Last Modified: Sat, 19 Mar 2022 04:13:28 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7c33b81b950f8a1a9022072b612f4c23fbe50467f65c51033c2e831bcd3b0f`  
		Last Modified: Sat, 19 Mar 2022 04:13:28 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721d2dd815280a880f5d95bd85e9bb025a5e6a013fed0c0872d3b93c362f0634`  
		Last Modified: Sat, 19 Mar 2022 04:13:28 GMT  
		Size: 5.0 KB (5014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1-alpine`

```console
$ docker pull influxdb@sha256:395e51987acc0a55fb770e5674b3a943e9ab84080690b4e72300648ca5b7c117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:06308c0090faf779227b2a0057b48021cdf5b979bc675fb7e70d5ddf793f7c2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127269412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3c34e321d28240dcdc466f99d27eaa497de4868fa297bd5b0d1b4d4c33ad63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 19 Mar 2022 08:56:20 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 08:56:20 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 08:56:23 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 08:56:50 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 19 Mar 2022 08:56:56 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 19 Mar 2022 08:56:56 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 19 Mar 2022 08:56:59 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 19 Mar 2022 08:57:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 08:57:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 08:57:00 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 08:57:00 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Sat, 19 Mar 2022 08:57:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:57:00 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 08:57:00 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:57:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 08:57:01 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 08:57:01 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 08:57:01 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d7448b2ddd8d77f4ff33830a3b6999154e9ad8524d87d2c68bd0b4d3b4a388`  
		Last Modified: Sat, 19 Mar 2022 09:02:26 GMT  
		Size: 9.8 MB (9836358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2c7a943976e02f6571ee342a1aa333db1e733ea9ba13bc2a9d4347c69c1b09`  
		Last Modified: Sat, 19 Mar 2022 09:02:24 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe0c4b4cfa9b6fe3d275579024680036078029c8c0e7c805cc5672657336a12`  
		Last Modified: Sat, 19 Mar 2022 09:02:22 GMT  
		Size: 960.6 KB (960606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8273224c835999f81b70b6478092ff8a5cf3c164b7cdc3c11e41a7a63c4c60`  
		Last Modified: Sat, 19 Mar 2022 09:03:09 GMT  
		Size: 108.3 MB (108324825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22a8380e9706c9c21d9696ceac7bb845110af0da04c8ff382fcc5521e3387d`  
		Last Modified: Sat, 19 Mar 2022 09:03:02 GMT  
		Size: 5.3 MB (5324482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4121aab9803357f0d56cabfb46cc0597de95b01d0c3ce7e85db5324feea62c9`  
		Last Modified: Sat, 19 Mar 2022 09:03:01 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38e3f55ee8efeec4483ea2558aa6161b63726de238ca24403dda0aa85ec5242`  
		Last Modified: Sat, 19 Mar 2022 09:03:01 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66654efea0efd57f17a079e7845a2a8569f8b30d9ee124712e0cb9c6e30f9456`  
		Last Modified: Sat, 19 Mar 2022 09:03:01 GMT  
		Size: 5.0 KB (5014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ddff68e6377af62bd283f4e9f143d2b9d2b9ea3df07d68144e54d8e5136f5949
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129091224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b620a352032301f93661396eb1fca8a4107e72d45b1409b8c9bf0c7fae7f4a8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:55:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 29 Mar 2022 11:55:21 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 29 Mar 2022 11:55:22 GMT
ENV GOSU_VER=1.12
# Tue, 29 Mar 2022 11:55:26 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 11:56:05 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 29 Mar 2022 11:56:14 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 29 Mar 2022 11:56:14 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 29 Mar 2022 11:56:19 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 29 Mar 2022 11:56:20 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 29 Mar 2022 11:56:21 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 29 Mar 2022 11:56:23 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 29 Mar 2022 11:56:24 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Tue, 29 Mar 2022 11:56:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:56:25 GMT
CMD ["influxd"]
# Tue, 29 Mar 2022 11:56:26 GMT
EXPOSE 8086
# Tue, 29 Mar 2022 11:56:27 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 29 Mar 2022 11:56:28 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 29 Mar 2022 11:56:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 29 Mar 2022 11:56:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d05fbec0985dd4e2437413ad065a5e9de75bd6c2b3d8ddf507f114b646ae286`  
		Last Modified: Tue, 29 Mar 2022 11:57:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1d1662bf96050f7b6919306a6d549c24ffdd1b8c572aeb04f46aaed1f1261b`  
		Last Modified: Tue, 29 Mar 2022 11:57:14 GMT  
		Size: 9.7 MB (9672483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f2be565408f265515dccdc66af14c3289ea56a405f7ddc1377cb21ee637b7`  
		Last Modified: Tue, 29 Mar 2022 11:57:12 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e0a53cc77406effa83102261ce01a8855c9bd7c7ed944976b69bb337a8dda7`  
		Last Modified: Tue, 29 Mar 2022 11:57:10 GMT  
		Size: 896.1 KB (896076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81bc505e8165f74a9d27dd342d7d3d79f685491cb6e9c9abe729578c8149061`  
		Last Modified: Tue, 29 Mar 2022 11:57:43 GMT  
		Size: 110.9 MB (110891593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22645a3eccc37c9e1f2aed8d97dacd06be4b114efca585f300ea4ed68802df0`  
		Last Modified: Tue, 29 Mar 2022 11:57:35 GMT  
		Size: 4.9 MB (4906732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e37f4bf83c351e8926f204ee2d9f204cfea970ac8b5ab3e31f98d5659d5d0f`  
		Last Modified: Tue, 29 Mar 2022 11:57:34 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d4a874b49998b6c39fca72812e50c58c6e1d1c9538d5118d6e4e89dcf088bd`  
		Last Modified: Tue, 29 Mar 2022 11:57:34 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1d3f354f0bfd5fec69a97e80a505a7f3fa26c0952106699c8e0078bb699901`  
		Last Modified: Tue, 29 Mar 2022 11:57:34 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1.1`

```console
$ docker pull influxdb@sha256:799aace0d410205ee8f37041acc6072ca4d5fff643119727a140d213f8ae44c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1` - linux; amd64

```console
$ docker pull influxdb@sha256:a29e5df3e1cca465176376e64ee2e6ed0120f10ab04b330b5324faa22eed6daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182886325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d67ab18943c7df0b5d0da16348608c3aa8eb6a5d54d21ac2a3c236a74927189`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:10 GMT
ADD file:28eba36c2d43c343d9dfd5ace80db0043e1f92aa3afb4aa95d6cbb54d7e6efef in / 
# Thu, 17 Mar 2022 04:04:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:32:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:55:58 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 08:55:58 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 08:56:03 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 19 Mar 2022 08:56:34 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 19 Mar 2022 08:56:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 19 Mar 2022 08:56:40 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 19 Mar 2022 08:56:44 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 19 Mar 2022 08:56:45 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 08:56:45 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 08:56:45 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 08:56:45 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:56:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:56:45 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 08:56:45 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:56:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 08:56:45 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 08:56:46 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 08:56:46 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:7d66b83ec869a899bc8364af9c9eb0f1a5ba6907f699ef52f3182e19e2598924`  
		Last Modified: Thu, 17 Mar 2022 04:10:29 GMT  
		Size: 50.4 MB (50437294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88439e7b50a5f3923f67f432b6863c1e11adf4e45bf9740515d2cc01fd8e155`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 7.8 MB (7834140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22360a9558f73f04bb5e4dbe6dbe1584cb913040ae66388a8db66fc2ed131002`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 10.0 MB (9997260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9d2c016e5c17deb8126e44153c5ba641cfc920a91ed6a5e11a669c544e02fe`  
		Last Modified: Sat, 19 Mar 2022 09:02:05 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f676b1914da4ce851ebca49deca0e782ff75c061dd08f73c41961196b6ac03f8`  
		Last Modified: Sat, 19 Mar 2022 09:02:03 GMT  
		Size: 961.0 KB (960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fec6e1b6230576c5a7ba164c88e323a9c9a31a35b2b1dc32a469aa3e0836106`  
		Last Modified: Sat, 19 Mar 2022 09:02:48 GMT  
		Size: 108.3 MB (108324841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d103a21252e57304f7629ada34a8fa20a029aa543d776fb2441ed008a32da6b2`  
		Last Modified: Sat, 19 Mar 2022 09:02:41 GMT  
		Size: 5.3 MB (5324471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c306a07eeb6fd70d1ff7c64b17285949364b8134a40c1d1ef7bb4f07e8631f0e`  
		Last Modified: Sat, 19 Mar 2022 09:02:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c1726c8842101f5068807f0e578eb641c94902a76ac0955589c3ccef36b32d`  
		Last Modified: Sat, 19 Mar 2022 09:02:40 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588dc4b1425218e636903757e933d54958e5166579505d6a00fe9d72712dc46`  
		Last Modified: Sat, 19 Mar 2022 09:02:40 GMT  
		Size: 5.0 KB (5012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:1de096d85e07563fde58e70656b71785f95932cc934b2f76e2b07d5192a4d840
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183387337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa46e52834181a5c7409d6cf0496f7a8bf7f54a936ad2eb29c8adc606f3a4621`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:08 GMT
ADD file:37cabd1fec04269c22fc158f62ce5bc655934f2e58fb1ff3a1e366a33ba9bc18 in / 
# Thu, 17 Mar 2022 03:22:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:12:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:12:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:10:41 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 04:10:42 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 04:10:46 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 19 Mar 2022 04:11:16 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 19 Mar 2022 04:11:29 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 19 Mar 2022 04:11:29 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 19 Mar 2022 04:11:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 19 Mar 2022 04:11:34 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 04:11:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 04:11:37 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 04:11:38 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sat, 19 Mar 2022 04:11:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:11:39 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 04:11:40 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 04:11:41 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 04:11:42 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 04:11:43 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 04:11:44 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3996f04b7c6c17d8b25c04c7287353b896b4a0b10ab440f47d00573a7d5c3e17`  
		Last Modified: Thu, 17 Mar 2022 03:28:59 GMT  
		Size: 49.2 MB (49222993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80907b498681187ef4aa817ec6f39ba351e376afbb4fcf4415841ab9015cfc59`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 7.7 MB (7695349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8327dc7899c1a628cf11f95bb594fca3c86e45d1f4f0eb73d2ba9058eba5927`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 9.8 MB (9767203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444eeb277652a3ac4ff0d84540a509c644cdf53587304b3cf527e6f63ad3af4d`  
		Last Modified: Sat, 19 Mar 2022 04:13:06 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d0fc7c44655b4f54d98daf50549faa19be0ae99d7b70b04906ca9262d4d8e`  
		Last Modified: Sat, 19 Mar 2022 04:13:04 GMT  
		Size: 896.3 KB (896338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ac9bfc5c9efe3c16232111ecb45ddbce1a26a960c87244ca416a1a08566426`  
		Last Modified: Sat, 19 Mar 2022 04:13:38 GMT  
		Size: 110.9 MB (110891609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c2245c9f8827d2cae66e3c93ac8a5e69bfe5a533d4cb5f342ec87219ae468`  
		Last Modified: Sat, 19 Mar 2022 04:13:29 GMT  
		Size: 4.9 MB (4906725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eb5f55c031ecf1698fa52d24bcc7293768ec4b8354a9fcb027d7df82bcd29c`  
		Last Modified: Sat, 19 Mar 2022 04:13:28 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7c33b81b950f8a1a9022072b612f4c23fbe50467f65c51033c2e831bcd3b0f`  
		Last Modified: Sat, 19 Mar 2022 04:13:28 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721d2dd815280a880f5d95bd85e9bb025a5e6a013fed0c0872d3b93c362f0634`  
		Last Modified: Sat, 19 Mar 2022 04:13:28 GMT  
		Size: 5.0 KB (5014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:2.1.1-alpine`

```console
$ docker pull influxdb@sha256:395e51987acc0a55fb770e5674b3a943e9ab84080690b4e72300648ca5b7c117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:2.1.1-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:06308c0090faf779227b2a0057b48021cdf5b979bc675fb7e70d5ddf793f7c2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127269412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3c34e321d28240dcdc466f99d27eaa497de4868fa297bd5b0d1b4d4c33ad63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 19 Mar 2022 08:56:20 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 08:56:20 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 08:56:23 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 08:56:50 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 19 Mar 2022 08:56:56 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 19 Mar 2022 08:56:56 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 19 Mar 2022 08:56:59 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 19 Mar 2022 08:57:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 08:57:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 08:57:00 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 08:57:00 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Sat, 19 Mar 2022 08:57:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:57:00 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 08:57:00 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:57:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 08:57:01 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 08:57:01 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 08:57:01 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d7448b2ddd8d77f4ff33830a3b6999154e9ad8524d87d2c68bd0b4d3b4a388`  
		Last Modified: Sat, 19 Mar 2022 09:02:26 GMT  
		Size: 9.8 MB (9836358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2c7a943976e02f6571ee342a1aa333db1e733ea9ba13bc2a9d4347c69c1b09`  
		Last Modified: Sat, 19 Mar 2022 09:02:24 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe0c4b4cfa9b6fe3d275579024680036078029c8c0e7c805cc5672657336a12`  
		Last Modified: Sat, 19 Mar 2022 09:02:22 GMT  
		Size: 960.6 KB (960606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8273224c835999f81b70b6478092ff8a5cf3c164b7cdc3c11e41a7a63c4c60`  
		Last Modified: Sat, 19 Mar 2022 09:03:09 GMT  
		Size: 108.3 MB (108324825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22a8380e9706c9c21d9696ceac7bb845110af0da04c8ff382fcc5521e3387d`  
		Last Modified: Sat, 19 Mar 2022 09:03:02 GMT  
		Size: 5.3 MB (5324482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4121aab9803357f0d56cabfb46cc0597de95b01d0c3ce7e85db5324feea62c9`  
		Last Modified: Sat, 19 Mar 2022 09:03:01 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38e3f55ee8efeec4483ea2558aa6161b63726de238ca24403dda0aa85ec5242`  
		Last Modified: Sat, 19 Mar 2022 09:03:01 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66654efea0efd57f17a079e7845a2a8569f8b30d9ee124712e0cb9c6e30f9456`  
		Last Modified: Sat, 19 Mar 2022 09:03:01 GMT  
		Size: 5.0 KB (5014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:2.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ddff68e6377af62bd283f4e9f143d2b9d2b9ea3df07d68144e54d8e5136f5949
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129091224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b620a352032301f93661396eb1fca8a4107e72d45b1409b8c9bf0c7fae7f4a8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:55:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 29 Mar 2022 11:55:21 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 29 Mar 2022 11:55:22 GMT
ENV GOSU_VER=1.12
# Tue, 29 Mar 2022 11:55:26 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 11:56:05 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 29 Mar 2022 11:56:14 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 29 Mar 2022 11:56:14 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 29 Mar 2022 11:56:19 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 29 Mar 2022 11:56:20 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 29 Mar 2022 11:56:21 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 29 Mar 2022 11:56:23 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 29 Mar 2022 11:56:24 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Tue, 29 Mar 2022 11:56:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:56:25 GMT
CMD ["influxd"]
# Tue, 29 Mar 2022 11:56:26 GMT
EXPOSE 8086
# Tue, 29 Mar 2022 11:56:27 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 29 Mar 2022 11:56:28 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 29 Mar 2022 11:56:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 29 Mar 2022 11:56:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d05fbec0985dd4e2437413ad065a5e9de75bd6c2b3d8ddf507f114b646ae286`  
		Last Modified: Tue, 29 Mar 2022 11:57:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1d1662bf96050f7b6919306a6d549c24ffdd1b8c572aeb04f46aaed1f1261b`  
		Last Modified: Tue, 29 Mar 2022 11:57:14 GMT  
		Size: 9.7 MB (9672483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f2be565408f265515dccdc66af14c3289ea56a405f7ddc1377cb21ee637b7`  
		Last Modified: Tue, 29 Mar 2022 11:57:12 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e0a53cc77406effa83102261ce01a8855c9bd7c7ed944976b69bb337a8dda7`  
		Last Modified: Tue, 29 Mar 2022 11:57:10 GMT  
		Size: 896.1 KB (896076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81bc505e8165f74a9d27dd342d7d3d79f685491cb6e9c9abe729578c8149061`  
		Last Modified: Tue, 29 Mar 2022 11:57:43 GMT  
		Size: 110.9 MB (110891593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22645a3eccc37c9e1f2aed8d97dacd06be4b114efca585f300ea4ed68802df0`  
		Last Modified: Tue, 29 Mar 2022 11:57:35 GMT  
		Size: 4.9 MB (4906732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e37f4bf83c351e8926f204ee2d9f204cfea970ac8b5ab3e31f98d5659d5d0f`  
		Last Modified: Tue, 29 Mar 2022 11:57:34 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d4a874b49998b6c39fca72812e50c58c6e1d1c9538d5118d6e4e89dcf088bd`  
		Last Modified: Tue, 29 Mar 2022 11:57:34 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1d3f354f0bfd5fec69a97e80a505a7f3fa26c0952106699c8e0078bb699901`  
		Last Modified: Tue, 29 Mar 2022 11:57:34 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:alpine`

```console
$ docker pull influxdb@sha256:395e51987acc0a55fb770e5674b3a943e9ab84080690b4e72300648ca5b7c117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:06308c0090faf779227b2a0057b48021cdf5b979bc675fb7e70d5ddf793f7c2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127269412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3c34e321d28240dcdc466f99d27eaa497de4868fa297bd5b0d1b4d4c33ad63`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Sat, 19 Mar 2022 08:56:20 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 08:56:20 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 08:56:23 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 08:56:50 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 19 Mar 2022 08:56:56 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 19 Mar 2022 08:56:56 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 19 Mar 2022 08:56:59 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 19 Mar 2022 08:57:00 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 08:57:00 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 08:57:00 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 08:57:00 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Sat, 19 Mar 2022 08:57:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:57:00 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 08:57:00 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:57:00 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 08:57:01 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 08:57:01 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 08:57:01 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d7448b2ddd8d77f4ff33830a3b6999154e9ad8524d87d2c68bd0b4d3b4a388`  
		Last Modified: Sat, 19 Mar 2022 09:02:26 GMT  
		Size: 9.8 MB (9836358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2c7a943976e02f6571ee342a1aa333db1e733ea9ba13bc2a9d4347c69c1b09`  
		Last Modified: Sat, 19 Mar 2022 09:02:24 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe0c4b4cfa9b6fe3d275579024680036078029c8c0e7c805cc5672657336a12`  
		Last Modified: Sat, 19 Mar 2022 09:02:22 GMT  
		Size: 960.6 KB (960606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8273224c835999f81b70b6478092ff8a5cf3c164b7cdc3c11e41a7a63c4c60`  
		Last Modified: Sat, 19 Mar 2022 09:03:09 GMT  
		Size: 108.3 MB (108324825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22a8380e9706c9c21d9696ceac7bb845110af0da04c8ff382fcc5521e3387d`  
		Last Modified: Sat, 19 Mar 2022 09:03:02 GMT  
		Size: 5.3 MB (5324482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4121aab9803357f0d56cabfb46cc0597de95b01d0c3ce7e85db5324feea62c9`  
		Last Modified: Sat, 19 Mar 2022 09:03:01 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38e3f55ee8efeec4483ea2558aa6161b63726de238ca24403dda0aa85ec5242`  
		Last Modified: Sat, 19 Mar 2022 09:03:01 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66654efea0efd57f17a079e7845a2a8569f8b30d9ee124712e0cb9c6e30f9456`  
		Last Modified: Sat, 19 Mar 2022 09:03:01 GMT  
		Size: 5.0 KB (5014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:alpine` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:ddff68e6377af62bd283f4e9f143d2b9d2b9ea3df07d68144e54d8e5136f5949
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129091224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b620a352032301f93661396eb1fca8a4107e72d45b1409b8c9bf0c7fae7f4a8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:55:20 GMT
RUN apk add --no-cache tzdata bash ca-certificates gnupg run-parts &&     update-ca-certificates
# Tue, 29 Mar 2022 11:55:21 GMT
RUN addgroup -S -g 1000 influxdb &&     adduser -S -G influxdb -u 1000 -h /home/influxdb -s /bin/sh influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Tue, 29 Mar 2022 11:55:22 GMT
ENV GOSU_VER=1.12
# Tue, 29 Mar 2022 11:55:26 GMT
RUN set -eux;     ARCH="$(apk --print-arch)" &&     case "${ARCH}" in         x86_64)  ARCH=amd64;;         aarch64) ARCH=arm64;;         *)       echo "Unsupported architecture: ${ARCH}"; exit 1;;     esac && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$ARCH.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 11:56:05 GMT
ENV INFLUXDB_VERSION=2.1.1
# Tue, 29 Mar 2022 11:56:14 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Tue, 29 Mar 2022 11:56:14 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Tue, 29 Mar 2022 11:56:19 GMT
RUN set -eux &&     ARCH="$(apk --print-arch)" &&     if [ ${ARCH} = x86_64 ]; then         ARCH=amd64;     elif [ ${ARCH} = aarch64 ]; then         ARCH=arm64;     else         echo "Unsupported architecture: ${ARCH}" && exit 1;     fi &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Tue, 29 Mar 2022 11:56:20 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Tue, 29 Mar 2022 11:56:21 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Tue, 29 Mar 2022 11:56:23 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Tue, 29 Mar 2022 11:56:24 GMT
COPY file:2bb0090d5bd94b26299db34eae2a7f9cc567840d43e1bba3e59b735fd488fc0d in /entrypoint.sh 
# Tue, 29 Mar 2022 11:56:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:56:25 GMT
CMD ["influxd"]
# Tue, 29 Mar 2022 11:56:26 GMT
EXPOSE 8086
# Tue, 29 Mar 2022 11:56:27 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Tue, 29 Mar 2022 11:56:28 GMT
ENV INFLUXD_INIT_PORT=9999
# Tue, 29 Mar 2022 11:56:29 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Tue, 29 Mar 2022 11:56:30 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d05fbec0985dd4e2437413ad065a5e9de75bd6c2b3d8ddf507f114b646ae286`  
		Last Modified: Tue, 29 Mar 2022 11:57:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1d1662bf96050f7b6919306a6d549c24ffdd1b8c572aeb04f46aaed1f1261b`  
		Last Modified: Tue, 29 Mar 2022 11:57:14 GMT  
		Size: 9.7 MB (9672483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f2be565408f265515dccdc66af14c3289ea56a405f7ddc1377cb21ee637b7`  
		Last Modified: Tue, 29 Mar 2022 11:57:12 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e0a53cc77406effa83102261ce01a8855c9bd7c7ed944976b69bb337a8dda7`  
		Last Modified: Tue, 29 Mar 2022 11:57:10 GMT  
		Size: 896.1 KB (896076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81bc505e8165f74a9d27dd342d7d3d79f685491cb6e9c9abe729578c8149061`  
		Last Modified: Tue, 29 Mar 2022 11:57:43 GMT  
		Size: 110.9 MB (110891593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22645a3eccc37c9e1f2aed8d97dacd06be4b114efca585f300ea4ed68802df0`  
		Last Modified: Tue, 29 Mar 2022 11:57:35 GMT  
		Size: 4.9 MB (4906732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e37f4bf83c351e8926f204ee2d9f204cfea970ac8b5ab3e31f98d5659d5d0f`  
		Last Modified: Tue, 29 Mar 2022 11:57:34 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d4a874b49998b6c39fca72812e50c58c6e1d1c9538d5118d6e4e89dcf088bd`  
		Last Modified: Tue, 29 Mar 2022 11:57:34 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1d3f354f0bfd5fec69a97e80a505a7f3fa26c0952106699c8e0078bb699901`  
		Last Modified: Tue, 29 Mar 2022 11:57:34 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data`

```console
$ docker pull influxdb@sha256:4adfd68bca455c5c804ad58e4198991d2174de8ac9f3d09a5506d2313132ec5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:ba9a258ea5df77d3788b60655ff7034525f0ae60edf607007e23b459eaf101df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117787247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc9a2aea6ebfb56517ef166d9738e75f6e72019dcf6a8740c32f5f5ae94c9b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:52:18 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:52:24 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:52:24 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:52:24 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:52:24 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:52:24 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:52:24 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:52:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:52:24 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550eb93b184ae327ebbe4e87ba6c3f6b72123e2ff51cdbf8b894e380c0bc9f78`  
		Last Modified: Sat, 19 Mar 2022 09:00:10 GMT  
		Size: 56.7 MB (56709155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcd6f8e29a97d8f8e9fc790faefe89969811575bef2e745063df15e584f9922`  
		Last Modified: Sat, 19 Mar 2022 09:00:03 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2694323f619607cd2e22f8fcc0558fd67d95225a567dc9ee7a5869d3acf190`  
		Last Modified: Sat, 19 Mar 2022 09:00:03 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08d6800f658e5286060c2cec18f42454d14f14f9f9ef709eae90f1cf4494f45`  
		Last Modified: Sat, 19 Mar 2022 09:00:03 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:7102c7ea58d0a3729140ab83049d423e0f137c7948e69ced1f82becf4e452bc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:ce0834c6c67f4955122723fd09db4e983cd013adedff43e74c05146581a0175b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60796867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e69c05e78ef8c082da94810348cb501b5d32f210cf04d092989b17e2a0e8acff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:52:27 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:53:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:53:11 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Sat, 19 Mar 2022 08:53:11 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:53:11 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:53:11 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:53:11 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Sat, 19 Mar 2022 08:53:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:53:11 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1352e4303694301bbf45526ed2c20f6e2fbe7e6434cd8fe0e79bc9869ffe7b35`  
		Last Modified: Sat, 19 Mar 2022 09:00:30 GMT  
		Size: 56.5 MB (56503726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905d7114896f9e29bd5019dcbe803a2b817d827c3828e375485cc5dc2c35e00b`  
		Last Modified: Sat, 19 Mar 2022 09:00:23 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfa2ebc20c8b652b37aad6032d184c6f2b2925f1c872c8dea5e718e32045032`  
		Last Modified: Sat, 19 Mar 2022 09:00:23 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b410d84e27dad55d0faab8229945215a48627443e6e6824328fe6672acb911b1`  
		Last Modified: Sat, 19 Mar 2022 09:00:23 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:latest`

```console
$ docker pull influxdb@sha256:799aace0d410205ee8f37041acc6072ca4d5fff643119727a140d213f8ae44c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `influxdb:latest` - linux; amd64

```console
$ docker pull influxdb@sha256:a29e5df3e1cca465176376e64ee2e6ed0120f10ab04b330b5324faa22eed6daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.9 MB (182886325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d67ab18943c7df0b5d0da16348608c3aa8eb6a5d54d21ac2a3c236a74927189`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:10 GMT
ADD file:28eba36c2d43c343d9dfd5ace80db0043e1f92aa3afb4aa95d6cbb54d7e6efef in / 
# Thu, 17 Mar 2022 04:04:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:32:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:55:58 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 08:55:58 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 08:56:03 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 19 Mar 2022 08:56:34 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 19 Mar 2022 08:56:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 19 Mar 2022 08:56:40 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 19 Mar 2022 08:56:44 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 19 Mar 2022 08:56:45 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 08:56:45 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 08:56:45 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 08:56:45 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:56:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:56:45 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 08:56:45 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 08:56:45 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 08:56:45 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 08:56:46 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 08:56:46 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:7d66b83ec869a899bc8364af9c9eb0f1a5ba6907f699ef52f3182e19e2598924`  
		Last Modified: Thu, 17 Mar 2022 04:10:29 GMT  
		Size: 50.4 MB (50437294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88439e7b50a5f3923f67f432b6863c1e11adf4e45bf9740515d2cc01fd8e155`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 7.8 MB (7834140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22360a9558f73f04bb5e4dbe6dbe1584cb913040ae66388a8db66fc2ed131002`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 10.0 MB (9997260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9d2c016e5c17deb8126e44153c5ba641cfc920a91ed6a5e11a669c544e02fe`  
		Last Modified: Sat, 19 Mar 2022 09:02:05 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f676b1914da4ce851ebca49deca0e782ff75c061dd08f73c41961196b6ac03f8`  
		Last Modified: Sat, 19 Mar 2022 09:02:03 GMT  
		Size: 961.0 KB (960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fec6e1b6230576c5a7ba164c88e323a9c9a31a35b2b1dc32a469aa3e0836106`  
		Last Modified: Sat, 19 Mar 2022 09:02:48 GMT  
		Size: 108.3 MB (108324841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d103a21252e57304f7629ada34a8fa20a029aa543d776fb2441ed008a32da6b2`  
		Last Modified: Sat, 19 Mar 2022 09:02:41 GMT  
		Size: 5.3 MB (5324471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c306a07eeb6fd70d1ff7c64b17285949364b8134a40c1d1ef7bb4f07e8631f0e`  
		Last Modified: Sat, 19 Mar 2022 09:02:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c1726c8842101f5068807f0e578eb641c94902a76ac0955589c3ccef36b32d`  
		Last Modified: Sat, 19 Mar 2022 09:02:40 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588dc4b1425218e636903757e933d54958e5166579505d6a00fe9d72712dc46`  
		Last Modified: Sat, 19 Mar 2022 09:02:40 GMT  
		Size: 5.0 KB (5012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `influxdb:latest` - linux; arm64 variant v8

```console
$ docker pull influxdb@sha256:1de096d85e07563fde58e70656b71785f95932cc934b2f76e2b07d5192a4d840
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.4 MB (183387337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa46e52834181a5c7409d6cf0496f7a8bf7f54a936ad2eb29c8adc606f3a4621`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:08 GMT
ADD file:37cabd1fec04269c22fc158f62ce5bc655934f2e58fb1ff3a1e366a33ba9bc18 in / 
# Thu, 17 Mar 2022 03:22:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:12:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:12:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:10:41 GMT
RUN groupadd -r influxdb --gid=1000 &&     useradd -r -g influxdb --uid=1000 --home-dir=/home/influxdb --shell=/bin/bash influxdb &&     mkdir -p /home/influxdb &&     chown -R influxdb:influxdb /home/influxdb
# Sat, 19 Mar 2022 04:10:42 GMT
ENV GOSU_VER=1.12
# Sat, 19 Mar 2022 04:10:46 GMT
RUN set -eux; 	dpkgArch="$(dpkg --print-architecture)" && 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch" && 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VER/gosu-$dpkgArch.asc" && 	export GNUPGHOME="$(mktemp -d)" && 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu && 	gpgconf --kill all && 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc && 	chmod +x /usr/local/bin/gosu && 	gosu --version && 	gosu nobody true
# Sat, 19 Mar 2022 04:11:16 GMT
ENV INFLUXDB_VERSION=2.1.1
# Sat, 19 Mar 2022 04:11:29 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}/influxd /usr/local/bin/influxd &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-${INFLUXDB_VERSION}-linux-${ARCH}* &&     influxd version
# Sat, 19 Mar 2022 04:11:29 GMT
ENV INFLUX_CLI_VERSION=2.2.1
# Sat, 19 Mar 2022 04:11:33 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/influxdb/releases/influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver keys.openpgp.org --recv-keys 8C2D403D3C3BDB81A4C27C883C3E4B7317FFE40A &&     gpg --batch --verify influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz.asc influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     tar xzf influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}.tar.gz &&     cp influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}/influx /usr/local/bin/influx &&     rm -rf "$GNUPGHOME" influxdb2.key influxdb2-client-${INFLUX_CLI_VERSION}-linux-${ARCH}* &&     influx version
# Sat, 19 Mar 2022 04:11:34 GMT
RUN mkdir /docker-entrypoint-initdb.d &&     mkdir -p /var/lib/influxdb2 &&     chown -R influxdb:influxdb /var/lib/influxdb2 &&     mkdir -p /etc/influxdb2 &&     chown -R influxdb:influxdb /etc/influxdb2
# Sat, 19 Mar 2022 04:11:35 GMT
VOLUME [/var/lib/influxdb2 /etc/influxdb2]
# Sat, 19 Mar 2022 04:11:37 GMT
COPY file:77129326da9464dfa98aab4911582df608de5d5bf6a6f6ed89619b704cac95bc in /etc/defaults/influxdb2/config.yml 
# Sat, 19 Mar 2022 04:11:38 GMT
COPY file:a64302f264563d538089431198a37bdc67423165f65d702bc1fe865140128cf1 in /entrypoint.sh 
# Sat, 19 Mar 2022 04:11:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:11:39 GMT
CMD ["influxd"]
# Sat, 19 Mar 2022 04:11:40 GMT
EXPOSE 8086
# Sat, 19 Mar 2022 04:11:41 GMT
ENV INFLUX_CONFIGS_PATH=/etc/influxdb2/influx-configs
# Sat, 19 Mar 2022 04:11:42 GMT
ENV INFLUXD_INIT_PORT=9999
# Sat, 19 Mar 2022 04:11:43 GMT
ENV INFLUXD_INIT_PING_ATTEMPTS=600
# Sat, 19 Mar 2022 04:11:44 GMT
ENV DOCKER_INFLUXDB_INIT_CLI_CONFIG_NAME=default
```

-	Layers:
	-	`sha256:3996f04b7c6c17d8b25c04c7287353b896b4a0b10ab440f47d00573a7d5c3e17`  
		Last Modified: Thu, 17 Mar 2022 03:28:59 GMT  
		Size: 49.2 MB (49222993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80907b498681187ef4aa817ec6f39ba351e376afbb4fcf4415841ab9015cfc59`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 7.7 MB (7695349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8327dc7899c1a628cf11f95bb594fca3c86e45d1f4f0eb73d2ba9058eba5927`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 9.8 MB (9767203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444eeb277652a3ac4ff0d84540a509c644cdf53587304b3cf527e6f63ad3af4d`  
		Last Modified: Sat, 19 Mar 2022 04:13:06 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d0fc7c44655b4f54d98daf50549faa19be0ae99d7b70b04906ca9262d4d8e`  
		Last Modified: Sat, 19 Mar 2022 04:13:04 GMT  
		Size: 896.3 KB (896338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ac9bfc5c9efe3c16232111ecb45ddbce1a26a960c87244ca416a1a08566426`  
		Last Modified: Sat, 19 Mar 2022 04:13:38 GMT  
		Size: 110.9 MB (110891609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c2245c9f8827d2cae66e3c93ac8a5e69bfe5a533d4cb5f342ec87219ae468`  
		Last Modified: Sat, 19 Mar 2022 04:13:29 GMT  
		Size: 4.9 MB (4906725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eb5f55c031ecf1698fa52d24bcc7293768ec4b8354a9fcb027d7df82bcd29c`  
		Last Modified: Sat, 19 Mar 2022 04:13:28 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7c33b81b950f8a1a9022072b612f4c23fbe50467f65c51033c2e831bcd3b0f`  
		Last Modified: Sat, 19 Mar 2022 04:13:28 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721d2dd815280a880f5d95bd85e9bb025a5e6a013fed0c0872d3b93c362f0634`  
		Last Modified: Sat, 19 Mar 2022 04:13:28 GMT  
		Size: 5.0 KB (5014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta`

```console
$ docker pull influxdb@sha256:d0240f21f89ae3d7cec4acd7f8cd750f44d0dd00e0ba18f508969130dff47471
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:b76d35eb1b56e57f22a38b623f452c15770822e38f9f309b870fd15588757801
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84493855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:081ce2abdbb8d32f017e6fa5582fd9bd760c9f9004f91ab420a02940519e09e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 08:48:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 08:52:18 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:53:19 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Sat, 19 Mar 2022 08:53:19 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:53:19 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:53:19 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:53:19 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:53:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:53:19 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed2a5dd9f694ca3959c4d1f4dac396d982b53c52b10b27d008da8f4aba040b8`  
		Last Modified: Sat, 19 Mar 2022 08:57:45 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4992723de53d8c0fbf3427d7d82e32278cdc6fb974adf1f202d282f2803846b3`  
		Last Modified: Sat, 19 Mar 2022 09:00:46 GMT  
		Size: 23.4 MB (23416969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f938aaece62656aeed448d46875c5090e41b32f0dc6292cef7ad512a7a6f67`  
		Last Modified: Sat, 19 Mar 2022 09:00:42 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38110311c491242933400eb982b1c811e8ceef8cc16a07d8396623de246a369`  
		Last Modified: Sat, 19 Mar 2022 09:00:42 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:f9ebef848c77b595c77ee0eaf6ab978b8dc69468ef104b3f9b7fa4a88ae10092
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:866f5587dba36266786414c65d3b322628296778c30561297a69b84070f2e5e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27584917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83b8b4d5495d637ee6649737dda3c65582ed6d18009f548712d8a1fbc65488`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 19 Mar 2022 08:48:10 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Sat, 19 Mar 2022 08:52:27 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Sat, 19 Mar 2022 08:54:02 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 19 Mar 2022 08:54:02 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Sat, 19 Mar 2022 08:54:02 GMT
EXPOSE 8091
# Sat, 19 Mar 2022 08:54:02 GMT
VOLUME [/var/lib/influxdb]
# Sat, 19 Mar 2022 08:54:02 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Sat, 19 Mar 2022 08:54:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 08:54:02 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa1326b35d047e371043a2411e65bd818c27909ab1ecf1ce37b55741744e890`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd267c51008fbf4dfa853c781b9b36b889d7d37878a84951119e28c74ba724e`  
		Last Modified: Sat, 19 Mar 2022 08:58:03 GMT  
		Size: 1.5 MB (1475021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0043723f2d668517ea2dd3c7f050fc58c203aef11bc2f8a374f2f98397286d5`  
		Last Modified: Sat, 19 Mar 2022 09:01:01 GMT  
		Size: 23.3 MB (23292980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005777352236f2ef3b11e4ba9451d590459f4f8d684f356cece973ba5782c54a`  
		Last Modified: Sat, 19 Mar 2022 09:00:58 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5c86b33a986181c1f1bb66954a31888f6ed2907d490db462a2da4a8a28060`  
		Last Modified: Sat, 19 Mar 2022 09:00:58 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
