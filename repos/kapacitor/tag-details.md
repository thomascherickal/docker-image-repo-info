<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.5`](#kapacitor15)
-	[`kapacitor:1.5-alpine`](#kapacitor15-alpine)
-	[`kapacitor:1.5.9`](#kapacitor159)
-	[`kapacitor:1.5.9-alpine`](#kapacitor159-alpine)
-	[`kapacitor:1.6`](#kapacitor16)
-	[`kapacitor:1.6-alpine`](#kapacitor16-alpine)
-	[`kapacitor:1.6.4`](#kapacitor164)
-	[`kapacitor:1.6.4-alpine`](#kapacitor164-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.5`

```console
$ docker pull kapacitor@sha256:89e53790fa3727525a456683878e497dbf76e29453caf7b88937eb0b09217bae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:43ed1e460617ce971fc3a62851038348c2a7f831e0a62950215950bbbd838ced
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111720075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08f4fdc77586d54a85ea9b7de07f7a292c463a22a2180b1e264e39571238b5ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:18:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 01:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:18:56 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sun, 29 May 2022 01:19:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 01:19:00 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 01:19:00 GMT
EXPOSE 9092
# Sun, 29 May 2022 01:19:00 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 01:19:00 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 01:19:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:19:01 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1727216bd01238dbacd5b2e37b678af815c9c87331baa86b3c53b67f97d367`  
		Last Modified: Sun, 29 May 2022 01:19:31 GMT  
		Size: 13.4 MB (13421085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b1d7606415586e476777f810a27be4853e38f99cbf4354a36f224463a2fbf0`  
		Last Modified: Sun, 29 May 2022 01:19:29 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048368c6761d75d18890a862e8db98d6485a3a7555fcb542aceb170afffd84e2`  
		Last Modified: Sun, 29 May 2022 01:19:34 GMT  
		Size: 37.2 MB (37219961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66cacd3c7e5cb147f9d10973d46d50c781e1e19b9bbdd197ef8789b0b853d28`  
		Last Modified: Sun, 29 May 2022 01:19:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5228fe78e88b384f3c1ec64b2cf100d6dac19c2acbe704af7e797cb6cc4c3`  
		Last Modified: Sun, 29 May 2022 01:19:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:820f790129ebe84c849d28cf7b0e13721936210266b26b05b7c2fbdad0206581
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104423700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdce1444c67c497a7f24942f7c0385aabf0ba5aa17370cfe531b4647d3578665`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 01:05:16 GMT
ADD file:f859825c79355490a08b5fd55799cc3eb1643e21abfeebe59a3a4b08e54e3f7f in / 
# Sat, 28 May 2022 01:05:17 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:54:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 22:29:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 22:29:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 22:29:38 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sun, 29 May 2022 22:29:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 22:29:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 22:29:48 GMT
EXPOSE 9092
# Sun, 29 May 2022 22:29:48 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 22:29:49 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 22:29:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 22:29:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:ae3d55ab33f9bf9aa2c47629e66da1c4e679da10d83c29941f39b04140996e4b`  
		Last Modified: Sat, 28 May 2022 01:21:38 GMT  
		Size: 42.2 MB (42150781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d277a5551d8d3385d5cf64c67234fe8db9bad96903365595e8c6c61146e48d2b`  
		Last Modified: Sat, 28 May 2022 03:17:39 GMT  
		Size: 10.0 MB (9957035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2055cd14260ece06830786d784271b3008f3ce2ea3279123620a6d78a2afecfa`  
		Last Modified: Sat, 28 May 2022 03:17:36 GMT  
		Size: 3.9 MB (3921757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f8b3a1717b33ce0c5402304ad961ad9fd7f93b13778279c2f54643b463c51d`  
		Last Modified: Sun, 29 May 2022 22:30:16 GMT  
		Size: 13.6 MB (13603779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cacfeae2772a038f750027e6af5e4bcdb9e93302a2b5c625efdc38d2268239a`  
		Last Modified: Sun, 29 May 2022 22:30:11 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee3da87fc8b8e9131bbd3bc5f63b30a4fb19b33790eee55219649ec08c0f9d4`  
		Last Modified: Sun, 29 May 2022 22:30:28 GMT  
		Size: 34.8 MB (34787037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4d0617fb82de6a03733e8299dde12ee5469872a9d943977fbd313e796cdd9f`  
		Last Modified: Sun, 29 May 2022 22:30:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4851abcfa730fa43d72e11a166df9b1ba141a1eaec01c1faba17c6cd1ff2f8ab`  
		Last Modified: Sun, 29 May 2022 22:30:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:34ba8b3dda52146cbb004ed0108ed215a01167ee8812d258aa2dfe7076bc39ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104771886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659fc101ad9f20fd125ecd8cb81139d464e81e33baa231431558ccf95b470112`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 00:42:45 GMT
ADD file:93d675ee0bc32a88dc4d6c0872276c4678dc31f0b6eb8b936cb823f191bc07f0 in / 
# Sat, 28 May 2022 00:42:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:10:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:11:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 00:31:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 00:31:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 00:31:28 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sun, 29 May 2022 00:31:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 00:31:34 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 00:31:34 GMT
EXPOSE 9092
# Sun, 29 May 2022 00:31:35 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 00:31:37 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 00:31:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 00:31:38 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:de7fc2a3b80bcd193de687188fc9051c8be6c61ec81fec3aeae61c079f71e69e`  
		Last Modified: Sat, 28 May 2022 00:51:21 GMT  
		Size: 43.2 MB (43212871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee73573552502f742607ea1dcdefcee9aeafa4ad8d5deca24b48a262f4ba108`  
		Last Modified: Sat, 28 May 2022 11:20:36 GMT  
		Size: 10.2 MB (10218522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05d3983d65175e68348dcb2cd43933f2af4d2d8c1bf36c9d5f237394c9fa53b`  
		Last Modified: Sat, 28 May 2022 11:20:35 GMT  
		Size: 3.9 MB (3874461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8f74dae4587aae058149bbff22363d653b738ecb28be02f413d1bf034b7c6`  
		Last Modified: Sun, 29 May 2022 00:32:16 GMT  
		Size: 12.9 MB (12902056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d454c1b46feace219c701415f116ab5443d39199d58e0c949182ad86976c1a03`  
		Last Modified: Sun, 29 May 2022 00:32:14 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babe2d7fb2be947885b7436703bc34e3da4700d4fb33e9a837645e95457ae52f`  
		Last Modified: Sun, 29 May 2022 00:32:19 GMT  
		Size: 34.6 MB (34560692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d136e987b425ae0a91d0f46621e4211cc445798a0014b568f91f72d50f7103d`  
		Last Modified: Sun, 29 May 2022 00:32:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d32ad681eda580819dba926dd0ad58aeec03cdca102be49f978a429e82bbb8`  
		Last Modified: Sun, 29 May 2022 00:32:14 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:72166d96c41aecc792347bb7207fd7fce8fb6ad0214d9ff7d37c1582cce51d9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:abdce74128d00c6dbcba46427b043488e574b4f2bb5177da9162bd62e1111fbf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22631715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f19f25f0ae1d10d68e6fb9becb4a276fc272a896bdcc115d27bf4ffdd83580a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 07:16:44 GMT
ENV KAPACITOR_VERSION=1.5.9
# Tue, 05 Apr 2022 07:16:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 07:16:52 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 05 Apr 2022 07:16:52 GMT
EXPOSE 9092
# Tue, 05 Apr 2022 07:16:52 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 05 Apr 2022 07:16:52 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Tue, 05 Apr 2022 07:16:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:16:52 GMT
CMD ["kapacitord"]
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
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0eb59b0a9e02ad3acd30214bf6e9be9b5dd3a8473b5333645e05cefab6f995`  
		Last Modified: Tue, 05 Apr 2022 07:17:27 GMT  
		Size: 19.5 MB (19541034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d327126ef09ae07f5d34516658ea1877eab819728ce1905d1a4328490af252c`  
		Last Modified: Tue, 05 Apr 2022 07:17:23 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044949500ea9f07b81cf7142e7cfeacebc25114f7bef3cc97c0f5ab3de23fa94`  
		Last Modified: Tue, 05 Apr 2022 07:17:23 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9`

```console
$ docker pull kapacitor@sha256:89e53790fa3727525a456683878e497dbf76e29453caf7b88937eb0b09217bae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.9` - linux; amd64

```console
$ docker pull kapacitor@sha256:43ed1e460617ce971fc3a62851038348c2a7f831e0a62950215950bbbd838ced
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111720075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08f4fdc77586d54a85ea9b7de07f7a292c463a22a2180b1e264e39571238b5ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:18:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 01:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:18:56 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sun, 29 May 2022 01:19:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 01:19:00 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 01:19:00 GMT
EXPOSE 9092
# Sun, 29 May 2022 01:19:00 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 01:19:00 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 01:19:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:19:01 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1727216bd01238dbacd5b2e37b678af815c9c87331baa86b3c53b67f97d367`  
		Last Modified: Sun, 29 May 2022 01:19:31 GMT  
		Size: 13.4 MB (13421085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b1d7606415586e476777f810a27be4853e38f99cbf4354a36f224463a2fbf0`  
		Last Modified: Sun, 29 May 2022 01:19:29 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048368c6761d75d18890a862e8db98d6485a3a7555fcb542aceb170afffd84e2`  
		Last Modified: Sun, 29 May 2022 01:19:34 GMT  
		Size: 37.2 MB (37219961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66cacd3c7e5cb147f9d10973d46d50c781e1e19b9bbdd197ef8789b0b853d28`  
		Last Modified: Sun, 29 May 2022 01:19:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5228fe78e88b384f3c1ec64b2cf100d6dac19c2acbe704af7e797cb6cc4c3`  
		Last Modified: Sun, 29 May 2022 01:19:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:820f790129ebe84c849d28cf7b0e13721936210266b26b05b7c2fbdad0206581
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104423700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdce1444c67c497a7f24942f7c0385aabf0ba5aa17370cfe531b4647d3578665`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 01:05:16 GMT
ADD file:f859825c79355490a08b5fd55799cc3eb1643e21abfeebe59a3a4b08e54e3f7f in / 
# Sat, 28 May 2022 01:05:17 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:54:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 22:29:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 22:29:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 22:29:38 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sun, 29 May 2022 22:29:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 22:29:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 22:29:48 GMT
EXPOSE 9092
# Sun, 29 May 2022 22:29:48 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 22:29:49 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 22:29:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 22:29:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:ae3d55ab33f9bf9aa2c47629e66da1c4e679da10d83c29941f39b04140996e4b`  
		Last Modified: Sat, 28 May 2022 01:21:38 GMT  
		Size: 42.2 MB (42150781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d277a5551d8d3385d5cf64c67234fe8db9bad96903365595e8c6c61146e48d2b`  
		Last Modified: Sat, 28 May 2022 03:17:39 GMT  
		Size: 10.0 MB (9957035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2055cd14260ece06830786d784271b3008f3ce2ea3279123620a6d78a2afecfa`  
		Last Modified: Sat, 28 May 2022 03:17:36 GMT  
		Size: 3.9 MB (3921757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f8b3a1717b33ce0c5402304ad961ad9fd7f93b13778279c2f54643b463c51d`  
		Last Modified: Sun, 29 May 2022 22:30:16 GMT  
		Size: 13.6 MB (13603779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cacfeae2772a038f750027e6af5e4bcdb9e93302a2b5c625efdc38d2268239a`  
		Last Modified: Sun, 29 May 2022 22:30:11 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee3da87fc8b8e9131bbd3bc5f63b30a4fb19b33790eee55219649ec08c0f9d4`  
		Last Modified: Sun, 29 May 2022 22:30:28 GMT  
		Size: 34.8 MB (34787037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4d0617fb82de6a03733e8299dde12ee5469872a9d943977fbd313e796cdd9f`  
		Last Modified: Sun, 29 May 2022 22:30:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4851abcfa730fa43d72e11a166df9b1ba141a1eaec01c1faba17c6cd1ff2f8ab`  
		Last Modified: Sun, 29 May 2022 22:30:11 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:34ba8b3dda52146cbb004ed0108ed215a01167ee8812d258aa2dfe7076bc39ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104771886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659fc101ad9f20fd125ecd8cb81139d464e81e33baa231431558ccf95b470112`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 00:42:45 GMT
ADD file:93d675ee0bc32a88dc4d6c0872276c4678dc31f0b6eb8b936cb823f191bc07f0 in / 
# Sat, 28 May 2022 00:42:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:10:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:11:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 00:31:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 00:31:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 00:31:28 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sun, 29 May 2022 00:31:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 00:31:34 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 00:31:34 GMT
EXPOSE 9092
# Sun, 29 May 2022 00:31:35 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 00:31:37 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 00:31:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 00:31:38 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:de7fc2a3b80bcd193de687188fc9051c8be6c61ec81fec3aeae61c079f71e69e`  
		Last Modified: Sat, 28 May 2022 00:51:21 GMT  
		Size: 43.2 MB (43212871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee73573552502f742607ea1dcdefcee9aeafa4ad8d5deca24b48a262f4ba108`  
		Last Modified: Sat, 28 May 2022 11:20:36 GMT  
		Size: 10.2 MB (10218522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05d3983d65175e68348dcb2cd43933f2af4d2d8c1bf36c9d5f237394c9fa53b`  
		Last Modified: Sat, 28 May 2022 11:20:35 GMT  
		Size: 3.9 MB (3874461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8f74dae4587aae058149bbff22363d653b738ecb28be02f413d1bf034b7c6`  
		Last Modified: Sun, 29 May 2022 00:32:16 GMT  
		Size: 12.9 MB (12902056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d454c1b46feace219c701415f116ab5443d39199d58e0c949182ad86976c1a03`  
		Last Modified: Sun, 29 May 2022 00:32:14 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babe2d7fb2be947885b7436703bc34e3da4700d4fb33e9a837645e95457ae52f`  
		Last Modified: Sun, 29 May 2022 00:32:19 GMT  
		Size: 34.6 MB (34560692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d136e987b425ae0a91d0f46621e4211cc445798a0014b568f91f72d50f7103d`  
		Last Modified: Sun, 29 May 2022 00:32:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d32ad681eda580819dba926dd0ad58aeec03cdca102be49f978a429e82bbb8`  
		Last Modified: Sun, 29 May 2022 00:32:14 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9-alpine`

```console
$ docker pull kapacitor@sha256:72166d96c41aecc792347bb7207fd7fce8fb6ad0214d9ff7d37c1582cce51d9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5.9-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:abdce74128d00c6dbcba46427b043488e574b4f2bb5177da9162bd62e1111fbf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22631715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f19f25f0ae1d10d68e6fb9becb4a276fc272a896bdcc115d27bf4ffdd83580a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 07:16:44 GMT
ENV KAPACITOR_VERSION=1.5.9
# Tue, 05 Apr 2022 07:16:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 07:16:52 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 05 Apr 2022 07:16:52 GMT
EXPOSE 9092
# Tue, 05 Apr 2022 07:16:52 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 05 Apr 2022 07:16:52 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Tue, 05 Apr 2022 07:16:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:16:52 GMT
CMD ["kapacitord"]
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
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0eb59b0a9e02ad3acd30214bf6e9be9b5dd3a8473b5333645e05cefab6f995`  
		Last Modified: Tue, 05 Apr 2022 07:17:27 GMT  
		Size: 19.5 MB (19541034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d327126ef09ae07f5d34516658ea1877eab819728ce1905d1a4328490af252c`  
		Last Modified: Tue, 05 Apr 2022 07:17:23 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044949500ea9f07b81cf7142e7cfeacebc25114f7bef3cc97c0f5ab3de23fa94`  
		Last Modified: Tue, 05 Apr 2022 07:17:23 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6`

```console
$ docker pull kapacitor@sha256:0bc661fb71d972b2ba70d936b03bb5702b35002f2dd1cfc3072e19d74cf7e57b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:6e2f2bbb9fae3266627f0c4ce9a8be79dfc54bb4f65e0c77dac9b003998100f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135241720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117064c8b608cdb51cfb40d02f43fe531f1806cbc4b3b7e8cd9346126f69a1c5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:18:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 01:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:19:06 GMT
ENV KAPACITOR_VERSION=1.6.4
# Sun, 29 May 2022 01:19:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 01:19:12 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 01:19:12 GMT
EXPOSE 9092
# Sun, 29 May 2022 01:19:12 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 01:19:12 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 01:19:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:19:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1727216bd01238dbacd5b2e37b678af815c9c87331baa86b3c53b67f97d367`  
		Last Modified: Sun, 29 May 2022 01:19:31 GMT  
		Size: 13.4 MB (13421085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b1d7606415586e476777f810a27be4853e38f99cbf4354a36f224463a2fbf0`  
		Last Modified: Sun, 29 May 2022 01:19:29 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7335d53f5f2ff4604a3aa7dde55a5ad9dcf21dbf22d99d6a225c262136d84a8a`  
		Last Modified: Sun, 29 May 2022 01:19:52 GMT  
		Size: 60.7 MB (60741608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebed7cd15a3229a0ac2a47efd9bbb6b4220d8b302e65d0b72fe5fd3b00daf7e1`  
		Last Modified: Sun, 29 May 2022 01:19:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fcac5b1822dcceaba86ccea6e00250d50f56713c9599d0b1a59802e0d89693`  
		Last Modified: Sun, 29 May 2022 01:19:45 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:0453659e300b211a8e0f06f997c3a52a4aa936dfcbaaf143648a9e268949d6cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127206755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bc55ffd190130f7a4e75667387f5ce9a7f73688297215047444595575e3a115`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 00:42:45 GMT
ADD file:93d675ee0bc32a88dc4d6c0872276c4678dc31f0b6eb8b936cb823f191bc07f0 in / 
# Sat, 28 May 2022 00:42:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:10:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:11:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 00:31:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 00:31:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 00:31:46 GMT
ENV KAPACITOR_VERSION=1.6.4
# Sun, 29 May 2022 00:31:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 00:31:53 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 00:31:53 GMT
EXPOSE 9092
# Sun, 29 May 2022 00:31:54 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 00:31:56 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 00:31:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 00:31:57 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:de7fc2a3b80bcd193de687188fc9051c8be6c61ec81fec3aeae61c079f71e69e`  
		Last Modified: Sat, 28 May 2022 00:51:21 GMT  
		Size: 43.2 MB (43212871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee73573552502f742607ea1dcdefcee9aeafa4ad8d5deca24b48a262f4ba108`  
		Last Modified: Sat, 28 May 2022 11:20:36 GMT  
		Size: 10.2 MB (10218522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05d3983d65175e68348dcb2cd43933f2af4d2d8c1bf36c9d5f237394c9fa53b`  
		Last Modified: Sat, 28 May 2022 11:20:35 GMT  
		Size: 3.9 MB (3874461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8f74dae4587aae058149bbff22363d653b738ecb28be02f413d1bf034b7c6`  
		Last Modified: Sun, 29 May 2022 00:32:16 GMT  
		Size: 12.9 MB (12902056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d454c1b46feace219c701415f116ab5443d39199d58e0c949182ad86976c1a03`  
		Last Modified: Sun, 29 May 2022 00:32:14 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3851da6043768a64a997e2f7785dcc44f251fc1765506c856ed744937bc288`  
		Last Modified: Sun, 29 May 2022 00:32:38 GMT  
		Size: 57.0 MB (56995561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4de92e6d38a9dfb8350dbaf6671cd7d65f183c3081d8baf3c9330569aa4f82`  
		Last Modified: Sun, 29 May 2022 00:32:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66f3b4f34ed8366d81c4218b1cbf18d2d9abc857a7ed9918142dd75d2402b8b`  
		Last Modified: Sun, 29 May 2022 00:32:30 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6-alpine`

```console
$ docker pull kapacitor@sha256:0aa9d9db2692a9efd69dec3fc7cf657b9d3be7f852b91d1adcdbacb115ba21fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:56cc852ef0db0e9d846808de310e003295335e54426a0095bad5ef7f66a6ab19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63761508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a2b7595165f3cf12a482ef8d999ae05416d93ec4d965bfd253f9cfbb136ac5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 07:16:57 GMT
ENV KAPACITOR_VERSION=1.6.4
# Tue, 05 Apr 2022 07:17:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 07:17:06 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 05 Apr 2022 07:17:06 GMT
EXPOSE 9092
# Tue, 05 Apr 2022 07:17:06 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 05 Apr 2022 07:17:06 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Tue, 05 Apr 2022 07:17:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:17:06 GMT
CMD ["kapacitord"]
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
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e125e1e43433c8cee41026f15278127447e06aa7720d45e1f22108a4e3fe5eaa`  
		Last Modified: Tue, 05 Apr 2022 07:17:45 GMT  
		Size: 60.7 MB (60670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f0a25df483e67319e534f4c9ef34d654da2ceb8dd065099f633e439b82b64d`  
		Last Modified: Tue, 05 Apr 2022 07:17:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c6845b70b2213da8c8dceb9d1dbfc31a9d12e92f53812edbde7e342e6c24e9`  
		Last Modified: Tue, 05 Apr 2022 07:17:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.4`

```console
$ docker pull kapacitor@sha256:0bc661fb71d972b2ba70d936b03bb5702b35002f2dd1cfc3072e19d74cf7e57b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6.4` - linux; amd64

```console
$ docker pull kapacitor@sha256:6e2f2bbb9fae3266627f0c4ce9a8be79dfc54bb4f65e0c77dac9b003998100f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135241720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117064c8b608cdb51cfb40d02f43fe531f1806cbc4b3b7e8cd9346126f69a1c5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:18:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 01:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:19:06 GMT
ENV KAPACITOR_VERSION=1.6.4
# Sun, 29 May 2022 01:19:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 01:19:12 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 01:19:12 GMT
EXPOSE 9092
# Sun, 29 May 2022 01:19:12 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 01:19:12 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 01:19:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:19:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1727216bd01238dbacd5b2e37b678af815c9c87331baa86b3c53b67f97d367`  
		Last Modified: Sun, 29 May 2022 01:19:31 GMT  
		Size: 13.4 MB (13421085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b1d7606415586e476777f810a27be4853e38f99cbf4354a36f224463a2fbf0`  
		Last Modified: Sun, 29 May 2022 01:19:29 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7335d53f5f2ff4604a3aa7dde55a5ad9dcf21dbf22d99d6a225c262136d84a8a`  
		Last Modified: Sun, 29 May 2022 01:19:52 GMT  
		Size: 60.7 MB (60741608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebed7cd15a3229a0ac2a47efd9bbb6b4220d8b302e65d0b72fe5fd3b00daf7e1`  
		Last Modified: Sun, 29 May 2022 01:19:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fcac5b1822dcceaba86ccea6e00250d50f56713c9599d0b1a59802e0d89693`  
		Last Modified: Sun, 29 May 2022 01:19:45 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6.4` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:0453659e300b211a8e0f06f997c3a52a4aa936dfcbaaf143648a9e268949d6cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127206755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bc55ffd190130f7a4e75667387f5ce9a7f73688297215047444595575e3a115`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 00:42:45 GMT
ADD file:93d675ee0bc32a88dc4d6c0872276c4678dc31f0b6eb8b936cb823f191bc07f0 in / 
# Sat, 28 May 2022 00:42:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:10:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:11:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 00:31:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 00:31:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 00:31:46 GMT
ENV KAPACITOR_VERSION=1.6.4
# Sun, 29 May 2022 00:31:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 00:31:53 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 00:31:53 GMT
EXPOSE 9092
# Sun, 29 May 2022 00:31:54 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 00:31:56 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 00:31:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 00:31:57 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:de7fc2a3b80bcd193de687188fc9051c8be6c61ec81fec3aeae61c079f71e69e`  
		Last Modified: Sat, 28 May 2022 00:51:21 GMT  
		Size: 43.2 MB (43212871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee73573552502f742607ea1dcdefcee9aeafa4ad8d5deca24b48a262f4ba108`  
		Last Modified: Sat, 28 May 2022 11:20:36 GMT  
		Size: 10.2 MB (10218522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05d3983d65175e68348dcb2cd43933f2af4d2d8c1bf36c9d5f237394c9fa53b`  
		Last Modified: Sat, 28 May 2022 11:20:35 GMT  
		Size: 3.9 MB (3874461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8f74dae4587aae058149bbff22363d653b738ecb28be02f413d1bf034b7c6`  
		Last Modified: Sun, 29 May 2022 00:32:16 GMT  
		Size: 12.9 MB (12902056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d454c1b46feace219c701415f116ab5443d39199d58e0c949182ad86976c1a03`  
		Last Modified: Sun, 29 May 2022 00:32:14 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3851da6043768a64a997e2f7785dcc44f251fc1765506c856ed744937bc288`  
		Last Modified: Sun, 29 May 2022 00:32:38 GMT  
		Size: 57.0 MB (56995561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4de92e6d38a9dfb8350dbaf6671cd7d65f183c3081d8baf3c9330569aa4f82`  
		Last Modified: Sun, 29 May 2022 00:32:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66f3b4f34ed8366d81c4218b1cbf18d2d9abc857a7ed9918142dd75d2402b8b`  
		Last Modified: Sun, 29 May 2022 00:32:30 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.4-alpine`

```console
$ docker pull kapacitor@sha256:0aa9d9db2692a9efd69dec3fc7cf657b9d3be7f852b91d1adcdbacb115ba21fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6.4-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:56cc852ef0db0e9d846808de310e003295335e54426a0095bad5ef7f66a6ab19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63761508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a2b7595165f3cf12a482ef8d999ae05416d93ec4d965bfd253f9cfbb136ac5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 07:16:57 GMT
ENV KAPACITOR_VERSION=1.6.4
# Tue, 05 Apr 2022 07:17:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 07:17:06 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 05 Apr 2022 07:17:06 GMT
EXPOSE 9092
# Tue, 05 Apr 2022 07:17:06 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 05 Apr 2022 07:17:06 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Tue, 05 Apr 2022 07:17:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:17:06 GMT
CMD ["kapacitord"]
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
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e125e1e43433c8cee41026f15278127447e06aa7720d45e1f22108a4e3fe5eaa`  
		Last Modified: Tue, 05 Apr 2022 07:17:45 GMT  
		Size: 60.7 MB (60670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f0a25df483e67319e534f4c9ef34d654da2ceb8dd065099f633e439b82b64d`  
		Last Modified: Tue, 05 Apr 2022 07:17:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c6845b70b2213da8c8dceb9d1dbfc31a9d12e92f53812edbde7e342e6c24e9`  
		Last Modified: Tue, 05 Apr 2022 07:17:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:0aa9d9db2692a9efd69dec3fc7cf657b9d3be7f852b91d1adcdbacb115ba21fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:56cc852ef0db0e9d846808de310e003295335e54426a0095bad5ef7f66a6ab19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63761508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a2b7595165f3cf12a482ef8d999ae05416d93ec4d965bfd253f9cfbb136ac5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:26:14 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:26:16 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Tue, 05 Apr 2022 07:16:57 GMT
ENV KAPACITOR_VERSION=1.6.4
# Tue, 05 Apr 2022 07:17:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 05 Apr 2022 07:17:06 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 05 Apr 2022 07:17:06 GMT
EXPOSE 9092
# Tue, 05 Apr 2022 07:17:06 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 05 Apr 2022 07:17:06 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Tue, 05 Apr 2022 07:17:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:17:06 GMT
CMD ["kapacitord"]
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
	-	`sha256:58beb826c7b7288de69f85c4476fd6f04b58ceed760dd1b9e51a7d80aeb0e471`  
		Last Modified: Tue, 05 Apr 2022 04:27:20 GMT  
		Size: 271.7 KB (271678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e125e1e43433c8cee41026f15278127447e06aa7720d45e1f22108a4e3fe5eaa`  
		Last Modified: Tue, 05 Apr 2022 07:17:45 GMT  
		Size: 60.7 MB (60670853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f0a25df483e67319e534f4c9ef34d654da2ceb8dd065099f633e439b82b64d`  
		Last Modified: Tue, 05 Apr 2022 07:17:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c6845b70b2213da8c8dceb9d1dbfc31a9d12e92f53812edbde7e342e6c24e9`  
		Last Modified: Tue, 05 Apr 2022 07:17:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:0bc661fb71d972b2ba70d936b03bb5702b35002f2dd1cfc3072e19d74cf7e57b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:6e2f2bbb9fae3266627f0c4ce9a8be79dfc54bb4f65e0c77dac9b003998100f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135241720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117064c8b608cdb51cfb40d02f43fe531f1806cbc4b3b7e8cd9346126f69a1c5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 01:22:09 GMT
ADD file:ba5db69738244d00088ef591ca43fa8b3189e78fba56bc69b70a232e6f04c7e4 in / 
# Sat, 28 May 2022 01:22:10 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 01:18:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 01:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 01:19:06 GMT
ENV KAPACITOR_VERSION=1.6.4
# Sun, 29 May 2022 01:19:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 01:19:12 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 01:19:12 GMT
EXPOSE 9092
# Sun, 29 May 2022 01:19:12 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 01:19:12 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 01:19:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 01:19:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d3d4e1d44a24e0c5abd41b803d14f211ba153bc7963871713cba8ee5fc687888`  
		Last Modified: Sat, 28 May 2022 01:28:41 GMT  
		Size: 45.4 MB (45429730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec8bceb2e238bbbbec9e458cf83c1342015ed1b717be0f88b50d267c52437d`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 11.3 MB (11302994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aa521faedb4a16c079e9574f537b51a05c2ad4fbabd16f83d9bd58c365bac`  
		Last Modified: Sat, 28 May 2022 02:52:34 GMT  
		Size: 4.3 MB (4342992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1727216bd01238dbacd5b2e37b678af815c9c87331baa86b3c53b67f97d367`  
		Last Modified: Sun, 29 May 2022 01:19:31 GMT  
		Size: 13.4 MB (13421085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b1d7606415586e476777f810a27be4853e38f99cbf4354a36f224463a2fbf0`  
		Last Modified: Sun, 29 May 2022 01:19:29 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7335d53f5f2ff4604a3aa7dde55a5ad9dcf21dbf22d99d6a225c262136d84a8a`  
		Last Modified: Sun, 29 May 2022 01:19:52 GMT  
		Size: 60.7 MB (60741608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebed7cd15a3229a0ac2a47efd9bbb6b4220d8b302e65d0b72fe5fd3b00daf7e1`  
		Last Modified: Sun, 29 May 2022 01:19:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fcac5b1822dcceaba86ccea6e00250d50f56713c9599d0b1a59802e0d89693`  
		Last Modified: Sun, 29 May 2022 01:19:45 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:0453659e300b211a8e0f06f997c3a52a4aa936dfcbaaf143648a9e268949d6cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127206755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bc55ffd190130f7a4e75667387f5ce9a7f73688297215047444595575e3a115`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Sat, 28 May 2022 00:42:45 GMT
ADD file:93d675ee0bc32a88dc4d6c0872276c4678dc31f0b6eb8b936cb823f191bc07f0 in / 
# Sat, 28 May 2022 00:42:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:10:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:11:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 00:31:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sun, 29 May 2022 00:31:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 29 May 2022 00:31:46 GMT
ENV KAPACITOR_VERSION=1.6.4
# Sun, 29 May 2022 00:31:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sun, 29 May 2022 00:31:53 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sun, 29 May 2022 00:31:53 GMT
EXPOSE 9092
# Sun, 29 May 2022 00:31:54 GMT
VOLUME [/var/lib/kapacitor]
# Sun, 29 May 2022 00:31:56 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sun, 29 May 2022 00:31:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 29 May 2022 00:31:57 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:de7fc2a3b80bcd193de687188fc9051c8be6c61ec81fec3aeae61c079f71e69e`  
		Last Modified: Sat, 28 May 2022 00:51:21 GMT  
		Size: 43.2 MB (43212871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee73573552502f742607ea1dcdefcee9aeafa4ad8d5deca24b48a262f4ba108`  
		Last Modified: Sat, 28 May 2022 11:20:36 GMT  
		Size: 10.2 MB (10218522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05d3983d65175e68348dcb2cd43933f2af4d2d8c1bf36c9d5f237394c9fa53b`  
		Last Modified: Sat, 28 May 2022 11:20:35 GMT  
		Size: 3.9 MB (3874461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8f74dae4587aae058149bbff22363d653b738ecb28be02f413d1bf034b7c6`  
		Last Modified: Sun, 29 May 2022 00:32:16 GMT  
		Size: 12.9 MB (12902056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d454c1b46feace219c701415f116ab5443d39199d58e0c949182ad86976c1a03`  
		Last Modified: Sun, 29 May 2022 00:32:14 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3851da6043768a64a997e2f7785dcc44f251fc1765506c856ed744937bc288`  
		Last Modified: Sun, 29 May 2022 00:32:38 GMT  
		Size: 57.0 MB (56995561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4de92e6d38a9dfb8350dbaf6671cd7d65f183c3081d8baf3c9330569aa4f82`  
		Last Modified: Sun, 29 May 2022 00:32:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66f3b4f34ed8366d81c4218b1cbf18d2d9abc857a7ed9918142dd75d2402b8b`  
		Last Modified: Sun, 29 May 2022 00:32:30 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
