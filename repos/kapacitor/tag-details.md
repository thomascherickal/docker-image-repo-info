<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.6`](#kapacitor16)
-	[`kapacitor:1.6-alpine`](#kapacitor16-alpine)
-	[`kapacitor:1.6.6`](#kapacitor166)
-	[`kapacitor:1.6.6-alpine`](#kapacitor166-alpine)
-	[`kapacitor:1.7`](#kapacitor17)
-	[`kapacitor:1.7-alpine`](#kapacitor17-alpine)
-	[`kapacitor:1.7.1`](#kapacitor171)
-	[`kapacitor:1.7.1-alpine`](#kapacitor171-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.6`

```console
$ docker pull kapacitor@sha256:bffd61db8dc7b77ff14005b9e5cb29ca214f995492348617ca36ed95910f49cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:108bcb804fd9407b08108d328406076feb2047cc70b3b33bebb51ed183f53748
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136318669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd58791edbb53abccfdab76ede90895fbc360b467ad4d6482a0466b88083a23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 12:39:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 02 Dec 2023 12:39:39 GMT
ENV KAPACITOR_VERSION=1.6.6
# Sat, 02 Dec 2023 12:39:45 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 02 Dec 2023 12:39:46 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 02 Dec 2023 12:39:46 GMT
EXPOSE 9092
# Sat, 02 Dec 2023 12:39:46 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 02 Dec 2023 12:39:46 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 02 Dec 2023 12:39:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 12:39:46 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477f20426928d47720e5a46878100e6fce0a039a472138a9f53239c8bf2630b8`  
		Last Modified: Sat, 02 Dec 2023 04:28:12 GMT  
		Size: 7.1 MB (7120280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ab435dbead8177acc8665501f6929d1d89ca3c464647563b7fd3f6a1ab021`  
		Last Modified: Sat, 02 Dec 2023 12:40:13 GMT  
		Size: 33.1 MB (33078984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f06c3d709deeea9d5b54d879ad7bd1180530d591a03c6a4edabe80b4c6c294`  
		Last Modified: Sat, 02 Dec 2023 12:40:18 GMT  
		Size: 65.7 MB (65672626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7827af41609524fa809c4bdfa05ae5429a6f60c18b2e8f59356d5615aae7e21`  
		Last Modified: Sat, 02 Dec 2023 12:40:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65454840e13d5dd3f5c9262379f5e1aade885518bae4a8ec20fbe73db3c01097`  
		Last Modified: Sat, 02 Dec 2023 12:40:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:b6ede375dab3e1eb784a49ab086e9ab4bd6f85f8700ea321a17b38ced69f862b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127842289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2587e0103956f1251a8390b580cb15db109e00afc80e173beef22e851fd25ed7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:12:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 08:35:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 02 Dec 2023 08:35:34 GMT
ENV KAPACITOR_VERSION=1.6.6
# Sat, 02 Dec 2023 08:35:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 02 Dec 2023 08:35:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 02 Dec 2023 08:35:41 GMT
EXPOSE 9092
# Sat, 02 Dec 2023 08:35:41 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 02 Dec 2023 08:35:41 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 02 Dec 2023 08:35:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 08:35:41 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a564c3a376a8286cb7726b7672399295eb2499b4e4f9624cda57245e41994a7`  
		Last Modified: Sat, 02 Dec 2023 05:27:38 GMT  
		Size: 7.1 MB (7066877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fce5fa786130714e3e02e2a56d83e31d31b7b10e42f627095ca64d181ec449`  
		Last Modified: Sat, 02 Dec 2023 08:36:05 GMT  
		Size: 30.7 MB (30704487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0255d2b772094dd49858b4ceeadf0593d66c92737749191fcbfe0db75132f7e7`  
		Last Modified: Sat, 02 Dec 2023 08:36:08 GMT  
		Size: 61.7 MB (61670531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539831abdaaa77f608266a80c18fb9b431915aa934d8929a2d9fae2e13501f64`  
		Last Modified: Sat, 02 Dec 2023 08:36:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1e429b9366e0f1cac5f55d92c5db7ddf9018fb136f179c2197befd23ec7a59`  
		Last Modified: Sat, 02 Dec 2023 08:36:02 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6-alpine`

```console
$ docker pull kapacitor@sha256:770470f0121116d4a954eef3b2ca51ba13eb86759dc1e8849046281d3e858791
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:19bb27862d145ea62492fe4fbcfb8882807bbd5b647ddefca77cb53cb2e1d411
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68673548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e411e715556ee4ccefc10b2a30efc720a53b3ac1971425840f79a8fec6de34`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 30 Nov 2023 23:23:05 GMT
ADD file:282274bb02b29182f35c732f021f3dab6de9f16a1ae24460061ad1abdca6444a in / 
# Thu, 30 Nov 2023 23:23:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:45:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:45:56 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 01 Dec 2023 06:45:56 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 01 Dec 2023 06:46:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 01 Dec 2023 06:46:05 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 01 Dec 2023 06:46:05 GMT
EXPOSE 9092
# Fri, 01 Dec 2023 06:46:05 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 01 Dec 2023 06:46:05 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 01 Dec 2023 06:46:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:46:05 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:070eb51debd997eca763a31532c01e2579afe94e43b110d84282a81cb576e342`  
		Last Modified: Thu, 30 Nov 2023 23:23:49 GMT  
		Size: 2.8 MB (2807782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29daf0c6dba8eae98e14270b54bfd982b50b5e3c2fbaf7d3b24b2ec907038da1`  
		Last Modified: Fri, 01 Dec 2023 06:46:35 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962db77fd55500a128d3b8bb0e438340db96929708d9cbddb62c0f545955b5e`  
		Last Modified: Fri, 01 Dec 2023 06:46:35 GMT  
		Size: 284.9 KB (284894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc34c2bc595174d47e07236c1de55d0c19a213ffe074ae43dfd9a91f535fce4d`  
		Last Modified: Fri, 01 Dec 2023 06:46:42 GMT  
		Size: 65.6 MB (65580139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f06cf33a3e774067e8b1d2f05b279ceb18c34c580a20ebb8bbddeae395a92fd`  
		Last Modified: Fri, 01 Dec 2023 06:46:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e00b1d8f5de33522a98d7d658e0a5462056ad2b8812e62a35dce18a3301e3ae`  
		Last Modified: Fri, 01 Dec 2023 06:46:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.6`

```console
$ docker pull kapacitor@sha256:bffd61db8dc7b77ff14005b9e5cb29ca214f995492348617ca36ed95910f49cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:108bcb804fd9407b08108d328406076feb2047cc70b3b33bebb51ed183f53748
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136318669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd58791edbb53abccfdab76ede90895fbc360b467ad4d6482a0466b88083a23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 12:39:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 02 Dec 2023 12:39:39 GMT
ENV KAPACITOR_VERSION=1.6.6
# Sat, 02 Dec 2023 12:39:45 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 02 Dec 2023 12:39:46 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 02 Dec 2023 12:39:46 GMT
EXPOSE 9092
# Sat, 02 Dec 2023 12:39:46 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 02 Dec 2023 12:39:46 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 02 Dec 2023 12:39:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 12:39:46 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477f20426928d47720e5a46878100e6fce0a039a472138a9f53239c8bf2630b8`  
		Last Modified: Sat, 02 Dec 2023 04:28:12 GMT  
		Size: 7.1 MB (7120280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ab435dbead8177acc8665501f6929d1d89ca3c464647563b7fd3f6a1ab021`  
		Last Modified: Sat, 02 Dec 2023 12:40:13 GMT  
		Size: 33.1 MB (33078984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f06c3d709deeea9d5b54d879ad7bd1180530d591a03c6a4edabe80b4c6c294`  
		Last Modified: Sat, 02 Dec 2023 12:40:18 GMT  
		Size: 65.7 MB (65672626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7827af41609524fa809c4bdfa05ae5429a6f60c18b2e8f59356d5615aae7e21`  
		Last Modified: Sat, 02 Dec 2023 12:40:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65454840e13d5dd3f5c9262379f5e1aade885518bae4a8ec20fbe73db3c01097`  
		Last Modified: Sat, 02 Dec 2023 12:40:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:b6ede375dab3e1eb784a49ab086e9ab4bd6f85f8700ea321a17b38ced69f862b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127842289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2587e0103956f1251a8390b580cb15db109e00afc80e173beef22e851fd25ed7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:12:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 08:35:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 02 Dec 2023 08:35:34 GMT
ENV KAPACITOR_VERSION=1.6.6
# Sat, 02 Dec 2023 08:35:40 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 02 Dec 2023 08:35:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 02 Dec 2023 08:35:41 GMT
EXPOSE 9092
# Sat, 02 Dec 2023 08:35:41 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 02 Dec 2023 08:35:41 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 02 Dec 2023 08:35:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 08:35:41 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a564c3a376a8286cb7726b7672399295eb2499b4e4f9624cda57245e41994a7`  
		Last Modified: Sat, 02 Dec 2023 05:27:38 GMT  
		Size: 7.1 MB (7066877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fce5fa786130714e3e02e2a56d83e31d31b7b10e42f627095ca64d181ec449`  
		Last Modified: Sat, 02 Dec 2023 08:36:05 GMT  
		Size: 30.7 MB (30704487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0255d2b772094dd49858b4ceeadf0593d66c92737749191fcbfe0db75132f7e7`  
		Last Modified: Sat, 02 Dec 2023 08:36:08 GMT  
		Size: 61.7 MB (61670531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539831abdaaa77f608266a80c18fb9b431915aa934d8929a2d9fae2e13501f64`  
		Last Modified: Sat, 02 Dec 2023 08:36:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1e429b9366e0f1cac5f55d92c5db7ddf9018fb136f179c2197befd23ec7a59`  
		Last Modified: Sat, 02 Dec 2023 08:36:02 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.6-alpine`

```console
$ docker pull kapacitor@sha256:770470f0121116d4a954eef3b2ca51ba13eb86759dc1e8849046281d3e858791
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:19bb27862d145ea62492fe4fbcfb8882807bbd5b647ddefca77cb53cb2e1d411
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68673548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e411e715556ee4ccefc10b2a30efc720a53b3ac1971425840f79a8fec6de34`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 30 Nov 2023 23:23:05 GMT
ADD file:282274bb02b29182f35c732f021f3dab6de9f16a1ae24460061ad1abdca6444a in / 
# Thu, 30 Nov 2023 23:23:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:45:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:45:56 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 01 Dec 2023 06:45:56 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 01 Dec 2023 06:46:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 01 Dec 2023 06:46:05 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 01 Dec 2023 06:46:05 GMT
EXPOSE 9092
# Fri, 01 Dec 2023 06:46:05 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 01 Dec 2023 06:46:05 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 01 Dec 2023 06:46:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:46:05 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:070eb51debd997eca763a31532c01e2579afe94e43b110d84282a81cb576e342`  
		Last Modified: Thu, 30 Nov 2023 23:23:49 GMT  
		Size: 2.8 MB (2807782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29daf0c6dba8eae98e14270b54bfd982b50b5e3c2fbaf7d3b24b2ec907038da1`  
		Last Modified: Fri, 01 Dec 2023 06:46:35 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962db77fd55500a128d3b8bb0e438340db96929708d9cbddb62c0f545955b5e`  
		Last Modified: Fri, 01 Dec 2023 06:46:35 GMT  
		Size: 284.9 KB (284894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc34c2bc595174d47e07236c1de55d0c19a213ffe074ae43dfd9a91f535fce4d`  
		Last Modified: Fri, 01 Dec 2023 06:46:42 GMT  
		Size: 65.6 MB (65580139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f06cf33a3e774067e8b1d2f05b279ceb18c34c580a20ebb8bbddeae395a92fd`  
		Last Modified: Fri, 01 Dec 2023 06:46:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e00b1d8f5de33522a98d7d658e0a5462056ad2b8812e62a35dce18a3301e3ae`  
		Last Modified: Fri, 01 Dec 2023 06:46:35 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.7`

```console
$ docker pull kapacitor@sha256:c549fc87e29a8264cc6533e1a4f83a15430fb247bacf79eb9041ad32ad8ddbce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.7` - linux; amd64

```console
$ docker pull kapacitor@sha256:ce6c7d0dfd8abeda512a77ed915c6c7573a13eb31624e1b2f2f3d02e45dad0cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137395674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c2c22412365a3c71f3e8d7249b3a07edc39a32e58c0bd69af790850de8f3ed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 12:39:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 02 Dec 2023 12:39:51 GMT
ENV KAPACITOR_VERSION=1.7.1
# Sat, 02 Dec 2023 12:39:56 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 02 Dec 2023 12:39:56 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 02 Dec 2023 12:39:57 GMT
EXPOSE 9092
# Sat, 02 Dec 2023 12:39:57 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 02 Dec 2023 12:39:57 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 02 Dec 2023 12:39:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 12:39:57 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477f20426928d47720e5a46878100e6fce0a039a472138a9f53239c8bf2630b8`  
		Last Modified: Sat, 02 Dec 2023 04:28:12 GMT  
		Size: 7.1 MB (7120280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ab435dbead8177acc8665501f6929d1d89ca3c464647563b7fd3f6a1ab021`  
		Last Modified: Sat, 02 Dec 2023 12:40:13 GMT  
		Size: 33.1 MB (33078984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd40c477509e01a52934bedc128a76b4e055065d615771dd1d9dca945a2d3da`  
		Last Modified: Sat, 02 Dec 2023 12:40:34 GMT  
		Size: 66.7 MB (66749631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76f76b0507ab6c5de6b8845458543d0106858d67210b355667714f717bf9d3`  
		Last Modified: Sat, 02 Dec 2023 12:40:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6036390738bd4b58d50194d1feaa6a60e2e2c2d237a9b53cbd04c6b2bdaaa2f`  
		Last Modified: Sat, 02 Dec 2023 12:40:26 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.7` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:afc8be6df43397039e091f6c5b89eaa3d93f6774ba353608f68605589aa5217d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128480589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8537b539aa8c3e2c49d5171ef3625b875e47ec4271c2be4cf25a3abfca32ca1f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:12:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 08:35:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 02 Dec 2023 08:35:44 GMT
ENV KAPACITOR_VERSION=1.7.1
# Sat, 02 Dec 2023 08:35:51 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 02 Dec 2023 08:35:52 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 02 Dec 2023 08:35:52 GMT
EXPOSE 9092
# Sat, 02 Dec 2023 08:35:52 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 02 Dec 2023 08:35:52 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 02 Dec 2023 08:35:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 08:35:52 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a564c3a376a8286cb7726b7672399295eb2499b4e4f9624cda57245e41994a7`  
		Last Modified: Sat, 02 Dec 2023 05:27:38 GMT  
		Size: 7.1 MB (7066877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fce5fa786130714e3e02e2a56d83e31d31b7b10e42f627095ca64d181ec449`  
		Last Modified: Sat, 02 Dec 2023 08:36:05 GMT  
		Size: 30.7 MB (30704487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19eed67e4a091716f780057123ccaf956877fe00546273888e827351251af137`  
		Last Modified: Sat, 02 Dec 2023 08:36:21 GMT  
		Size: 62.3 MB (62308828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ce6909c9575beb43d836b723d8d66e4d8b2eba6e8d136c9fa62ec55b775ad4`  
		Last Modified: Sat, 02 Dec 2023 08:36:15 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2ee2aebe330379a831bae167e748ecd5de63bae2a4427c5a3967d1b56e373c`  
		Last Modified: Sat, 02 Dec 2023 08:36:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.7-alpine`

```console
$ docker pull kapacitor@sha256:f55bf1d34d160d84fbd45f5b7a0eae6e5da897ab7387d24de0074f49b2507857
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.7-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:b072d72098ba1367c0a499550376c19e857d3ffefa1f51816d8748635101cc3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70368818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0cda841ba7ab1dbf90a27492fcc9f542e36896fa5576fda59b6286d2dc089b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:23:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:36:21 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 01 Dec 2023 06:46:11 GMT
ENV KAPACITOR_VERSION=1.7.1
# Fri, 01 Dec 2023 06:46:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 01 Dec 2023 06:46:22 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 01 Dec 2023 06:46:22 GMT
EXPOSE 9092
# Fri, 01 Dec 2023 06:46:22 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 01 Dec 2023 06:46:23 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 01 Dec 2023 06:46:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:46:23 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e958f39c4082f015dd7de32b1c116ef56e1e54010a31e991ec0c10e7feecc`  
		Last Modified: Fri, 01 Dec 2023 05:25:29 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822880f5cd7c4ada55339070e05a9bbdebfa8ffe320d8e04ef9484a76cce73b1`  
		Last Modified: Fri, 01 Dec 2023 06:37:19 GMT  
		Size: 284.7 KB (284691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab22e452e974cffc167b121dbd8b6c0155914a2fa051d859205749f7c1619ac`  
		Last Modified: Fri, 01 Dec 2023 06:46:59 GMT  
		Size: 66.7 MB (66680972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40a8ba1af30e277561a113de97fd0ebd420cd720493d70e4aab49bbffd1456f`  
		Last Modified: Fri, 01 Dec 2023 06:46:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde775a0479ab002c35ce9024783ff1289f9f8571195b60b1825540e39906c84`  
		Last Modified: Fri, 01 Dec 2023 06:46:51 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.7.1`

```console
$ docker pull kapacitor@sha256:c549fc87e29a8264cc6533e1a4f83a15430fb247bacf79eb9041ad32ad8ddbce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.7.1` - linux; amd64

```console
$ docker pull kapacitor@sha256:ce6c7d0dfd8abeda512a77ed915c6c7573a13eb31624e1b2f2f3d02e45dad0cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137395674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c2c22412365a3c71f3e8d7249b3a07edc39a32e58c0bd69af790850de8f3ed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 12:39:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 02 Dec 2023 12:39:51 GMT
ENV KAPACITOR_VERSION=1.7.1
# Sat, 02 Dec 2023 12:39:56 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 02 Dec 2023 12:39:56 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 02 Dec 2023 12:39:57 GMT
EXPOSE 9092
# Sat, 02 Dec 2023 12:39:57 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 02 Dec 2023 12:39:57 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 02 Dec 2023 12:39:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 12:39:57 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477f20426928d47720e5a46878100e6fce0a039a472138a9f53239c8bf2630b8`  
		Last Modified: Sat, 02 Dec 2023 04:28:12 GMT  
		Size: 7.1 MB (7120280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ab435dbead8177acc8665501f6929d1d89ca3c464647563b7fd3f6a1ab021`  
		Last Modified: Sat, 02 Dec 2023 12:40:13 GMT  
		Size: 33.1 MB (33078984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd40c477509e01a52934bedc128a76b4e055065d615771dd1d9dca945a2d3da`  
		Last Modified: Sat, 02 Dec 2023 12:40:34 GMT  
		Size: 66.7 MB (66749631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76f76b0507ab6c5de6b8845458543d0106858d67210b355667714f717bf9d3`  
		Last Modified: Sat, 02 Dec 2023 12:40:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6036390738bd4b58d50194d1feaa6a60e2e2c2d237a9b53cbd04c6b2bdaaa2f`  
		Last Modified: Sat, 02 Dec 2023 12:40:26 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.7.1` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:afc8be6df43397039e091f6c5b89eaa3d93f6774ba353608f68605589aa5217d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128480589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8537b539aa8c3e2c49d5171ef3625b875e47ec4271c2be4cf25a3abfca32ca1f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:12:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 08:35:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 02 Dec 2023 08:35:44 GMT
ENV KAPACITOR_VERSION=1.7.1
# Sat, 02 Dec 2023 08:35:51 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 02 Dec 2023 08:35:52 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 02 Dec 2023 08:35:52 GMT
EXPOSE 9092
# Sat, 02 Dec 2023 08:35:52 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 02 Dec 2023 08:35:52 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 02 Dec 2023 08:35:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 08:35:52 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a564c3a376a8286cb7726b7672399295eb2499b4e4f9624cda57245e41994a7`  
		Last Modified: Sat, 02 Dec 2023 05:27:38 GMT  
		Size: 7.1 MB (7066877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fce5fa786130714e3e02e2a56d83e31d31b7b10e42f627095ca64d181ec449`  
		Last Modified: Sat, 02 Dec 2023 08:36:05 GMT  
		Size: 30.7 MB (30704487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19eed67e4a091716f780057123ccaf956877fe00546273888e827351251af137`  
		Last Modified: Sat, 02 Dec 2023 08:36:21 GMT  
		Size: 62.3 MB (62308828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ce6909c9575beb43d836b723d8d66e4d8b2eba6e8d136c9fa62ec55b775ad4`  
		Last Modified: Sat, 02 Dec 2023 08:36:15 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2ee2aebe330379a831bae167e748ecd5de63bae2a4427c5a3967d1b56e373c`  
		Last Modified: Sat, 02 Dec 2023 08:36:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.7.1-alpine`

```console
$ docker pull kapacitor@sha256:f55bf1d34d160d84fbd45f5b7a0eae6e5da897ab7387d24de0074f49b2507857
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.7.1-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:b072d72098ba1367c0a499550376c19e857d3ffefa1f51816d8748635101cc3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70368818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0cda841ba7ab1dbf90a27492fcc9f542e36896fa5576fda59b6286d2dc089b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:23:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:36:21 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 01 Dec 2023 06:46:11 GMT
ENV KAPACITOR_VERSION=1.7.1
# Fri, 01 Dec 2023 06:46:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 01 Dec 2023 06:46:22 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 01 Dec 2023 06:46:22 GMT
EXPOSE 9092
# Fri, 01 Dec 2023 06:46:22 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 01 Dec 2023 06:46:23 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 01 Dec 2023 06:46:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:46:23 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e958f39c4082f015dd7de32b1c116ef56e1e54010a31e991ec0c10e7feecc`  
		Last Modified: Fri, 01 Dec 2023 05:25:29 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822880f5cd7c4ada55339070e05a9bbdebfa8ffe320d8e04ef9484a76cce73b1`  
		Last Modified: Fri, 01 Dec 2023 06:37:19 GMT  
		Size: 284.7 KB (284691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab22e452e974cffc167b121dbd8b6c0155914a2fa051d859205749f7c1619ac`  
		Last Modified: Fri, 01 Dec 2023 06:46:59 GMT  
		Size: 66.7 MB (66680972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40a8ba1af30e277561a113de97fd0ebd420cd720493d70e4aab49bbffd1456f`  
		Last Modified: Fri, 01 Dec 2023 06:46:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde775a0479ab002c35ce9024783ff1289f9f8571195b60b1825540e39906c84`  
		Last Modified: Fri, 01 Dec 2023 06:46:51 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:f55bf1d34d160d84fbd45f5b7a0eae6e5da897ab7387d24de0074f49b2507857
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:b072d72098ba1367c0a499550376c19e857d3ffefa1f51816d8748635101cc3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70368818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0cda841ba7ab1dbf90a27492fcc9f542e36896fa5576fda59b6286d2dc089b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:23:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:36:21 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 01 Dec 2023 06:46:11 GMT
ENV KAPACITOR_VERSION=1.7.1
# Fri, 01 Dec 2023 06:46:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-v${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 01 Dec 2023 06:46:22 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 01 Dec 2023 06:46:22 GMT
EXPOSE 9092
# Fri, 01 Dec 2023 06:46:22 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 01 Dec 2023 06:46:23 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 01 Dec 2023 06:46:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:46:23 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e958f39c4082f015dd7de32b1c116ef56e1e54010a31e991ec0c10e7feecc`  
		Last Modified: Fri, 01 Dec 2023 05:25:29 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822880f5cd7c4ada55339070e05a9bbdebfa8ffe320d8e04ef9484a76cce73b1`  
		Last Modified: Fri, 01 Dec 2023 06:37:19 GMT  
		Size: 284.7 KB (284691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab22e452e974cffc167b121dbd8b6c0155914a2fa051d859205749f7c1619ac`  
		Last Modified: Fri, 01 Dec 2023 06:46:59 GMT  
		Size: 66.7 MB (66680972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40a8ba1af30e277561a113de97fd0ebd420cd720493d70e4aab49bbffd1456f`  
		Last Modified: Fri, 01 Dec 2023 06:46:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde775a0479ab002c35ce9024783ff1289f9f8571195b60b1825540e39906c84`  
		Last Modified: Fri, 01 Dec 2023 06:46:51 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:c549fc87e29a8264cc6533e1a4f83a15430fb247bacf79eb9041ad32ad8ddbce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:ce6c7d0dfd8abeda512a77ed915c6c7573a13eb31624e1b2f2f3d02e45dad0cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137395674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c2c22412365a3c71f3e8d7249b3a07edc39a32e58c0bd69af790850de8f3ed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 12:39:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 02 Dec 2023 12:39:51 GMT
ENV KAPACITOR_VERSION=1.7.1
# Sat, 02 Dec 2023 12:39:56 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 02 Dec 2023 12:39:56 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 02 Dec 2023 12:39:57 GMT
EXPOSE 9092
# Sat, 02 Dec 2023 12:39:57 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 02 Dec 2023 12:39:57 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 02 Dec 2023 12:39:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 12:39:57 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477f20426928d47720e5a46878100e6fce0a039a472138a9f53239c8bf2630b8`  
		Last Modified: Sat, 02 Dec 2023 04:28:12 GMT  
		Size: 7.1 MB (7120280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ab435dbead8177acc8665501f6929d1d89ca3c464647563b7fd3f6a1ab021`  
		Last Modified: Sat, 02 Dec 2023 12:40:13 GMT  
		Size: 33.1 MB (33078984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd40c477509e01a52934bedc128a76b4e055065d615771dd1d9dca945a2d3da`  
		Last Modified: Sat, 02 Dec 2023 12:40:34 GMT  
		Size: 66.7 MB (66749631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76f76b0507ab6c5de6b8845458543d0106858d67210b355667714f717bf9d3`  
		Last Modified: Sat, 02 Dec 2023 12:40:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6036390738bd4b58d50194d1feaa6a60e2e2c2d237a9b53cbd04c6b2bdaaa2f`  
		Last Modified: Sat, 02 Dec 2023 12:40:26 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:afc8be6df43397039e091f6c5b89eaa3d93f6774ba353608f68605589aa5217d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128480589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8537b539aa8c3e2c49d5171ef3625b875e47ec4271c2be4cf25a3abfca32ca1f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:12:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 08:35:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 02 Dec 2023 08:35:44 GMT
ENV KAPACITOR_VERSION=1.7.1
# Sat, 02 Dec 2023 08:35:51 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 02 Dec 2023 08:35:52 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 02 Dec 2023 08:35:52 GMT
EXPOSE 9092
# Sat, 02 Dec 2023 08:35:52 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 02 Dec 2023 08:35:52 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 02 Dec 2023 08:35:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 08:35:52 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a564c3a376a8286cb7726b7672399295eb2499b4e4f9624cda57245e41994a7`  
		Last Modified: Sat, 02 Dec 2023 05:27:38 GMT  
		Size: 7.1 MB (7066877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fce5fa786130714e3e02e2a56d83e31d31b7b10e42f627095ca64d181ec449`  
		Last Modified: Sat, 02 Dec 2023 08:36:05 GMT  
		Size: 30.7 MB (30704487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19eed67e4a091716f780057123ccaf956877fe00546273888e827351251af137`  
		Last Modified: Sat, 02 Dec 2023 08:36:21 GMT  
		Size: 62.3 MB (62308828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ce6909c9575beb43d836b723d8d66e4d8b2eba6e8d136c9fa62ec55b775ad4`  
		Last Modified: Sat, 02 Dec 2023 08:36:15 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2ee2aebe330379a831bae167e748ecd5de63bae2a4427c5a3967d1b56e373c`  
		Last Modified: Sat, 02 Dec 2023 08:36:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
