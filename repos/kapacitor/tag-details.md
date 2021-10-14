<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.5`](#kapacitor15)
-	[`kapacitor:1.5-alpine`](#kapacitor15-alpine)
-	[`kapacitor:1.5.9`](#kapacitor159)
-	[`kapacitor:1.5.9-alpine`](#kapacitor159-alpine)
-	[`kapacitor:1.6`](#kapacitor16)
-	[`kapacitor:1.6-alpine`](#kapacitor16-alpine)
-	[`kapacitor:1.6.2`](#kapacitor162)
-	[`kapacitor:1.6.2-alpine`](#kapacitor162-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.5`

```console
$ docker pull kapacitor@sha256:840bc938ff958cc47ebef6cdf53ffe9657fe7eb65e966c7759f9744fe5b7259a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:aa34bf72705a3b15bc8c38a20c0c869b2b939355502001e28aae8726b58075f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111588330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6227dabe40b98bfff74449844ee5142357dc9349d2f95191849b059c43aaa505`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:48:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:48:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 07:11:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 13 Oct 2021 07:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 07:11:37 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 13 Oct 2021 07:11:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 07:11:42 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 13 Oct 2021 07:11:42 GMT
EXPOSE 9092
# Wed, 13 Oct 2021 07:11:42 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 13 Oct 2021 07:11:43 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 13 Oct 2021 07:11:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 07:11:43 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a43d3c11106306de19fd422e9da4a6f9b96de147d92c6213d6dbbc395be81b3`  
		Last Modified: Tue, 12 Oct 2021 15:57:10 GMT  
		Size: 11.3 MB (11301072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243ae34810fbd860a43ecf1a7da887386e7a1155913bf13ed95681c98a1cfa84`  
		Last Modified: Tue, 12 Oct 2021 15:57:08 GMT  
		Size: 4.3 MB (4342414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cd6f91698d25d624ba6891bcf4d34b7ef3fd9327e7d1bbff0e12954876b950`  
		Last Modified: Wed, 13 Oct 2021 07:12:15 GMT  
		Size: 13.3 MB (13342530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02e14e16b5ee4daac6cb07e20f5225f19f591382d3fa089d0c79930178b9b9b`  
		Last Modified: Wed, 13 Oct 2021 07:12:13 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03589196ff1e94fa14a14aaf773b907270d5a285ebc8b8587ef269019af86b1`  
		Last Modified: Wed, 13 Oct 2021 07:12:18 GMT  
		Size: 37.2 MB (37219352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da64d6b31562d1eba37457b40b1f036fc58739238dafa9eeb14e2c98dc48b49`  
		Last Modified: Wed, 13 Oct 2021 07:12:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89778bbf9d2659c924794cd28619323378e78cad283b4c42d700df785eac8125`  
		Last Modified: Wed, 13 Oct 2021 07:12:13 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:4f30ff73691778b06f87716e48a7612df9fb9b31250406f0b475ef1184df4128
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104309675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0be24c1ef4ae8160ff0cff442bc766d3f66f32a483c556e68491b81519b5df5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:34:07 GMT
ADD file:eb5955ccd54a486767e85aeb1c03ffc6d8667b5476d0cf17b892ca407f1c8853 in / 
# Tue, 12 Oct 2021 01:34:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:48:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 Oct 2021 01:57:13 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 14 Oct 2021 01:57:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 14 Oct 2021 01:57:18 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 14 Oct 2021 01:57:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 14 Oct 2021 01:57:28 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 14 Oct 2021 01:57:29 GMT
EXPOSE 9092
# Thu, 14 Oct 2021 01:57:29 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 14 Oct 2021 01:57:30 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 14 Oct 2021 01:57:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 Oct 2021 01:57:31 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:8e9db3616ec4491d75e6c28254ff2376f24900797e7c4cc464f36a0c502b111f`  
		Last Modified: Tue, 12 Oct 2021 01:51:20 GMT  
		Size: 42.1 MB (42119423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdf02e61fe0ab1563ba0431b63fade0e2dc7930d82d8c1a7ec6ee395072fdb3`  
		Last Modified: Tue, 12 Oct 2021 19:06:50 GMT  
		Size: 10.0 MB (9955968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a752ebf54d1b82943abce28e108346c5d28e94fdb8f419cfffea0b639341ce6`  
		Last Modified: Tue, 12 Oct 2021 19:06:46 GMT  
		Size: 3.9 MB (3921159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab2179b52fc97fb3efbeb0074bf4676f0ba0f98eb4e1f5f3b2c6e4163c57c43`  
		Last Modified: Thu, 14 Oct 2021 01:57:58 GMT  
		Size: 13.5 MB (13523159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c120359436ee59ece0abe53eb9ab23ba2fbf5ac40ea152490173dfec89f825e`  
		Last Modified: Thu, 14 Oct 2021 01:57:53 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962cfb92c58a56529d6b0933af4a95db4233844ef7edbc170944a04b2d993022`  
		Last Modified: Thu, 14 Oct 2021 01:58:10 GMT  
		Size: 34.8 MB (34786657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aecc1c6d351affc51cafe14ac438533167e9734fa4bcc429a2726090eacd034`  
		Last Modified: Thu, 14 Oct 2021 01:57:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c23daf6b6dc28efeb623345819c8eab96f949cb5d35936e97d5eac17e1fb1c`  
		Last Modified: Thu, 14 Oct 2021 01:57:53 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:0cd6b17d7c216eeea181207819f47e22bc4eb11a9a713dd68dfa5be44405bc29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.9 MB (104873946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6d46ebabb73ed9d28f7db42d6f63ab0400a496e86a35d3f9fc16d34516a6cb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 21:54:49 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Oct 2021 21:55:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 12 Oct 2021 21:55:02 GMT
ENV KAPACITOR_VERSION=1.5.9
# Tue, 12 Oct 2021 21:55:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Tue, 12 Oct 2021 21:55:08 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 12 Oct 2021 21:55:08 GMT
EXPOSE 9092
# Tue, 12 Oct 2021 21:55:09 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 12 Oct 2021 21:55:11 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 12 Oct 2021 21:55:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 21:55:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6106ce195cfc2ea7282dab1677e8563168fee21f184a937b32a9370944ccc077`  
		Last Modified: Tue, 12 Oct 2021 02:22:54 GMT  
		Size: 10.2 MB (10217927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499bc8ad963810c8e2cef0d22542dfad2339032cf43a8210066a9a817fd6a869`  
		Last Modified: Tue, 12 Oct 2021 02:22:53 GMT  
		Size: 4.1 MB (4096622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42793e78a888c99031cc5e588b1eb4d0b64b64214ac85dbe53b8792f0c1ac8d4`  
		Last Modified: Tue, 12 Oct 2021 21:55:54 GMT  
		Size: 12.8 MB (12819333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4226bc2244600763630c84a3d1beb498757c8261edc34262a1774cdbd72c30`  
		Last Modified: Tue, 12 Oct 2021 21:55:52 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729a236c01e5d7ca8b87ec7dd5d39f947cedabf5556cb081b5b45eca0daf62f8`  
		Last Modified: Tue, 12 Oct 2021 21:55:57 GMT  
		Size: 34.6 MB (34560086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c8e7e34bb8a1213f5a9282bbd7e7d810f47c4814a01ecd0da1ec279e5be6c`  
		Last Modified: Tue, 12 Oct 2021 21:55:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5a5a997363fe193a8f796e2ab856c981c2a1c7bd8e33391ddde394a58d3e11`  
		Last Modified: Tue, 12 Oct 2021 21:55:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:4810111c8b5ca5282097a34087bf96532a51a1cc52da0c89f01f8cf632c2b478
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:51d2fb975938739305d358c02f93b97e8a72c673cda03ae3db533c9289028bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22638136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a01cd92d530d7709eb2701c7d64f5cb0c185f8546e7472d8dc5faf0c655b138`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Sep 2021 18:21:29 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 30 Sep 2021 18:21:29 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 30 Sep 2021 18:21:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 30 Sep 2021 18:21:42 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 30 Sep 2021 18:21:42 GMT
EXPOSE 9092
# Thu, 30 Sep 2021 18:21:42 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 30 Sep 2021 18:21:42 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 30 Sep 2021 18:21:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Sep 2021 18:21:43 GMT
CMD ["kapacitord"]
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
	-	`sha256:35128f89929d86c35c1dfabaaea2552df6e9c25e7ec0d08e798390d47c11a85b`  
		Last Modified: Thu, 30 Sep 2021 18:22:31 GMT  
		Size: 281.5 KB (281501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8941cb4f84e13a3cb29f190a03e180b1b297e0314b3bc1a8796f167dca86c084`  
		Last Modified: Thu, 30 Sep 2021 18:22:35 GMT  
		Size: 19.5 MB (19541561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6ebaa527a1648949550f567922fa16a6cab211eb5a9c1355582bcaaf72d1c7`  
		Last Modified: Thu, 30 Sep 2021 18:22:32 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9be2946e0da2c5c7d6767a931cc7dda146a30557bb2d902c215199d604bb2a9`  
		Last Modified: Thu, 30 Sep 2021 18:22:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9`

```console
$ docker pull kapacitor@sha256:840bc938ff958cc47ebef6cdf53ffe9657fe7eb65e966c7759f9744fe5b7259a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.9` - linux; amd64

```console
$ docker pull kapacitor@sha256:aa34bf72705a3b15bc8c38a20c0c869b2b939355502001e28aae8726b58075f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111588330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6227dabe40b98bfff74449844ee5142357dc9349d2f95191849b059c43aaa505`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:48:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:48:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 07:11:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 13 Oct 2021 07:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 07:11:37 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 13 Oct 2021 07:11:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 07:11:42 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 13 Oct 2021 07:11:42 GMT
EXPOSE 9092
# Wed, 13 Oct 2021 07:11:42 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 13 Oct 2021 07:11:43 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 13 Oct 2021 07:11:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 07:11:43 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a43d3c11106306de19fd422e9da4a6f9b96de147d92c6213d6dbbc395be81b3`  
		Last Modified: Tue, 12 Oct 2021 15:57:10 GMT  
		Size: 11.3 MB (11301072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243ae34810fbd860a43ecf1a7da887386e7a1155913bf13ed95681c98a1cfa84`  
		Last Modified: Tue, 12 Oct 2021 15:57:08 GMT  
		Size: 4.3 MB (4342414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cd6f91698d25d624ba6891bcf4d34b7ef3fd9327e7d1bbff0e12954876b950`  
		Last Modified: Wed, 13 Oct 2021 07:12:15 GMT  
		Size: 13.3 MB (13342530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02e14e16b5ee4daac6cb07e20f5225f19f591382d3fa089d0c79930178b9b9b`  
		Last Modified: Wed, 13 Oct 2021 07:12:13 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03589196ff1e94fa14a14aaf773b907270d5a285ebc8b8587ef269019af86b1`  
		Last Modified: Wed, 13 Oct 2021 07:12:18 GMT  
		Size: 37.2 MB (37219352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da64d6b31562d1eba37457b40b1f036fc58739238dafa9eeb14e2c98dc48b49`  
		Last Modified: Wed, 13 Oct 2021 07:12:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89778bbf9d2659c924794cd28619323378e78cad283b4c42d700df785eac8125`  
		Last Modified: Wed, 13 Oct 2021 07:12:13 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:4f30ff73691778b06f87716e48a7612df9fb9b31250406f0b475ef1184df4128
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104309675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0be24c1ef4ae8160ff0cff442bc766d3f66f32a483c556e68491b81519b5df5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:34:07 GMT
ADD file:eb5955ccd54a486767e85aeb1c03ffc6d8667b5476d0cf17b892ca407f1c8853 in / 
# Tue, 12 Oct 2021 01:34:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:48:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 Oct 2021 01:57:13 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 14 Oct 2021 01:57:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 14 Oct 2021 01:57:18 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 14 Oct 2021 01:57:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 14 Oct 2021 01:57:28 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 14 Oct 2021 01:57:29 GMT
EXPOSE 9092
# Thu, 14 Oct 2021 01:57:29 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 14 Oct 2021 01:57:30 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 14 Oct 2021 01:57:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 Oct 2021 01:57:31 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:8e9db3616ec4491d75e6c28254ff2376f24900797e7c4cc464f36a0c502b111f`  
		Last Modified: Tue, 12 Oct 2021 01:51:20 GMT  
		Size: 42.1 MB (42119423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdf02e61fe0ab1563ba0431b63fade0e2dc7930d82d8c1a7ec6ee395072fdb3`  
		Last Modified: Tue, 12 Oct 2021 19:06:50 GMT  
		Size: 10.0 MB (9955968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a752ebf54d1b82943abce28e108346c5d28e94fdb8f419cfffea0b639341ce6`  
		Last Modified: Tue, 12 Oct 2021 19:06:46 GMT  
		Size: 3.9 MB (3921159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab2179b52fc97fb3efbeb0074bf4676f0ba0f98eb4e1f5f3b2c6e4163c57c43`  
		Last Modified: Thu, 14 Oct 2021 01:57:58 GMT  
		Size: 13.5 MB (13523159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c120359436ee59ece0abe53eb9ab23ba2fbf5ac40ea152490173dfec89f825e`  
		Last Modified: Thu, 14 Oct 2021 01:57:53 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962cfb92c58a56529d6b0933af4a95db4233844ef7edbc170944a04b2d993022`  
		Last Modified: Thu, 14 Oct 2021 01:58:10 GMT  
		Size: 34.8 MB (34786657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aecc1c6d351affc51cafe14ac438533167e9734fa4bcc429a2726090eacd034`  
		Last Modified: Thu, 14 Oct 2021 01:57:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c23daf6b6dc28efeb623345819c8eab96f949cb5d35936e97d5eac17e1fb1c`  
		Last Modified: Thu, 14 Oct 2021 01:57:53 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:0cd6b17d7c216eeea181207819f47e22bc4eb11a9a713dd68dfa5be44405bc29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.9 MB (104873946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6d46ebabb73ed9d28f7db42d6f63ab0400a496e86a35d3f9fc16d34516a6cb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 21:54:49 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Oct 2021 21:55:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 12 Oct 2021 21:55:02 GMT
ENV KAPACITOR_VERSION=1.5.9
# Tue, 12 Oct 2021 21:55:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Tue, 12 Oct 2021 21:55:08 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 12 Oct 2021 21:55:08 GMT
EXPOSE 9092
# Tue, 12 Oct 2021 21:55:09 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 12 Oct 2021 21:55:11 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 12 Oct 2021 21:55:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 21:55:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6106ce195cfc2ea7282dab1677e8563168fee21f184a937b32a9370944ccc077`  
		Last Modified: Tue, 12 Oct 2021 02:22:54 GMT  
		Size: 10.2 MB (10217927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499bc8ad963810c8e2cef0d22542dfad2339032cf43a8210066a9a817fd6a869`  
		Last Modified: Tue, 12 Oct 2021 02:22:53 GMT  
		Size: 4.1 MB (4096622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42793e78a888c99031cc5e588b1eb4d0b64b64214ac85dbe53b8792f0c1ac8d4`  
		Last Modified: Tue, 12 Oct 2021 21:55:54 GMT  
		Size: 12.8 MB (12819333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4226bc2244600763630c84a3d1beb498757c8261edc34262a1774cdbd72c30`  
		Last Modified: Tue, 12 Oct 2021 21:55:52 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729a236c01e5d7ca8b87ec7dd5d39f947cedabf5556cb081b5b45eca0daf62f8`  
		Last Modified: Tue, 12 Oct 2021 21:55:57 GMT  
		Size: 34.6 MB (34560086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c8e7e34bb8a1213f5a9282bbd7e7d810f47c4814a01ecd0da1ec279e5be6c`  
		Last Modified: Tue, 12 Oct 2021 21:55:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5a5a997363fe193a8f796e2ab856c981c2a1c7bd8e33391ddde394a58d3e11`  
		Last Modified: Tue, 12 Oct 2021 21:55:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9-alpine`

```console
$ docker pull kapacitor@sha256:4810111c8b5ca5282097a34087bf96532a51a1cc52da0c89f01f8cf632c2b478
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5.9-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:51d2fb975938739305d358c02f93b97e8a72c673cda03ae3db533c9289028bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22638136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a01cd92d530d7709eb2701c7d64f5cb0c185f8546e7472d8dc5faf0c655b138`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Sep 2021 18:21:29 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 30 Sep 2021 18:21:29 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 30 Sep 2021 18:21:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 30 Sep 2021 18:21:42 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 30 Sep 2021 18:21:42 GMT
EXPOSE 9092
# Thu, 30 Sep 2021 18:21:42 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 30 Sep 2021 18:21:42 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 30 Sep 2021 18:21:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Sep 2021 18:21:43 GMT
CMD ["kapacitord"]
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
	-	`sha256:35128f89929d86c35c1dfabaaea2552df6e9c25e7ec0d08e798390d47c11a85b`  
		Last Modified: Thu, 30 Sep 2021 18:22:31 GMT  
		Size: 281.5 KB (281501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8941cb4f84e13a3cb29f190a03e180b1b297e0314b3bc1a8796f167dca86c084`  
		Last Modified: Thu, 30 Sep 2021 18:22:35 GMT  
		Size: 19.5 MB (19541561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6ebaa527a1648949550f567922fa16a6cab211eb5a9c1355582bcaaf72d1c7`  
		Last Modified: Thu, 30 Sep 2021 18:22:32 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9be2946e0da2c5c7d6767a931cc7dda146a30557bb2d902c215199d604bb2a9`  
		Last Modified: Thu, 30 Sep 2021 18:22:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6`

```console
$ docker pull kapacitor@sha256:b5eac70b636530cc0f3f99709c809b9988cbcb0cb8438e0665a286beda5188bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:73e5db8a9ba89f21eaddf45adc67abdb216f872955c751579da075f33f13ade2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132771298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c37a95bcd945e8964ceaba40abab6723719f7d73d4f80b86e29489eb7b01948`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:48:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:48:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 07:11:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 13 Oct 2021 07:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 07:11:49 GMT
ENV KAPACITOR_VERSION=1.6.2
# Wed, 13 Oct 2021 07:11:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 07:11:55 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 13 Oct 2021 07:11:56 GMT
EXPOSE 9092
# Wed, 13 Oct 2021 07:11:56 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 13 Oct 2021 07:11:56 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 13 Oct 2021 07:11:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 07:11:56 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a43d3c11106306de19fd422e9da4a6f9b96de147d92c6213d6dbbc395be81b3`  
		Last Modified: Tue, 12 Oct 2021 15:57:10 GMT  
		Size: 11.3 MB (11301072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243ae34810fbd860a43ecf1a7da887386e7a1155913bf13ed95681c98a1cfa84`  
		Last Modified: Tue, 12 Oct 2021 15:57:08 GMT  
		Size: 4.3 MB (4342414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cd6f91698d25d624ba6891bcf4d34b7ef3fd9327e7d1bbff0e12954876b950`  
		Last Modified: Wed, 13 Oct 2021 07:12:15 GMT  
		Size: 13.3 MB (13342530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02e14e16b5ee4daac6cb07e20f5225f19f591382d3fa089d0c79930178b9b9b`  
		Last Modified: Wed, 13 Oct 2021 07:12:13 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf4f4dd0e5913ab75ee96d57c02a65812f5552c4cdcb1fc499c56527086daad`  
		Last Modified: Wed, 13 Oct 2021 07:12:37 GMT  
		Size: 58.4 MB (58402322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c0ab65ab94bc2ad7c04ac554bab37baa6159ed5218223b8edf65d7b38838ce`  
		Last Modified: Wed, 13 Oct 2021 07:12:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878218f4ee01430afab7fd4e20ef3817a87ef871f7d57c98cbe8ef0bc3cd230d`  
		Last Modified: Wed, 13 Oct 2021 07:12:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:163a91e45a6984f37649b4a47e20f83746fbca6e57052f7da89434c124807fc0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124751312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235dfcb8886839547ea238cbe685a6aa8369bf27c67b221806ac982a9e42b981`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 21:54:49 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Oct 2021 21:55:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 12 Oct 2021 21:55:21 GMT
ENV KAPACITOR_VERSION=1.6.2
# Tue, 12 Oct 2021 21:55:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Tue, 12 Oct 2021 21:55:28 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 12 Oct 2021 21:55:28 GMT
EXPOSE 9092
# Tue, 12 Oct 2021 21:55:29 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 12 Oct 2021 21:55:31 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 12 Oct 2021 21:55:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 21:55:32 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6106ce195cfc2ea7282dab1677e8563168fee21f184a937b32a9370944ccc077`  
		Last Modified: Tue, 12 Oct 2021 02:22:54 GMT  
		Size: 10.2 MB (10217927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499bc8ad963810c8e2cef0d22542dfad2339032cf43a8210066a9a817fd6a869`  
		Last Modified: Tue, 12 Oct 2021 02:22:53 GMT  
		Size: 4.1 MB (4096622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42793e78a888c99031cc5e588b1eb4d0b64b64214ac85dbe53b8792f0c1ac8d4`  
		Last Modified: Tue, 12 Oct 2021 21:55:54 GMT  
		Size: 12.8 MB (12819333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4226bc2244600763630c84a3d1beb498757c8261edc34262a1774cdbd72c30`  
		Last Modified: Tue, 12 Oct 2021 21:55:52 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc47eaed34d6c70bbbb28128e0264d650bcbeb1db500f9f87a3714ef19a0ce`  
		Last Modified: Tue, 12 Oct 2021 21:56:15 GMT  
		Size: 54.4 MB (54437453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48f4da4749dc7ff39b49ef4303dc8dbc04b51c8eb8308da2f909df304fbbfd5`  
		Last Modified: Tue, 12 Oct 2021 21:56:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39c642dc9fb58c271b9882a6a3bd66f2d0036317435744b6d7151aa1a021ebb`  
		Last Modified: Tue, 12 Oct 2021 21:56:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6-alpine`

```console
$ docker pull kapacitor@sha256:08149a688dddb6174e8a14ce34d3dae52b05b9079b0119e14822f67f057fe283
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:63a731cc73e4d105cc09626f2d02c74b8dee108ef4faa655834b21f2570e2b79
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61428116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34af74ca321f9f0f15370d8abd1235fd5e4ba6517714f413156e0b503d83a698`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Sep 2021 18:21:29 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 30 Sep 2021 18:21:58 GMT
ENV KAPACITOR_VERSION=1.6.2
# Thu, 07 Oct 2021 19:56:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 07 Oct 2021 19:56:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 07 Oct 2021 19:56:31 GMT
EXPOSE 9092
# Thu, 07 Oct 2021 19:56:32 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 07 Oct 2021 19:56:32 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 07 Oct 2021 19:56:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:56:32 GMT
CMD ["kapacitord"]
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
	-	`sha256:35128f89929d86c35c1dfabaaea2552df6e9c25e7ec0d08e798390d47c11a85b`  
		Last Modified: Thu, 30 Sep 2021 18:22:31 GMT  
		Size: 281.5 KB (281501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516aad966cd4cc065db1821d5d1cbc26bb9b3a8c8ace7d5b4ba37b8d118056e3`  
		Last Modified: Thu, 07 Oct 2021 19:56:59 GMT  
		Size: 58.3 MB (58331562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744988bc2e03a02b20ef5c3ed06d2535e5cfbdac463502680dbe74af369f37f6`  
		Last Modified: Thu, 07 Oct 2021 19:56:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9b0b48185ad7f8e4ea4c843c0358ae53fed5bc0afc2500e2915aa0e00eb4bf`  
		Last Modified: Thu, 07 Oct 2021 19:56:52 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.2`

```console
$ docker pull kapacitor@sha256:b5eac70b636530cc0f3f99709c809b9988cbcb0cb8438e0665a286beda5188bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6.2` - linux; amd64

```console
$ docker pull kapacitor@sha256:73e5db8a9ba89f21eaddf45adc67abdb216f872955c751579da075f33f13ade2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132771298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c37a95bcd945e8964ceaba40abab6723719f7d73d4f80b86e29489eb7b01948`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:48:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:48:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 07:11:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 13 Oct 2021 07:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 07:11:49 GMT
ENV KAPACITOR_VERSION=1.6.2
# Wed, 13 Oct 2021 07:11:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 07:11:55 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 13 Oct 2021 07:11:56 GMT
EXPOSE 9092
# Wed, 13 Oct 2021 07:11:56 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 13 Oct 2021 07:11:56 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 13 Oct 2021 07:11:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 07:11:56 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a43d3c11106306de19fd422e9da4a6f9b96de147d92c6213d6dbbc395be81b3`  
		Last Modified: Tue, 12 Oct 2021 15:57:10 GMT  
		Size: 11.3 MB (11301072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243ae34810fbd860a43ecf1a7da887386e7a1155913bf13ed95681c98a1cfa84`  
		Last Modified: Tue, 12 Oct 2021 15:57:08 GMT  
		Size: 4.3 MB (4342414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cd6f91698d25d624ba6891bcf4d34b7ef3fd9327e7d1bbff0e12954876b950`  
		Last Modified: Wed, 13 Oct 2021 07:12:15 GMT  
		Size: 13.3 MB (13342530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02e14e16b5ee4daac6cb07e20f5225f19f591382d3fa089d0c79930178b9b9b`  
		Last Modified: Wed, 13 Oct 2021 07:12:13 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf4f4dd0e5913ab75ee96d57c02a65812f5552c4cdcb1fc499c56527086daad`  
		Last Modified: Wed, 13 Oct 2021 07:12:37 GMT  
		Size: 58.4 MB (58402322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c0ab65ab94bc2ad7c04ac554bab37baa6159ed5218223b8edf65d7b38838ce`  
		Last Modified: Wed, 13 Oct 2021 07:12:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878218f4ee01430afab7fd4e20ef3817a87ef871f7d57c98cbe8ef0bc3cd230d`  
		Last Modified: Wed, 13 Oct 2021 07:12:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6.2` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:163a91e45a6984f37649b4a47e20f83746fbca6e57052f7da89434c124807fc0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124751312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235dfcb8886839547ea238cbe685a6aa8369bf27c67b221806ac982a9e42b981`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 21:54:49 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Oct 2021 21:55:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 12 Oct 2021 21:55:21 GMT
ENV KAPACITOR_VERSION=1.6.2
# Tue, 12 Oct 2021 21:55:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Tue, 12 Oct 2021 21:55:28 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 12 Oct 2021 21:55:28 GMT
EXPOSE 9092
# Tue, 12 Oct 2021 21:55:29 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 12 Oct 2021 21:55:31 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 12 Oct 2021 21:55:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 21:55:32 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6106ce195cfc2ea7282dab1677e8563168fee21f184a937b32a9370944ccc077`  
		Last Modified: Tue, 12 Oct 2021 02:22:54 GMT  
		Size: 10.2 MB (10217927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499bc8ad963810c8e2cef0d22542dfad2339032cf43a8210066a9a817fd6a869`  
		Last Modified: Tue, 12 Oct 2021 02:22:53 GMT  
		Size: 4.1 MB (4096622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42793e78a888c99031cc5e588b1eb4d0b64b64214ac85dbe53b8792f0c1ac8d4`  
		Last Modified: Tue, 12 Oct 2021 21:55:54 GMT  
		Size: 12.8 MB (12819333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4226bc2244600763630c84a3d1beb498757c8261edc34262a1774cdbd72c30`  
		Last Modified: Tue, 12 Oct 2021 21:55:52 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc47eaed34d6c70bbbb28128e0264d650bcbeb1db500f9f87a3714ef19a0ce`  
		Last Modified: Tue, 12 Oct 2021 21:56:15 GMT  
		Size: 54.4 MB (54437453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48f4da4749dc7ff39b49ef4303dc8dbc04b51c8eb8308da2f909df304fbbfd5`  
		Last Modified: Tue, 12 Oct 2021 21:56:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39c642dc9fb58c271b9882a6a3bd66f2d0036317435744b6d7151aa1a021ebb`  
		Last Modified: Tue, 12 Oct 2021 21:56:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.2-alpine`

```console
$ docker pull kapacitor@sha256:08149a688dddb6174e8a14ce34d3dae52b05b9079b0119e14822f67f057fe283
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6.2-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:63a731cc73e4d105cc09626f2d02c74b8dee108ef4faa655834b21f2570e2b79
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61428116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34af74ca321f9f0f15370d8abd1235fd5e4ba6517714f413156e0b503d83a698`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Sep 2021 18:21:29 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 30 Sep 2021 18:21:58 GMT
ENV KAPACITOR_VERSION=1.6.2
# Thu, 07 Oct 2021 19:56:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 07 Oct 2021 19:56:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 07 Oct 2021 19:56:31 GMT
EXPOSE 9092
# Thu, 07 Oct 2021 19:56:32 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 07 Oct 2021 19:56:32 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 07 Oct 2021 19:56:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:56:32 GMT
CMD ["kapacitord"]
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
	-	`sha256:35128f89929d86c35c1dfabaaea2552df6e9c25e7ec0d08e798390d47c11a85b`  
		Last Modified: Thu, 30 Sep 2021 18:22:31 GMT  
		Size: 281.5 KB (281501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516aad966cd4cc065db1821d5d1cbc26bb9b3a8c8ace7d5b4ba37b8d118056e3`  
		Last Modified: Thu, 07 Oct 2021 19:56:59 GMT  
		Size: 58.3 MB (58331562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744988bc2e03a02b20ef5c3ed06d2535e5cfbdac463502680dbe74af369f37f6`  
		Last Modified: Thu, 07 Oct 2021 19:56:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9b0b48185ad7f8e4ea4c843c0358ae53fed5bc0afc2500e2915aa0e00eb4bf`  
		Last Modified: Thu, 07 Oct 2021 19:56:52 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:08149a688dddb6174e8a14ce34d3dae52b05b9079b0119e14822f67f057fe283
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:63a731cc73e4d105cc09626f2d02c74b8dee108ef4faa655834b21f2570e2b79
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61428116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34af74ca321f9f0f15370d8abd1235fd5e4ba6517714f413156e0b503d83a698`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Sep 2021 18:21:29 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 30 Sep 2021 18:21:58 GMT
ENV KAPACITOR_VERSION=1.6.2
# Thu, 07 Oct 2021 19:56:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 07 Oct 2021 19:56:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 07 Oct 2021 19:56:31 GMT
EXPOSE 9092
# Thu, 07 Oct 2021 19:56:32 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 07 Oct 2021 19:56:32 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 07 Oct 2021 19:56:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 19:56:32 GMT
CMD ["kapacitord"]
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
	-	`sha256:35128f89929d86c35c1dfabaaea2552df6e9c25e7ec0d08e798390d47c11a85b`  
		Last Modified: Thu, 30 Sep 2021 18:22:31 GMT  
		Size: 281.5 KB (281501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516aad966cd4cc065db1821d5d1cbc26bb9b3a8c8ace7d5b4ba37b8d118056e3`  
		Last Modified: Thu, 07 Oct 2021 19:56:59 GMT  
		Size: 58.3 MB (58331562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744988bc2e03a02b20ef5c3ed06d2535e5cfbdac463502680dbe74af369f37f6`  
		Last Modified: Thu, 07 Oct 2021 19:56:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9b0b48185ad7f8e4ea4c843c0358ae53fed5bc0afc2500e2915aa0e00eb4bf`  
		Last Modified: Thu, 07 Oct 2021 19:56:52 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:b5eac70b636530cc0f3f99709c809b9988cbcb0cb8438e0665a286beda5188bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:73e5db8a9ba89f21eaddf45adc67abdb216f872955c751579da075f33f13ade2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132771298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c37a95bcd945e8964ceaba40abab6723719f7d73d4f80b86e29489eb7b01948`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:48:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:48:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 07:11:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 13 Oct 2021 07:11:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 07:11:49 GMT
ENV KAPACITOR_VERSION=1.6.2
# Wed, 13 Oct 2021 07:11:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 07:11:55 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 13 Oct 2021 07:11:56 GMT
EXPOSE 9092
# Wed, 13 Oct 2021 07:11:56 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 13 Oct 2021 07:11:56 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 13 Oct 2021 07:11:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 07:11:56 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a43d3c11106306de19fd422e9da4a6f9b96de147d92c6213d6dbbc395be81b3`  
		Last Modified: Tue, 12 Oct 2021 15:57:10 GMT  
		Size: 11.3 MB (11301072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243ae34810fbd860a43ecf1a7da887386e7a1155913bf13ed95681c98a1cfa84`  
		Last Modified: Tue, 12 Oct 2021 15:57:08 GMT  
		Size: 4.3 MB (4342414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cd6f91698d25d624ba6891bcf4d34b7ef3fd9327e7d1bbff0e12954876b950`  
		Last Modified: Wed, 13 Oct 2021 07:12:15 GMT  
		Size: 13.3 MB (13342530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02e14e16b5ee4daac6cb07e20f5225f19f591382d3fa089d0c79930178b9b9b`  
		Last Modified: Wed, 13 Oct 2021 07:12:13 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf4f4dd0e5913ab75ee96d57c02a65812f5552c4cdcb1fc499c56527086daad`  
		Last Modified: Wed, 13 Oct 2021 07:12:37 GMT  
		Size: 58.4 MB (58402322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c0ab65ab94bc2ad7c04ac554bab37baa6159ed5218223b8edf65d7b38838ce`  
		Last Modified: Wed, 13 Oct 2021 07:12:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878218f4ee01430afab7fd4e20ef3817a87ef871f7d57c98cbe8ef0bc3cd230d`  
		Last Modified: Wed, 13 Oct 2021 07:12:29 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:163a91e45a6984f37649b4a47e20f83746fbca6e57052f7da89434c124807fc0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124751312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235dfcb8886839547ea238cbe685a6aa8369bf27c67b221806ac982a9e42b981`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 21:54:49 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Tue, 12 Oct 2021 21:55:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 12 Oct 2021 21:55:21 GMT
ENV KAPACITOR_VERSION=1.6.2
# Tue, 12 Oct 2021 21:55:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Tue, 12 Oct 2021 21:55:28 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Tue, 12 Oct 2021 21:55:28 GMT
EXPOSE 9092
# Tue, 12 Oct 2021 21:55:29 GMT
VOLUME [/var/lib/kapacitor]
# Tue, 12 Oct 2021 21:55:31 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Tue, 12 Oct 2021 21:55:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 21:55:32 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6106ce195cfc2ea7282dab1677e8563168fee21f184a937b32a9370944ccc077`  
		Last Modified: Tue, 12 Oct 2021 02:22:54 GMT  
		Size: 10.2 MB (10217927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499bc8ad963810c8e2cef0d22542dfad2339032cf43a8210066a9a817fd6a869`  
		Last Modified: Tue, 12 Oct 2021 02:22:53 GMT  
		Size: 4.1 MB (4096622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42793e78a888c99031cc5e588b1eb4d0b64b64214ac85dbe53b8792f0c1ac8d4`  
		Last Modified: Tue, 12 Oct 2021 21:55:54 GMT  
		Size: 12.8 MB (12819333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4226bc2244600763630c84a3d1beb498757c8261edc34262a1774cdbd72c30`  
		Last Modified: Tue, 12 Oct 2021 21:55:52 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc47eaed34d6c70bbbb28128e0264d650bcbeb1db500f9f87a3714ef19a0ce`  
		Last Modified: Tue, 12 Oct 2021 21:56:15 GMT  
		Size: 54.4 MB (54437453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48f4da4749dc7ff39b49ef4303dc8dbc04b51c8eb8308da2f909df304fbbfd5`  
		Last Modified: Tue, 12 Oct 2021 21:56:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39c642dc9fb58c271b9882a6a3bd66f2d0036317435744b6d7151aa1a021ebb`  
		Last Modified: Tue, 12 Oct 2021 21:56:07 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
