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
$ docker pull kapacitor@sha256:f94c55450aec48c07ecc45c915c19ed38a7c98944f8633402d8048edbd697419
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
$ docker pull kapacitor@sha256:e8f0361ff09974bcfad045b250fcf1f6f436ea44a2ce21b3f5230d34d5b9b85a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104651429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2be15d5772635a986e0cffc76ed8ad5f7b2548ae2d1f7cec1ad53749e702455`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:03:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:03:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 09:53:35 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 Oct 2021 09:53:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 09:53:43 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 16 Oct 2021 09:53:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 09:53:49 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 Oct 2021 09:53:49 GMT
EXPOSE 9092
# Sat, 16 Oct 2021 09:53:50 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 Oct 2021 09:53:52 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 Oct 2021 09:53:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 09:53:53 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607051b9b8b0e248adc1dbae78b910c62d134181c4945e4df5e165ba533f7dea`  
		Last Modified: Sat, 16 Oct 2021 03:18:13 GMT  
		Size: 10.2 MB (10216060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c91f590ca18c241c146cf6ad6fb66517634bedc0681afcc69d37ee25828046`  
		Last Modified: Sat, 16 Oct 2021 03:18:12 GMT  
		Size: 3.9 MB (3873851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5f3fa2583e3c53938d7087706dc1c4b0036145635f3a217c9d608a9b36d5e3`  
		Last Modified: Sat, 16 Oct 2021 09:54:32 GMT  
		Size: 12.8 MB (12821542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5214dbab5b308c965390e967acfa0ca9f7a34c6eec550a3b8c110fe5db297b`  
		Last Modified: Sat, 16 Oct 2021 09:54:30 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6f27495cee29766e332775e6402a1ce9a4ed9b00b43a1a07315aba1b2bfb35`  
		Last Modified: Sat, 16 Oct 2021 09:54:34 GMT  
		Size: 34.6 MB (34559999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9503c39e1cf29a5f8b68809e20f1f32bc99a1f8c0ffb45cbb1a05aa31528b6d`  
		Last Modified: Sat, 16 Oct 2021 09:54:30 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec227ff6ad9055add20ee1a38208c5b30145451d654026eb8a1dceaa33635ef6`  
		Last Modified: Sat, 16 Oct 2021 09:54:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:751918e56fde6040974138659942dcb1dfefda5ea61321e20023e70f5b5c6d97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:ebfc4af599b8126bdce9d95186ae296a9ac80697a0ae97bb758d6e15576915ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22646477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15f8972ccc76427f5cba40c5b78c201cbdde44e128e47e642190767bb79e8c6e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 06:07:23 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 13 Nov 2021 06:07:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 06:07:29 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 13 Nov 2021 06:07:29 GMT
EXPOSE 9092
# Sat, 13 Nov 2021 06:07:29 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 13 Nov 2021 06:07:30 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Sat, 13 Nov 2021 06:07:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:07:30 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a486c6344f55af907ec99dd18980cfac4d88970868515c05e6228b0fd8cfeff`  
		Last Modified: Sat, 13 Nov 2021 06:08:12 GMT  
		Size: 19.5 MB (19540901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4e6d3e0710bdc72f26e2a54c0fed4abe60bc4496eb1c111287663d4257421c`  
		Last Modified: Sat, 13 Nov 2021 06:08:09 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4d938d5c3e3a42543955a737542599f0936f8268da48dbb42b3d23c4b512c0`  
		Last Modified: Sat, 13 Nov 2021 06:08:09 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9`

```console
$ docker pull kapacitor@sha256:f94c55450aec48c07ecc45c915c19ed38a7c98944f8633402d8048edbd697419
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
$ docker pull kapacitor@sha256:e8f0361ff09974bcfad045b250fcf1f6f436ea44a2ce21b3f5230d34d5b9b85a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104651429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2be15d5772635a986e0cffc76ed8ad5f7b2548ae2d1f7cec1ad53749e702455`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:03:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:03:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 09:53:35 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 Oct 2021 09:53:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 09:53:43 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 16 Oct 2021 09:53:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 09:53:49 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 Oct 2021 09:53:49 GMT
EXPOSE 9092
# Sat, 16 Oct 2021 09:53:50 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 Oct 2021 09:53:52 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 Oct 2021 09:53:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 09:53:53 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607051b9b8b0e248adc1dbae78b910c62d134181c4945e4df5e165ba533f7dea`  
		Last Modified: Sat, 16 Oct 2021 03:18:13 GMT  
		Size: 10.2 MB (10216060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c91f590ca18c241c146cf6ad6fb66517634bedc0681afcc69d37ee25828046`  
		Last Modified: Sat, 16 Oct 2021 03:18:12 GMT  
		Size: 3.9 MB (3873851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5f3fa2583e3c53938d7087706dc1c4b0036145635f3a217c9d608a9b36d5e3`  
		Last Modified: Sat, 16 Oct 2021 09:54:32 GMT  
		Size: 12.8 MB (12821542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5214dbab5b308c965390e967acfa0ca9f7a34c6eec550a3b8c110fe5db297b`  
		Last Modified: Sat, 16 Oct 2021 09:54:30 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6f27495cee29766e332775e6402a1ce9a4ed9b00b43a1a07315aba1b2bfb35`  
		Last Modified: Sat, 16 Oct 2021 09:54:34 GMT  
		Size: 34.6 MB (34559999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9503c39e1cf29a5f8b68809e20f1f32bc99a1f8c0ffb45cbb1a05aa31528b6d`  
		Last Modified: Sat, 16 Oct 2021 09:54:30 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec227ff6ad9055add20ee1a38208c5b30145451d654026eb8a1dceaa33635ef6`  
		Last Modified: Sat, 16 Oct 2021 09:54:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9-alpine`

```console
$ docker pull kapacitor@sha256:751918e56fde6040974138659942dcb1dfefda5ea61321e20023e70f5b5c6d97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5.9-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:ebfc4af599b8126bdce9d95186ae296a9ac80697a0ae97bb758d6e15576915ce
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22646477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15f8972ccc76427f5cba40c5b78c201cbdde44e128e47e642190767bb79e8c6e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 06:07:23 GMT
ENV KAPACITOR_VERSION=1.5.9
# Sat, 13 Nov 2021 06:07:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 06:07:29 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 13 Nov 2021 06:07:29 GMT
EXPOSE 9092
# Sat, 13 Nov 2021 06:07:29 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 13 Nov 2021 06:07:30 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Sat, 13 Nov 2021 06:07:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:07:30 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a486c6344f55af907ec99dd18980cfac4d88970868515c05e6228b0fd8cfeff`  
		Last Modified: Sat, 13 Nov 2021 06:08:12 GMT  
		Size: 19.5 MB (19540901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4e6d3e0710bdc72f26e2a54c0fed4abe60bc4496eb1c111287663d4257421c`  
		Last Modified: Sat, 13 Nov 2021 06:08:09 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4d938d5c3e3a42543955a737542599f0936f8268da48dbb42b3d23c4b512c0`  
		Last Modified: Sat, 13 Nov 2021 06:08:09 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6`

```console
$ docker pull kapacitor@sha256:4b034291f426f213b0a3c7ab76dfbeaeeee713b5f6ba5e11f5721a50cea01b87
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
$ docker pull kapacitor@sha256:aa11214436e0a37f03f84f025458f2be5a330c906601c80593a79cb53d8350fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124528930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b370313b3cc169743d517418ad60dc893f07a3e6d1fad99c20d84b44d7cf3a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:03:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:03:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 09:53:35 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 Oct 2021 09:53:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 09:54:01 GMT
ENV KAPACITOR_VERSION=1.6.2
# Sat, 16 Oct 2021 09:54:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 09:54:08 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 Oct 2021 09:54:08 GMT
EXPOSE 9092
# Sat, 16 Oct 2021 09:54:09 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 Oct 2021 09:54:11 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 Oct 2021 09:54:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 09:54:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607051b9b8b0e248adc1dbae78b910c62d134181c4945e4df5e165ba533f7dea`  
		Last Modified: Sat, 16 Oct 2021 03:18:13 GMT  
		Size: 10.2 MB (10216060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c91f590ca18c241c146cf6ad6fb66517634bedc0681afcc69d37ee25828046`  
		Last Modified: Sat, 16 Oct 2021 03:18:12 GMT  
		Size: 3.9 MB (3873851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5f3fa2583e3c53938d7087706dc1c4b0036145635f3a217c9d608a9b36d5e3`  
		Last Modified: Sat, 16 Oct 2021 09:54:32 GMT  
		Size: 12.8 MB (12821542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5214dbab5b308c965390e967acfa0ca9f7a34c6eec550a3b8c110fe5db297b`  
		Last Modified: Sat, 16 Oct 2021 09:54:30 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a89d670eac694a41f1d79f02b89849fb3455b235b7bb8f2f2a50f8458c0a2a`  
		Last Modified: Sat, 16 Oct 2021 09:54:58 GMT  
		Size: 54.4 MB (54437499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e00db6d1e4882e7dc460fdecfaaac61095a0488633d2fe622c79bc5e7200b`  
		Last Modified: Sat, 16 Oct 2021 09:54:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf6a670ecb987e88233dbd32fe23312ff77734c8b00a56094fefcaf95d2bd7c`  
		Last Modified: Sat, 16 Oct 2021 09:54:45 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6-alpine`

```console
$ docker pull kapacitor@sha256:687ded863d65e17d1de1116d4fd822dcf0a186585cf7ca574965a2d61870d603
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:c36254ee5403831ea98c53f60dc936a7fef5d62fce45f6a4dca587159e74752a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61437295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac578e9f11ba81e0d8f8f846b33ca6843afcb4fe9391065a287347dba18c9d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 06:07:34 GMT
ENV KAPACITOR_VERSION=1.6.2
# Sat, 13 Nov 2021 06:07:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 06:07:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 13 Nov 2021 06:07:48 GMT
EXPOSE 9092
# Sat, 13 Nov 2021 06:07:48 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 13 Nov 2021 06:07:49 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Sat, 13 Nov 2021 06:07:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:07:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9f697ca0ecf495918d19b823ae9ceaad61642f48e8c2168b9f7d20101240fb`  
		Last Modified: Sat, 13 Nov 2021 06:08:36 GMT  
		Size: 58.3 MB (58331742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee43f60026c5642edede78b38600e56689be599032cfd63788fa2f9ac3d526e`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f1710db3944f0a85a27d4b802091e849ac354869af8b3d1de733a6093db189`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.2`

```console
$ docker pull kapacitor@sha256:4b034291f426f213b0a3c7ab76dfbeaeeee713b5f6ba5e11f5721a50cea01b87
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
$ docker pull kapacitor@sha256:aa11214436e0a37f03f84f025458f2be5a330c906601c80593a79cb53d8350fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124528930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b370313b3cc169743d517418ad60dc893f07a3e6d1fad99c20d84b44d7cf3a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:03:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:03:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 09:53:35 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 Oct 2021 09:53:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 09:54:01 GMT
ENV KAPACITOR_VERSION=1.6.2
# Sat, 16 Oct 2021 09:54:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 09:54:08 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 Oct 2021 09:54:08 GMT
EXPOSE 9092
# Sat, 16 Oct 2021 09:54:09 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 Oct 2021 09:54:11 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 Oct 2021 09:54:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 09:54:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607051b9b8b0e248adc1dbae78b910c62d134181c4945e4df5e165ba533f7dea`  
		Last Modified: Sat, 16 Oct 2021 03:18:13 GMT  
		Size: 10.2 MB (10216060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c91f590ca18c241c146cf6ad6fb66517634bedc0681afcc69d37ee25828046`  
		Last Modified: Sat, 16 Oct 2021 03:18:12 GMT  
		Size: 3.9 MB (3873851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5f3fa2583e3c53938d7087706dc1c4b0036145635f3a217c9d608a9b36d5e3`  
		Last Modified: Sat, 16 Oct 2021 09:54:32 GMT  
		Size: 12.8 MB (12821542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5214dbab5b308c965390e967acfa0ca9f7a34c6eec550a3b8c110fe5db297b`  
		Last Modified: Sat, 16 Oct 2021 09:54:30 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a89d670eac694a41f1d79f02b89849fb3455b235b7bb8f2f2a50f8458c0a2a`  
		Last Modified: Sat, 16 Oct 2021 09:54:58 GMT  
		Size: 54.4 MB (54437499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e00db6d1e4882e7dc460fdecfaaac61095a0488633d2fe622c79bc5e7200b`  
		Last Modified: Sat, 16 Oct 2021 09:54:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf6a670ecb987e88233dbd32fe23312ff77734c8b00a56094fefcaf95d2bd7c`  
		Last Modified: Sat, 16 Oct 2021 09:54:45 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.2-alpine`

```console
$ docker pull kapacitor@sha256:687ded863d65e17d1de1116d4fd822dcf0a186585cf7ca574965a2d61870d603
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6.2-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:c36254ee5403831ea98c53f60dc936a7fef5d62fce45f6a4dca587159e74752a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61437295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac578e9f11ba81e0d8f8f846b33ca6843afcb4fe9391065a287347dba18c9d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 06:07:34 GMT
ENV KAPACITOR_VERSION=1.6.2
# Sat, 13 Nov 2021 06:07:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 06:07:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 13 Nov 2021 06:07:48 GMT
EXPOSE 9092
# Sat, 13 Nov 2021 06:07:48 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 13 Nov 2021 06:07:49 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Sat, 13 Nov 2021 06:07:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:07:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9f697ca0ecf495918d19b823ae9ceaad61642f48e8c2168b9f7d20101240fb`  
		Last Modified: Sat, 13 Nov 2021 06:08:36 GMT  
		Size: 58.3 MB (58331742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee43f60026c5642edede78b38600e56689be599032cfd63788fa2f9ac3d526e`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f1710db3944f0a85a27d4b802091e849ac354869af8b3d1de733a6093db189`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:687ded863d65e17d1de1116d4fd822dcf0a186585cf7ca574965a2d61870d603
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:c36254ee5403831ea98c53f60dc936a7fef5d62fce45f6a4dca587159e74752a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61437295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac578e9f11ba81e0d8f8f846b33ca6843afcb4fe9391065a287347dba18c9d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:55:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Sat, 13 Nov 2021 06:07:34 GMT
ENV KAPACITOR_VERSION=1.6.2
# Sat, 13 Nov 2021 06:07:47 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Sat, 13 Nov 2021 06:07:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 13 Nov 2021 06:07:48 GMT
EXPOSE 9092
# Sat, 13 Nov 2021 06:07:48 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 13 Nov 2021 06:07:49 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Sat, 13 Nov 2021 06:07:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Nov 2021 06:07:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aac166cdd02de2f1baf9250ebe4e1a5bec54cc49a59dbb3716570ed37d5bf63`  
		Last Modified: Fri, 12 Nov 2021 21:56:43 GMT  
		Size: 282.0 KB (281961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9f697ca0ecf495918d19b823ae9ceaad61642f48e8c2168b9f7d20101240fb`  
		Last Modified: Sat, 13 Nov 2021 06:08:36 GMT  
		Size: 58.3 MB (58331742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee43f60026c5642edede78b38600e56689be599032cfd63788fa2f9ac3d526e`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f1710db3944f0a85a27d4b802091e849ac354869af8b3d1de733a6093db189`  
		Last Modified: Sat, 13 Nov 2021 06:08:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:4b034291f426f213b0a3c7ab76dfbeaeeee713b5f6ba5e11f5721a50cea01b87
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
$ docker pull kapacitor@sha256:aa11214436e0a37f03f84f025458f2be5a330c906601c80593a79cb53d8350fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124528930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b370313b3cc169743d517418ad60dc893f07a3e6d1fad99c20d84b44d7cf3a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:03:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:03:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 09:53:35 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 Oct 2021 09:53:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 09:54:01 GMT
ENV KAPACITOR_VERSION=1.6.2
# Sat, 16 Oct 2021 09:54:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 09:54:08 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 Oct 2021 09:54:08 GMT
EXPOSE 9092
# Sat, 16 Oct 2021 09:54:09 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 Oct 2021 09:54:11 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 Oct 2021 09:54:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 09:54:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607051b9b8b0e248adc1dbae78b910c62d134181c4945e4df5e165ba533f7dea`  
		Last Modified: Sat, 16 Oct 2021 03:18:13 GMT  
		Size: 10.2 MB (10216060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c91f590ca18c241c146cf6ad6fb66517634bedc0681afcc69d37ee25828046`  
		Last Modified: Sat, 16 Oct 2021 03:18:12 GMT  
		Size: 3.9 MB (3873851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5f3fa2583e3c53938d7087706dc1c4b0036145635f3a217c9d608a9b36d5e3`  
		Last Modified: Sat, 16 Oct 2021 09:54:32 GMT  
		Size: 12.8 MB (12821542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5214dbab5b308c965390e967acfa0ca9f7a34c6eec550a3b8c110fe5db297b`  
		Last Modified: Sat, 16 Oct 2021 09:54:30 GMT  
		Size: 2.8 KB (2825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a89d670eac694a41f1d79f02b89849fb3455b235b7bb8f2f2a50f8458c0a2a`  
		Last Modified: Sat, 16 Oct 2021 09:54:58 GMT  
		Size: 54.4 MB (54437499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e00db6d1e4882e7dc460fdecfaaac61095a0488633d2fe622c79bc5e7200b`  
		Last Modified: Sat, 16 Oct 2021 09:54:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf6a670ecb987e88233dbd32fe23312ff77734c8b00a56094fefcaf95d2bd7c`  
		Last Modified: Sat, 16 Oct 2021 09:54:45 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
