<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.4`](#kapacitor14)
-	[`kapacitor:1.4-alpine`](#kapacitor14-alpine)
-	[`kapacitor:1.4.1`](#kapacitor141)
-	[`kapacitor:1.4.1-alpine`](#kapacitor141-alpine)
-	[`kapacitor:1.5`](#kapacitor15)
-	[`kapacitor:1.5-alpine`](#kapacitor15-alpine)
-	[`kapacitor:1.5.9`](#kapacitor159)
-	[`kapacitor:1.5.9-alpine`](#kapacitor159-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.4`

```console
$ docker pull kapacitor@sha256:f6ee3067575d17f0d8db1260bcd6b0fb140fcd8ef1cbdf355d44da9c7bc40458
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.4` - linux; amd64

```console
$ docker pull kapacitor@sha256:295dd1a0eb8f5bbecb19cdd1a918187f5c1dc8f8de0d9abee913560d91524105
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96974411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36c0b3c4a9aedbf3168e68d8e79795b457caddc1265b57432e47ce238c10b033`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:08:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:08:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:17:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 31 Mar 2021 22:17:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:17:11 GMT
ENV KAPACITOR_VERSION=1.4.1
# Wed, 31 Mar 2021 22:17:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Wed, 31 Mar 2021 22:17:15 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 31 Mar 2021 22:17:15 GMT
EXPOSE 9092
# Wed, 31 Mar 2021 22:17:15 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 31 Mar 2021 22:17:15 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 31 Mar 2021 22:17:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:17:16 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da61ad49fa9961d6dfe53dc067fd690133f205498e8045e8f7ef6b9da0d42bd2`  
		Last Modified: Tue, 30 Mar 2021 23:17:25 GMT  
		Size: 11.3 MB (11286658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af62e04c0f85ed10801df4314d8cb9ba5e6c391f6a3c1db1080a0a78c8d4ed9d`  
		Last Modified: Tue, 30 Mar 2021 23:17:23 GMT  
		Size: 4.3 MB (4342466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b870193fc38be94939bb7fbe783b410156fc584bde3a54194d5a3ae4a989b23`  
		Last Modified: Wed, 31 Mar 2021 22:18:03 GMT  
		Size: 13.3 MB (13266613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a020a4b7bf4554f3f71151d5ac74dc6f09f88a5b7df3f65ab56a2aaaee6ae418`  
		Last Modified: Wed, 31 Mar 2021 22:18:01 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2656a1b1990c47d37eb0101c959aa902af116d9c6182bd4960194a1fc15eefd`  
		Last Modified: Wed, 31 Mar 2021 22:18:07 GMT  
		Size: 22.7 MB (22695416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e305c342166e78515230d7811ab3ccc1cda6a83d2f90eaab7b7efd30cf27ac0`  
		Last Modified: Wed, 31 Mar 2021 22:18:02 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c19e91b10497d43067e2e1ba39cea40f1757287dbad7c9486427d109e28181`  
		Last Modified: Wed, 31 Mar 2021 22:18:01 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:d3b41f46e34b8c6dc5f6840afae845659147cd4b3608cf9839023f0a51c9458c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90739414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0a28f4aa0fb974eb34c5b2145b5b386919888f8d2832afef33588dce9f357a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 10 Apr 2021 01:02:42 GMT
ADD file:4c101c517b88a8d25a4997ab4d938ea50aaa265c7f88a4e63edaaed37d89a288 in / 
# Sat, 10 Apr 2021 01:02:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:12:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:19:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 10 Apr 2021 22:19:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:19:14 GMT
ENV KAPACITOR_VERSION=1.4.1
# Sat, 10 Apr 2021 22:19:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 22:19:25 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 10 Apr 2021 22:19:26 GMT
EXPOSE 9092
# Sat, 10 Apr 2021 22:19:27 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 10 Apr 2021 22:19:28 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 10 Apr 2021 22:19:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:19:30 GMT
CMD ["kapacitord"]
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
	-	`sha256:3a5548ddb837034d70efcad767473405f5cb3380e6240f994493984e8a5870f6`  
		Last Modified: Sat, 10 Apr 2021 22:20:12 GMT  
		Size: 13.4 MB (13445663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5045a113b1bd33cb8071aba12beb91cccc1f56bd71df1c263569b5eb43f335`  
		Last Modified: Sat, 10 Apr 2021 22:20:10 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29df9843748caedb40f0a0be37b6caee66205ddaeb0f9f2f0633adc114a7b352`  
		Last Modified: Sat, 10 Apr 2021 22:20:18 GMT  
		Size: 21.3 MB (21308998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72d9ba94ef17ffde60ebee24ff5465ef67bb8eb57933e0b18969c64c120075e`  
		Last Modified: Sat, 10 Apr 2021 22:20:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a24e59deadfb360ee6cb59de0b6a750e0412651a8ad12c569c3b5e09f0361`  
		Last Modified: Sat, 10 Apr 2021 22:20:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:e6e4a85f1d1264e7f7b9d7e747a4ce9f6ef3893be4e33a170ee2bac96dec26bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.8 MB (91758171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2a93e3442d85e25db5e2a9a5c608ca48849ac10a7e018fd8836dfbef99158b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:45 GMT
ADD file:0546f28e5d1be54699d1e0756275203da731735b3212f2ff1a87cd7f8dcc9049 in / 
# Tue, 30 Mar 2021 21:49:50 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:22:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:22:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:54:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 31 Mar 2021 23:54:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 23:54:55 GMT
ENV KAPACITOR_VERSION=1.4.1
# Wed, 31 Mar 2021 23:55:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Wed, 31 Mar 2021 23:55:04 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 31 Mar 2021 23:55:05 GMT
EXPOSE 9092
# Wed, 31 Mar 2021 23:55:07 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 31 Mar 2021 23:55:08 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 31 Mar 2021 23:55:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 23:55:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:9317dc7ea567b49ade0ea730b5530d1363b065549e8b75a198e0b60bdde1f1d7`  
		Last Modified: Tue, 30 Mar 2021 21:56:46 GMT  
		Size: 43.2 MB (43177588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaf1b7b1bdfdc23af33da7d1fc9670524e63a8408bb04de9aebdf95979c5635`  
		Last Modified: Wed, 31 Mar 2021 00:33:12 GMT  
		Size: 10.2 MB (10201033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4446041554682b465ef9a0e853a5067e7d794fa1c840946d140beab2ddeb51`  
		Last Modified: Wed, 31 Mar 2021 00:33:09 GMT  
		Size: 4.1 MB (4096741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3dc15e7533d447948dcd93d1c2f0479b526a4598e8bfc031d614c1812c5f7`  
		Last Modified: Wed, 31 Mar 2021 23:56:01 GMT  
		Size: 13.0 MB (12970931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fed03b06f2aea621c1ada316476dffe2e5c986d773ca9c37ac5a4f0f0dd56f`  
		Last Modified: Wed, 31 Mar 2021 23:55:59 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c393647a09dfbc4b0dcfae327c601ab44fe269429f666eaabbdf02c7537a63`  
		Last Modified: Wed, 31 Mar 2021 23:56:05 GMT  
		Size: 21.3 MB (21308569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811acfb332f9ab508e64e5ef0893f9008ec7310b44bb7b82eca169b37923381b`  
		Last Modified: Wed, 31 Mar 2021 23:55:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5ee1271e65222cca89593b203b303300d824a95cb88d15ea8abe4009cb8124`  
		Last Modified: Wed, 31 Mar 2021 23:56:01 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4-alpine`

```console
$ docker pull kapacitor@sha256:b9334db486e49d760f0a25c872769b917c89fd1373330da73588d0aea94282c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.4-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:42af065728b6b2c84e860e6aba8ebdac297210bc6f6477087691246516b6eb4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.7 MB (19679747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183b5b662f1682b17f40493563658a3b798819b0d3cd7e4f1e107a7e738f4551`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:17:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 31 Mar 2021 22:17:20 GMT
ENV KAPACITOR_VERSION=1.4.1
# Wed, 31 Mar 2021 22:17:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 31 Mar 2021 22:17:24 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 31 Mar 2021 22:17:24 GMT
EXPOSE 9092
# Wed, 31 Mar 2021 22:17:25 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 31 Mar 2021 22:17:25 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Wed, 31 Mar 2021 22:17:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:17:25 GMT
CMD ["kapacitord"]
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
	-	`sha256:b28ec0c47ed2e19e5d27fab02ef23b68ffd819172e08050fa1da307311f9c707`  
		Last Modified: Wed, 31 Mar 2021 22:18:17 GMT  
		Size: 280.9 KB (280883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80e9ef08a0b0ffa9172562a23b8e4d4069ae60ccc7e7db14a48bbced2e76502`  
		Last Modified: Wed, 31 Mar 2021 22:18:21 GMT  
		Size: 16.6 MB (16598517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddf07f1ee8244273ef0f860feef98629d132690c01d9ff88b4309c1d73f360f`  
		Last Modified: Wed, 31 Mar 2021 22:18:17 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2865f6f9b429a0b657521a428d992d31a675e45ebbcba6d649d6c0408ba1007`  
		Last Modified: Wed, 31 Mar 2021 22:18:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4.1`

```console
$ docker pull kapacitor@sha256:f6ee3067575d17f0d8db1260bcd6b0fb140fcd8ef1cbdf355d44da9c7bc40458
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.4.1` - linux; amd64

```console
$ docker pull kapacitor@sha256:295dd1a0eb8f5bbecb19cdd1a918187f5c1dc8f8de0d9abee913560d91524105
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96974411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36c0b3c4a9aedbf3168e68d8e79795b457caddc1265b57432e47ce238c10b033`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:08:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:08:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:17:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 31 Mar 2021 22:17:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 22:17:11 GMT
ENV KAPACITOR_VERSION=1.4.1
# Wed, 31 Mar 2021 22:17:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Wed, 31 Mar 2021 22:17:15 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 31 Mar 2021 22:17:15 GMT
EXPOSE 9092
# Wed, 31 Mar 2021 22:17:15 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 31 Mar 2021 22:17:15 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 31 Mar 2021 22:17:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:17:16 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da61ad49fa9961d6dfe53dc067fd690133f205498e8045e8f7ef6b9da0d42bd2`  
		Last Modified: Tue, 30 Mar 2021 23:17:25 GMT  
		Size: 11.3 MB (11286658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af62e04c0f85ed10801df4314d8cb9ba5e6c391f6a3c1db1080a0a78c8d4ed9d`  
		Last Modified: Tue, 30 Mar 2021 23:17:23 GMT  
		Size: 4.3 MB (4342466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b870193fc38be94939bb7fbe783b410156fc584bde3a54194d5a3ae4a989b23`  
		Last Modified: Wed, 31 Mar 2021 22:18:03 GMT  
		Size: 13.3 MB (13266613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a020a4b7bf4554f3f71151d5ac74dc6f09f88a5b7df3f65ab56a2aaaee6ae418`  
		Last Modified: Wed, 31 Mar 2021 22:18:01 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2656a1b1990c47d37eb0101c959aa902af116d9c6182bd4960194a1fc15eefd`  
		Last Modified: Wed, 31 Mar 2021 22:18:07 GMT  
		Size: 22.7 MB (22695416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e305c342166e78515230d7811ab3ccc1cda6a83d2f90eaab7b7efd30cf27ac0`  
		Last Modified: Wed, 31 Mar 2021 22:18:02 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c19e91b10497d43067e2e1ba39cea40f1757287dbad7c9486427d109e28181`  
		Last Modified: Wed, 31 Mar 2021 22:18:01 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4.1` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:d3b41f46e34b8c6dc5f6840afae845659147cd4b3608cf9839023f0a51c9458c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90739414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0a28f4aa0fb974eb34c5b2145b5b386919888f8d2832afef33588dce9f357a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 10 Apr 2021 01:02:42 GMT
ADD file:4c101c517b88a8d25a4997ab4d938ea50aaa265c7f88a4e63edaaed37d89a288 in / 
# Sat, 10 Apr 2021 01:02:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:12:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:19:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 10 Apr 2021 22:19:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:19:14 GMT
ENV KAPACITOR_VERSION=1.4.1
# Sat, 10 Apr 2021 22:19:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Sat, 10 Apr 2021 22:19:25 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 10 Apr 2021 22:19:26 GMT
EXPOSE 9092
# Sat, 10 Apr 2021 22:19:27 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 10 Apr 2021 22:19:28 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 10 Apr 2021 22:19:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:19:30 GMT
CMD ["kapacitord"]
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
	-	`sha256:3a5548ddb837034d70efcad767473405f5cb3380e6240f994493984e8a5870f6`  
		Last Modified: Sat, 10 Apr 2021 22:20:12 GMT  
		Size: 13.4 MB (13445663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5045a113b1bd33cb8071aba12beb91cccc1f56bd71df1c263569b5eb43f335`  
		Last Modified: Sat, 10 Apr 2021 22:20:10 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29df9843748caedb40f0a0be37b6caee66205ddaeb0f9f2f0633adc114a7b352`  
		Last Modified: Sat, 10 Apr 2021 22:20:18 GMT  
		Size: 21.3 MB (21308998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72d9ba94ef17ffde60ebee24ff5465ef67bb8eb57933e0b18969c64c120075e`  
		Last Modified: Sat, 10 Apr 2021 22:20:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a24e59deadfb360ee6cb59de0b6a750e0412651a8ad12c569c3b5e09f0361`  
		Last Modified: Sat, 10 Apr 2021 22:20:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4.1` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:e6e4a85f1d1264e7f7b9d7e747a4ce9f6ef3893be4e33a170ee2bac96dec26bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.8 MB (91758171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2a93e3442d85e25db5e2a9a5c608ca48849ac10a7e018fd8836dfbef99158b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:45 GMT
ADD file:0546f28e5d1be54699d1e0756275203da731735b3212f2ff1a87cd7f8dcc9049 in / 
# Tue, 30 Mar 2021 21:49:50 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:22:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:22:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:54:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 31 Mar 2021 23:54:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 31 Mar 2021 23:54:55 GMT
ENV KAPACITOR_VERSION=1.4.1
# Wed, 31 Mar 2021 23:55:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Wed, 31 Mar 2021 23:55:04 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 31 Mar 2021 23:55:05 GMT
EXPOSE 9092
# Wed, 31 Mar 2021 23:55:07 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 31 Mar 2021 23:55:08 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 31 Mar 2021 23:55:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 23:55:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:9317dc7ea567b49ade0ea730b5530d1363b065549e8b75a198e0b60bdde1f1d7`  
		Last Modified: Tue, 30 Mar 2021 21:56:46 GMT  
		Size: 43.2 MB (43177588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaf1b7b1bdfdc23af33da7d1fc9670524e63a8408bb04de9aebdf95979c5635`  
		Last Modified: Wed, 31 Mar 2021 00:33:12 GMT  
		Size: 10.2 MB (10201033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4446041554682b465ef9a0e853a5067e7d794fa1c840946d140beab2ddeb51`  
		Last Modified: Wed, 31 Mar 2021 00:33:09 GMT  
		Size: 4.1 MB (4096741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3dc15e7533d447948dcd93d1c2f0479b526a4598e8bfc031d614c1812c5f7`  
		Last Modified: Wed, 31 Mar 2021 23:56:01 GMT  
		Size: 13.0 MB (12970931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fed03b06f2aea621c1ada316476dffe2e5c986d773ca9c37ac5a4f0f0dd56f`  
		Last Modified: Wed, 31 Mar 2021 23:55:59 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c393647a09dfbc4b0dcfae327c601ab44fe269429f666eaabbdf02c7537a63`  
		Last Modified: Wed, 31 Mar 2021 23:56:05 GMT  
		Size: 21.3 MB (21308569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811acfb332f9ab508e64e5ef0893f9008ec7310b44bb7b82eca169b37923381b`  
		Last Modified: Wed, 31 Mar 2021 23:55:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5ee1271e65222cca89593b203b303300d824a95cb88d15ea8abe4009cb8124`  
		Last Modified: Wed, 31 Mar 2021 23:56:01 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4.1-alpine`

```console
$ docker pull kapacitor@sha256:b9334db486e49d760f0a25c872769b917c89fd1373330da73588d0aea94282c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.4.1-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:42af065728b6b2c84e860e6aba8ebdac297210bc6f6477087691246516b6eb4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.7 MB (19679747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183b5b662f1682b17f40493563658a3b798819b0d3cd7e4f1e107a7e738f4551`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:17:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 31 Mar 2021 22:17:20 GMT
ENV KAPACITOR_VERSION=1.4.1
# Wed, 31 Mar 2021 22:17:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 31 Mar 2021 22:17:24 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 31 Mar 2021 22:17:24 GMT
EXPOSE 9092
# Wed, 31 Mar 2021 22:17:25 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 31 Mar 2021 22:17:25 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Wed, 31 Mar 2021 22:17:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 22:17:25 GMT
CMD ["kapacitord"]
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
	-	`sha256:b28ec0c47ed2e19e5d27fab02ef23b68ffd819172e08050fa1da307311f9c707`  
		Last Modified: Wed, 31 Mar 2021 22:18:17 GMT  
		Size: 280.9 KB (280883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80e9ef08a0b0ffa9172562a23b8e4d4069ae60ccc7e7db14a48bbced2e76502`  
		Last Modified: Wed, 31 Mar 2021 22:18:21 GMT  
		Size: 16.6 MB (16598517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddf07f1ee8244273ef0f860feef98629d132690c01d9ff88b4309c1d73f360f`  
		Last Modified: Wed, 31 Mar 2021 22:18:17 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2865f6f9b429a0b657521a428d992d31a675e45ebbcba6d649d6c0408ba1007`  
		Last Modified: Wed, 31 Mar 2021 22:18:18 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5`

```console
$ docker pull kapacitor@sha256:f7fd31a567e4a82a3a584786ec0276d38f319f6e80e11aaf358d5edd7a5088af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:b030edee22fa4f839d3ca557a58a35f20647fdcf0e2bd53a28c4d002d80b06d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111498604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d597f818955cc06b1e9332491992b1d077e352b23132c064673e6a58dfa5bf6f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:08:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:08:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:17:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 31 Mar 2021 22:17:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 07 Apr 2021 19:49:20 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 07 Apr 2021 19:49:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 07 Apr 2021 19:49:26 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 07 Apr 2021 19:49:26 GMT
EXPOSE 9092
# Wed, 07 Apr 2021 19:49:26 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 07 Apr 2021 19:49:27 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 07 Apr 2021 19:49:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Apr 2021 19:49:27 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da61ad49fa9961d6dfe53dc067fd690133f205498e8045e8f7ef6b9da0d42bd2`  
		Last Modified: Tue, 30 Mar 2021 23:17:25 GMT  
		Size: 11.3 MB (11286658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af62e04c0f85ed10801df4314d8cb9ba5e6c391f6a3c1db1080a0a78c8d4ed9d`  
		Last Modified: Tue, 30 Mar 2021 23:17:23 GMT  
		Size: 4.3 MB (4342466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b870193fc38be94939bb7fbe783b410156fc584bde3a54194d5a3ae4a989b23`  
		Last Modified: Wed, 31 Mar 2021 22:18:03 GMT  
		Size: 13.3 MB (13266613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a020a4b7bf4554f3f71151d5ac74dc6f09f88a5b7df3f65ab56a2aaaee6ae418`  
		Last Modified: Wed, 31 Mar 2021 22:18:01 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec2191a90e8349484b8250ff37abac63f0e3fa748b0ef645db3e554cb0b2f93`  
		Last Modified: Wed, 07 Apr 2021 19:50:05 GMT  
		Size: 37.2 MB (37219610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95ce9e4e1b9ad1c25d028367b1a024e5413730f4faf3b226202afe0106b5ab`  
		Last Modified: Wed, 07 Apr 2021 19:50:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6a17ab8add9729a2d1b5c28fbca02584529826e5dc5bedec574fc55517f70`  
		Last Modified: Wed, 07 Apr 2021 19:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:7e4937080fbd4806d62c0af9966eddcadc65503a14d3c064c5fb81532a2eb776
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104217134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e5c22aa9395a72175b951ac5318d2b54754ecc118737e008b2f4ce78e31bf2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 10 Apr 2021 01:02:42 GMT
ADD file:4c101c517b88a8d25a4997ab4d938ea50aaa265c7f88a4e63edaaed37d89a288 in / 
# Sat, 10 Apr 2021 01:02:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:12:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:19:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 10 Apr 2021 22:19:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:19:38 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 10 Apr 2021 22:19:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 10 Apr 2021 22:19:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 10 Apr 2021 22:19:48 GMT
EXPOSE 9092
# Sat, 10 Apr 2021 22:19:49 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 10 Apr 2021 22:19:50 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 10 Apr 2021 22:19:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:19:52 GMT
CMD ["kapacitord"]
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
	-	`sha256:3a5548ddb837034d70efcad767473405f5cb3380e6240f994493984e8a5870f6`  
		Last Modified: Sat, 10 Apr 2021 22:20:12 GMT  
		Size: 13.4 MB (13445663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5045a113b1bd33cb8071aba12beb91cccc1f56bd71df1c263569b5eb43f335`  
		Last Modified: Sat, 10 Apr 2021 22:20:10 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8f30e9b3c3e1ec40d1be5575efc59c1f0ee44f014c8e3f4b2caa03f71bc066`  
		Last Modified: Sat, 10 Apr 2021 22:20:34 GMT  
		Size: 34.8 MB (34786719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6875f4362395dbf5a4c5d1a7bbfb75726815726d14ae3c233657dfa4d9fa41fc`  
		Last Modified: Sat, 10 Apr 2021 22:20:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed4941758985f029983895a46025f3ef3fefe7b839797451b9d619b3556c14d`  
		Last Modified: Sat, 10 Apr 2021 22:20:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:32c0a91fa46f4e180ebc4ca65d3d8d6ff342ba087295c2d7beeeaf435cc43624
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105010703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:999d3e60be3ca4003b36323c68bc498688ef62139b79e0e044457b231bdacf38`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:45 GMT
ADD file:0546f28e5d1be54699d1e0756275203da731735b3212f2ff1a87cd7f8dcc9049 in / 
# Tue, 30 Mar 2021 21:49:50 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:22:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:22:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:54:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 31 Mar 2021 23:54:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 07 Apr 2021 20:38:36 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 07 Apr 2021 20:38:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 07 Apr 2021 20:38:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 07 Apr 2021 20:38:46 GMT
EXPOSE 9092
# Wed, 07 Apr 2021 20:38:47 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 07 Apr 2021 20:38:48 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 07 Apr 2021 20:38:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Apr 2021 20:38:51 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:9317dc7ea567b49ade0ea730b5530d1363b065549e8b75a198e0b60bdde1f1d7`  
		Last Modified: Tue, 30 Mar 2021 21:56:46 GMT  
		Size: 43.2 MB (43177588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaf1b7b1bdfdc23af33da7d1fc9670524e63a8408bb04de9aebdf95979c5635`  
		Last Modified: Wed, 31 Mar 2021 00:33:12 GMT  
		Size: 10.2 MB (10201033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4446041554682b465ef9a0e853a5067e7d794fa1c840946d140beab2ddeb51`  
		Last Modified: Wed, 31 Mar 2021 00:33:09 GMT  
		Size: 4.1 MB (4096741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3dc15e7533d447948dcd93d1c2f0479b526a4598e8bfc031d614c1812c5f7`  
		Last Modified: Wed, 31 Mar 2021 23:56:01 GMT  
		Size: 13.0 MB (12970931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fed03b06f2aea621c1ada316476dffe2e5c986d773ca9c37ac5a4f0f0dd56f`  
		Last Modified: Wed, 31 Mar 2021 23:55:59 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fdc549861116b0c6c92170a7745c50d4575b07fee1c93dc915a07614d4bf40`  
		Last Modified: Wed, 07 Apr 2021 20:39:16 GMT  
		Size: 34.6 MB (34561102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5188dafeda31980d9092ec2ec844e3995fb39a74b9eb04a2c9949cbe927f078f`  
		Last Modified: Wed, 07 Apr 2021 20:39:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f560ef7a984096f4d0b7ee42645a7696974e4365796e82f979fb1170259cdc0`  
		Last Modified: Wed, 07 Apr 2021 20:39:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:643e0987f06b95cc22468d0b934d4edccdd45489706dac37bfd6052a6c433d80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:77a3c115eae04e8c0875a4a2442b03d41dc94caf765079b35df614eb73b48e8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22623249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a991f59f6d2ecf69ad4e38c7a07a40b9a8fe6a6f12ee69fad1430d0e9363e46e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:17:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 07 Apr 2021 19:49:30 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 07 Apr 2021 19:49:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 07 Apr 2021 19:49:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 07 Apr 2021 19:49:41 GMT
EXPOSE 9092
# Wed, 07 Apr 2021 19:49:41 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 07 Apr 2021 19:49:42 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Wed, 07 Apr 2021 19:49:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Apr 2021 19:49:42 GMT
CMD ["kapacitord"]
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
	-	`sha256:b28ec0c47ed2e19e5d27fab02ef23b68ffd819172e08050fa1da307311f9c707`  
		Last Modified: Wed, 31 Mar 2021 22:18:17 GMT  
		Size: 280.9 KB (280883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ad40eee90293c66241284dbdbeab001785e6e38000e3fd6928d9d4e8111c8f`  
		Last Modified: Wed, 07 Apr 2021 19:50:23 GMT  
		Size: 19.5 MB (19542021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6d2b276a6dc27fa4410d5acb930abde902d01fbe7779dcd2a729e41ffff329`  
		Last Modified: Wed, 07 Apr 2021 19:50:21 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf60751781e3e2e58cbbe91ab28976f50c1d4bfdf7baabfb6c1dacbcb2193701`  
		Last Modified: Wed, 07 Apr 2021 19:50:19 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9`

```console
$ docker pull kapacitor@sha256:f7fd31a567e4a82a3a584786ec0276d38f319f6e80e11aaf358d5edd7a5088af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.9` - linux; amd64

```console
$ docker pull kapacitor@sha256:b030edee22fa4f839d3ca557a58a35f20647fdcf0e2bd53a28c4d002d80b06d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111498604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d597f818955cc06b1e9332491992b1d077e352b23132c064673e6a58dfa5bf6f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:08:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:08:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:17:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 31 Mar 2021 22:17:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 07 Apr 2021 19:49:20 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 07 Apr 2021 19:49:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 07 Apr 2021 19:49:26 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 07 Apr 2021 19:49:26 GMT
EXPOSE 9092
# Wed, 07 Apr 2021 19:49:26 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 07 Apr 2021 19:49:27 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 07 Apr 2021 19:49:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Apr 2021 19:49:27 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da61ad49fa9961d6dfe53dc067fd690133f205498e8045e8f7ef6b9da0d42bd2`  
		Last Modified: Tue, 30 Mar 2021 23:17:25 GMT  
		Size: 11.3 MB (11286658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af62e04c0f85ed10801df4314d8cb9ba5e6c391f6a3c1db1080a0a78c8d4ed9d`  
		Last Modified: Tue, 30 Mar 2021 23:17:23 GMT  
		Size: 4.3 MB (4342466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b870193fc38be94939bb7fbe783b410156fc584bde3a54194d5a3ae4a989b23`  
		Last Modified: Wed, 31 Mar 2021 22:18:03 GMT  
		Size: 13.3 MB (13266613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a020a4b7bf4554f3f71151d5ac74dc6f09f88a5b7df3f65ab56a2aaaee6ae418`  
		Last Modified: Wed, 31 Mar 2021 22:18:01 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec2191a90e8349484b8250ff37abac63f0e3fa748b0ef645db3e554cb0b2f93`  
		Last Modified: Wed, 07 Apr 2021 19:50:05 GMT  
		Size: 37.2 MB (37219610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95ce9e4e1b9ad1c25d028367b1a024e5413730f4faf3b226202afe0106b5ab`  
		Last Modified: Wed, 07 Apr 2021 19:50:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6a17ab8add9729a2d1b5c28fbca02584529826e5dc5bedec574fc55517f70`  
		Last Modified: Wed, 07 Apr 2021 19:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:7e4937080fbd4806d62c0af9966eddcadc65503a14d3c064c5fb81532a2eb776
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104217134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e5c22aa9395a72175b951ac5318d2b54754ecc118737e008b2f4ce78e31bf2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 10 Apr 2021 01:02:42 GMT
ADD file:4c101c517b88a8d25a4997ab4d938ea50aaa265c7f88a4e63edaaed37d89a288 in / 
# Sat, 10 Apr 2021 01:02:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:12:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:19:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 10 Apr 2021 22:19:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:19:38 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 10 Apr 2021 22:19:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 10 Apr 2021 22:19:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 10 Apr 2021 22:19:48 GMT
EXPOSE 9092
# Sat, 10 Apr 2021 22:19:49 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 10 Apr 2021 22:19:50 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 10 Apr 2021 22:19:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:19:52 GMT
CMD ["kapacitord"]
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
	-	`sha256:3a5548ddb837034d70efcad767473405f5cb3380e6240f994493984e8a5870f6`  
		Last Modified: Sat, 10 Apr 2021 22:20:12 GMT  
		Size: 13.4 MB (13445663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5045a113b1bd33cb8071aba12beb91cccc1f56bd71df1c263569b5eb43f335`  
		Last Modified: Sat, 10 Apr 2021 22:20:10 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8f30e9b3c3e1ec40d1be5575efc59c1f0ee44f014c8e3f4b2caa03f71bc066`  
		Last Modified: Sat, 10 Apr 2021 22:20:34 GMT  
		Size: 34.8 MB (34786719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6875f4362395dbf5a4c5d1a7bbfb75726815726d14ae3c233657dfa4d9fa41fc`  
		Last Modified: Sat, 10 Apr 2021 22:20:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed4941758985f029983895a46025f3ef3fefe7b839797451b9d619b3556c14d`  
		Last Modified: Sat, 10 Apr 2021 22:20:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:32c0a91fa46f4e180ebc4ca65d3d8d6ff342ba087295c2d7beeeaf435cc43624
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105010703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:999d3e60be3ca4003b36323c68bc498688ef62139b79e0e044457b231bdacf38`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:45 GMT
ADD file:0546f28e5d1be54699d1e0756275203da731735b3212f2ff1a87cd7f8dcc9049 in / 
# Tue, 30 Mar 2021 21:49:50 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:22:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:22:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:54:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 31 Mar 2021 23:54:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 07 Apr 2021 20:38:36 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 07 Apr 2021 20:38:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 07 Apr 2021 20:38:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 07 Apr 2021 20:38:46 GMT
EXPOSE 9092
# Wed, 07 Apr 2021 20:38:47 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 07 Apr 2021 20:38:48 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 07 Apr 2021 20:38:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Apr 2021 20:38:51 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:9317dc7ea567b49ade0ea730b5530d1363b065549e8b75a198e0b60bdde1f1d7`  
		Last Modified: Tue, 30 Mar 2021 21:56:46 GMT  
		Size: 43.2 MB (43177588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaf1b7b1bdfdc23af33da7d1fc9670524e63a8408bb04de9aebdf95979c5635`  
		Last Modified: Wed, 31 Mar 2021 00:33:12 GMT  
		Size: 10.2 MB (10201033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4446041554682b465ef9a0e853a5067e7d794fa1c840946d140beab2ddeb51`  
		Last Modified: Wed, 31 Mar 2021 00:33:09 GMT  
		Size: 4.1 MB (4096741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3dc15e7533d447948dcd93d1c2f0479b526a4598e8bfc031d614c1812c5f7`  
		Last Modified: Wed, 31 Mar 2021 23:56:01 GMT  
		Size: 13.0 MB (12970931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fed03b06f2aea621c1ada316476dffe2e5c986d773ca9c37ac5a4f0f0dd56f`  
		Last Modified: Wed, 31 Mar 2021 23:55:59 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fdc549861116b0c6c92170a7745c50d4575b07fee1c93dc915a07614d4bf40`  
		Last Modified: Wed, 07 Apr 2021 20:39:16 GMT  
		Size: 34.6 MB (34561102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5188dafeda31980d9092ec2ec844e3995fb39a74b9eb04a2c9949cbe927f078f`  
		Last Modified: Wed, 07 Apr 2021 20:39:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f560ef7a984096f4d0b7ee42645a7696974e4365796e82f979fb1170259cdc0`  
		Last Modified: Wed, 07 Apr 2021 20:39:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9-alpine`

```console
$ docker pull kapacitor@sha256:643e0987f06b95cc22468d0b934d4edccdd45489706dac37bfd6052a6c433d80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.5.9-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:77a3c115eae04e8c0875a4a2442b03d41dc94caf765079b35df614eb73b48e8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22623249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a991f59f6d2ecf69ad4e38c7a07a40b9a8fe6a6f12ee69fad1430d0e9363e46e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:17:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 07 Apr 2021 19:49:30 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 07 Apr 2021 19:49:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 07 Apr 2021 19:49:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 07 Apr 2021 19:49:41 GMT
EXPOSE 9092
# Wed, 07 Apr 2021 19:49:41 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 07 Apr 2021 19:49:42 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Wed, 07 Apr 2021 19:49:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Apr 2021 19:49:42 GMT
CMD ["kapacitord"]
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
	-	`sha256:b28ec0c47ed2e19e5d27fab02ef23b68ffd819172e08050fa1da307311f9c707`  
		Last Modified: Wed, 31 Mar 2021 22:18:17 GMT  
		Size: 280.9 KB (280883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ad40eee90293c66241284dbdbeab001785e6e38000e3fd6928d9d4e8111c8f`  
		Last Modified: Wed, 07 Apr 2021 19:50:23 GMT  
		Size: 19.5 MB (19542021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6d2b276a6dc27fa4410d5acb930abde902d01fbe7779dcd2a729e41ffff329`  
		Last Modified: Wed, 07 Apr 2021 19:50:21 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf60751781e3e2e58cbbe91ab28976f50c1d4bfdf7baabfb6c1dacbcb2193701`  
		Last Modified: Wed, 07 Apr 2021 19:50:19 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:643e0987f06b95cc22468d0b934d4edccdd45489706dac37bfd6052a6c433d80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:77a3c115eae04e8c0875a4a2442b03d41dc94caf765079b35df614eb73b48e8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22623249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a991f59f6d2ecf69ad4e38c7a07a40b9a8fe6a6f12ee69fad1430d0e9363e46e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:08:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 31 Mar 2021 22:17:19 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 07 Apr 2021 19:49:30 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 07 Apr 2021 19:49:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 07 Apr 2021 19:49:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 07 Apr 2021 19:49:41 GMT
EXPOSE 9092
# Wed, 07 Apr 2021 19:49:41 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 07 Apr 2021 19:49:42 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Wed, 07 Apr 2021 19:49:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Apr 2021 19:49:42 GMT
CMD ["kapacitord"]
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
	-	`sha256:b28ec0c47ed2e19e5d27fab02ef23b68ffd819172e08050fa1da307311f9c707`  
		Last Modified: Wed, 31 Mar 2021 22:18:17 GMT  
		Size: 280.9 KB (280883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ad40eee90293c66241284dbdbeab001785e6e38000e3fd6928d9d4e8111c8f`  
		Last Modified: Wed, 07 Apr 2021 19:50:23 GMT  
		Size: 19.5 MB (19542021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6d2b276a6dc27fa4410d5acb930abde902d01fbe7779dcd2a729e41ffff329`  
		Last Modified: Wed, 07 Apr 2021 19:50:21 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf60751781e3e2e58cbbe91ab28976f50c1d4bfdf7baabfb6c1dacbcb2193701`  
		Last Modified: Wed, 07 Apr 2021 19:50:19 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:f7fd31a567e4a82a3a584786ec0276d38f319f6e80e11aaf358d5edd7a5088af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:b030edee22fa4f839d3ca557a58a35f20647fdcf0e2bd53a28c4d002d80b06d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111498604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d597f818955cc06b1e9332491992b1d077e352b23132c064673e6a58dfa5bf6f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:08:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:08:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 22:17:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 31 Mar 2021 22:17:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 07 Apr 2021 19:49:20 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 07 Apr 2021 19:49:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 07 Apr 2021 19:49:26 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 07 Apr 2021 19:49:26 GMT
EXPOSE 9092
# Wed, 07 Apr 2021 19:49:26 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 07 Apr 2021 19:49:27 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 07 Apr 2021 19:49:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Apr 2021 19:49:27 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da61ad49fa9961d6dfe53dc067fd690133f205498e8045e8f7ef6b9da0d42bd2`  
		Last Modified: Tue, 30 Mar 2021 23:17:25 GMT  
		Size: 11.3 MB (11286658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af62e04c0f85ed10801df4314d8cb9ba5e6c391f6a3c1db1080a0a78c8d4ed9d`  
		Last Modified: Tue, 30 Mar 2021 23:17:23 GMT  
		Size: 4.3 MB (4342466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b870193fc38be94939bb7fbe783b410156fc584bde3a54194d5a3ae4a989b23`  
		Last Modified: Wed, 31 Mar 2021 22:18:03 GMT  
		Size: 13.3 MB (13266613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a020a4b7bf4554f3f71151d5ac74dc6f09f88a5b7df3f65ab56a2aaaee6ae418`  
		Last Modified: Wed, 31 Mar 2021 22:18:01 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec2191a90e8349484b8250ff37abac63f0e3fa748b0ef645db3e554cb0b2f93`  
		Last Modified: Wed, 07 Apr 2021 19:50:05 GMT  
		Size: 37.2 MB (37219610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c95ce9e4e1b9ad1c25d028367b1a024e5413730f4faf3b226202afe0106b5ab`  
		Last Modified: Wed, 07 Apr 2021 19:50:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc6a17ab8add9729a2d1b5c28fbca02584529826e5dc5bedec574fc55517f70`  
		Last Modified: Wed, 07 Apr 2021 19:50:00 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:7e4937080fbd4806d62c0af9966eddcadc65503a14d3c064c5fb81532a2eb776
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104217134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e5c22aa9395a72175b951ac5318d2b54754ecc118737e008b2f4ce78e31bf2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 10 Apr 2021 01:02:42 GMT
ADD file:4c101c517b88a8d25a4997ab4d938ea50aaa265c7f88a4e63edaaed37d89a288 in / 
# Sat, 10 Apr 2021 01:02:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:12:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 22:19:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 10 Apr 2021 22:19:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 10 Apr 2021 22:19:38 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 10 Apr 2021 22:19:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 10 Apr 2021 22:19:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 10 Apr 2021 22:19:48 GMT
EXPOSE 9092
# Sat, 10 Apr 2021 22:19:49 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 10 Apr 2021 22:19:50 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 10 Apr 2021 22:19:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 10 Apr 2021 22:19:52 GMT
CMD ["kapacitord"]
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
	-	`sha256:3a5548ddb837034d70efcad767473405f5cb3380e6240f994493984e8a5870f6`  
		Last Modified: Sat, 10 Apr 2021 22:20:12 GMT  
		Size: 13.4 MB (13445663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5045a113b1bd33cb8071aba12beb91cccc1f56bd71df1c263569b5eb43f335`  
		Last Modified: Sat, 10 Apr 2021 22:20:10 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8f30e9b3c3e1ec40d1be5575efc59c1f0ee44f014c8e3f4b2caa03f71bc066`  
		Last Modified: Sat, 10 Apr 2021 22:20:34 GMT  
		Size: 34.8 MB (34786719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6875f4362395dbf5a4c5d1a7bbfb75726815726d14ae3c233657dfa4d9fa41fc`  
		Last Modified: Sat, 10 Apr 2021 22:20:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed4941758985f029983895a46025f3ef3fefe7b839797451b9d619b3556c14d`  
		Last Modified: Sat, 10 Apr 2021 22:20:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:32c0a91fa46f4e180ebc4ca65d3d8d6ff342ba087295c2d7beeeaf435cc43624
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105010703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:999d3e60be3ca4003b36323c68bc498688ef62139b79e0e044457b231bdacf38`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:45 GMT
ADD file:0546f28e5d1be54699d1e0756275203da731735b3212f2ff1a87cd7f8dcc9049 in / 
# Tue, 30 Mar 2021 21:49:50 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:22:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:22:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 23:54:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 31 Mar 2021 23:54:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 07 Apr 2021 20:38:36 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 07 Apr 2021 20:38:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 07 Apr 2021 20:38:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 07 Apr 2021 20:38:46 GMT
EXPOSE 9092
# Wed, 07 Apr 2021 20:38:47 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 07 Apr 2021 20:38:48 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 07 Apr 2021 20:38:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 07 Apr 2021 20:38:51 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:9317dc7ea567b49ade0ea730b5530d1363b065549e8b75a198e0b60bdde1f1d7`  
		Last Modified: Tue, 30 Mar 2021 21:56:46 GMT  
		Size: 43.2 MB (43177588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaf1b7b1bdfdc23af33da7d1fc9670524e63a8408bb04de9aebdf95979c5635`  
		Last Modified: Wed, 31 Mar 2021 00:33:12 GMT  
		Size: 10.2 MB (10201033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4446041554682b465ef9a0e853a5067e7d794fa1c840946d140beab2ddeb51`  
		Last Modified: Wed, 31 Mar 2021 00:33:09 GMT  
		Size: 4.1 MB (4096741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a3dc15e7533d447948dcd93d1c2f0479b526a4598e8bfc031d614c1812c5f7`  
		Last Modified: Wed, 31 Mar 2021 23:56:01 GMT  
		Size: 13.0 MB (12970931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fed03b06f2aea621c1ada316476dffe2e5c986d773ca9c37ac5a4f0f0dd56f`  
		Last Modified: Wed, 31 Mar 2021 23:55:59 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fdc549861116b0c6c92170a7745c50d4575b07fee1c93dc915a07614d4bf40`  
		Last Modified: Wed, 07 Apr 2021 20:39:16 GMT  
		Size: 34.6 MB (34561102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5188dafeda31980d9092ec2ec844e3995fb39a74b9eb04a2c9949cbe927f078f`  
		Last Modified: Wed, 07 Apr 2021 20:39:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f560ef7a984096f4d0b7ee42645a7696974e4365796e82f979fb1170259cdc0`  
		Last Modified: Wed, 07 Apr 2021 20:39:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
