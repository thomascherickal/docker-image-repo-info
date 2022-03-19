<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.5`](#kapacitor15)
-	[`kapacitor:1.5-alpine`](#kapacitor15-alpine)
-	[`kapacitor:1.5.9`](#kapacitor159)
-	[`kapacitor:1.5.9-alpine`](#kapacitor159-alpine)
-	[`kapacitor:1.6`](#kapacitor16)
-	[`kapacitor:1.6-alpine`](#kapacitor16-alpine)
-	[`kapacitor:1.6.3`](#kapacitor163)
-	[`kapacitor:1.6.3-alpine`](#kapacitor163-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.5`

```console
$ docker pull kapacitor@sha256:bbd0cc31c51b5d683cbbdb76c229fcb2bc1bdd1a4c04a449b0e5536df3624a90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:9ccc0758034c82ba295f354d0c18870881981d7cdefd33e9963e5b4546a198ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111698604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf32b1faec278352fc6d9f26454ece0c14eeb903fc91589676b01a1a763bb27d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 10:15:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 19 Mar 2022 10:15:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 10:15:47 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 19 Mar 2022 10:15:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 19 Mar 2022 10:15:51 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 19 Mar 2022 10:15:51 GMT
EXPOSE 9092
# Sat, 19 Mar 2022 10:15:51 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 19 Mar 2022 10:15:51 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 19 Mar 2022 10:15:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 10:15:51 GMT
CMD ["kapacitord"]
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
	-	`sha256:74bd605f09bf4ce1d7a3f9e141747b1589865a9a501eaeef3f235cc1532b41d3`  
		Last Modified: Sat, 19 Mar 2022 10:16:22 GMT  
		Size: 13.4 MB (13401836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8853406dc402076fb253f0aa43a4408396f9a69a0ac9831ef88a97449c8ecc`  
		Last Modified: Sat, 19 Mar 2022 10:16:20 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a33ed592d3300721c71c79c7129685d4660f8ee71f3763cbe145e1eea598c5`  
		Last Modified: Sat, 19 Mar 2022 10:16:25 GMT  
		Size: 37.2 MB (37219995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404018c383a4d689a6c147f8369f59775a6df7ea614893ed9f31efd7816b35c4`  
		Last Modified: Sat, 19 Mar 2022 10:16:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfa4d1d2a1471edaf8616e3ebcb532fc80480fa0f84508361045aed6d6d3f1a`  
		Last Modified: Sat, 19 Mar 2022 10:16:20 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:00458a44a830e931099de4572619de3e34f453567185bf1223dd0e268b0b7c17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104389100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8af867acf6d272e77ce2af232a0881e457510abfb2da64a45a25b63d44a65381`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:52 GMT
ADD file:32b09ecc1f1473cc68b2fe74354febc64a9530d26aa83549020fed06caa8ba8b in / 
# Tue, 01 Mar 2022 02:08:53 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 09:37:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 09:37:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 03 Mar 2022 00:02:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 03 Mar 2022 00:02:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 03 Mar 2022 00:02:54 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 03 Mar 2022 00:03:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 03 Mar 2022 00:03:04 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 03 Mar 2022 00:03:04 GMT
EXPOSE 9092
# Thu, 03 Mar 2022 00:03:04 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 03 Mar 2022 00:03:05 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 03 Mar 2022 00:03:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Mar 2022 00:03:06 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:57f32f9fdf459a27691c3a29131c270edd06bf53c003de1f42bb0a6ff8824e31`  
		Last Modified: Tue, 01 Mar 2022 02:25:39 GMT  
		Size: 42.1 MB (42116971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e724a8423f66e29c28d1f7eb411c0fc8b5e925a2dba9d9984b26ba548383e5`  
		Last Modified: Tue, 01 Mar 2022 09:59:33 GMT  
		Size: 10.0 MB (9956523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdac683edae6f35034917112b5fe629e9a55d8911f2afdd7746b8dfba6c1638`  
		Last Modified: Tue, 01 Mar 2022 09:59:30 GMT  
		Size: 3.9 MB (3921197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b51f304ced008df762f87103ce9c6f5b76e08fe423b21e946a4b8a7b6b8ec8`  
		Last Modified: Thu, 03 Mar 2022 00:03:36 GMT  
		Size: 13.6 MB (13604428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdca0ebdb8f3db575c3de9c5bc5938194e1324ecffa0545c2b06c35495f780fa`  
		Last Modified: Thu, 03 Mar 2022 00:03:31 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d771c1b1681d0543e3ca75984b8cb7fb7912e6a95af3d968c58c959235cca4`  
		Last Modified: Thu, 03 Mar 2022 00:03:49 GMT  
		Size: 34.8 MB (34786674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1bbda531539ff18afe11cdc8b3d07924d66317df7fa86ebcbf8cedf6e34ee0`  
		Last Modified: Thu, 03 Mar 2022 00:03:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee871f65bd4a0902a68461fa115010b1f29017c774dea3f1482ae916fa4a7c65`  
		Last Modified: Thu, 03 Mar 2022 00:03:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:6d483f2dae6a40cb8f93da6da34eb614856c2e5bcbd5aed6b2b4be49c85ba7cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104753430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e333077394f6b5aaacdd1bbbe063b17062c56644d971b94abb0ca0c6fe6236fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:02 GMT
ADD file:eb07f8b0889bb0b4499fbba08599cdf04f3efaafdec453e96fa4175723f4fec1 in / 
# Thu, 17 Mar 2022 03:24:03 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:22:58 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 19 Mar 2022 04:23:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 04:23:48 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 19 Mar 2022 04:23:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 19 Mar 2022 04:23:54 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 19 Mar 2022 04:23:54 GMT
EXPOSE 9092
# Sat, 19 Mar 2022 04:23:55 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 19 Mar 2022 04:23:57 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 19 Mar 2022 04:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:23:58 GMT
CMD ["kapacitord"]
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
	-	`sha256:2dc70972149614573a1d84f649d3fde352f56f60b73996afb764a1f64194341a`  
		Last Modified: Sat, 19 Mar 2022 04:24:35 GMT  
		Size: 12.9 MB (12884209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fed60d2511addc2b808917019f6a27229f034177c2d2e80eeffadea9eeada`  
		Last Modified: Sat, 19 Mar 2022 04:24:34 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f440f8a241ded5ba5e8a594fd0b503102c085e7702e3a114f7872ba1ef92b262`  
		Last Modified: Sat, 19 Mar 2022 04:24:39 GMT  
		Size: 34.6 MB (34560727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a747bf761a3186c9a5a03ec69ea5100e6a03a8d9a1e4154b94b3a45c433d87`  
		Last Modified: Sat, 19 Mar 2022 04:24:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe8fc86f9aed45fa1defd146113d2dc5d07c65afd1f90f387630698f1d573ce`  
		Last Modified: Sat, 19 Mar 2022 04:24:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:e5d94ed98b1029cba0ea9b5b70ea8997f488932fee6ce116130f9bd653096814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:5070bc0ef5a7915cfff2b4c3d2e4570c9bd8976ee3c3a04e22333040fef7c4bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22629516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c91b266aeca6aa86751ee3a5842f11095fc77996d737130e21f56fc0eaf362bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Mar 2022 18:05:43 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Mar 2022 18:05:44 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 17 Mar 2022 18:06:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Mar 2022 18:06:16 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 17 Mar 2022 18:06:16 GMT
EXPOSE 9092
# Thu, 17 Mar 2022 18:06:16 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 17 Mar 2022 18:06:16 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 17 Mar 2022 18:06:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 18:06:17 GMT
CMD ["kapacitord"]
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
	-	`sha256:85eb6277290b589d592446e2f538670a432e8a6e60772ee08f89a2055bef71ec`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 271.7 KB (271670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eb17274894983a9cf1c86dd872773ba3b097a405c808fcc653754ff50e628f`  
		Last Modified: Thu, 17 Mar 2022 18:07:17 GMT  
		Size: 19.5 MB (19541044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada19f7011baae255470ce7e1a4400498e6f8773313e6b880278572cd486901a`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6242d1cb98d91d428ce29cc1a2cc7663f3e19980edb8ed4c2e7584cdbfe70f11`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9`

```console
$ docker pull kapacitor@sha256:bbd0cc31c51b5d683cbbdb76c229fcb2bc1bdd1a4c04a449b0e5536df3624a90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.9` - linux; amd64

```console
$ docker pull kapacitor@sha256:9ccc0758034c82ba295f354d0c18870881981d7cdefd33e9963e5b4546a198ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111698604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf32b1faec278352fc6d9f26454ece0c14eeb903fc91589676b01a1a763bb27d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 10:15:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 19 Mar 2022 10:15:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 10:15:47 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 19 Mar 2022 10:15:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 19 Mar 2022 10:15:51 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 19 Mar 2022 10:15:51 GMT
EXPOSE 9092
# Sat, 19 Mar 2022 10:15:51 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 19 Mar 2022 10:15:51 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 19 Mar 2022 10:15:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 10:15:51 GMT
CMD ["kapacitord"]
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
	-	`sha256:74bd605f09bf4ce1d7a3f9e141747b1589865a9a501eaeef3f235cc1532b41d3`  
		Last Modified: Sat, 19 Mar 2022 10:16:22 GMT  
		Size: 13.4 MB (13401836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8853406dc402076fb253f0aa43a4408396f9a69a0ac9831ef88a97449c8ecc`  
		Last Modified: Sat, 19 Mar 2022 10:16:20 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a33ed592d3300721c71c79c7129685d4660f8ee71f3763cbe145e1eea598c5`  
		Last Modified: Sat, 19 Mar 2022 10:16:25 GMT  
		Size: 37.2 MB (37219995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404018c383a4d689a6c147f8369f59775a6df7ea614893ed9f31efd7816b35c4`  
		Last Modified: Sat, 19 Mar 2022 10:16:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfa4d1d2a1471edaf8616e3ebcb532fc80480fa0f84508361045aed6d6d3f1a`  
		Last Modified: Sat, 19 Mar 2022 10:16:20 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:00458a44a830e931099de4572619de3e34f453567185bf1223dd0e268b0b7c17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104389100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8af867acf6d272e77ce2af232a0881e457510abfb2da64a45a25b63d44a65381`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:52 GMT
ADD file:32b09ecc1f1473cc68b2fe74354febc64a9530d26aa83549020fed06caa8ba8b in / 
# Tue, 01 Mar 2022 02:08:53 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 09:37:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 09:37:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 03 Mar 2022 00:02:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 03 Mar 2022 00:02:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 03 Mar 2022 00:02:54 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 03 Mar 2022 00:03:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 03 Mar 2022 00:03:04 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 03 Mar 2022 00:03:04 GMT
EXPOSE 9092
# Thu, 03 Mar 2022 00:03:04 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 03 Mar 2022 00:03:05 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 03 Mar 2022 00:03:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 03 Mar 2022 00:03:06 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:57f32f9fdf459a27691c3a29131c270edd06bf53c003de1f42bb0a6ff8824e31`  
		Last Modified: Tue, 01 Mar 2022 02:25:39 GMT  
		Size: 42.1 MB (42116971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e724a8423f66e29c28d1f7eb411c0fc8b5e925a2dba9d9984b26ba548383e5`  
		Last Modified: Tue, 01 Mar 2022 09:59:33 GMT  
		Size: 10.0 MB (9956523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdac683edae6f35034917112b5fe629e9a55d8911f2afdd7746b8dfba6c1638`  
		Last Modified: Tue, 01 Mar 2022 09:59:30 GMT  
		Size: 3.9 MB (3921197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b51f304ced008df762f87103ce9c6f5b76e08fe423b21e946a4b8a7b6b8ec8`  
		Last Modified: Thu, 03 Mar 2022 00:03:36 GMT  
		Size: 13.6 MB (13604428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdca0ebdb8f3db575c3de9c5bc5938194e1324ecffa0545c2b06c35495f780fa`  
		Last Modified: Thu, 03 Mar 2022 00:03:31 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d771c1b1681d0543e3ca75984b8cb7fb7912e6a95af3d968c58c959235cca4`  
		Last Modified: Thu, 03 Mar 2022 00:03:49 GMT  
		Size: 34.8 MB (34786674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1bbda531539ff18afe11cdc8b3d07924d66317df7fa86ebcbf8cedf6e34ee0`  
		Last Modified: Thu, 03 Mar 2022 00:03:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee871f65bd4a0902a68461fa115010b1f29017c774dea3f1482ae916fa4a7c65`  
		Last Modified: Thu, 03 Mar 2022 00:03:31 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:6d483f2dae6a40cb8f93da6da34eb614856c2e5bcbd5aed6b2b4be49c85ba7cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104753430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e333077394f6b5aaacdd1bbbe063b17062c56644d971b94abb0ca0c6fe6236fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:02 GMT
ADD file:eb07f8b0889bb0b4499fbba08599cdf04f3efaafdec453e96fa4175723f4fec1 in / 
# Thu, 17 Mar 2022 03:24:03 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:22:58 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 19 Mar 2022 04:23:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 04:23:48 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 19 Mar 2022 04:23:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 19 Mar 2022 04:23:54 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 19 Mar 2022 04:23:54 GMT
EXPOSE 9092
# Sat, 19 Mar 2022 04:23:55 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 19 Mar 2022 04:23:57 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 19 Mar 2022 04:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:23:58 GMT
CMD ["kapacitord"]
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
	-	`sha256:2dc70972149614573a1d84f649d3fde352f56f60b73996afb764a1f64194341a`  
		Last Modified: Sat, 19 Mar 2022 04:24:35 GMT  
		Size: 12.9 MB (12884209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fed60d2511addc2b808917019f6a27229f034177c2d2e80eeffadea9eeada`  
		Last Modified: Sat, 19 Mar 2022 04:24:34 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f440f8a241ded5ba5e8a594fd0b503102c085e7702e3a114f7872ba1ef92b262`  
		Last Modified: Sat, 19 Mar 2022 04:24:39 GMT  
		Size: 34.6 MB (34560727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a747bf761a3186c9a5a03ec69ea5100e6a03a8d9a1e4154b94b3a45c433d87`  
		Last Modified: Sat, 19 Mar 2022 04:24:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe8fc86f9aed45fa1defd146113d2dc5d07c65afd1f90f387630698f1d573ce`  
		Last Modified: Sat, 19 Mar 2022 04:24:34 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9-alpine`

```console
$ docker pull kapacitor@sha256:e5d94ed98b1029cba0ea9b5b70ea8997f488932fee6ce116130f9bd653096814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5.9-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:5070bc0ef5a7915cfff2b4c3d2e4570c9bd8976ee3c3a04e22333040fef7c4bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22629516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c91b266aeca6aa86751ee3a5842f11095fc77996d737130e21f56fc0eaf362bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Mar 2022 18:05:43 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Mar 2022 18:05:44 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 17 Mar 2022 18:06:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Mar 2022 18:06:16 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 17 Mar 2022 18:06:16 GMT
EXPOSE 9092
# Thu, 17 Mar 2022 18:06:16 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 17 Mar 2022 18:06:16 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 17 Mar 2022 18:06:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 18:06:17 GMT
CMD ["kapacitord"]
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
	-	`sha256:85eb6277290b589d592446e2f538670a432e8a6e60772ee08f89a2055bef71ec`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 271.7 KB (271670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eb17274894983a9cf1c86dd872773ba3b097a405c808fcc653754ff50e628f`  
		Last Modified: Thu, 17 Mar 2022 18:07:17 GMT  
		Size: 19.5 MB (19541044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada19f7011baae255470ce7e1a4400498e6f8773313e6b880278572cd486901a`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6242d1cb98d91d428ce29cc1a2cc7663f3e19980edb8ed4c2e7584cdbfe70f11`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6`

```console
$ docker pull kapacitor@sha256:7232f6388a4d4175ee6bcd147999035abddc62049df9cbb74504a3e0b8483018
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:bb7bc0e600d9b2dc0cb4d1a7f3790cc5e2a37218a9f87fe8619f27e22358f572
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132904781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1306253418f5da002766b6a10a490f4dd3cc535e23f1bd5b93ce248ced8b9c6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 10:15:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 19 Mar 2022 10:15:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 10:15:55 GMT
ENV KAPACITOR_VERSION=1.6.3
# Sat, 19 Mar 2022 10:15:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 19 Mar 2022 10:16:00 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 19 Mar 2022 10:16:00 GMT
EXPOSE 9092
# Sat, 19 Mar 2022 10:16:00 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 19 Mar 2022 10:16:00 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 19 Mar 2022 10:16:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 10:16:00 GMT
CMD ["kapacitord"]
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
	-	`sha256:74bd605f09bf4ce1d7a3f9e141747b1589865a9a501eaeef3f235cc1532b41d3`  
		Last Modified: Sat, 19 Mar 2022 10:16:22 GMT  
		Size: 13.4 MB (13401836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8853406dc402076fb253f0aa43a4408396f9a69a0ac9831ef88a97449c8ecc`  
		Last Modified: Sat, 19 Mar 2022 10:16:20 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07913ffef6ec1b3a316aeb92010b581cf41ad4453164b07aaaebdc75145a3d97`  
		Last Modified: Sat, 19 Mar 2022 10:16:45 GMT  
		Size: 58.4 MB (58426174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6ca9869384970dcd334de34c117ab3cebba6674bd31e425c30daf3e6c1f1a1`  
		Last Modified: Sat, 19 Mar 2022 10:16:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdb05d868f6d1ccdbf4eeb81a4eb1502991f6fbb065c684c505a8e21286b84`  
		Last Modified: Sat, 19 Mar 2022 10:16:36 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:eba6e3c4a8cbbb5366bade71e48e75b945fd44773461183a2bd35363e49fd72e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124689773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10924d29fe99675f32ac28d86d81c663a8c3b9fe72dc9cae92b30e86f3f508d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:02 GMT
ADD file:eb07f8b0889bb0b4499fbba08599cdf04f3efaafdec453e96fa4175723f4fec1 in / 
# Thu, 17 Mar 2022 03:24:03 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:22:58 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 19 Mar 2022 04:23:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 04:24:06 GMT
ENV KAPACITOR_VERSION=1.6.3
# Sat, 19 Mar 2022 04:24:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 19 Mar 2022 04:24:13 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 19 Mar 2022 04:24:13 GMT
EXPOSE 9092
# Sat, 19 Mar 2022 04:24:14 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 19 Mar 2022 04:24:16 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 19 Mar 2022 04:24:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:24:17 GMT
CMD ["kapacitord"]
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
	-	`sha256:2dc70972149614573a1d84f649d3fde352f56f60b73996afb764a1f64194341a`  
		Last Modified: Sat, 19 Mar 2022 04:24:35 GMT  
		Size: 12.9 MB (12884209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fed60d2511addc2b808917019f6a27229f034177c2d2e80eeffadea9eeada`  
		Last Modified: Sat, 19 Mar 2022 04:24:34 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4905364defcb7c7fa74bcef0eaf2ac823038c3922a81c6c8b97dbe2be772c3`  
		Last Modified: Sat, 19 Mar 2022 04:24:57 GMT  
		Size: 54.5 MB (54497071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efbef128d899037e17f8c416f683e9dab5167a4919b66466898b5966eb3b05c`  
		Last Modified: Sat, 19 Mar 2022 04:24:50 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c49999de587fb482dc6e1918784e4a00af0f14a7ebc880c113242262f6f884`  
		Last Modified: Sat, 19 Mar 2022 04:24:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6-alpine`

```console
$ docker pull kapacitor@sha256:9d1fea13f74037a873977f35976edc7f524287c85ee2ca78798443311d8e1794
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:7b80b18e0b03667ed5646cbb8f99ac28757a4f4740a2dc65d3b7d53f3e4e5b61
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61448749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deab38f6e54c02a09af803e498e85900c59830648fc96707b475abc2e857902c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Mar 2022 18:05:43 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Mar 2022 18:06:24 GMT
ENV KAPACITOR_VERSION=1.6.3
# Thu, 17 Mar 2022 18:06:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Mar 2022 18:06:53 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 17 Mar 2022 18:06:53 GMT
EXPOSE 9092
# Thu, 17 Mar 2022 18:06:53 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 17 Mar 2022 18:06:53 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 17 Mar 2022 18:06:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 18:06:53 GMT
CMD ["kapacitord"]
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
	-	`sha256:85eb6277290b589d592446e2f538670a432e8a6e60772ee08f89a2055bef71ec`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 271.7 KB (271670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4ad12656fe460f674ab7f5ec540772003d0372d5fd248843987826b0977f2f`  
		Last Modified: Thu, 17 Mar 2022 18:07:36 GMT  
		Size: 58.4 MB (58360302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641a70ee4993f9c1c1c87380e01bb51c766fdcfbb98fd0f4bedefdacd566b962`  
		Last Modified: Thu, 17 Mar 2022 18:07:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb68c806ef27ef0b5cf3bdbba4fa0c5d9ec667945ee6da1ba24571ab50e7be3`  
		Last Modified: Thu, 17 Mar 2022 18:07:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.3`

```console
$ docker pull kapacitor@sha256:7232f6388a4d4175ee6bcd147999035abddc62049df9cbb74504a3e0b8483018
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6.3` - linux; amd64

```console
$ docker pull kapacitor@sha256:bb7bc0e600d9b2dc0cb4d1a7f3790cc5e2a37218a9f87fe8619f27e22358f572
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132904781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1306253418f5da002766b6a10a490f4dd3cc535e23f1bd5b93ce248ced8b9c6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 10:15:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 19 Mar 2022 10:15:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 10:15:55 GMT
ENV KAPACITOR_VERSION=1.6.3
# Sat, 19 Mar 2022 10:15:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 19 Mar 2022 10:16:00 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 19 Mar 2022 10:16:00 GMT
EXPOSE 9092
# Sat, 19 Mar 2022 10:16:00 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 19 Mar 2022 10:16:00 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 19 Mar 2022 10:16:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 10:16:00 GMT
CMD ["kapacitord"]
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
	-	`sha256:74bd605f09bf4ce1d7a3f9e141747b1589865a9a501eaeef3f235cc1532b41d3`  
		Last Modified: Sat, 19 Mar 2022 10:16:22 GMT  
		Size: 13.4 MB (13401836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8853406dc402076fb253f0aa43a4408396f9a69a0ac9831ef88a97449c8ecc`  
		Last Modified: Sat, 19 Mar 2022 10:16:20 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07913ffef6ec1b3a316aeb92010b581cf41ad4453164b07aaaebdc75145a3d97`  
		Last Modified: Sat, 19 Mar 2022 10:16:45 GMT  
		Size: 58.4 MB (58426174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6ca9869384970dcd334de34c117ab3cebba6674bd31e425c30daf3e6c1f1a1`  
		Last Modified: Sat, 19 Mar 2022 10:16:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdb05d868f6d1ccdbf4eeb81a4eb1502991f6fbb065c684c505a8e21286b84`  
		Last Modified: Sat, 19 Mar 2022 10:16:36 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6.3` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:eba6e3c4a8cbbb5366bade71e48e75b945fd44773461183a2bd35363e49fd72e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124689773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10924d29fe99675f32ac28d86d81c663a8c3b9fe72dc9cae92b30e86f3f508d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:02 GMT
ADD file:eb07f8b0889bb0b4499fbba08599cdf04f3efaafdec453e96fa4175723f4fec1 in / 
# Thu, 17 Mar 2022 03:24:03 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:22:58 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 19 Mar 2022 04:23:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 04:24:06 GMT
ENV KAPACITOR_VERSION=1.6.3
# Sat, 19 Mar 2022 04:24:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 19 Mar 2022 04:24:13 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 19 Mar 2022 04:24:13 GMT
EXPOSE 9092
# Sat, 19 Mar 2022 04:24:14 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 19 Mar 2022 04:24:16 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 19 Mar 2022 04:24:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:24:17 GMT
CMD ["kapacitord"]
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
	-	`sha256:2dc70972149614573a1d84f649d3fde352f56f60b73996afb764a1f64194341a`  
		Last Modified: Sat, 19 Mar 2022 04:24:35 GMT  
		Size: 12.9 MB (12884209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fed60d2511addc2b808917019f6a27229f034177c2d2e80eeffadea9eeada`  
		Last Modified: Sat, 19 Mar 2022 04:24:34 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4905364defcb7c7fa74bcef0eaf2ac823038c3922a81c6c8b97dbe2be772c3`  
		Last Modified: Sat, 19 Mar 2022 04:24:57 GMT  
		Size: 54.5 MB (54497071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efbef128d899037e17f8c416f683e9dab5167a4919b66466898b5966eb3b05c`  
		Last Modified: Sat, 19 Mar 2022 04:24:50 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c49999de587fb482dc6e1918784e4a00af0f14a7ebc880c113242262f6f884`  
		Last Modified: Sat, 19 Mar 2022 04:24:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.3-alpine`

```console
$ docker pull kapacitor@sha256:9d1fea13f74037a873977f35976edc7f524287c85ee2ca78798443311d8e1794
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6.3-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:7b80b18e0b03667ed5646cbb8f99ac28757a4f4740a2dc65d3b7d53f3e4e5b61
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61448749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deab38f6e54c02a09af803e498e85900c59830648fc96707b475abc2e857902c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Mar 2022 18:05:43 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Mar 2022 18:06:24 GMT
ENV KAPACITOR_VERSION=1.6.3
# Thu, 17 Mar 2022 18:06:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Mar 2022 18:06:53 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 17 Mar 2022 18:06:53 GMT
EXPOSE 9092
# Thu, 17 Mar 2022 18:06:53 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 17 Mar 2022 18:06:53 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 17 Mar 2022 18:06:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 18:06:53 GMT
CMD ["kapacitord"]
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
	-	`sha256:85eb6277290b589d592446e2f538670a432e8a6e60772ee08f89a2055bef71ec`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 271.7 KB (271670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4ad12656fe460f674ab7f5ec540772003d0372d5fd248843987826b0977f2f`  
		Last Modified: Thu, 17 Mar 2022 18:07:36 GMT  
		Size: 58.4 MB (58360302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641a70ee4993f9c1c1c87380e01bb51c766fdcfbb98fd0f4bedefdacd566b962`  
		Last Modified: Thu, 17 Mar 2022 18:07:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb68c806ef27ef0b5cf3bdbba4fa0c5d9ec667945ee6da1ba24571ab50e7be3`  
		Last Modified: Thu, 17 Mar 2022 18:07:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:9d1fea13f74037a873977f35976edc7f524287c85ee2ca78798443311d8e1794
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:7b80b18e0b03667ed5646cbb8f99ac28757a4f4740a2dc65d3b7d53f3e4e5b61
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61448749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deab38f6e54c02a09af803e498e85900c59830648fc96707b475abc2e857902c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:05:42 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Mar 2022 18:05:43 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 17 Mar 2022 18:06:24 GMT
ENV KAPACITOR_VERSION=1.6.3
# Thu, 17 Mar 2022 18:06:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Mar 2022 18:06:53 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 17 Mar 2022 18:06:53 GMT
EXPOSE 9092
# Thu, 17 Mar 2022 18:06:53 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 17 Mar 2022 18:06:53 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 17 Mar 2022 18:06:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 18:06:53 GMT
CMD ["kapacitord"]
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
	-	`sha256:85eb6277290b589d592446e2f538670a432e8a6e60772ee08f89a2055bef71ec`  
		Last Modified: Thu, 17 Mar 2022 18:07:13 GMT  
		Size: 271.7 KB (271670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4ad12656fe460f674ab7f5ec540772003d0372d5fd248843987826b0977f2f`  
		Last Modified: Thu, 17 Mar 2022 18:07:36 GMT  
		Size: 58.4 MB (58360302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641a70ee4993f9c1c1c87380e01bb51c766fdcfbb98fd0f4bedefdacd566b962`  
		Last Modified: Thu, 17 Mar 2022 18:07:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb68c806ef27ef0b5cf3bdbba4fa0c5d9ec667945ee6da1ba24571ab50e7be3`  
		Last Modified: Thu, 17 Mar 2022 18:07:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:7232f6388a4d4175ee6bcd147999035abddc62049df9cbb74504a3e0b8483018
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:bb7bc0e600d9b2dc0cb4d1a7f3790cc5e2a37218a9f87fe8619f27e22358f572
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132904781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1306253418f5da002766b6a10a490f4dd3cc535e23f1bd5b93ce248ced8b9c6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 10:15:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 19 Mar 2022 10:15:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 10:15:55 GMT
ENV KAPACITOR_VERSION=1.6.3
# Sat, 19 Mar 2022 10:15:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 19 Mar 2022 10:16:00 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 19 Mar 2022 10:16:00 GMT
EXPOSE 9092
# Sat, 19 Mar 2022 10:16:00 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 19 Mar 2022 10:16:00 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 19 Mar 2022 10:16:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 10:16:00 GMT
CMD ["kapacitord"]
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
	-	`sha256:74bd605f09bf4ce1d7a3f9e141747b1589865a9a501eaeef3f235cc1532b41d3`  
		Last Modified: Sat, 19 Mar 2022 10:16:22 GMT  
		Size: 13.4 MB (13401836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8853406dc402076fb253f0aa43a4408396f9a69a0ac9831ef88a97449c8ecc`  
		Last Modified: Sat, 19 Mar 2022 10:16:20 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07913ffef6ec1b3a316aeb92010b581cf41ad4453164b07aaaebdc75145a3d97`  
		Last Modified: Sat, 19 Mar 2022 10:16:45 GMT  
		Size: 58.4 MB (58426174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6ca9869384970dcd334de34c117ab3cebba6674bd31e425c30daf3e6c1f1a1`  
		Last Modified: Sat, 19 Mar 2022 10:16:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdb05d868f6d1ccdbf4eeb81a4eb1502991f6fbb065c684c505a8e21286b84`  
		Last Modified: Sat, 19 Mar 2022 10:16:36 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:eba6e3c4a8cbbb5366bade71e48e75b945fd44773461183a2bd35363e49fd72e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124689773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10924d29fe99675f32ac28d86d81c663a8c3b9fe72dc9cae92b30e86f3f508d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:02 GMT
ADD file:eb07f8b0889bb0b4499fbba08599cdf04f3efaafdec453e96fa4175723f4fec1 in / 
# Thu, 17 Mar 2022 03:24:03 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 04:22:58 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 19 Mar 2022 04:23:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 19 Mar 2022 04:24:06 GMT
ENV KAPACITOR_VERSION=1.6.3
# Sat, 19 Mar 2022 04:24:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 19 Mar 2022 04:24:13 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 19 Mar 2022 04:24:13 GMT
EXPOSE 9092
# Sat, 19 Mar 2022 04:24:14 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 19 Mar 2022 04:24:16 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 19 Mar 2022 04:24:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Mar 2022 04:24:17 GMT
CMD ["kapacitord"]
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
	-	`sha256:2dc70972149614573a1d84f649d3fde352f56f60b73996afb764a1f64194341a`  
		Last Modified: Sat, 19 Mar 2022 04:24:35 GMT  
		Size: 12.9 MB (12884209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7fed60d2511addc2b808917019f6a27229f034177c2d2e80eeffadea9eeada`  
		Last Modified: Sat, 19 Mar 2022 04:24:34 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4905364defcb7c7fa74bcef0eaf2ac823038c3922a81c6c8b97dbe2be772c3`  
		Last Modified: Sat, 19 Mar 2022 04:24:57 GMT  
		Size: 54.5 MB (54497071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efbef128d899037e17f8c416f683e9dab5167a4919b66466898b5966eb3b05c`  
		Last Modified: Sat, 19 Mar 2022 04:24:50 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c49999de587fb482dc6e1918784e4a00af0f14a7ebc880c113242262f6f884`  
		Last Modified: Sat, 19 Mar 2022 04:24:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
