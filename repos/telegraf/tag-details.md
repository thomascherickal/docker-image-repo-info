<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.19`](#telegraf119)
-	[`telegraf:1.19-alpine`](#telegraf119-alpine)
-	[`telegraf:1.19.3`](#telegraf1193)
-	[`telegraf:1.19.3-alpine`](#telegraf1193-alpine)
-	[`telegraf:1.20`](#telegraf120)
-	[`telegraf:1.20-alpine`](#telegraf120-alpine)
-	[`telegraf:1.20.4`](#telegraf1204)
-	[`telegraf:1.20.4-alpine`](#telegraf1204-alpine)
-	[`telegraf:1.21`](#telegraf121)
-	[`telegraf:1.21-alpine`](#telegraf121-alpine)
-	[`telegraf:1.21.3`](#telegraf1213)
-	[`telegraf:1.21.3-alpine`](#telegraf1213-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.19`

```console
$ docker pull telegraf@sha256:3bbdb3f342e9b58716cc51bbe58f8f73d2727d5b871f469b66aa9c02884b4271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.19` - linux; amd64

```console
$ docker pull telegraf@sha256:4835322f484f6bccae0e3363f07d2f0d8f64dc4dec0c63ddf956e79bfcc3783a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123887496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae61a77d2e17c31a0a20c9fc0c9924b844069dd81c7eb50a926bb530247cc44`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:25:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:26:02 GMT
ENV TELEGRAF_VERSION=1.19.3
# Fri, 28 Jan 2022 23:26:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:26:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:26:08 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:26:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:26:08 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a79e2bea7607ea4697b1955cfc012bb0ed97c80871af8bdd8bb1b63b9584b0`  
		Last Modified: Fri, 28 Jan 2022 23:29:33 GMT  
		Size: 18.8 MB (18760423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc2c7895804f68943ae0ea3a6aeece4d418d0c7e76d1c1140329c3f76ef6dab`  
		Last Modified: Fri, 28 Jan 2022 23:29:29 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8996f8645ba520e0b2c73328b4b29b49a12d880802c086d91c8461cafcb7b925`  
		Last Modified: Fri, 28 Jan 2022 23:29:36 GMT  
		Size: 34.2 MB (34182192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f945ab70ad543c5164552df76ff5db0f78b995b719791fb9a11082578c5fdad5`  
		Last Modified: Fri, 28 Jan 2022 23:29:29 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:73b426362fc5365fcf672ed1409c32487ed403e7fd196da04abe06720937b6f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114411002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4449c175c64d1d3f8a9692cecf4dc33fcd27da5ff1db512bbff79083035286a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:30 GMT
ADD file:19419917274a4a5aa3eceb0a6202f89e5b508368314f2bd0105897a847db4930 in / 
# Wed, 26 Jan 2022 01:41:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:37:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:38:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 29 Jan 2022 13:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 29 Jan 2022 13:45:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 29 Jan 2022 13:45:11 GMT
ENV TELEGRAF_VERSION=1.19.3
# Sat, 29 Jan 2022 13:45:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 29 Jan 2022 13:45:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 29 Jan 2022 13:45:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sat, 29 Jan 2022 13:45:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 29 Jan 2022 13:45:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:046501ac4c58f014cc320324f6023bbef17f28025428833449198a62a97849c0`  
		Last Modified: Wed, 26 Jan 2022 01:57:13 GMT  
		Size: 50.1 MB (50117358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29bf76217944d3c3b29fb3234ed71ba5a004ffcec0595d3704c6e6cfa169b68`  
		Last Modified: Wed, 26 Jan 2022 17:03:48 GMT  
		Size: 4.9 MB (4922334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0e88eaa9f33e97d48fa77ed2c178123150031494073f10c97755b3bd6370c1`  
		Last Modified: Wed, 26 Jan 2022 17:03:50 GMT  
		Size: 10.2 MB (10216891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f07aa7c84ba4dfe8f5cfc222c2afb20a1e0dd5dd52438027cc57cd5de81b344`  
		Last Modified: Sat, 29 Jan 2022 13:47:19 GMT  
		Size: 17.5 MB (17462211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c4a7f93f28554a0e10aa9ae7f34609c1c37058e73de11f9155c43400d8c777`  
		Last Modified: Sat, 29 Jan 2022 13:47:07 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e306cfe030b430161ee89eaece012dadc8334a2f4179f2b42760c6d8a4fea`  
		Last Modified: Sat, 29 Jan 2022 13:47:29 GMT  
		Size: 31.7 MB (31688958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8980353c4985cf9c2c758f84012fa346f6088fca0e9783bdb727a11a9a6c0083`  
		Last Modified: Sat, 29 Jan 2022 13:47:07 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:d63873ec13910564af893cef1e0b60c1970f864c7c91a299123027b81cc31cd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118754559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5ff17e5cb25fe092adb79f73e99827113f06ebda89c91641d5e032312f03167`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:52:09 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:52:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:52:55 GMT
ENV TELEGRAF_VERSION=1.19.3
# Fri, 28 Jan 2022 23:52:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:53:00 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:53:01 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:53:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:53:02 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9665c78b20b5f67d05c7907cd13b6c08e535420cb76afdea17f75af7cc25a2fc`  
		Last Modified: Fri, 28 Jan 2022 23:54:05 GMT  
		Size: 18.4 MB (18383003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b756b6770d48353a8db8cd3e2c6a904a166050daf8d31f38d5204c8d281ba39`  
		Last Modified: Fri, 28 Jan 2022 23:54:00 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1f3f3f2535e8e68e86a6391f7c2495823e820603e3118618a98f7796a75b43`  
		Last Modified: Fri, 28 Jan 2022 23:54:07 GMT  
		Size: 31.0 MB (30962011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c779e60f5e4610ea3e7c0e6419e455b69467c7e730a414932dd5537f92c1615`  
		Last Modified: Fri, 28 Jan 2022 23:54:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19-alpine`

```console
$ docker pull telegraf@sha256:c9f5a809f4f6d03f71cbdddfb484705760ba4b75439f9e087678fe3e8cdedbb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.19-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:85fc0f81de036e9f59876c1a82a409b2db79d004f2a11c14a546c574e0eab748
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40236525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8f0959c579b8738588ca0178551012ab445b16b168d5e35a254df298dffd3f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 23:26:22 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Jan 2022 23:26:24 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 28 Jan 2022 23:26:24 GMT
ENV TELEGRAF_VERSION=1.19.3
# Fri, 28 Jan 2022 23:27:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 28 Jan 2022 23:27:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:27:13 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 28 Jan 2022 23:27:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:27:13 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c171b8d76913f15ff251f40de7410868a7687d5a27eae89b156861bf6477559b`  
		Last Modified: Fri, 28 Jan 2022 23:29:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed6bc2d7abca8a1c07cd86d761c6e06ff959d03f351e8f99971d71d5a61775`  
		Last Modified: Fri, 28 Jan 2022 23:29:47 GMT  
		Size: 3.4 MB (3371423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f0e184d8efed716707d9c11baad98db4d37edaf9080a94d1866e6770f95f62`  
		Last Modified: Fri, 28 Jan 2022 23:29:53 GMT  
		Size: 34.0 MB (34046207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466d2a91d9e57a42ad1bc05a782c5cb992d5cbfa3a04c739e8b88a3a0b3950eb`  
		Last Modified: Fri, 28 Jan 2022 23:29:46 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19.3`

```console
$ docker pull telegraf@sha256:3bbdb3f342e9b58716cc51bbe58f8f73d2727d5b871f469b66aa9c02884b4271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.19.3` - linux; amd64

```console
$ docker pull telegraf@sha256:4835322f484f6bccae0e3363f07d2f0d8f64dc4dec0c63ddf956e79bfcc3783a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123887496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae61a77d2e17c31a0a20c9fc0c9924b844069dd81c7eb50a926bb530247cc44`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:25:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:26:02 GMT
ENV TELEGRAF_VERSION=1.19.3
# Fri, 28 Jan 2022 23:26:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:26:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:26:08 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:26:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:26:08 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a79e2bea7607ea4697b1955cfc012bb0ed97c80871af8bdd8bb1b63b9584b0`  
		Last Modified: Fri, 28 Jan 2022 23:29:33 GMT  
		Size: 18.8 MB (18760423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc2c7895804f68943ae0ea3a6aeece4d418d0c7e76d1c1140329c3f76ef6dab`  
		Last Modified: Fri, 28 Jan 2022 23:29:29 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8996f8645ba520e0b2c73328b4b29b49a12d880802c086d91c8461cafcb7b925`  
		Last Modified: Fri, 28 Jan 2022 23:29:36 GMT  
		Size: 34.2 MB (34182192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f945ab70ad543c5164552df76ff5db0f78b995b719791fb9a11082578c5fdad5`  
		Last Modified: Fri, 28 Jan 2022 23:29:29 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:73b426362fc5365fcf672ed1409c32487ed403e7fd196da04abe06720937b6f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114411002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4449c175c64d1d3f8a9692cecf4dc33fcd27da5ff1db512bbff79083035286a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:30 GMT
ADD file:19419917274a4a5aa3eceb0a6202f89e5b508368314f2bd0105897a847db4930 in / 
# Wed, 26 Jan 2022 01:41:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:37:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:38:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 29 Jan 2022 13:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 29 Jan 2022 13:45:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 29 Jan 2022 13:45:11 GMT
ENV TELEGRAF_VERSION=1.19.3
# Sat, 29 Jan 2022 13:45:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 29 Jan 2022 13:45:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 29 Jan 2022 13:45:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sat, 29 Jan 2022 13:45:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 29 Jan 2022 13:45:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:046501ac4c58f014cc320324f6023bbef17f28025428833449198a62a97849c0`  
		Last Modified: Wed, 26 Jan 2022 01:57:13 GMT  
		Size: 50.1 MB (50117358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29bf76217944d3c3b29fb3234ed71ba5a004ffcec0595d3704c6e6cfa169b68`  
		Last Modified: Wed, 26 Jan 2022 17:03:48 GMT  
		Size: 4.9 MB (4922334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0e88eaa9f33e97d48fa77ed2c178123150031494073f10c97755b3bd6370c1`  
		Last Modified: Wed, 26 Jan 2022 17:03:50 GMT  
		Size: 10.2 MB (10216891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f07aa7c84ba4dfe8f5cfc222c2afb20a1e0dd5dd52438027cc57cd5de81b344`  
		Last Modified: Sat, 29 Jan 2022 13:47:19 GMT  
		Size: 17.5 MB (17462211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c4a7f93f28554a0e10aa9ae7f34609c1c37058e73de11f9155c43400d8c777`  
		Last Modified: Sat, 29 Jan 2022 13:47:07 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e306cfe030b430161ee89eaece012dadc8334a2f4179f2b42760c6d8a4fea`  
		Last Modified: Sat, 29 Jan 2022 13:47:29 GMT  
		Size: 31.7 MB (31688958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8980353c4985cf9c2c758f84012fa346f6088fca0e9783bdb727a11a9a6c0083`  
		Last Modified: Sat, 29 Jan 2022 13:47:07 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:d63873ec13910564af893cef1e0b60c1970f864c7c91a299123027b81cc31cd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118754559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5ff17e5cb25fe092adb79f73e99827113f06ebda89c91641d5e032312f03167`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:52:09 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:52:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:52:55 GMT
ENV TELEGRAF_VERSION=1.19.3
# Fri, 28 Jan 2022 23:52:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:53:00 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:53:01 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:53:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:53:02 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9665c78b20b5f67d05c7907cd13b6c08e535420cb76afdea17f75af7cc25a2fc`  
		Last Modified: Fri, 28 Jan 2022 23:54:05 GMT  
		Size: 18.4 MB (18383003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b756b6770d48353a8db8cd3e2c6a904a166050daf8d31f38d5204c8d281ba39`  
		Last Modified: Fri, 28 Jan 2022 23:54:00 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1f3f3f2535e8e68e86a6391f7c2495823e820603e3118618a98f7796a75b43`  
		Last Modified: Fri, 28 Jan 2022 23:54:07 GMT  
		Size: 31.0 MB (30962011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c779e60f5e4610ea3e7c0e6419e455b69467c7e730a414932dd5537f92c1615`  
		Last Modified: Fri, 28 Jan 2022 23:54:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19.3-alpine`

```console
$ docker pull telegraf@sha256:c9f5a809f4f6d03f71cbdddfb484705760ba4b75439f9e087678fe3e8cdedbb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.19.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:85fc0f81de036e9f59876c1a82a409b2db79d004f2a11c14a546c574e0eab748
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40236525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8f0959c579b8738588ca0178551012ab445b16b168d5e35a254df298dffd3f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 23:26:22 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Jan 2022 23:26:24 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 28 Jan 2022 23:26:24 GMT
ENV TELEGRAF_VERSION=1.19.3
# Fri, 28 Jan 2022 23:27:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 28 Jan 2022 23:27:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:27:13 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 28 Jan 2022 23:27:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:27:13 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c171b8d76913f15ff251f40de7410868a7687d5a27eae89b156861bf6477559b`  
		Last Modified: Fri, 28 Jan 2022 23:29:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed6bc2d7abca8a1c07cd86d761c6e06ff959d03f351e8f99971d71d5a61775`  
		Last Modified: Fri, 28 Jan 2022 23:29:47 GMT  
		Size: 3.4 MB (3371423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f0e184d8efed716707d9c11baad98db4d37edaf9080a94d1866e6770f95f62`  
		Last Modified: Fri, 28 Jan 2022 23:29:53 GMT  
		Size: 34.0 MB (34046207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466d2a91d9e57a42ad1bc05a782c5cb992d5cbfa3a04c739e8b88a3a0b3950eb`  
		Last Modified: Fri, 28 Jan 2022 23:29:46 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20`

```console
$ docker pull telegraf@sha256:50a78839075ad232d4ec8a5f9ee72e7bdeaa35d5b65ecd78cf22e4ad103f64d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.20` - linux; amd64

```console
$ docker pull telegraf@sha256:cf66e29cd2104d0ded41e3e353cd726be22c657906c3c5583fc286fca92abf53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125333484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c176090ea2b0ba5690c8cde9507bf6672fc33088a137ad194f7b4034420cc51`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:25:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:27:19 GMT
ENV TELEGRAF_VERSION=1.20.4
# Fri, 28 Jan 2022 23:27:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:27:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:27:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:27:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a79e2bea7607ea4697b1955cfc012bb0ed97c80871af8bdd8bb1b63b9584b0`  
		Last Modified: Fri, 28 Jan 2022 23:29:33 GMT  
		Size: 18.8 MB (18760423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc2c7895804f68943ae0ea3a6aeece4d418d0c7e76d1c1140329c3f76ef6dab`  
		Last Modified: Fri, 28 Jan 2022 23:29:29 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb284e47fe2346c0b73b142b0426bdd8043efb681ae4fc62669719c2e075113`  
		Last Modified: Fri, 28 Jan 2022 23:30:09 GMT  
		Size: 35.6 MB (35628181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba5e4f97cfc9b657c1a46d66c22f837a80dc0f8858581e7ff06864eda3d2589`  
		Last Modified: Fri, 28 Jan 2022 23:30:03 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:cc43e5a0882f996085cc601d01623d146d54ac9ab7080dbea14cbd829ba21749
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115811581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f1cefe00c96a28d2fa66c96c0f162094950a75300aca2a0703e20a05b26a11d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:30 GMT
ADD file:19419917274a4a5aa3eceb0a6202f89e5b508368314f2bd0105897a847db4930 in / 
# Wed, 26 Jan 2022 01:41:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:37:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:38:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 29 Jan 2022 13:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 29 Jan 2022 13:45:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 29 Jan 2022 13:45:38 GMT
ENV TELEGRAF_VERSION=1.20.4
# Sat, 29 Jan 2022 13:45:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 29 Jan 2022 13:45:52 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 29 Jan 2022 13:45:52 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sat, 29 Jan 2022 13:45:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 29 Jan 2022 13:45:53 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:046501ac4c58f014cc320324f6023bbef17f28025428833449198a62a97849c0`  
		Last Modified: Wed, 26 Jan 2022 01:57:13 GMT  
		Size: 50.1 MB (50117358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29bf76217944d3c3b29fb3234ed71ba5a004ffcec0595d3704c6e6cfa169b68`  
		Last Modified: Wed, 26 Jan 2022 17:03:48 GMT  
		Size: 4.9 MB (4922334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0e88eaa9f33e97d48fa77ed2c178123150031494073f10c97755b3bd6370c1`  
		Last Modified: Wed, 26 Jan 2022 17:03:50 GMT  
		Size: 10.2 MB (10216891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f07aa7c84ba4dfe8f5cfc222c2afb20a1e0dd5dd52438027cc57cd5de81b344`  
		Last Modified: Sat, 29 Jan 2022 13:47:19 GMT  
		Size: 17.5 MB (17462211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c4a7f93f28554a0e10aa9ae7f34609c1c37058e73de11f9155c43400d8c777`  
		Last Modified: Sat, 29 Jan 2022 13:47:07 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a792b5eccce5498dff1a842700935aed4893fb2a392d5109aecd9b673ab46ea2`  
		Last Modified: Sat, 29 Jan 2022 13:48:04 GMT  
		Size: 33.1 MB (33089538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699210925450b7446fff21e8af4fc08e87dd120c28a24a8e53d6d3e2f945665d`  
		Last Modified: Sat, 29 Jan 2022 13:47:41 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3b47fc10a7237b18de3c44fb243ded8003368d54712843dce04c1e8fbb4eef5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120156790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3543f1e2de0bec1ea0cd27cd234398ba38b82d610fa053ec707d48b12a0df5f4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:52:09 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:52:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:53:16 GMT
ENV TELEGRAF_VERSION=1.20.4
# Fri, 28 Jan 2022 23:53:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:53:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:53:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:53:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:53:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9665c78b20b5f67d05c7907cd13b6c08e535420cb76afdea17f75af7cc25a2fc`  
		Last Modified: Fri, 28 Jan 2022 23:54:05 GMT  
		Size: 18.4 MB (18383003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b756b6770d48353a8db8cd3e2c6a904a166050daf8d31f38d5204c8d281ba39`  
		Last Modified: Fri, 28 Jan 2022 23:54:00 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a60be4c7aba05af09a1c126e9d44fcfd19e23b510d5b8cbcd246f42441bb4ea`  
		Last Modified: Fri, 28 Jan 2022 23:54:24 GMT  
		Size: 32.4 MB (32364241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb935cf458ac29469125d7aca141e6a5bc2807546ae3349c581fe60931b1873`  
		Last Modified: Fri, 28 Jan 2022 23:54:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20-alpine`

```console
$ docker pull telegraf@sha256:aa03baeda0abfa8dc32065529e420cd75386f49ee41ac45e7963768a8ac8bfd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.20-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:d2fff1c5de0a5a654dde91a7eebf9df1e8ecd347f0e4db18dd4db32616d726ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41660453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da896b6a94aa585e273ea2b40050cd6eac36cbbfb2b4326568c50408641acce9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 23:26:22 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Jan 2022 23:26:24 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 28 Jan 2022 23:27:27 GMT
ENV TELEGRAF_VERSION=1.20.4
# Fri, 28 Jan 2022 23:28:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 28 Jan 2022 23:28:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:28:12 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 28 Jan 2022 23:28:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:28:12 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c171b8d76913f15ff251f40de7410868a7687d5a27eae89b156861bf6477559b`  
		Last Modified: Fri, 28 Jan 2022 23:29:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed6bc2d7abca8a1c07cd86d761c6e06ff959d03f351e8f99971d71d5a61775`  
		Last Modified: Fri, 28 Jan 2022 23:29:47 GMT  
		Size: 3.4 MB (3371423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84619f4c63ebf6103fb02510821a7243d9dac501bd3c742e9be7a02bdcfd789e`  
		Last Modified: Fri, 28 Jan 2022 23:30:25 GMT  
		Size: 35.5 MB (35470136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5b34219d3fc381b7a40e51ad7b32a1f09c0be29aea593a90e7e3c56da83c42`  
		Last Modified: Fri, 28 Jan 2022 23:30:19 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20.4`

```console
$ docker pull telegraf@sha256:50a78839075ad232d4ec8a5f9ee72e7bdeaa35d5b65ecd78cf22e4ad103f64d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.20.4` - linux; amd64

```console
$ docker pull telegraf@sha256:cf66e29cd2104d0ded41e3e353cd726be22c657906c3c5583fc286fca92abf53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125333484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c176090ea2b0ba5690c8cde9507bf6672fc33088a137ad194f7b4034420cc51`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:25:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:27:19 GMT
ENV TELEGRAF_VERSION=1.20.4
# Fri, 28 Jan 2022 23:27:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:27:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:27:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:27:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a79e2bea7607ea4697b1955cfc012bb0ed97c80871af8bdd8bb1b63b9584b0`  
		Last Modified: Fri, 28 Jan 2022 23:29:33 GMT  
		Size: 18.8 MB (18760423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc2c7895804f68943ae0ea3a6aeece4d418d0c7e76d1c1140329c3f76ef6dab`  
		Last Modified: Fri, 28 Jan 2022 23:29:29 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb284e47fe2346c0b73b142b0426bdd8043efb681ae4fc62669719c2e075113`  
		Last Modified: Fri, 28 Jan 2022 23:30:09 GMT  
		Size: 35.6 MB (35628181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba5e4f97cfc9b657c1a46d66c22f837a80dc0f8858581e7ff06864eda3d2589`  
		Last Modified: Fri, 28 Jan 2022 23:30:03 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:cc43e5a0882f996085cc601d01623d146d54ac9ab7080dbea14cbd829ba21749
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115811581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f1cefe00c96a28d2fa66c96c0f162094950a75300aca2a0703e20a05b26a11d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:30 GMT
ADD file:19419917274a4a5aa3eceb0a6202f89e5b508368314f2bd0105897a847db4930 in / 
# Wed, 26 Jan 2022 01:41:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:37:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:38:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 29 Jan 2022 13:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 29 Jan 2022 13:45:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 29 Jan 2022 13:45:38 GMT
ENV TELEGRAF_VERSION=1.20.4
# Sat, 29 Jan 2022 13:45:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 29 Jan 2022 13:45:52 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 29 Jan 2022 13:45:52 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sat, 29 Jan 2022 13:45:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 29 Jan 2022 13:45:53 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:046501ac4c58f014cc320324f6023bbef17f28025428833449198a62a97849c0`  
		Last Modified: Wed, 26 Jan 2022 01:57:13 GMT  
		Size: 50.1 MB (50117358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29bf76217944d3c3b29fb3234ed71ba5a004ffcec0595d3704c6e6cfa169b68`  
		Last Modified: Wed, 26 Jan 2022 17:03:48 GMT  
		Size: 4.9 MB (4922334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0e88eaa9f33e97d48fa77ed2c178123150031494073f10c97755b3bd6370c1`  
		Last Modified: Wed, 26 Jan 2022 17:03:50 GMT  
		Size: 10.2 MB (10216891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f07aa7c84ba4dfe8f5cfc222c2afb20a1e0dd5dd52438027cc57cd5de81b344`  
		Last Modified: Sat, 29 Jan 2022 13:47:19 GMT  
		Size: 17.5 MB (17462211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c4a7f93f28554a0e10aa9ae7f34609c1c37058e73de11f9155c43400d8c777`  
		Last Modified: Sat, 29 Jan 2022 13:47:07 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a792b5eccce5498dff1a842700935aed4893fb2a392d5109aecd9b673ab46ea2`  
		Last Modified: Sat, 29 Jan 2022 13:48:04 GMT  
		Size: 33.1 MB (33089538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699210925450b7446fff21e8af4fc08e87dd120c28a24a8e53d6d3e2f945665d`  
		Last Modified: Sat, 29 Jan 2022 13:47:41 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3b47fc10a7237b18de3c44fb243ded8003368d54712843dce04c1e8fbb4eef5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120156790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3543f1e2de0bec1ea0cd27cd234398ba38b82d610fa053ec707d48b12a0df5f4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:52:09 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:52:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:53:16 GMT
ENV TELEGRAF_VERSION=1.20.4
# Fri, 28 Jan 2022 23:53:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:53:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:53:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:53:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:53:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9665c78b20b5f67d05c7907cd13b6c08e535420cb76afdea17f75af7cc25a2fc`  
		Last Modified: Fri, 28 Jan 2022 23:54:05 GMT  
		Size: 18.4 MB (18383003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b756b6770d48353a8db8cd3e2c6a904a166050daf8d31f38d5204c8d281ba39`  
		Last Modified: Fri, 28 Jan 2022 23:54:00 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a60be4c7aba05af09a1c126e9d44fcfd19e23b510d5b8cbcd246f42441bb4ea`  
		Last Modified: Fri, 28 Jan 2022 23:54:24 GMT  
		Size: 32.4 MB (32364241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb935cf458ac29469125d7aca141e6a5bc2807546ae3349c581fe60931b1873`  
		Last Modified: Fri, 28 Jan 2022 23:54:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20.4-alpine`

```console
$ docker pull telegraf@sha256:aa03baeda0abfa8dc32065529e420cd75386f49ee41ac45e7963768a8ac8bfd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.20.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:d2fff1c5de0a5a654dde91a7eebf9df1e8ecd347f0e4db18dd4db32616d726ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41660453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da896b6a94aa585e273ea2b40050cd6eac36cbbfb2b4326568c50408641acce9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 23:26:22 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Jan 2022 23:26:24 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 28 Jan 2022 23:27:27 GMT
ENV TELEGRAF_VERSION=1.20.4
# Fri, 28 Jan 2022 23:28:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 28 Jan 2022 23:28:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:28:12 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 28 Jan 2022 23:28:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:28:12 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c171b8d76913f15ff251f40de7410868a7687d5a27eae89b156861bf6477559b`  
		Last Modified: Fri, 28 Jan 2022 23:29:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed6bc2d7abca8a1c07cd86d761c6e06ff959d03f351e8f99971d71d5a61775`  
		Last Modified: Fri, 28 Jan 2022 23:29:47 GMT  
		Size: 3.4 MB (3371423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84619f4c63ebf6103fb02510821a7243d9dac501bd3c742e9be7a02bdcfd789e`  
		Last Modified: Fri, 28 Jan 2022 23:30:25 GMT  
		Size: 35.5 MB (35470136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5b34219d3fc381b7a40e51ad7b32a1f09c0be29aea593a90e7e3c56da83c42`  
		Last Modified: Fri, 28 Jan 2022 23:30:19 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21`

```console
$ docker pull telegraf@sha256:67e87c2587a45aa8afb6c25816ca622244916559b0edd3fdcd1c7ad3a7dd51ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.21` - linux; amd64

```console
$ docker pull telegraf@sha256:c211d523b235c2689145a17bff97947c7d945b67643e8e4baf8e8bf7c54e4893
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126360633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26fe59ae9f545a0cdf0f33e64927d84ca81a292b60d304df1750a38deabf7f57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:25:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:28:15 GMT
ENV TELEGRAF_VERSION=1.21.3
# Fri, 28 Jan 2022 23:28:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:28:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:28:19 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:28:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:28:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a79e2bea7607ea4697b1955cfc012bb0ed97c80871af8bdd8bb1b63b9584b0`  
		Last Modified: Fri, 28 Jan 2022 23:29:33 GMT  
		Size: 18.8 MB (18760423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc2c7895804f68943ae0ea3a6aeece4d418d0c7e76d1c1140329c3f76ef6dab`  
		Last Modified: Fri, 28 Jan 2022 23:29:29 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2a38225cfce41fe953343750113cb7a5b3d439c26d6732058f980336a3dac1`  
		Last Modified: Fri, 28 Jan 2022 23:30:41 GMT  
		Size: 36.7 MB (36655328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8507884f731d8be3ba24a6f77d13ca607bd840baba7f6053b5b9a618bb31ea1d`  
		Last Modified: Fri, 28 Jan 2022 23:30:35 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:e3698467c203120b926fa88b656f3d713bfcd6dd2b9a8c1002a8dba080ca8b72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116697145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b246266aa499bfbed882048abba3254fc7d7ba70cf44091b3349ea71b635b74b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:30 GMT
ADD file:19419917274a4a5aa3eceb0a6202f89e5b508368314f2bd0105897a847db4930 in / 
# Wed, 26 Jan 2022 01:41:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:37:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:38:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 29 Jan 2022 13:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 29 Jan 2022 13:45:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 29 Jan 2022 13:46:05 GMT
ENV TELEGRAF_VERSION=1.21.3
# Sat, 29 Jan 2022 13:46:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 29 Jan 2022 13:46:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 29 Jan 2022 13:46:19 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sat, 29 Jan 2022 13:46:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 29 Jan 2022 13:46:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:046501ac4c58f014cc320324f6023bbef17f28025428833449198a62a97849c0`  
		Last Modified: Wed, 26 Jan 2022 01:57:13 GMT  
		Size: 50.1 MB (50117358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29bf76217944d3c3b29fb3234ed71ba5a004ffcec0595d3704c6e6cfa169b68`  
		Last Modified: Wed, 26 Jan 2022 17:03:48 GMT  
		Size: 4.9 MB (4922334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0e88eaa9f33e97d48fa77ed2c178123150031494073f10c97755b3bd6370c1`  
		Last Modified: Wed, 26 Jan 2022 17:03:50 GMT  
		Size: 10.2 MB (10216891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f07aa7c84ba4dfe8f5cfc222c2afb20a1e0dd5dd52438027cc57cd5de81b344`  
		Last Modified: Sat, 29 Jan 2022 13:47:19 GMT  
		Size: 17.5 MB (17462211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c4a7f93f28554a0e10aa9ae7f34609c1c37058e73de11f9155c43400d8c777`  
		Last Modified: Sat, 29 Jan 2022 13:47:07 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d1b7e72a275f75e811d88df1a5ae10c921825a1473e41b29ec52a975164865`  
		Last Modified: Sat, 29 Jan 2022 13:48:40 GMT  
		Size: 34.0 MB (33975104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bb0a6707ff9222bdb3c5659c13cc45048a6795e940f8308a46f897e87fff84`  
		Last Modified: Sat, 29 Jan 2022 13:48:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:22da85a304e370d58ed66a3e8bf934f44af72677d53418b82968fa0a63ae7a02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121051528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f6d0364452d9f2eec44619d8fdbe1d0f43ca4b91dae249762b167a8febbd1a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:52:09 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:52:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:53:30 GMT
ENV TELEGRAF_VERSION=1.21.3
# Fri, 28 Jan 2022 23:53:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:53:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:53:37 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:53:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:53:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9665c78b20b5f67d05c7907cd13b6c08e535420cb76afdea17f75af7cc25a2fc`  
		Last Modified: Fri, 28 Jan 2022 23:54:05 GMT  
		Size: 18.4 MB (18383003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b756b6770d48353a8db8cd3e2c6a904a166050daf8d31f38d5204c8d281ba39`  
		Last Modified: Fri, 28 Jan 2022 23:54:00 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4de1414d58946d002c2e158b170383f566f798146bfa40bb5a9321c5d682e40`  
		Last Modified: Fri, 28 Jan 2022 23:54:40 GMT  
		Size: 33.3 MB (33258980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be80f793c1416b90d5c727f361f23da506a6b49cbb7c79e3c8107b285a5569e`  
		Last Modified: Fri, 28 Jan 2022 23:54:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21-alpine`

```console
$ docker pull telegraf@sha256:89942f98fc29476bb3fd2dbef701ce799b4c7d786ea1fa2be7513bc22862b937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.21-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:6c6414799ca0050388518cb49b6663a574a29685d7577f9fa1ffa18b06f58bcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42692659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a67941483c88e155c94bf66f279ed555367f8236298ee1154edbebdab0e3ef6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 23:26:22 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Jan 2022 23:26:24 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 28 Jan 2022 23:28:23 GMT
ENV TELEGRAF_VERSION=1.21.3
# Fri, 28 Jan 2022 23:29:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 28 Jan 2022 23:29:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:29:08 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 28 Jan 2022 23:29:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:29:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c171b8d76913f15ff251f40de7410868a7687d5a27eae89b156861bf6477559b`  
		Last Modified: Fri, 28 Jan 2022 23:29:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed6bc2d7abca8a1c07cd86d761c6e06ff959d03f351e8f99971d71d5a61775`  
		Last Modified: Fri, 28 Jan 2022 23:29:47 GMT  
		Size: 3.4 MB (3371423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc71f81d0cecff211281c26661d2e288b57e81bd4a532fb59952b3a39959129`  
		Last Modified: Fri, 28 Jan 2022 23:31:01 GMT  
		Size: 36.5 MB (36502342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87d7775bbd6592711eb67db858acbd12d1b451c944ed34f96272979ff395db4`  
		Last Modified: Fri, 28 Jan 2022 23:30:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21.3`

```console
$ docker pull telegraf@sha256:67e87c2587a45aa8afb6c25816ca622244916559b0edd3fdcd1c7ad3a7dd51ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.21.3` - linux; amd64

```console
$ docker pull telegraf@sha256:c211d523b235c2689145a17bff97947c7d945b67643e8e4baf8e8bf7c54e4893
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126360633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26fe59ae9f545a0cdf0f33e64927d84ca81a292b60d304df1750a38deabf7f57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:25:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:28:15 GMT
ENV TELEGRAF_VERSION=1.21.3
# Fri, 28 Jan 2022 23:28:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:28:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:28:19 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:28:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:28:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a79e2bea7607ea4697b1955cfc012bb0ed97c80871af8bdd8bb1b63b9584b0`  
		Last Modified: Fri, 28 Jan 2022 23:29:33 GMT  
		Size: 18.8 MB (18760423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc2c7895804f68943ae0ea3a6aeece4d418d0c7e76d1c1140329c3f76ef6dab`  
		Last Modified: Fri, 28 Jan 2022 23:29:29 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2a38225cfce41fe953343750113cb7a5b3d439c26d6732058f980336a3dac1`  
		Last Modified: Fri, 28 Jan 2022 23:30:41 GMT  
		Size: 36.7 MB (36655328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8507884f731d8be3ba24a6f77d13ca607bd840baba7f6053b5b9a618bb31ea1d`  
		Last Modified: Fri, 28 Jan 2022 23:30:35 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:e3698467c203120b926fa88b656f3d713bfcd6dd2b9a8c1002a8dba080ca8b72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116697145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b246266aa499bfbed882048abba3254fc7d7ba70cf44091b3349ea71b635b74b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:30 GMT
ADD file:19419917274a4a5aa3eceb0a6202f89e5b508368314f2bd0105897a847db4930 in / 
# Wed, 26 Jan 2022 01:41:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:37:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:38:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 29 Jan 2022 13:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 29 Jan 2022 13:45:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 29 Jan 2022 13:46:05 GMT
ENV TELEGRAF_VERSION=1.21.3
# Sat, 29 Jan 2022 13:46:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 29 Jan 2022 13:46:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 29 Jan 2022 13:46:19 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sat, 29 Jan 2022 13:46:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 29 Jan 2022 13:46:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:046501ac4c58f014cc320324f6023bbef17f28025428833449198a62a97849c0`  
		Last Modified: Wed, 26 Jan 2022 01:57:13 GMT  
		Size: 50.1 MB (50117358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29bf76217944d3c3b29fb3234ed71ba5a004ffcec0595d3704c6e6cfa169b68`  
		Last Modified: Wed, 26 Jan 2022 17:03:48 GMT  
		Size: 4.9 MB (4922334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0e88eaa9f33e97d48fa77ed2c178123150031494073f10c97755b3bd6370c1`  
		Last Modified: Wed, 26 Jan 2022 17:03:50 GMT  
		Size: 10.2 MB (10216891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f07aa7c84ba4dfe8f5cfc222c2afb20a1e0dd5dd52438027cc57cd5de81b344`  
		Last Modified: Sat, 29 Jan 2022 13:47:19 GMT  
		Size: 17.5 MB (17462211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c4a7f93f28554a0e10aa9ae7f34609c1c37058e73de11f9155c43400d8c777`  
		Last Modified: Sat, 29 Jan 2022 13:47:07 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d1b7e72a275f75e811d88df1a5ae10c921825a1473e41b29ec52a975164865`  
		Last Modified: Sat, 29 Jan 2022 13:48:40 GMT  
		Size: 34.0 MB (33975104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bb0a6707ff9222bdb3c5659c13cc45048a6795e940f8308a46f897e87fff84`  
		Last Modified: Sat, 29 Jan 2022 13:48:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:22da85a304e370d58ed66a3e8bf934f44af72677d53418b82968fa0a63ae7a02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121051528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f6d0364452d9f2eec44619d8fdbe1d0f43ca4b91dae249762b167a8febbd1a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:52:09 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:52:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:53:30 GMT
ENV TELEGRAF_VERSION=1.21.3
# Fri, 28 Jan 2022 23:53:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:53:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:53:37 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:53:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:53:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9665c78b20b5f67d05c7907cd13b6c08e535420cb76afdea17f75af7cc25a2fc`  
		Last Modified: Fri, 28 Jan 2022 23:54:05 GMT  
		Size: 18.4 MB (18383003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b756b6770d48353a8db8cd3e2c6a904a166050daf8d31f38d5204c8d281ba39`  
		Last Modified: Fri, 28 Jan 2022 23:54:00 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4de1414d58946d002c2e158b170383f566f798146bfa40bb5a9321c5d682e40`  
		Last Modified: Fri, 28 Jan 2022 23:54:40 GMT  
		Size: 33.3 MB (33258980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be80f793c1416b90d5c727f361f23da506a6b49cbb7c79e3c8107b285a5569e`  
		Last Modified: Fri, 28 Jan 2022 23:54:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21.3-alpine`

```console
$ docker pull telegraf@sha256:89942f98fc29476bb3fd2dbef701ce799b4c7d786ea1fa2be7513bc22862b937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.21.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:6c6414799ca0050388518cb49b6663a574a29685d7577f9fa1ffa18b06f58bcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42692659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a67941483c88e155c94bf66f279ed555367f8236298ee1154edbebdab0e3ef6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 23:26:22 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Jan 2022 23:26:24 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 28 Jan 2022 23:28:23 GMT
ENV TELEGRAF_VERSION=1.21.3
# Fri, 28 Jan 2022 23:29:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 28 Jan 2022 23:29:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:29:08 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 28 Jan 2022 23:29:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:29:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c171b8d76913f15ff251f40de7410868a7687d5a27eae89b156861bf6477559b`  
		Last Modified: Fri, 28 Jan 2022 23:29:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed6bc2d7abca8a1c07cd86d761c6e06ff959d03f351e8f99971d71d5a61775`  
		Last Modified: Fri, 28 Jan 2022 23:29:47 GMT  
		Size: 3.4 MB (3371423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc71f81d0cecff211281c26661d2e288b57e81bd4a532fb59952b3a39959129`  
		Last Modified: Fri, 28 Jan 2022 23:31:01 GMT  
		Size: 36.5 MB (36502342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87d7775bbd6592711eb67db858acbd12d1b451c944ed34f96272979ff395db4`  
		Last Modified: Fri, 28 Jan 2022 23:30:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:89942f98fc29476bb3fd2dbef701ce799b4c7d786ea1fa2be7513bc22862b937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:6c6414799ca0050388518cb49b6663a574a29685d7577f9fa1ffa18b06f58bcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42692659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a67941483c88e155c94bf66f279ed555367f8236298ee1154edbebdab0e3ef6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 23:26:22 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 28 Jan 2022 23:26:24 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 28 Jan 2022 23:28:23 GMT
ENV TELEGRAF_VERSION=1.21.3
# Fri, 28 Jan 2022 23:29:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 28 Jan 2022 23:29:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:29:08 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 28 Jan 2022 23:29:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:29:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c171b8d76913f15ff251f40de7410868a7687d5a27eae89b156861bf6477559b`  
		Last Modified: Fri, 28 Jan 2022 23:29:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed6bc2d7abca8a1c07cd86d761c6e06ff959d03f351e8f99971d71d5a61775`  
		Last Modified: Fri, 28 Jan 2022 23:29:47 GMT  
		Size: 3.4 MB (3371423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc71f81d0cecff211281c26661d2e288b57e81bd4a532fb59952b3a39959129`  
		Last Modified: Fri, 28 Jan 2022 23:31:01 GMT  
		Size: 36.5 MB (36502342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87d7775bbd6592711eb67db858acbd12d1b451c944ed34f96272979ff395db4`  
		Last Modified: Fri, 28 Jan 2022 23:30:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:67e87c2587a45aa8afb6c25816ca622244916559b0edd3fdcd1c7ad3a7dd51ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:c211d523b235c2689145a17bff97947c7d945b67643e8e4baf8e8bf7c54e4893
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126360633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26fe59ae9f545a0cdf0f33e64927d84ca81a292b60d304df1750a38deabf7f57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:25:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:26:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:28:15 GMT
ENV TELEGRAF_VERSION=1.21.3
# Fri, 28 Jan 2022 23:28:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:28:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:28:19 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:28:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:28:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a79e2bea7607ea4697b1955cfc012bb0ed97c80871af8bdd8bb1b63b9584b0`  
		Last Modified: Fri, 28 Jan 2022 23:29:33 GMT  
		Size: 18.8 MB (18760423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc2c7895804f68943ae0ea3a6aeece4d418d0c7e76d1c1140329c3f76ef6dab`  
		Last Modified: Fri, 28 Jan 2022 23:29:29 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2a38225cfce41fe953343750113cb7a5b3d439c26d6732058f980336a3dac1`  
		Last Modified: Fri, 28 Jan 2022 23:30:41 GMT  
		Size: 36.7 MB (36655328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8507884f731d8be3ba24a6f77d13ca607bd840baba7f6053b5b9a618bb31ea1d`  
		Last Modified: Fri, 28 Jan 2022 23:30:35 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:e3698467c203120b926fa88b656f3d713bfcd6dd2b9a8c1002a8dba080ca8b72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116697145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b246266aa499bfbed882048abba3254fc7d7ba70cf44091b3349ea71b635b74b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:30 GMT
ADD file:19419917274a4a5aa3eceb0a6202f89e5b508368314f2bd0105897a847db4930 in / 
# Wed, 26 Jan 2022 01:41:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:37:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:38:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 29 Jan 2022 13:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sat, 29 Jan 2022 13:45:10 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 29 Jan 2022 13:46:05 GMT
ENV TELEGRAF_VERSION=1.21.3
# Sat, 29 Jan 2022 13:46:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 29 Jan 2022 13:46:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 29 Jan 2022 13:46:19 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sat, 29 Jan 2022 13:46:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 29 Jan 2022 13:46:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:046501ac4c58f014cc320324f6023bbef17f28025428833449198a62a97849c0`  
		Last Modified: Wed, 26 Jan 2022 01:57:13 GMT  
		Size: 50.1 MB (50117358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29bf76217944d3c3b29fb3234ed71ba5a004ffcec0595d3704c6e6cfa169b68`  
		Last Modified: Wed, 26 Jan 2022 17:03:48 GMT  
		Size: 4.9 MB (4922334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0e88eaa9f33e97d48fa77ed2c178123150031494073f10c97755b3bd6370c1`  
		Last Modified: Wed, 26 Jan 2022 17:03:50 GMT  
		Size: 10.2 MB (10216891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f07aa7c84ba4dfe8f5cfc222c2afb20a1e0dd5dd52438027cc57cd5de81b344`  
		Last Modified: Sat, 29 Jan 2022 13:47:19 GMT  
		Size: 17.5 MB (17462211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c4a7f93f28554a0e10aa9ae7f34609c1c37058e73de11f9155c43400d8c777`  
		Last Modified: Sat, 29 Jan 2022 13:47:07 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d1b7e72a275f75e811d88df1a5ae10c921825a1473e41b29ec52a975164865`  
		Last Modified: Sat, 29 Jan 2022 13:48:40 GMT  
		Size: 34.0 MB (33975104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bb0a6707ff9222bdb3c5659c13cc45048a6795e940f8308a46f897e87fff84`  
		Last Modified: Sat, 29 Jan 2022 13:48:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:22da85a304e370d58ed66a3e8bf934f44af72677d53418b82968fa0a63ae7a02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121051528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f6d0364452d9f2eec44619d8fdbe1d0f43ca4b91dae249762b167a8febbd1a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 28 Jan 2022 23:52:09 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jan 2022 23:52:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jan 2022 23:53:30 GMT
ENV TELEGRAF_VERSION=1.21.3
# Fri, 28 Jan 2022 23:53:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jan 2022 23:53:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jan 2022 23:53:37 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jan 2022 23:53:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jan 2022 23:53:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9665c78b20b5f67d05c7907cd13b6c08e535420cb76afdea17f75af7cc25a2fc`  
		Last Modified: Fri, 28 Jan 2022 23:54:05 GMT  
		Size: 18.4 MB (18383003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b756b6770d48353a8db8cd3e2c6a904a166050daf8d31f38d5204c8d281ba39`  
		Last Modified: Fri, 28 Jan 2022 23:54:00 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4de1414d58946d002c2e158b170383f566f798146bfa40bb5a9321c5d682e40`  
		Last Modified: Fri, 28 Jan 2022 23:54:40 GMT  
		Size: 33.3 MB (33258980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be80f793c1416b90d5c727f361f23da506a6b49cbb7c79e3c8107b285a5569e`  
		Last Modified: Fri, 28 Jan 2022 23:54:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
