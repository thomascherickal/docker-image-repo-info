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
$ docker pull kapacitor@sha256:324170fdc4fc67669c0fe086b0fb8a838f3e42d4b020ad2ab03d730c27765f5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:de5f3f942264ff8cc421cedc3cd3f6bf5ec87f4a06aec8d3810c9304c5570069
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111622342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1521ead0d9cd697133c99162cda5a78af21d7a5e5ae810df5ffe0d734a6d53f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:41:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 18 Nov 2021 09:41:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:41:43 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 18 Nov 2021 09:41:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 18 Nov 2021 09:41:50 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 18 Nov 2021 09:41:50 GMT
EXPOSE 9092
# Thu, 18 Nov 2021 09:41:51 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 18 Nov 2021 09:41:51 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 18 Nov 2021 09:41:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:41:52 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d339abff25f510a6cb77d3f5838a68d0be9f913e861eabe828b00da83964354`  
		Last Modified: Thu, 18 Nov 2021 09:42:39 GMT  
		Size: 13.4 MB (13375454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5b945d799f5e6ee0419c9e6d53a887424cbefd588dead34124e00fa0e6be85`  
		Last Modified: Thu, 18 Nov 2021 09:42:37 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104fa8961b0c17e89a49f29718e2611d8315c2ac2daac286f28858110f7e25fc`  
		Last Modified: Thu, 18 Nov 2021 09:42:43 GMT  
		Size: 37.2 MB (37219359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f4f1e7a54a8d86a5a3d8c9d488da634f06484ce858bf3a6dacffa3ca2b6bf8`  
		Last Modified: Thu, 18 Nov 2021 09:42:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bf50880aa71186f4839e2e35ec96f4a1cbd934f776eab4b8911e872ee0d36e`  
		Last Modified: Thu, 18 Nov 2021 09:42:37 GMT  
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
$ docker pull kapacitor@sha256:92751b83b481606b878cca5cdcb78dc37afa4668c3c865ada594b6fb0027b623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104675298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37616f6ce24429ee30974ab2c96277997ae3ce411b893e10eb9190d6d017aabf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:51:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 17 Nov 2021 21:51:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 17 Nov 2021 21:51:29 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 17 Nov 2021 21:51:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 17 Nov 2021 21:51:35 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 17 Nov 2021 21:51:35 GMT
EXPOSE 9092
# Wed, 17 Nov 2021 21:51:36 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 17 Nov 2021 21:51:38 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 17 Nov 2021 21:51:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:51:39 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb074bf5a62afe7dc5be79eea3c3d20629d53225b97bd84b3524d62e3dccaec`  
		Last Modified: Wed, 17 Nov 2021 21:52:18 GMT  
		Size: 12.8 MB (12846766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7b3488d8149e50e3ee19a0d88a8a2fda066b65ab5139fc907f9fd4b4ac8735`  
		Last Modified: Wed, 17 Nov 2021 21:52:17 GMT  
		Size: 2.8 KB (2823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce92b58d7d623a1f193a7066c3ef45d41db62f8244984e5244f05d4609183078`  
		Last Modified: Wed, 17 Nov 2021 21:52:22 GMT  
		Size: 34.6 MB (34560096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6221146ba22aee183299bed4ec3511fd4a93ef8dfa4b610a39049600ec660130`  
		Last Modified: Wed, 17 Nov 2021 21:52:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9670b5f27a46f3f8b883190aa3615ab48859f24a3f2cfc139179200a97ca5176`  
		Last Modified: Wed, 17 Nov 2021 21:52:17 GMT  
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
$ docker pull kapacitor@sha256:324170fdc4fc67669c0fe086b0fb8a838f3e42d4b020ad2ab03d730c27765f5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.9` - linux; amd64

```console
$ docker pull kapacitor@sha256:de5f3f942264ff8cc421cedc3cd3f6bf5ec87f4a06aec8d3810c9304c5570069
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111622342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1521ead0d9cd697133c99162cda5a78af21d7a5e5ae810df5ffe0d734a6d53f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:41:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 18 Nov 2021 09:41:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:41:43 GMT
ENV KAPACITOR_VERSION=1.5.9
# Thu, 18 Nov 2021 09:41:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 18 Nov 2021 09:41:50 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 18 Nov 2021 09:41:50 GMT
EXPOSE 9092
# Thu, 18 Nov 2021 09:41:51 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 18 Nov 2021 09:41:51 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 18 Nov 2021 09:41:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:41:52 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d339abff25f510a6cb77d3f5838a68d0be9f913e861eabe828b00da83964354`  
		Last Modified: Thu, 18 Nov 2021 09:42:39 GMT  
		Size: 13.4 MB (13375454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5b945d799f5e6ee0419c9e6d53a887424cbefd588dead34124e00fa0e6be85`  
		Last Modified: Thu, 18 Nov 2021 09:42:37 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104fa8961b0c17e89a49f29718e2611d8315c2ac2daac286f28858110f7e25fc`  
		Last Modified: Thu, 18 Nov 2021 09:42:43 GMT  
		Size: 37.2 MB (37219359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f4f1e7a54a8d86a5a3d8c9d488da634f06484ce858bf3a6dacffa3ca2b6bf8`  
		Last Modified: Thu, 18 Nov 2021 09:42:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bf50880aa71186f4839e2e35ec96f4a1cbd934f776eab4b8911e872ee0d36e`  
		Last Modified: Thu, 18 Nov 2021 09:42:37 GMT  
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
$ docker pull kapacitor@sha256:92751b83b481606b878cca5cdcb78dc37afa4668c3c865ada594b6fb0027b623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104675298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37616f6ce24429ee30974ab2c96277997ae3ce411b893e10eb9190d6d017aabf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:51:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 17 Nov 2021 21:51:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 17 Nov 2021 21:51:29 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 17 Nov 2021 21:51:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 17 Nov 2021 21:51:35 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 17 Nov 2021 21:51:35 GMT
EXPOSE 9092
# Wed, 17 Nov 2021 21:51:36 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 17 Nov 2021 21:51:38 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 17 Nov 2021 21:51:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:51:39 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb074bf5a62afe7dc5be79eea3c3d20629d53225b97bd84b3524d62e3dccaec`  
		Last Modified: Wed, 17 Nov 2021 21:52:18 GMT  
		Size: 12.8 MB (12846766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7b3488d8149e50e3ee19a0d88a8a2fda066b65ab5139fc907f9fd4b4ac8735`  
		Last Modified: Wed, 17 Nov 2021 21:52:17 GMT  
		Size: 2.8 KB (2823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce92b58d7d623a1f193a7066c3ef45d41db62f8244984e5244f05d4609183078`  
		Last Modified: Wed, 17 Nov 2021 21:52:22 GMT  
		Size: 34.6 MB (34560096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6221146ba22aee183299bed4ec3511fd4a93ef8dfa4b610a39049600ec660130`  
		Last Modified: Wed, 17 Nov 2021 21:52:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9670b5f27a46f3f8b883190aa3615ab48859f24a3f2cfc139179200a97ca5176`  
		Last Modified: Wed, 17 Nov 2021 21:52:17 GMT  
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
$ docker pull kapacitor@sha256:2f0a6cb6b430d8dc7dced626fcb9d2c40528b482b06adc0451cc6dac3a5e9efb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:f8176fc55701e62f9c751775b2c647ebb801ac83c1398ca05caaee906107dab0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132805261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050c84c499b8eff422bdfef3c56a9b276843f07b96426737e970181b091c8d3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:41:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 18 Nov 2021 09:41:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:42:01 GMT
ENV KAPACITOR_VERSION=1.6.2
# Thu, 18 Nov 2021 09:42:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 18 Nov 2021 09:42:10 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 18 Nov 2021 09:42:11 GMT
EXPOSE 9092
# Thu, 18 Nov 2021 09:42:11 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 18 Nov 2021 09:42:11 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 18 Nov 2021 09:42:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:42:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d339abff25f510a6cb77d3f5838a68d0be9f913e861eabe828b00da83964354`  
		Last Modified: Thu, 18 Nov 2021 09:42:39 GMT  
		Size: 13.4 MB (13375454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5b945d799f5e6ee0419c9e6d53a887424cbefd588dead34124e00fa0e6be85`  
		Last Modified: Thu, 18 Nov 2021 09:42:37 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e734913cb4c8c24df54c8494e15e986a5fdd3632510a3fa52ab0435346de201c`  
		Last Modified: Thu, 18 Nov 2021 09:43:01 GMT  
		Size: 58.4 MB (58402279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccff5a26f991fab17f0c3b82ed09d8569ad7f2f42d90e3493085d8baa3d1661f`  
		Last Modified: Thu, 18 Nov 2021 09:42:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a24d386b85f75db6b7592a4d672f572de51e2087acc0d5a6a2d59759794586`  
		Last Modified: Thu, 18 Nov 2021 09:42:53 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:e72a3e1a4f061e6f7e63e73065f3d2b16ee6942928b0b04c9986ddc0f7846643
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124552730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68a39f7ffbea20ad101dfeab0f56c0d67172e4166e9b4d76403eeefcbd86aef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:51:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 17 Nov 2021 21:51:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 17 Nov 2021 21:51:48 GMT
ENV KAPACITOR_VERSION=1.6.2
# Wed, 17 Nov 2021 21:51:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 17 Nov 2021 21:51:54 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 17 Nov 2021 21:51:54 GMT
EXPOSE 9092
# Wed, 17 Nov 2021 21:51:55 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 17 Nov 2021 21:51:57 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 17 Nov 2021 21:51:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:51:58 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb074bf5a62afe7dc5be79eea3c3d20629d53225b97bd84b3524d62e3dccaec`  
		Last Modified: Wed, 17 Nov 2021 21:52:18 GMT  
		Size: 12.8 MB (12846766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7b3488d8149e50e3ee19a0d88a8a2fda066b65ab5139fc907f9fd4b4ac8735`  
		Last Modified: Wed, 17 Nov 2021 21:52:17 GMT  
		Size: 2.8 KB (2823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f159654be800b81cc902f6858f28a52623dcbba93b84ad53cfa78c1e09edd70`  
		Last Modified: Wed, 17 Nov 2021 21:52:40 GMT  
		Size: 54.4 MB (54437526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e501cab1d3a8ff59e6cdea40627c7cd507f8be0083ca732099f6555f3b1f4509`  
		Last Modified: Wed, 17 Nov 2021 21:52:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a001bc754967bc1a696da1d4f70fefc0f46337ebf837c18b94e128f8e9e16abe`  
		Last Modified: Wed, 17 Nov 2021 21:52:32 GMT  
		Size: 232.0 B  
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
$ docker pull kapacitor@sha256:2f0a6cb6b430d8dc7dced626fcb9d2c40528b482b06adc0451cc6dac3a5e9efb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6.2` - linux; amd64

```console
$ docker pull kapacitor@sha256:f8176fc55701e62f9c751775b2c647ebb801ac83c1398ca05caaee906107dab0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132805261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050c84c499b8eff422bdfef3c56a9b276843f07b96426737e970181b091c8d3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:41:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 18 Nov 2021 09:41:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:42:01 GMT
ENV KAPACITOR_VERSION=1.6.2
# Thu, 18 Nov 2021 09:42:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 18 Nov 2021 09:42:10 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 18 Nov 2021 09:42:11 GMT
EXPOSE 9092
# Thu, 18 Nov 2021 09:42:11 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 18 Nov 2021 09:42:11 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 18 Nov 2021 09:42:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:42:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d339abff25f510a6cb77d3f5838a68d0be9f913e861eabe828b00da83964354`  
		Last Modified: Thu, 18 Nov 2021 09:42:39 GMT  
		Size: 13.4 MB (13375454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5b945d799f5e6ee0419c9e6d53a887424cbefd588dead34124e00fa0e6be85`  
		Last Modified: Thu, 18 Nov 2021 09:42:37 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e734913cb4c8c24df54c8494e15e986a5fdd3632510a3fa52ab0435346de201c`  
		Last Modified: Thu, 18 Nov 2021 09:43:01 GMT  
		Size: 58.4 MB (58402279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccff5a26f991fab17f0c3b82ed09d8569ad7f2f42d90e3493085d8baa3d1661f`  
		Last Modified: Thu, 18 Nov 2021 09:42:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a24d386b85f75db6b7592a4d672f572de51e2087acc0d5a6a2d59759794586`  
		Last Modified: Thu, 18 Nov 2021 09:42:53 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6.2` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:e72a3e1a4f061e6f7e63e73065f3d2b16ee6942928b0b04c9986ddc0f7846643
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124552730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68a39f7ffbea20ad101dfeab0f56c0d67172e4166e9b4d76403eeefcbd86aef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:51:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 17 Nov 2021 21:51:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 17 Nov 2021 21:51:48 GMT
ENV KAPACITOR_VERSION=1.6.2
# Wed, 17 Nov 2021 21:51:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 17 Nov 2021 21:51:54 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 17 Nov 2021 21:51:54 GMT
EXPOSE 9092
# Wed, 17 Nov 2021 21:51:55 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 17 Nov 2021 21:51:57 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 17 Nov 2021 21:51:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:51:58 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb074bf5a62afe7dc5be79eea3c3d20629d53225b97bd84b3524d62e3dccaec`  
		Last Modified: Wed, 17 Nov 2021 21:52:18 GMT  
		Size: 12.8 MB (12846766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7b3488d8149e50e3ee19a0d88a8a2fda066b65ab5139fc907f9fd4b4ac8735`  
		Last Modified: Wed, 17 Nov 2021 21:52:17 GMT  
		Size: 2.8 KB (2823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f159654be800b81cc902f6858f28a52623dcbba93b84ad53cfa78c1e09edd70`  
		Last Modified: Wed, 17 Nov 2021 21:52:40 GMT  
		Size: 54.4 MB (54437526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e501cab1d3a8ff59e6cdea40627c7cd507f8be0083ca732099f6555f3b1f4509`  
		Last Modified: Wed, 17 Nov 2021 21:52:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a001bc754967bc1a696da1d4f70fefc0f46337ebf837c18b94e128f8e9e16abe`  
		Last Modified: Wed, 17 Nov 2021 21:52:32 GMT  
		Size: 232.0 B  
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
$ docker pull kapacitor@sha256:2f0a6cb6b430d8dc7dced626fcb9d2c40528b482b06adc0451cc6dac3a5e9efb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:f8176fc55701e62f9c751775b2c647ebb801ac83c1398ca05caaee906107dab0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132805261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050c84c499b8eff422bdfef3c56a9b276843f07b96426737e970181b091c8d3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 18 Nov 2021 09:41:33 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 18 Nov 2021 09:41:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 18 Nov 2021 09:42:01 GMT
ENV KAPACITOR_VERSION=1.6.2
# Thu, 18 Nov 2021 09:42:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 18 Nov 2021 09:42:10 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 18 Nov 2021 09:42:11 GMT
EXPOSE 9092
# Thu, 18 Nov 2021 09:42:11 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 18 Nov 2021 09:42:11 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 18 Nov 2021 09:42:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Nov 2021 09:42:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d339abff25f510a6cb77d3f5838a68d0be9f913e861eabe828b00da83964354`  
		Last Modified: Thu, 18 Nov 2021 09:42:39 GMT  
		Size: 13.4 MB (13375454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5b945d799f5e6ee0419c9e6d53a887424cbefd588dead34124e00fa0e6be85`  
		Last Modified: Thu, 18 Nov 2021 09:42:37 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e734913cb4c8c24df54c8494e15e986a5fdd3632510a3fa52ab0435346de201c`  
		Last Modified: Thu, 18 Nov 2021 09:43:01 GMT  
		Size: 58.4 MB (58402279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccff5a26f991fab17f0c3b82ed09d8569ad7f2f42d90e3493085d8baa3d1661f`  
		Last Modified: Thu, 18 Nov 2021 09:42:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a24d386b85f75db6b7592a4d672f572de51e2087acc0d5a6a2d59759794586`  
		Last Modified: Thu, 18 Nov 2021 09:42:53 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:e72a3e1a4f061e6f7e63e73065f3d2b16ee6942928b0b04c9986ddc0f7846643
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124552730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68a39f7ffbea20ad101dfeab0f56c0d67172e4166e9b4d76403eeefcbd86aef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:33 GMT
ADD file:3225671be4edc3599e29ebd06516b95573246e68bf29649c402ed87c03c109b5 in / 
# Wed, 17 Nov 2021 02:42:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:32:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:32:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:51:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 17 Nov 2021 21:51:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 17 Nov 2021 21:51:48 GMT
ENV KAPACITOR_VERSION=1.6.2
# Wed, 17 Nov 2021 21:51:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 17 Nov 2021 21:51:54 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 17 Nov 2021 21:51:54 GMT
EXPOSE 9092
# Wed, 17 Nov 2021 21:51:55 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 17 Nov 2021 21:51:57 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 17 Nov 2021 21:51:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 21:51:58 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c64a4bafe4ad6fc05fcc6d76d2a06f168f331ffbc87e518fb4ca4ea22e75527e`  
		Last Modified: Wed, 17 Nov 2021 02:51:11 GMT  
		Size: 43.2 MB (43174478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaddc7c2a37cd151a9001bbe7816f06f5f36ac6d53cc0d02fe2b327f85a2c7e`  
		Last Modified: Wed, 17 Nov 2021 13:40:24 GMT  
		Size: 10.2 MB (10216788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61401ffc70123532d1f4886b9ebd00e11d1155a2363117bf5aab10353c373dc9`  
		Last Modified: Wed, 17 Nov 2021 13:40:23 GMT  
		Size: 3.9 MB (3873891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb074bf5a62afe7dc5be79eea3c3d20629d53225b97bd84b3524d62e3dccaec`  
		Last Modified: Wed, 17 Nov 2021 21:52:18 GMT  
		Size: 12.8 MB (12846766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7b3488d8149e50e3ee19a0d88a8a2fda066b65ab5139fc907f9fd4b4ac8735`  
		Last Modified: Wed, 17 Nov 2021 21:52:17 GMT  
		Size: 2.8 KB (2823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f159654be800b81cc902f6858f28a52623dcbba93b84ad53cfa78c1e09edd70`  
		Last Modified: Wed, 17 Nov 2021 21:52:40 GMT  
		Size: 54.4 MB (54437526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e501cab1d3a8ff59e6cdea40627c7cd507f8be0083ca732099f6555f3b1f4509`  
		Last Modified: Wed, 17 Nov 2021 21:52:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a001bc754967bc1a696da1d4f70fefc0f46337ebf837c18b94e128f8e9e16abe`  
		Last Modified: Wed, 17 Nov 2021 21:52:32 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
