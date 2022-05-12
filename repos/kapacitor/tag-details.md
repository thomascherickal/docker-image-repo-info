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
$ docker pull kapacitor@sha256:2dc2e049f3ec95241393c96f431af6aa13b6c5a0d9480e6d90bc25c14f5a5510
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:fb587ff56a2dce6a5c1ad6977d83e918713933fe0274adf23b85f738eda69968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111710117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d8389264b1d990123d0b338d1b47f561cf246323eab94ca7a7f79e6047699c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:19:07 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 11 May 2022 20:19:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:19:11 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 11 May 2022 20:19:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 11 May 2022 20:19:15 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 11 May 2022 20:19:15 GMT
EXPOSE 9092
# Wed, 11 May 2022 20:19:15 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 11 May 2022 20:19:15 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 11 May 2022 20:19:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:19:15 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba195b4bc21ef3724f088897d1aac8e7068de1417a81ee5d80a4b8e0092a038`  
		Last Modified: Wed, 11 May 2022 20:19:47 GMT  
		Size: 13.4 MB (13413735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9ee354c8a8e72692bd91bae5e779d1ca41bd63a0437089cb5e7cb46629d412`  
		Last Modified: Wed, 11 May 2022 20:19:46 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b26d611318e87d04879696fbbc0b2b3bd8f6906bc282a11950582d1ce2e8248`  
		Last Modified: Wed, 11 May 2022 20:19:51 GMT  
		Size: 37.2 MB (37219867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1d6508768f173ee694992af50ad2caacdd2ff48ded670ca0c76e9a1ba5c66f`  
		Last Modified: Wed, 11 May 2022 20:19:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a3379dd7643b028e54bc66856c3d8d1c7f07d5529bf2b88e22b17abc08cefb`  
		Last Modified: Wed, 11 May 2022 20:19:46 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:2f5487c04b9c0e6824aba12055f69d97bdd1b707489eb88be0003ffef7de4c32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104416340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc353b9f7eaa20889de2833d1a191507181f0ecdf88465311b0c71e73cc51797`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 01:54:33 GMT
ADD file:c679388ac7a37037465302aea3117354d9746d0c50c056e826b5c8c58aea5138 in / 
# Wed, 11 May 2022 01:54:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:33:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 12 May 2022 15:36:16 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 12 May 2022 15:36:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 12 May 2022 15:36:20 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 12 May 2022 15:36:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 12 May 2022 15:36:30 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 12 May 2022 15:36:30 GMT
EXPOSE 9092
# Thu, 12 May 2022 15:36:31 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 12 May 2022 15:36:31 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 12 May 2022 15:36:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 May 2022 15:36:32 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:629c5b996bdb9cea71f1d194d7a244d4aba271133bad4f5b88bfe38c4626349a`  
		Last Modified: Wed, 11 May 2022 02:11:17 GMT  
		Size: 42.2 MB (42151163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbf25ac5d0e3ca11a0fb961c2ac0f897f1982389c85b6e31ee0fa63a0293cc0`  
		Last Modified: Wed, 11 May 2022 03:55:11 GMT  
		Size: 10.0 MB (9956859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a3f9738e27d03b85306ba8927ec41f0ffd375d26fc501906f097e639a1047f`  
		Last Modified: Wed, 11 May 2022 03:55:08 GMT  
		Size: 3.9 MB (3921810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddedfc20151593a8ea9055091cbb117143a3bfd82e2ecd4f5f308f00f7043327`  
		Last Modified: Thu, 12 May 2022 15:36:58 GMT  
		Size: 13.6 MB (13596121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445aa379798adbb08447c5ab14d7152c9b300a0d14ae197a88c0e8b7590f4a01`  
		Last Modified: Thu, 12 May 2022 15:36:53 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e3cebe3fe3ec987a625244a08a35770565d5d7b0a0c6b8232c490c16fc685d`  
		Last Modified: Thu, 12 May 2022 15:37:11 GMT  
		Size: 34.8 MB (34787075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3aded3fca718db5f60f99a72475ae135f0f2a3b15ca3842afe2f52753b3b3b`  
		Last Modified: Thu, 12 May 2022 15:36:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1eca65012a42a4d7ea01f5afbf18090db174436cb776caa62967826917a7027`  
		Last Modified: Thu, 12 May 2022 15:36:53 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:80797b0b78cb807ffaa15f7c48496765303310411b34f911deddcc4a58954b59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104764319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ef2bbabca90ae95851862a06f7af44ae3d746b1c743be33040b58ce5c0380d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 00:49:08 GMT
ADD file:8949016fba61b18207f5a2309fc974562080c5cc80d1eb82adb35c4fa03f6f05 in / 
# Wed, 11 May 2022 00:49:09 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:29:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:30:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:53:03 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 11 May 2022 19:53:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 19:53:08 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 11 May 2022 19:53:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 11 May 2022 19:53:14 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 11 May 2022 19:53:14 GMT
EXPOSE 9092
# Wed, 11 May 2022 19:53:15 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 11 May 2022 19:53:17 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 11 May 2022 19:53:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:53:18 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:139065d8f4553df403babda56f830c32aa1f3e57f18d2145a3179468921a4bb8`  
		Last Modified: Wed, 11 May 2022 00:57:26 GMT  
		Size: 43.2 MB (43212478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0acfd1725613d968a54b7fbfe1f70f24b8a0dad792ad3cb28349035f7736fe`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 10.2 MB (10217776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002c314192ef0350d2ac1d1e49b4fddbc49dbcdc609e56e0e2567ee2dd37f0bc`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 3.9 MB (3874525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496f27b7f192b22433c9935e31905643e2224453cec24dd8a895fbc0ed124a61`  
		Last Modified: Wed, 11 May 2022 19:53:54 GMT  
		Size: 12.9 MB (12895614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c865c958dbaf4cdc7c502e2fa2e224ecd728970e3f5a6624c291b06f0f0fe724`  
		Last Modified: Wed, 11 May 2022 19:53:53 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbde5d976b7086151e9314fa513a46dbed36b87c8214481400fab570ece5dc1`  
		Last Modified: Wed, 11 May 2022 19:53:58 GMT  
		Size: 34.6 MB (34560648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c229f0a05541dc2b588fd4dc28eaff2a91092d38099fcb0a8a12ea6ba70745a`  
		Last Modified: Wed, 11 May 2022 19:53:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815438d08a64855bf0d0e0c5f33ecd31c963c6786e48e604aa6b2e69be666f65`  
		Last Modified: Wed, 11 May 2022 19:53:53 GMT  
		Size: 230.0 B  
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
$ docker pull kapacitor@sha256:2dc2e049f3ec95241393c96f431af6aa13b6c5a0d9480e6d90bc25c14f5a5510
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.9` - linux; amd64

```console
$ docker pull kapacitor@sha256:fb587ff56a2dce6a5c1ad6977d83e918713933fe0274adf23b85f738eda69968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111710117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d8389264b1d990123d0b338d1b47f561cf246323eab94ca7a7f79e6047699c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:19:07 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 11 May 2022 20:19:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:19:11 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 11 May 2022 20:19:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 11 May 2022 20:19:15 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 11 May 2022 20:19:15 GMT
EXPOSE 9092
# Wed, 11 May 2022 20:19:15 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 11 May 2022 20:19:15 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 11 May 2022 20:19:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:19:15 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba195b4bc21ef3724f088897d1aac8e7068de1417a81ee5d80a4b8e0092a038`  
		Last Modified: Wed, 11 May 2022 20:19:47 GMT  
		Size: 13.4 MB (13413735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9ee354c8a8e72692bd91bae5e779d1ca41bd63a0437089cb5e7cb46629d412`  
		Last Modified: Wed, 11 May 2022 20:19:46 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b26d611318e87d04879696fbbc0b2b3bd8f6906bc282a11950582d1ce2e8248`  
		Last Modified: Wed, 11 May 2022 20:19:51 GMT  
		Size: 37.2 MB (37219867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1d6508768f173ee694992af50ad2caacdd2ff48ded670ca0c76e9a1ba5c66f`  
		Last Modified: Wed, 11 May 2022 20:19:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a3379dd7643b028e54bc66856c3d8d1c7f07d5529bf2b88e22b17abc08cefb`  
		Last Modified: Wed, 11 May 2022 20:19:46 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:2f5487c04b9c0e6824aba12055f69d97bdd1b707489eb88be0003ffef7de4c32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104416340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc353b9f7eaa20889de2833d1a191507181f0ecdf88465311b0c71e73cc51797`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 01:54:33 GMT
ADD file:c679388ac7a37037465302aea3117354d9746d0c50c056e826b5c8c58aea5138 in / 
# Wed, 11 May 2022 01:54:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:33:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 12 May 2022 15:36:16 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 12 May 2022 15:36:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 12 May 2022 15:36:20 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 12 May 2022 15:36:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 12 May 2022 15:36:30 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 12 May 2022 15:36:30 GMT
EXPOSE 9092
# Thu, 12 May 2022 15:36:31 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 12 May 2022 15:36:31 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 12 May 2022 15:36:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 May 2022 15:36:32 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:629c5b996bdb9cea71f1d194d7a244d4aba271133bad4f5b88bfe38c4626349a`  
		Last Modified: Wed, 11 May 2022 02:11:17 GMT  
		Size: 42.2 MB (42151163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbf25ac5d0e3ca11a0fb961c2ac0f897f1982389c85b6e31ee0fa63a0293cc0`  
		Last Modified: Wed, 11 May 2022 03:55:11 GMT  
		Size: 10.0 MB (9956859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a3f9738e27d03b85306ba8927ec41f0ffd375d26fc501906f097e639a1047f`  
		Last Modified: Wed, 11 May 2022 03:55:08 GMT  
		Size: 3.9 MB (3921810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddedfc20151593a8ea9055091cbb117143a3bfd82e2ecd4f5f308f00f7043327`  
		Last Modified: Thu, 12 May 2022 15:36:58 GMT  
		Size: 13.6 MB (13596121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445aa379798adbb08447c5ab14d7152c9b300a0d14ae197a88c0e8b7590f4a01`  
		Last Modified: Thu, 12 May 2022 15:36:53 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e3cebe3fe3ec987a625244a08a35770565d5d7b0a0c6b8232c490c16fc685d`  
		Last Modified: Thu, 12 May 2022 15:37:11 GMT  
		Size: 34.8 MB (34787075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3aded3fca718db5f60f99a72475ae135f0f2a3b15ca3842afe2f52753b3b3b`  
		Last Modified: Thu, 12 May 2022 15:36:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1eca65012a42a4d7ea01f5afbf18090db174436cb776caa62967826917a7027`  
		Last Modified: Thu, 12 May 2022 15:36:53 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:80797b0b78cb807ffaa15f7c48496765303310411b34f911deddcc4a58954b59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104764319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ef2bbabca90ae95851862a06f7af44ae3d746b1c743be33040b58ce5c0380d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 00:49:08 GMT
ADD file:8949016fba61b18207f5a2309fc974562080c5cc80d1eb82adb35c4fa03f6f05 in / 
# Wed, 11 May 2022 00:49:09 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:29:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:30:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:53:03 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 11 May 2022 19:53:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 19:53:08 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 11 May 2022 19:53:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 11 May 2022 19:53:14 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 11 May 2022 19:53:14 GMT
EXPOSE 9092
# Wed, 11 May 2022 19:53:15 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 11 May 2022 19:53:17 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 11 May 2022 19:53:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:53:18 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:139065d8f4553df403babda56f830c32aa1f3e57f18d2145a3179468921a4bb8`  
		Last Modified: Wed, 11 May 2022 00:57:26 GMT  
		Size: 43.2 MB (43212478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0acfd1725613d968a54b7fbfe1f70f24b8a0dad792ad3cb28349035f7736fe`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 10.2 MB (10217776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002c314192ef0350d2ac1d1e49b4fddbc49dbcdc609e56e0e2567ee2dd37f0bc`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 3.9 MB (3874525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496f27b7f192b22433c9935e31905643e2224453cec24dd8a895fbc0ed124a61`  
		Last Modified: Wed, 11 May 2022 19:53:54 GMT  
		Size: 12.9 MB (12895614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c865c958dbaf4cdc7c502e2fa2e224ecd728970e3f5a6624c291b06f0f0fe724`  
		Last Modified: Wed, 11 May 2022 19:53:53 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbde5d976b7086151e9314fa513a46dbed36b87c8214481400fab570ece5dc1`  
		Last Modified: Wed, 11 May 2022 19:53:58 GMT  
		Size: 34.6 MB (34560648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c229f0a05541dc2b588fd4dc28eaff2a91092d38099fcb0a8a12ea6ba70745a`  
		Last Modified: Wed, 11 May 2022 19:53:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815438d08a64855bf0d0e0c5f33ecd31c963c6786e48e604aa6b2e69be666f65`  
		Last Modified: Wed, 11 May 2022 19:53:53 GMT  
		Size: 230.0 B  
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
$ docker pull kapacitor@sha256:51e6e692564e09f1cacafa1526b486ddb228e040fd100a899e5b568c7096995f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:12683525b8aadd049bbb22c3d51d91e1c009a0d114d35f98469e25bbe4b6ce9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135231814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f4f2e21e2a902417b6ca2f4e7bf8e0c25b644e311a3de0bd0d69e0c222d7ef8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:19:07 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 11 May 2022 20:19:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:19:20 GMT
ENV KAPACITOR_VERSION=1.6.4
# Wed, 11 May 2022 20:19:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 11 May 2022 20:19:27 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 11 May 2022 20:19:27 GMT
EXPOSE 9092
# Wed, 11 May 2022 20:19:27 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 11 May 2022 20:19:27 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 11 May 2022 20:19:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:19:27 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba195b4bc21ef3724f088897d1aac8e7068de1417a81ee5d80a4b8e0092a038`  
		Last Modified: Wed, 11 May 2022 20:19:47 GMT  
		Size: 13.4 MB (13413735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9ee354c8a8e72692bd91bae5e779d1ca41bd63a0437089cb5e7cb46629d412`  
		Last Modified: Wed, 11 May 2022 20:19:46 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491e40cfb28334046f70a3c70214a052de63e68cb16450865444c462fdd3f51a`  
		Last Modified: Wed, 11 May 2022 20:20:09 GMT  
		Size: 60.7 MB (60741566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2763a3617f4aa0a2e4415718effb031aedcf1a18bc26845c46c9d5e3a1a0cb0`  
		Last Modified: Wed, 11 May 2022 20:20:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249e566eed48ae124d6205ee9f5d5a6342a3e4e89e1273d9abc38cbc3fc1fad4`  
		Last Modified: Wed, 11 May 2022 20:20:01 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:a0ea377d14794289194320acc8cd74433d7bba0275cd30355faa9104b95f3a62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127199217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec513cad13280cdf4cf04a414c22fdd873882f4b348ae97d0ba9b86f7363b556`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 00:49:08 GMT
ADD file:8949016fba61b18207f5a2309fc974562080c5cc80d1eb82adb35c4fa03f6f05 in / 
# Wed, 11 May 2022 00:49:09 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:29:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:30:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:53:03 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 11 May 2022 19:53:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 19:53:25 GMT
ENV KAPACITOR_VERSION=1.6.4
# Wed, 11 May 2022 19:53:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 11 May 2022 19:53:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 11 May 2022 19:53:31 GMT
EXPOSE 9092
# Wed, 11 May 2022 19:53:32 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 11 May 2022 19:53:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 11 May 2022 19:53:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:53:35 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:139065d8f4553df403babda56f830c32aa1f3e57f18d2145a3179468921a4bb8`  
		Last Modified: Wed, 11 May 2022 00:57:26 GMT  
		Size: 43.2 MB (43212478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0acfd1725613d968a54b7fbfe1f70f24b8a0dad792ad3cb28349035f7736fe`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 10.2 MB (10217776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002c314192ef0350d2ac1d1e49b4fddbc49dbcdc609e56e0e2567ee2dd37f0bc`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 3.9 MB (3874525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496f27b7f192b22433c9935e31905643e2224453cec24dd8a895fbc0ed124a61`  
		Last Modified: Wed, 11 May 2022 19:53:54 GMT  
		Size: 12.9 MB (12895614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c865c958dbaf4cdc7c502e2fa2e224ecd728970e3f5a6624c291b06f0f0fe724`  
		Last Modified: Wed, 11 May 2022 19:53:53 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9600783cb63804ab90b3c37bfc621d2f9ea15f4bc9aa6cf53f71f7ced8942550`  
		Last Modified: Wed, 11 May 2022 19:54:16 GMT  
		Size: 57.0 MB (56995547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb592b11071788c11c6233720ccfb56da4a2482aefa1388006bbd475bdfefd3`  
		Last Modified: Wed, 11 May 2022 19:54:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdfaac5862ab10711f77f97e571ce72394d53fb4584c1f3ba2a8d767228ea2d`  
		Last Modified: Wed, 11 May 2022 19:54:09 GMT  
		Size: 230.0 B  
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
$ docker pull kapacitor@sha256:51e6e692564e09f1cacafa1526b486ddb228e040fd100a899e5b568c7096995f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6.4` - linux; amd64

```console
$ docker pull kapacitor@sha256:12683525b8aadd049bbb22c3d51d91e1c009a0d114d35f98469e25bbe4b6ce9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135231814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f4f2e21e2a902417b6ca2f4e7bf8e0c25b644e311a3de0bd0d69e0c222d7ef8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:19:07 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 11 May 2022 20:19:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:19:20 GMT
ENV KAPACITOR_VERSION=1.6.4
# Wed, 11 May 2022 20:19:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 11 May 2022 20:19:27 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 11 May 2022 20:19:27 GMT
EXPOSE 9092
# Wed, 11 May 2022 20:19:27 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 11 May 2022 20:19:27 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 11 May 2022 20:19:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:19:27 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba195b4bc21ef3724f088897d1aac8e7068de1417a81ee5d80a4b8e0092a038`  
		Last Modified: Wed, 11 May 2022 20:19:47 GMT  
		Size: 13.4 MB (13413735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9ee354c8a8e72692bd91bae5e779d1ca41bd63a0437089cb5e7cb46629d412`  
		Last Modified: Wed, 11 May 2022 20:19:46 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491e40cfb28334046f70a3c70214a052de63e68cb16450865444c462fdd3f51a`  
		Last Modified: Wed, 11 May 2022 20:20:09 GMT  
		Size: 60.7 MB (60741566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2763a3617f4aa0a2e4415718effb031aedcf1a18bc26845c46c9d5e3a1a0cb0`  
		Last Modified: Wed, 11 May 2022 20:20:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249e566eed48ae124d6205ee9f5d5a6342a3e4e89e1273d9abc38cbc3fc1fad4`  
		Last Modified: Wed, 11 May 2022 20:20:01 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6.4` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:a0ea377d14794289194320acc8cd74433d7bba0275cd30355faa9104b95f3a62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127199217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec513cad13280cdf4cf04a414c22fdd873882f4b348ae97d0ba9b86f7363b556`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 00:49:08 GMT
ADD file:8949016fba61b18207f5a2309fc974562080c5cc80d1eb82adb35c4fa03f6f05 in / 
# Wed, 11 May 2022 00:49:09 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:29:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:30:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:53:03 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 11 May 2022 19:53:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 19:53:25 GMT
ENV KAPACITOR_VERSION=1.6.4
# Wed, 11 May 2022 19:53:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 11 May 2022 19:53:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 11 May 2022 19:53:31 GMT
EXPOSE 9092
# Wed, 11 May 2022 19:53:32 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 11 May 2022 19:53:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 11 May 2022 19:53:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:53:35 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:139065d8f4553df403babda56f830c32aa1f3e57f18d2145a3179468921a4bb8`  
		Last Modified: Wed, 11 May 2022 00:57:26 GMT  
		Size: 43.2 MB (43212478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0acfd1725613d968a54b7fbfe1f70f24b8a0dad792ad3cb28349035f7736fe`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 10.2 MB (10217776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002c314192ef0350d2ac1d1e49b4fddbc49dbcdc609e56e0e2567ee2dd37f0bc`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 3.9 MB (3874525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496f27b7f192b22433c9935e31905643e2224453cec24dd8a895fbc0ed124a61`  
		Last Modified: Wed, 11 May 2022 19:53:54 GMT  
		Size: 12.9 MB (12895614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c865c958dbaf4cdc7c502e2fa2e224ecd728970e3f5a6624c291b06f0f0fe724`  
		Last Modified: Wed, 11 May 2022 19:53:53 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9600783cb63804ab90b3c37bfc621d2f9ea15f4bc9aa6cf53f71f7ced8942550`  
		Last Modified: Wed, 11 May 2022 19:54:16 GMT  
		Size: 57.0 MB (56995547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb592b11071788c11c6233720ccfb56da4a2482aefa1388006bbd475bdfefd3`  
		Last Modified: Wed, 11 May 2022 19:54:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdfaac5862ab10711f77f97e571ce72394d53fb4584c1f3ba2a8d767228ea2d`  
		Last Modified: Wed, 11 May 2022 19:54:09 GMT  
		Size: 230.0 B  
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
$ docker pull kapacitor@sha256:51e6e692564e09f1cacafa1526b486ddb228e040fd100a899e5b568c7096995f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:12683525b8aadd049bbb22c3d51d91e1c009a0d114d35f98469e25bbe4b6ce9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135231814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f4f2e21e2a902417b6ca2f4e7bf8e0c25b644e311a3de0bd0d69e0c222d7ef8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 01:22:05 GMT
ADD file:00f57642edc8479d50e6470a3509ad679eb9353761912deade33251fb3d9daa8 in / 
# Wed, 11 May 2022 01:22:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:53:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:19:07 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 11 May 2022 20:19:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 20:19:20 GMT
ENV KAPACITOR_VERSION=1.6.4
# Wed, 11 May 2022 20:19:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 11 May 2022 20:19:27 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 11 May 2022 20:19:27 GMT
EXPOSE 9092
# Wed, 11 May 2022 20:19:27 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 11 May 2022 20:19:27 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 11 May 2022 20:19:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 20:19:27 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:06e39e28714dba08fe310ca1aafb43905427729ecf8e9586f811a7e5062fd09b`  
		Last Modified: Wed, 11 May 2022 01:28:34 GMT  
		Size: 45.4 MB (45428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2141afc44a4cc9b8f9bd9ae1ad4ec8921fdf75b6be9b192b60f1b7f8469919`  
		Last Modified: Wed, 11 May 2022 02:00:35 GMT  
		Size: 11.3 MB (11302273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38533702160421fc5a777d84e162c51816a24426e58139f426e8156fef69d7a7`  
		Last Modified: Wed, 11 May 2022 02:00:34 GMT  
		Size: 4.3 MB (4342926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba195b4bc21ef3724f088897d1aac8e7068de1417a81ee5d80a4b8e0092a038`  
		Last Modified: Wed, 11 May 2022 20:19:47 GMT  
		Size: 13.4 MB (13413735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9ee354c8a8e72692bd91bae5e779d1ca41bd63a0437089cb5e7cb46629d412`  
		Last Modified: Wed, 11 May 2022 20:19:46 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491e40cfb28334046f70a3c70214a052de63e68cb16450865444c462fdd3f51a`  
		Last Modified: Wed, 11 May 2022 20:20:09 GMT  
		Size: 60.7 MB (60741566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2763a3617f4aa0a2e4415718effb031aedcf1a18bc26845c46c9d5e3a1a0cb0`  
		Last Modified: Wed, 11 May 2022 20:20:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249e566eed48ae124d6205ee9f5d5a6342a3e4e89e1273d9abc38cbc3fc1fad4`  
		Last Modified: Wed, 11 May 2022 20:20:01 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:a0ea377d14794289194320acc8cd74433d7bba0275cd30355faa9104b95f3a62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127199217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec513cad13280cdf4cf04a414c22fdd873882f4b348ae97d0ba9b86f7363b556`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 11 May 2022 00:49:08 GMT
ADD file:8949016fba61b18207f5a2309fc974562080c5cc80d1eb82adb35c4fa03f6f05 in / 
# Wed, 11 May 2022 00:49:09 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:29:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:30:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 19:53:03 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 11 May 2022 19:53:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 11 May 2022 19:53:25 GMT
ENV KAPACITOR_VERSION=1.6.4
# Wed, 11 May 2022 19:53:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 11 May 2022 19:53:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 11 May 2022 19:53:31 GMT
EXPOSE 9092
# Wed, 11 May 2022 19:53:32 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 11 May 2022 19:53:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 11 May 2022 19:53:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 19:53:35 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:139065d8f4553df403babda56f830c32aa1f3e57f18d2145a3179468921a4bb8`  
		Last Modified: Wed, 11 May 2022 00:57:26 GMT  
		Size: 43.2 MB (43212478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0acfd1725613d968a54b7fbfe1f70f24b8a0dad792ad3cb28349035f7736fe`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 10.2 MB (10217776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002c314192ef0350d2ac1d1e49b4fddbc49dbcdc609e56e0e2567ee2dd37f0bc`  
		Last Modified: Wed, 11 May 2022 01:39:24 GMT  
		Size: 3.9 MB (3874525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496f27b7f192b22433c9935e31905643e2224453cec24dd8a895fbc0ed124a61`  
		Last Modified: Wed, 11 May 2022 19:53:54 GMT  
		Size: 12.9 MB (12895614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c865c958dbaf4cdc7c502e2fa2e224ecd728970e3f5a6624c291b06f0f0fe724`  
		Last Modified: Wed, 11 May 2022 19:53:53 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9600783cb63804ab90b3c37bfc621d2f9ea15f4bc9aa6cf53f71f7ced8942550`  
		Last Modified: Wed, 11 May 2022 19:54:16 GMT  
		Size: 57.0 MB (56995547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb592b11071788c11c6233720ccfb56da4a2482aefa1388006bbd475bdfefd3`  
		Last Modified: Wed, 11 May 2022 19:54:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdfaac5862ab10711f77f97e571ce72394d53fb4584c1f3ba2a8d767228ea2d`  
		Last Modified: Wed, 11 May 2022 19:54:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
