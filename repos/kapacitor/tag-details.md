<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.4`](#kapacitor14)
-	[`kapacitor:1.4.1`](#kapacitor141)
-	[`kapacitor:1.4.1-alpine`](#kapacitor141-alpine)
-	[`kapacitor:1.4-alpine`](#kapacitor14-alpine)
-	[`kapacitor:1.5`](#kapacitor15)
-	[`kapacitor:1.5.4`](#kapacitor154)
-	[`kapacitor:1.5.4-alpine`](#kapacitor154-alpine)
-	[`kapacitor:1.5-alpine`](#kapacitor15-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.4`

```console
$ docker pull kapacitor@sha256:da0c327d7d813b0f44516152521d83197f68414e75aeabc8e6d0d82882079463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.4` - linux; amd64

```console
$ docker pull kapacitor@sha256:b053a9acd2c0517976a968ad2ad8d32d6d923485a2f08d978e7fbd4d9cdd4405
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.3 MB (96312876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ebd37e8545fee1e717a189f28253ac54b925cd00b4deffc6e8acff68efe9583`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:43:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:43:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 May 2020 09:44:15 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 May 2020 09:44:18 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 16 May 2020 09:44:18 GMT
ENV KAPACITOR_VERSION=1.4.1
# Sat, 16 May 2020 09:44:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Sat, 16 May 2020 09:44:22 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 May 2020 09:44:22 GMT
EXPOSE 9092
# Sat, 16 May 2020 09:44:22 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 May 2020 09:44:23 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 May 2020 09:44:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 May 2020 09:44:23 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194b0e3c928807cfabf081055a117585ba5bf6697f65b2fede02225a5d73ad2`  
		Last Modified: Fri, 15 May 2020 17:55:27 GMT  
		Size: 10.8 MB (10797475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec00f35d5b2d1db6b8e925a3005c1a285365775028db0339903ddaeec4763`  
		Last Modified: Fri, 15 May 2020 17:55:29 GMT  
		Size: 4.3 MB (4340139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2384f0606b9fbbbd98395f99922e252f11cfa34e5a6630c12b5f0487f7f17011`  
		Last Modified: Sat, 16 May 2020 09:44:50 GMT  
		Size: 13.1 MB (13102550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c2bdba4f53fc9ba35acf2ec0682e9c71eabd9e0ea0f1e02e575885c572d2f`  
		Last Modified: Sat, 16 May 2020 09:44:48 GMT  
		Size: 2.8 KB (2774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604e999c809dd29a15a05b380ff888ce5d8f2f4e59d91dfd050a3b24ff298fe2`  
		Last Modified: Sat, 16 May 2020 09:44:54 GMT  
		Size: 22.7 MB (22694274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3cafb0bf044554bd54be0f8981c8e86298c073d30e66351d812cb533cf724c`  
		Last Modified: Sat, 16 May 2020 09:44:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306e48e47a264276ae324de2ff43768409fed2ec821ab689a45b357565f045d1`  
		Last Modified: Sat, 16 May 2020 09:44:49 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:823e316a4f5672a190699d9f2ab890c493682e4d1dc1d185716c939b4cfa790d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90105866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6065c9640a8944eab61fa36140c014c1a8064ad79ec6f7bf19d199f7a3a1802`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 15 May 2020 01:06:22 GMT
ADD file:89db8453485648b09e63411b6e2ad84f08844ee55cb115e59cdc8c8cb1c29a1f in / 
# Fri, 15 May 2020 01:06:23 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:49:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 May 2020 02:59:29 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 May 2020 02:59:33 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 16 May 2020 02:59:34 GMT
ENV KAPACITOR_VERSION=1.4.1
# Sat, 16 May 2020 02:59:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Sat, 16 May 2020 02:59:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 May 2020 02:59:42 GMT
EXPOSE 9092
# Sat, 16 May 2020 02:59:43 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 May 2020 02:59:43 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 May 2020 02:59:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 May 2020 02:59:45 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:11acdea2de14253903f5970d63a2076ff08912929430d1c33afe617c9fa6bf8f`  
		Last Modified: Fri, 15 May 2020 01:14:46 GMT  
		Size: 42.1 MB (42104346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99452f66748f5df5d89d2287e42b5c3d87c9d5e1e20c16ef729e87d463840cf7`  
		Last Modified: Fri, 15 May 2020 11:01:44 GMT  
		Size: 9.5 MB (9498344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cef06b7abe4487657829b47c97bd2992f14a34349e0bcf60a47de9c647bd3fb`  
		Last Modified: Fri, 15 May 2020 11:01:43 GMT  
		Size: 3.9 MB (3918713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a816593387c5d1c32f87e1b3c413dae1dab2eac6f8cac7fc43e22b5bc254d83a`  
		Last Modified: Sat, 16 May 2020 03:00:17 GMT  
		Size: 13.3 MB (13273150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f9f5d8409ab5c24f4eab5db4236913a69ccff0e5a81d55a07ebd7f0ab7d667`  
		Last Modified: Sat, 16 May 2020 03:00:15 GMT  
		Size: 2.8 KB (2800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2be052f14cc6dc85ac4caa6ab76b9980b6eda80c75096aa09b88d4b35329d4`  
		Last Modified: Sat, 16 May 2020 03:00:23 GMT  
		Size: 21.3 MB (21308058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa76ff55ba46eed7ab380121ad38cb6f0ce2d08c3a431219db617fa0dac1a4b7`  
		Last Modified: Sat, 16 May 2020 03:00:14 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff2ec7a40e713216d50469d7520cd8d49bee5268201da0058bb61d2ae139aab`  
		Last Modified: Sat, 16 May 2020 03:00:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:713703deb731265acade7afed50311b80f35a36b7d2e8ed5e1374bdf97814374
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91115917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ee14f22ea080d997c490f655244403d7e176b684a72849366028aa4f73794f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 18:20:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 23 Apr 2020 18:20:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 18:20:25 GMT
ENV KAPACITOR_VERSION=1.4.1
# Thu, 23 Apr 2020 18:20:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Thu, 23 Apr 2020 18:20:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 23 Apr 2020 18:20:31 GMT
EXPOSE 9092
# Thu, 23 Apr 2020 18:20:32 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 23 Apr 2020 18:20:33 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 23 Apr 2020 18:20:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 18:20:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2880f01126539717a8c176ecd9f66045832497fe1667dd1fe5eb10a99fa72b`  
		Last Modified: Thu, 23 Apr 2020 18:21:04 GMT  
		Size: 12.8 MB (12802819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f2b353fcdc47aa924ac04a3ffe383df13c8d2f97929e24492cb9dcb3718bb2`  
		Last Modified: Thu, 23 Apr 2020 18:21:02 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e75eaf09fdc3ceade56b3689d8b1f7dbc79c35563ec4083d6b64b5ae873fc0`  
		Last Modified: Thu, 23 Apr 2020 18:21:09 GMT  
		Size: 21.3 MB (21307845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92643273a3e2204522977ea783d691d24c924dcefdcf0f71ae0e95343e1f4b05`  
		Last Modified: Thu, 23 Apr 2020 18:21:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c467a0f82f0e479e58a4fc7a762623df12c48d5a15eff4eb41790a55b94bfd`  
		Last Modified: Thu, 23 Apr 2020 18:21:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4.1`

```console
$ docker pull kapacitor@sha256:da0c327d7d813b0f44516152521d83197f68414e75aeabc8e6d0d82882079463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.4.1` - linux; amd64

```console
$ docker pull kapacitor@sha256:b053a9acd2c0517976a968ad2ad8d32d6d923485a2f08d978e7fbd4d9cdd4405
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.3 MB (96312876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ebd37e8545fee1e717a189f28253ac54b925cd00b4deffc6e8acff68efe9583`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:43:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:43:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 May 2020 09:44:15 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 May 2020 09:44:18 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 16 May 2020 09:44:18 GMT
ENV KAPACITOR_VERSION=1.4.1
# Sat, 16 May 2020 09:44:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Sat, 16 May 2020 09:44:22 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 May 2020 09:44:22 GMT
EXPOSE 9092
# Sat, 16 May 2020 09:44:22 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 May 2020 09:44:23 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 May 2020 09:44:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 May 2020 09:44:23 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194b0e3c928807cfabf081055a117585ba5bf6697f65b2fede02225a5d73ad2`  
		Last Modified: Fri, 15 May 2020 17:55:27 GMT  
		Size: 10.8 MB (10797475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec00f35d5b2d1db6b8e925a3005c1a285365775028db0339903ddaeec4763`  
		Last Modified: Fri, 15 May 2020 17:55:29 GMT  
		Size: 4.3 MB (4340139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2384f0606b9fbbbd98395f99922e252f11cfa34e5a6630c12b5f0487f7f17011`  
		Last Modified: Sat, 16 May 2020 09:44:50 GMT  
		Size: 13.1 MB (13102550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c2bdba4f53fc9ba35acf2ec0682e9c71eabd9e0ea0f1e02e575885c572d2f`  
		Last Modified: Sat, 16 May 2020 09:44:48 GMT  
		Size: 2.8 KB (2774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604e999c809dd29a15a05b380ff888ce5d8f2f4e59d91dfd050a3b24ff298fe2`  
		Last Modified: Sat, 16 May 2020 09:44:54 GMT  
		Size: 22.7 MB (22694274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3cafb0bf044554bd54be0f8981c8e86298c073d30e66351d812cb533cf724c`  
		Last Modified: Sat, 16 May 2020 09:44:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306e48e47a264276ae324de2ff43768409fed2ec821ab689a45b357565f045d1`  
		Last Modified: Sat, 16 May 2020 09:44:49 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4.1` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:823e316a4f5672a190699d9f2ab890c493682e4d1dc1d185716c939b4cfa790d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90105866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6065c9640a8944eab61fa36140c014c1a8064ad79ec6f7bf19d199f7a3a1802`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 15 May 2020 01:06:22 GMT
ADD file:89db8453485648b09e63411b6e2ad84f08844ee55cb115e59cdc8c8cb1c29a1f in / 
# Fri, 15 May 2020 01:06:23 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:49:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 May 2020 02:59:29 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 May 2020 02:59:33 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 16 May 2020 02:59:34 GMT
ENV KAPACITOR_VERSION=1.4.1
# Sat, 16 May 2020 02:59:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Sat, 16 May 2020 02:59:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 May 2020 02:59:42 GMT
EXPOSE 9092
# Sat, 16 May 2020 02:59:43 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 May 2020 02:59:43 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 May 2020 02:59:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 May 2020 02:59:45 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:11acdea2de14253903f5970d63a2076ff08912929430d1c33afe617c9fa6bf8f`  
		Last Modified: Fri, 15 May 2020 01:14:46 GMT  
		Size: 42.1 MB (42104346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99452f66748f5df5d89d2287e42b5c3d87c9d5e1e20c16ef729e87d463840cf7`  
		Last Modified: Fri, 15 May 2020 11:01:44 GMT  
		Size: 9.5 MB (9498344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cef06b7abe4487657829b47c97bd2992f14a34349e0bcf60a47de9c647bd3fb`  
		Last Modified: Fri, 15 May 2020 11:01:43 GMT  
		Size: 3.9 MB (3918713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a816593387c5d1c32f87e1b3c413dae1dab2eac6f8cac7fc43e22b5bc254d83a`  
		Last Modified: Sat, 16 May 2020 03:00:17 GMT  
		Size: 13.3 MB (13273150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f9f5d8409ab5c24f4eab5db4236913a69ccff0e5a81d55a07ebd7f0ab7d667`  
		Last Modified: Sat, 16 May 2020 03:00:15 GMT  
		Size: 2.8 KB (2800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2be052f14cc6dc85ac4caa6ab76b9980b6eda80c75096aa09b88d4b35329d4`  
		Last Modified: Sat, 16 May 2020 03:00:23 GMT  
		Size: 21.3 MB (21308058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa76ff55ba46eed7ab380121ad38cb6f0ce2d08c3a431219db617fa0dac1a4b7`  
		Last Modified: Sat, 16 May 2020 03:00:14 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff2ec7a40e713216d50469d7520cd8d49bee5268201da0058bb61d2ae139aab`  
		Last Modified: Sat, 16 May 2020 03:00:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4.1` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:713703deb731265acade7afed50311b80f35a36b7d2e8ed5e1374bdf97814374
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91115917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ee14f22ea080d997c490f655244403d7e176b684a72849366028aa4f73794f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 18:20:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 23 Apr 2020 18:20:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 18:20:25 GMT
ENV KAPACITOR_VERSION=1.4.1
# Thu, 23 Apr 2020 18:20:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Thu, 23 Apr 2020 18:20:31 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 23 Apr 2020 18:20:31 GMT
EXPOSE 9092
# Thu, 23 Apr 2020 18:20:32 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 23 Apr 2020 18:20:33 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 23 Apr 2020 18:20:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 18:20:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2880f01126539717a8c176ecd9f66045832497fe1667dd1fe5eb10a99fa72b`  
		Last Modified: Thu, 23 Apr 2020 18:21:04 GMT  
		Size: 12.8 MB (12802819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f2b353fcdc47aa924ac04a3ffe383df13c8d2f97929e24492cb9dcb3718bb2`  
		Last Modified: Thu, 23 Apr 2020 18:21:02 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e75eaf09fdc3ceade56b3689d8b1f7dbc79c35563ec4083d6b64b5ae873fc0`  
		Last Modified: Thu, 23 Apr 2020 18:21:09 GMT  
		Size: 21.3 MB (21307845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92643273a3e2204522977ea783d691d24c924dcefdcf0f71ae0e95343e1f4b05`  
		Last Modified: Thu, 23 Apr 2020 18:21:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c467a0f82f0e479e58a4fc7a762623df12c48d5a15eff4eb41790a55b94bfd`  
		Last Modified: Thu, 23 Apr 2020 18:21:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4.1-alpine`

```console
$ docker pull kapacitor@sha256:8b0f86288ce5e80c0945fbb24a5f5d7aa5129fb48c6623697613113ba262c26e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.4.1-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:c7b1106644920eb2f651cfad13d77f603d62ffaf2aeab6876104da4827f36199
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.7 MB (19673755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6c8025603ebb4b75bfe5509147b8534d99582e3964158ca0ba0046f2b8bae4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 14:41:51 GMT
ENV KAPACITOR_VERSION=1.4.1
# Fri, 24 Apr 2020 14:41:55 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:41:56 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 24 Apr 2020 14:41:56 GMT
EXPOSE 9092
# Fri, 24 Apr 2020 14:41:56 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 24 Apr 2020 14:41:56 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 24 Apr 2020 14:41:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:41:57 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85169d009bd5f0c0ab3d615ff03bc83196402a467630fd52b525956c374af54`  
		Last Modified: Fri, 24 Apr 2020 14:42:25 GMT  
		Size: 16.6 MB (16598643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255366c4ce6923eee6adadbec2d9183c32883ccbb872f78f55012ca66353ef28`  
		Last Modified: Fri, 24 Apr 2020 14:42:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0fb6e436ba41bf7cfedcc84ac2aa94b71cf21e4a8bdea8a172cc1d441dd954`  
		Last Modified: Fri, 24 Apr 2020 14:42:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4-alpine`

```console
$ docker pull kapacitor@sha256:8b0f86288ce5e80c0945fbb24a5f5d7aa5129fb48c6623697613113ba262c26e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.4-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:c7b1106644920eb2f651cfad13d77f603d62ffaf2aeab6876104da4827f36199
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.7 MB (19673755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6c8025603ebb4b75bfe5509147b8534d99582e3964158ca0ba0046f2b8bae4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 14:41:51 GMT
ENV KAPACITOR_VERSION=1.4.1
# Fri, 24 Apr 2020 14:41:55 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:41:56 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 24 Apr 2020 14:41:56 GMT
EXPOSE 9092
# Fri, 24 Apr 2020 14:41:56 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 24 Apr 2020 14:41:56 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 24 Apr 2020 14:41:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:41:57 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85169d009bd5f0c0ab3d615ff03bc83196402a467630fd52b525956c374af54`  
		Last Modified: Fri, 24 Apr 2020 14:42:25 GMT  
		Size: 16.6 MB (16598643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255366c4ce6923eee6adadbec2d9183c32883ccbb872f78f55012ca66353ef28`  
		Last Modified: Fri, 24 Apr 2020 14:42:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0fb6e436ba41bf7cfedcc84ac2aa94b71cf21e4a8bdea8a172cc1d441dd954`  
		Last Modified: Fri, 24 Apr 2020 14:42:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5`

```console
$ docker pull kapacitor@sha256:1c8a4a6e154f2869f9aee0f482d0f7fd0df992345803194b528c4eb813449fb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:7a2b9ba6e6eeb9ea3449effbe4e7144537561758ede01448748bf6ca957ef09d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109929194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354e9f82dd3b6d2f79a7fb61178456e18a6c636a9d384b130e8a375da94bf0c6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:43:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:43:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 May 2020 09:44:15 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 May 2020 09:44:18 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 16 May 2020 09:44:31 GMT
ENV KAPACITOR_VERSION=1.5.4
# Sat, 16 May 2020 09:44:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 16 May 2020 09:44:35 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 May 2020 09:44:35 GMT
EXPOSE 9092
# Sat, 16 May 2020 09:44:35 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 May 2020 09:44:36 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 May 2020 09:44:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 May 2020 09:44:36 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194b0e3c928807cfabf081055a117585ba5bf6697f65b2fede02225a5d73ad2`  
		Last Modified: Fri, 15 May 2020 17:55:27 GMT  
		Size: 10.8 MB (10797475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec00f35d5b2d1db6b8e925a3005c1a285365775028db0339903ddaeec4763`  
		Last Modified: Fri, 15 May 2020 17:55:29 GMT  
		Size: 4.3 MB (4340139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2384f0606b9fbbbd98395f99922e252f11cfa34e5a6630c12b5f0487f7f17011`  
		Last Modified: Sat, 16 May 2020 09:44:50 GMT  
		Size: 13.1 MB (13102550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c2bdba4f53fc9ba35acf2ec0682e9c71eabd9e0ea0f1e02e575885c572d2f`  
		Last Modified: Sat, 16 May 2020 09:44:48 GMT  
		Size: 2.8 KB (2774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7da84fef47ce03360225d6d24cc691e5063e12b3bfdf12faa2a55970d8390b1`  
		Last Modified: Sat, 16 May 2020 09:45:04 GMT  
		Size: 36.3 MB (36310594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517f8a9626dbb2ed33f0765a392b9c6ff226301b0ec73018270ce740e4b222c5`  
		Last Modified: Sat, 16 May 2020 09:44:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7cba1fa962e0ffc68caa8d1fa5f066cb67b94e5f2e079147d57aa6574a6569`  
		Last Modified: Sat, 16 May 2020 09:44:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:63d2430fce8cc768570bbb894708435372513097b2de8cecdf48b2b677e9c8e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102847059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665e8ba1bf1a659f5c1c01caf4b02c6f31705c12f7bd911280d56f7cedb82ace`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 15 May 2020 01:06:22 GMT
ADD file:89db8453485648b09e63411b6e2ad84f08844ee55cb115e59cdc8c8cb1c29a1f in / 
# Fri, 15 May 2020 01:06:23 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:49:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 May 2020 02:59:29 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 May 2020 02:59:33 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 16 May 2020 02:59:54 GMT
ENV KAPACITOR_VERSION=1.5.4
# Sat, 16 May 2020 03:00:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 16 May 2020 03:00:02 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 May 2020 03:00:02 GMT
EXPOSE 9092
# Sat, 16 May 2020 03:00:03 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 May 2020 03:00:04 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 May 2020 03:00:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 May 2020 03:00:05 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:11acdea2de14253903f5970d63a2076ff08912929430d1c33afe617c9fa6bf8f`  
		Last Modified: Fri, 15 May 2020 01:14:46 GMT  
		Size: 42.1 MB (42104346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99452f66748f5df5d89d2287e42b5c3d87c9d5e1e20c16ef729e87d463840cf7`  
		Last Modified: Fri, 15 May 2020 11:01:44 GMT  
		Size: 9.5 MB (9498344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cef06b7abe4487657829b47c97bd2992f14a34349e0bcf60a47de9c647bd3fb`  
		Last Modified: Fri, 15 May 2020 11:01:43 GMT  
		Size: 3.9 MB (3918713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a816593387c5d1c32f87e1b3c413dae1dab2eac6f8cac7fc43e22b5bc254d83a`  
		Last Modified: Sat, 16 May 2020 03:00:17 GMT  
		Size: 13.3 MB (13273150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f9f5d8409ab5c24f4eab5db4236913a69ccff0e5a81d55a07ebd7f0ab7d667`  
		Last Modified: Sat, 16 May 2020 03:00:15 GMT  
		Size: 2.8 KB (2800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad1c5af560275a2322b9d0b8f2ae98928c12d432fdbf72076f57d84f59204d4`  
		Last Modified: Sat, 16 May 2020 03:00:38 GMT  
		Size: 34.0 MB (34049250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bf083077ea9238021be2679fa65ddaf3219e42633b5ee348ee1d918c165dae`  
		Last Modified: Sat, 16 May 2020 03:00:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad01ef573af25fe0eb944fec1b96237dbc87bbadc0f9e0d137fc0d9e45c71ee5`  
		Last Modified: Sat, 16 May 2020 03:00:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:faf2e9845b58a62ee345c1ac1a18ce80d28393cae6070b436d9ae495248810ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103857121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38fb7c1c936e9dfbbb6dd71f82b08f912f92ecef4b95eab26ec165df9e76a4db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 18:20:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 23 Apr 2020 18:20:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 18:20:42 GMT
ENV KAPACITOR_VERSION=1.5.4
# Thu, 23 Apr 2020 18:20:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 18:20:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 23 Apr 2020 18:20:48 GMT
EXPOSE 9092
# Thu, 23 Apr 2020 18:20:49 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 23 Apr 2020 18:20:49 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 23 Apr 2020 18:20:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 18:20:51 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2880f01126539717a8c176ecd9f66045832497fe1667dd1fe5eb10a99fa72b`  
		Last Modified: Thu, 23 Apr 2020 18:21:04 GMT  
		Size: 12.8 MB (12802819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f2b353fcdc47aa924ac04a3ffe383df13c8d2f97929e24492cb9dcb3718bb2`  
		Last Modified: Thu, 23 Apr 2020 18:21:02 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e87f0f1b8489d397a75f6381e4ddb5a9ee33a1e74c062d999e10a64bbfaef5`  
		Last Modified: Thu, 23 Apr 2020 18:21:24 GMT  
		Size: 34.0 MB (34049049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10c08087d948bb3c77899d0d0f6c98bb2bb6a52a92bbe94a77b32493d88aefe`  
		Last Modified: Thu, 23 Apr 2020 18:21:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adefabb4a902a578e48ff5c0f5de3c681c7c011a62a1ed198709b99ef63d72f`  
		Last Modified: Thu, 23 Apr 2020 18:21:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.4`

```console
$ docker pull kapacitor@sha256:1c8a4a6e154f2869f9aee0f482d0f7fd0df992345803194b528c4eb813449fb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.4` - linux; amd64

```console
$ docker pull kapacitor@sha256:7a2b9ba6e6eeb9ea3449effbe4e7144537561758ede01448748bf6ca957ef09d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109929194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354e9f82dd3b6d2f79a7fb61178456e18a6c636a9d384b130e8a375da94bf0c6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:43:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:43:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 May 2020 09:44:15 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 May 2020 09:44:18 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 16 May 2020 09:44:31 GMT
ENV KAPACITOR_VERSION=1.5.4
# Sat, 16 May 2020 09:44:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 16 May 2020 09:44:35 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 May 2020 09:44:35 GMT
EXPOSE 9092
# Sat, 16 May 2020 09:44:35 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 May 2020 09:44:36 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 May 2020 09:44:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 May 2020 09:44:36 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194b0e3c928807cfabf081055a117585ba5bf6697f65b2fede02225a5d73ad2`  
		Last Modified: Fri, 15 May 2020 17:55:27 GMT  
		Size: 10.8 MB (10797475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec00f35d5b2d1db6b8e925a3005c1a285365775028db0339903ddaeec4763`  
		Last Modified: Fri, 15 May 2020 17:55:29 GMT  
		Size: 4.3 MB (4340139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2384f0606b9fbbbd98395f99922e252f11cfa34e5a6630c12b5f0487f7f17011`  
		Last Modified: Sat, 16 May 2020 09:44:50 GMT  
		Size: 13.1 MB (13102550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c2bdba4f53fc9ba35acf2ec0682e9c71eabd9e0ea0f1e02e575885c572d2f`  
		Last Modified: Sat, 16 May 2020 09:44:48 GMT  
		Size: 2.8 KB (2774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7da84fef47ce03360225d6d24cc691e5063e12b3bfdf12faa2a55970d8390b1`  
		Last Modified: Sat, 16 May 2020 09:45:04 GMT  
		Size: 36.3 MB (36310594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517f8a9626dbb2ed33f0765a392b9c6ff226301b0ec73018270ce740e4b222c5`  
		Last Modified: Sat, 16 May 2020 09:44:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7cba1fa962e0ffc68caa8d1fa5f066cb67b94e5f2e079147d57aa6574a6569`  
		Last Modified: Sat, 16 May 2020 09:44:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.4` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:63d2430fce8cc768570bbb894708435372513097b2de8cecdf48b2b677e9c8e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102847059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665e8ba1bf1a659f5c1c01caf4b02c6f31705c12f7bd911280d56f7cedb82ace`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 15 May 2020 01:06:22 GMT
ADD file:89db8453485648b09e63411b6e2ad84f08844ee55cb115e59cdc8c8cb1c29a1f in / 
# Fri, 15 May 2020 01:06:23 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:49:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 May 2020 02:59:29 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 May 2020 02:59:33 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 16 May 2020 02:59:54 GMT
ENV KAPACITOR_VERSION=1.5.4
# Sat, 16 May 2020 03:00:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 16 May 2020 03:00:02 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 May 2020 03:00:02 GMT
EXPOSE 9092
# Sat, 16 May 2020 03:00:03 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 May 2020 03:00:04 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 May 2020 03:00:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 May 2020 03:00:05 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:11acdea2de14253903f5970d63a2076ff08912929430d1c33afe617c9fa6bf8f`  
		Last Modified: Fri, 15 May 2020 01:14:46 GMT  
		Size: 42.1 MB (42104346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99452f66748f5df5d89d2287e42b5c3d87c9d5e1e20c16ef729e87d463840cf7`  
		Last Modified: Fri, 15 May 2020 11:01:44 GMT  
		Size: 9.5 MB (9498344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cef06b7abe4487657829b47c97bd2992f14a34349e0bcf60a47de9c647bd3fb`  
		Last Modified: Fri, 15 May 2020 11:01:43 GMT  
		Size: 3.9 MB (3918713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a816593387c5d1c32f87e1b3c413dae1dab2eac6f8cac7fc43e22b5bc254d83a`  
		Last Modified: Sat, 16 May 2020 03:00:17 GMT  
		Size: 13.3 MB (13273150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f9f5d8409ab5c24f4eab5db4236913a69ccff0e5a81d55a07ebd7f0ab7d667`  
		Last Modified: Sat, 16 May 2020 03:00:15 GMT  
		Size: 2.8 KB (2800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad1c5af560275a2322b9d0b8f2ae98928c12d432fdbf72076f57d84f59204d4`  
		Last Modified: Sat, 16 May 2020 03:00:38 GMT  
		Size: 34.0 MB (34049250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bf083077ea9238021be2679fa65ddaf3219e42633b5ee348ee1d918c165dae`  
		Last Modified: Sat, 16 May 2020 03:00:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad01ef573af25fe0eb944fec1b96237dbc87bbadc0f9e0d137fc0d9e45c71ee5`  
		Last Modified: Sat, 16 May 2020 03:00:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.4` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:faf2e9845b58a62ee345c1ac1a18ce80d28393cae6070b436d9ae495248810ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103857121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38fb7c1c936e9dfbbb6dd71f82b08f912f92ecef4b95eab26ec165df9e76a4db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 18:20:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 23 Apr 2020 18:20:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 18:20:42 GMT
ENV KAPACITOR_VERSION=1.5.4
# Thu, 23 Apr 2020 18:20:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 18:20:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 23 Apr 2020 18:20:48 GMT
EXPOSE 9092
# Thu, 23 Apr 2020 18:20:49 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 23 Apr 2020 18:20:49 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 23 Apr 2020 18:20:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 18:20:51 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2880f01126539717a8c176ecd9f66045832497fe1667dd1fe5eb10a99fa72b`  
		Last Modified: Thu, 23 Apr 2020 18:21:04 GMT  
		Size: 12.8 MB (12802819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f2b353fcdc47aa924ac04a3ffe383df13c8d2f97929e24492cb9dcb3718bb2`  
		Last Modified: Thu, 23 Apr 2020 18:21:02 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e87f0f1b8489d397a75f6381e4ddb5a9ee33a1e74c062d999e10a64bbfaef5`  
		Last Modified: Thu, 23 Apr 2020 18:21:24 GMT  
		Size: 34.0 MB (34049049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10c08087d948bb3c77899d0d0f6c98bb2bb6a52a92bbe94a77b32493d88aefe`  
		Last Modified: Thu, 23 Apr 2020 18:21:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adefabb4a902a578e48ff5c0f5de3c681c7c011a62a1ed198709b99ef63d72f`  
		Last Modified: Thu, 23 Apr 2020 18:21:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.4-alpine`

```console
$ docker pull kapacitor@sha256:5a15b4f278b22929cf11ebc0c58e717f6600349de81e6ca80d37316a5f265cac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.5.4-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:aa605c5e74ff149da7d84f26a0d79ae92ae12038ce4086343482769df205e973
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23100428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cacac6e6e047ea1cb9bbd65a0aac14f532c60c336f82dad553a938c07548fbf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 14:42:04 GMT
ENV KAPACITOR_VERSION=1.5.4
# Fri, 24 Apr 2020 14:42:08 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:42:08 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 24 Apr 2020 14:42:09 GMT
EXPOSE 9092
# Fri, 24 Apr 2020 14:42:09 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 24 Apr 2020 14:42:09 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 24 Apr 2020 14:42:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:42:09 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161ba29b8c4be210a2aa0d6aff44ea1a8e7654e8a76c5c49cd153af81c6fccc8`  
		Last Modified: Fri, 24 Apr 2020 14:42:32 GMT  
		Size: 20.0 MB (20025317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4451a41250e65170a52cf51e2d450bd5fd2b0ef564f5775e45079116b08e31`  
		Last Modified: Fri, 24 Apr 2020 14:42:29 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ee9620905de433be23893da5c25b38efa5c05ea4d28122e98137b6c7d1e37a`  
		Last Modified: Fri, 24 Apr 2020 14:42:29 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:5a15b4f278b22929cf11ebc0c58e717f6600349de81e6ca80d37316a5f265cac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:aa605c5e74ff149da7d84f26a0d79ae92ae12038ce4086343482769df205e973
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23100428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cacac6e6e047ea1cb9bbd65a0aac14f532c60c336f82dad553a938c07548fbf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 14:42:04 GMT
ENV KAPACITOR_VERSION=1.5.4
# Fri, 24 Apr 2020 14:42:08 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:42:08 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 24 Apr 2020 14:42:09 GMT
EXPOSE 9092
# Fri, 24 Apr 2020 14:42:09 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 24 Apr 2020 14:42:09 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 24 Apr 2020 14:42:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:42:09 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161ba29b8c4be210a2aa0d6aff44ea1a8e7654e8a76c5c49cd153af81c6fccc8`  
		Last Modified: Fri, 24 Apr 2020 14:42:32 GMT  
		Size: 20.0 MB (20025317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4451a41250e65170a52cf51e2d450bd5fd2b0ef564f5775e45079116b08e31`  
		Last Modified: Fri, 24 Apr 2020 14:42:29 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ee9620905de433be23893da5c25b38efa5c05ea4d28122e98137b6c7d1e37a`  
		Last Modified: Fri, 24 Apr 2020 14:42:29 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:5a15b4f278b22929cf11ebc0c58e717f6600349de81e6ca80d37316a5f265cac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:aa605c5e74ff149da7d84f26a0d79ae92ae12038ce4086343482769df205e973
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23100428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cacac6e6e047ea1cb9bbd65a0aac14f532c60c336f82dad553a938c07548fbf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:15:55 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 24 Apr 2020 14:42:04 GMT
ENV KAPACITOR_VERSION=1.5.4
# Fri, 24 Apr 2020 14:42:08 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:42:08 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 24 Apr 2020 14:42:09 GMT
EXPOSE 9092
# Fri, 24 Apr 2020 14:42:09 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 24 Apr 2020 14:42:09 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 24 Apr 2020 14:42:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:42:09 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c949b60b63fb4b31e70314aba2aff2223f42a54c0d76cdb28917f161840b03`  
		Last Modified: Fri, 24 Apr 2020 14:16:39 GMT  
		Size: 301.1 KB (301092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161ba29b8c4be210a2aa0d6aff44ea1a8e7654e8a76c5c49cd153af81c6fccc8`  
		Last Modified: Fri, 24 Apr 2020 14:42:32 GMT  
		Size: 20.0 MB (20025317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4451a41250e65170a52cf51e2d450bd5fd2b0ef564f5775e45079116b08e31`  
		Last Modified: Fri, 24 Apr 2020 14:42:29 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ee9620905de433be23893da5c25b38efa5c05ea4d28122e98137b6c7d1e37a`  
		Last Modified: Fri, 24 Apr 2020 14:42:29 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:1c8a4a6e154f2869f9aee0f482d0f7fd0df992345803194b528c4eb813449fb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:7a2b9ba6e6eeb9ea3449effbe4e7144537561758ede01448748bf6ca957ef09d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109929194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354e9f82dd3b6d2f79a7fb61178456e18a6c636a9d384b130e8a375da94bf0c6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:43:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:43:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 May 2020 09:44:15 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 May 2020 09:44:18 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 16 May 2020 09:44:31 GMT
ENV KAPACITOR_VERSION=1.5.4
# Sat, 16 May 2020 09:44:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 16 May 2020 09:44:35 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 May 2020 09:44:35 GMT
EXPOSE 9092
# Sat, 16 May 2020 09:44:35 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 May 2020 09:44:36 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 May 2020 09:44:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 May 2020 09:44:36 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194b0e3c928807cfabf081055a117585ba5bf6697f65b2fede02225a5d73ad2`  
		Last Modified: Fri, 15 May 2020 17:55:27 GMT  
		Size: 10.8 MB (10797475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec00f35d5b2d1db6b8e925a3005c1a285365775028db0339903ddaeec4763`  
		Last Modified: Fri, 15 May 2020 17:55:29 GMT  
		Size: 4.3 MB (4340139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2384f0606b9fbbbd98395f99922e252f11cfa34e5a6630c12b5f0487f7f17011`  
		Last Modified: Sat, 16 May 2020 09:44:50 GMT  
		Size: 13.1 MB (13102550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c2bdba4f53fc9ba35acf2ec0682e9c71eabd9e0ea0f1e02e575885c572d2f`  
		Last Modified: Sat, 16 May 2020 09:44:48 GMT  
		Size: 2.8 KB (2774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7da84fef47ce03360225d6d24cc691e5063e12b3bfdf12faa2a55970d8390b1`  
		Last Modified: Sat, 16 May 2020 09:45:04 GMT  
		Size: 36.3 MB (36310594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517f8a9626dbb2ed33f0765a392b9c6ff226301b0ec73018270ce740e4b222c5`  
		Last Modified: Sat, 16 May 2020 09:44:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7cba1fa962e0ffc68caa8d1fa5f066cb67b94e5f2e079147d57aa6574a6569`  
		Last Modified: Sat, 16 May 2020 09:44:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:63d2430fce8cc768570bbb894708435372513097b2de8cecdf48b2b677e9c8e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102847059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665e8ba1bf1a659f5c1c01caf4b02c6f31705c12f7bd911280d56f7cedb82ace`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 15 May 2020 01:06:22 GMT
ADD file:89db8453485648b09e63411b6e2ad84f08844ee55cb115e59cdc8c8cb1c29a1f in / 
# Fri, 15 May 2020 01:06:23 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:49:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 May 2020 02:59:29 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 16 May 2020 02:59:33 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 16 May 2020 02:59:54 GMT
ENV KAPACITOR_VERSION=1.5.4
# Sat, 16 May 2020 03:00:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 16 May 2020 03:00:02 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 16 May 2020 03:00:02 GMT
EXPOSE 9092
# Sat, 16 May 2020 03:00:03 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 16 May 2020 03:00:04 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 16 May 2020 03:00:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 May 2020 03:00:05 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:11acdea2de14253903f5970d63a2076ff08912929430d1c33afe617c9fa6bf8f`  
		Last Modified: Fri, 15 May 2020 01:14:46 GMT  
		Size: 42.1 MB (42104346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99452f66748f5df5d89d2287e42b5c3d87c9d5e1e20c16ef729e87d463840cf7`  
		Last Modified: Fri, 15 May 2020 11:01:44 GMT  
		Size: 9.5 MB (9498344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cef06b7abe4487657829b47c97bd2992f14a34349e0bcf60a47de9c647bd3fb`  
		Last Modified: Fri, 15 May 2020 11:01:43 GMT  
		Size: 3.9 MB (3918713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a816593387c5d1c32f87e1b3c413dae1dab2eac6f8cac7fc43e22b5bc254d83a`  
		Last Modified: Sat, 16 May 2020 03:00:17 GMT  
		Size: 13.3 MB (13273150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f9f5d8409ab5c24f4eab5db4236913a69ccff0e5a81d55a07ebd7f0ab7d667`  
		Last Modified: Sat, 16 May 2020 03:00:15 GMT  
		Size: 2.8 KB (2800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad1c5af560275a2322b9d0b8f2ae98928c12d432fdbf72076f57d84f59204d4`  
		Last Modified: Sat, 16 May 2020 03:00:38 GMT  
		Size: 34.0 MB (34049250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bf083077ea9238021be2679fa65ddaf3219e42633b5ee348ee1d918c165dae`  
		Last Modified: Sat, 16 May 2020 03:00:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad01ef573af25fe0eb944fec1b96237dbc87bbadc0f9e0d137fc0d9e45c71ee5`  
		Last Modified: Sat, 16 May 2020 03:00:30 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:faf2e9845b58a62ee345c1ac1a18ce80d28393cae6070b436d9ae495248810ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103857121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38fb7c1c936e9dfbbb6dd71f82b08f912f92ecef4b95eab26ec165df9e76a4db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 18:20:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 23 Apr 2020 18:20:24 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 18:20:42 GMT
ENV KAPACITOR_VERSION=1.5.4
# Thu, 23 Apr 2020 18:20:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 18:20:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 23 Apr 2020 18:20:48 GMT
EXPOSE 9092
# Thu, 23 Apr 2020 18:20:49 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 23 Apr 2020 18:20:49 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 23 Apr 2020 18:20:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 18:20:51 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2880f01126539717a8c176ecd9f66045832497fe1667dd1fe5eb10a99fa72b`  
		Last Modified: Thu, 23 Apr 2020 18:21:04 GMT  
		Size: 12.8 MB (12802819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f2b353fcdc47aa924ac04a3ffe383df13c8d2f97929e24492cb9dcb3718bb2`  
		Last Modified: Thu, 23 Apr 2020 18:21:02 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e87f0f1b8489d397a75f6381e4ddb5a9ee33a1e74c062d999e10a64bbfaef5`  
		Last Modified: Thu, 23 Apr 2020 18:21:24 GMT  
		Size: 34.0 MB (34049049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10c08087d948bb3c77899d0d0f6c98bb2bb6a52a92bbe94a77b32493d88aefe`  
		Last Modified: Thu, 23 Apr 2020 18:21:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adefabb4a902a578e48ff5c0f5de3c681c7c011a62a1ed198709b99ef63d72f`  
		Last Modified: Thu, 23 Apr 2020 18:21:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
