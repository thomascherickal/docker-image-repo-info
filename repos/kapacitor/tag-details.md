<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.4`](#kapacitor14)
-	[`kapacitor:1.4.1`](#kapacitor141)
-	[`kapacitor:1.4.1-alpine`](#kapacitor141-alpine)
-	[`kapacitor:1.4-alpine`](#kapacitor14-alpine)
-	[`kapacitor:1.5`](#kapacitor15)
-	[`kapacitor:1.5.7`](#kapacitor157)
-	[`kapacitor:1.5.7-alpine`](#kapacitor157-alpine)
-	[`kapacitor:1.5-alpine`](#kapacitor15-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.4`

```console
$ docker pull kapacitor@sha256:adfd48bb0308ddfaf4097c457c256a9c870eb058a2e9299e343c8396ee642ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.4` - linux; amd64

```console
$ docker pull kapacitor@sha256:9f09b94d08a0d7e4d5bd663c0ae501512c8d20c51966f3705607178e4a5cdf5a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96375452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e282dd1718c5f785db309af503da65dc83b59f32e080d704d086ba58f129833`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:10 GMT
ADD file:373a8875589f170b51fa677a3bf736feeb46ea278c553950a3eb3169a2056c12 in / 
# Tue, 17 Nov 2020 20:24:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:43:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 19 Nov 2020 02:58:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 19 Nov 2020 02:58:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 19 Nov 2020 02:58:11 GMT
ENV KAPACITOR_VERSION=1.4.1
# Thu, 19 Nov 2020 02:58:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Thu, 19 Nov 2020 02:58:15 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 19 Nov 2020 02:58:15 GMT
EXPOSE 9092
# Thu, 19 Nov 2020 02:58:15 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 19 Nov 2020 02:58:15 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 19 Nov 2020 02:58:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Nov 2020 02:58:16 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:7919f5b7d60254cafc73c0d097b8ccffb72e0b6472957ece4dd5b378c5ca7cc1`  
		Last Modified: Tue, 17 Nov 2020 20:30:26 GMT  
		Size: 45.4 MB (45377037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e107167dcc5392ce7b34cb6af6bcfe1cf99f76f9e632d6c321526666558ab50`  
		Last Modified: Wed, 18 Nov 2020 00:54:39 GMT  
		Size: 10.8 MB (10752152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a456bba435b99e4c17dd5da957e63bef2c43ae5291b055ce82bd26d9153259`  
		Last Modified: Wed, 18 Nov 2020 00:54:37 GMT  
		Size: 4.3 MB (4340590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b048cb94809123b7360b06fcf7cdc40f6db32b7e4679612eb80812f9281589cc`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 13.2 MB (13208088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315e803a7acf0a2f7ea0534d3b00789832611a9209e0a52609039a760e3acc5c`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 2.8 KB (2827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecab6aded49c4d7c910b757fbc7ee91f7d4a2473e51bdd467bd86c4099af47f4`  
		Last Modified: Thu, 19 Nov 2020 02:58:50 GMT  
		Size: 22.7 MB (22694300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e746b6caad54a6b61d3b8a7a590882748257976204823ae9fd002cb779e2dfc3`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba68761006b14d29e7cd46a5114f64de970e2b79872c600da4729cd6d3f388b5`  
		Last Modified: Thu, 19 Nov 2020 02:58:44 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:86fa5b92eba32671d5c1c210cf6be710cfa680320ce6e9a711436ddf103c7b56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efd75b9bba9f77c5058b6c71b26d9605875feae327ce9c5932cb9f0a8783764c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:06 GMT
ADD file:e74dce76704e3faa6198db5cf4192fd431f5addf55f658277eb5b60d254fee8e in / 
# Fri, 11 Dec 2020 02:28:09 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:35:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:35:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 12 Dec 2020 07:16:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 12 Dec 2020 07:16:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 12 Dec 2020 07:16:40 GMT
ENV KAPACITOR_VERSION=1.4.1
# Sat, 12 Dec 2020 07:16:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Sat, 12 Dec 2020 07:16:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 12 Dec 2020 07:16:48 GMT
EXPOSE 9092
# Sat, 12 Dec 2020 07:16:49 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 12 Dec 2020 07:16:50 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 12 Dec 2020 07:16:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Dec 2020 07:16:52 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:062f5403576d7e3aca1c92115ff0a9ea110b270cb0b61013efa86744515666fb`  
		Last Modified: Fri, 11 Dec 2020 02:36:48 GMT  
		Size: 42.1 MB (42117949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5385e34f58366fad1da017d000782de279c46cc834d767686d02d13a59a570`  
		Last Modified: Fri, 11 Dec 2020 16:47:26 GMT  
		Size: 9.4 MB (9444537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba7ef5d6926f92eb8533178d7f708c2e385991e7d97edb8e2433c518f252af7`  
		Last Modified: Fri, 11 Dec 2020 16:47:24 GMT  
		Size: 3.9 MB (3920019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b78f5775b143974c905677d6d57824a7d9c1df56b0c5beb0b04042bdeee0ed`  
		Last Modified: Sat, 12 Dec 2020 07:17:28 GMT  
		Size: 13.4 MB (13428938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad9b956ce07ac5f129c4adcba522b127cc8c115e2cc3392a4e4f576c99416f6`  
		Last Modified: Sat, 12 Dec 2020 07:17:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293215cc916f1d4cf42444ccbd6cca8a35ff8384f195db76af5950bca67af03f`  
		Last Modified: Sat, 12 Dec 2020 07:17:33 GMT  
		Size: 21.3 MB (21308107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4ce82ef03670997fc776bf4fd4684b8d58f4f764d9728057e3feb2b4ba563d`  
		Last Modified: Sat, 12 Dec 2020 07:17:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a2800a03e7f95087381d5ebb2aa2fb66b43ab9241f422a16e0234371419e1a`  
		Last Modified: Sat, 12 Dec 2020 07:17:25 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:3916c73f5ba4c32ae47bea8722f22af38051805bc8d57326f4a16c78db75522f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91197712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a7d2880c5eb1442b3e42d4a9e2254d4f75bfffd663825f9ecc38b51f0a29b13`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:33 GMT
ADD file:d2e307c3e54ad69dff47f6bdacca7c8ee0957a09346bb21baec02b9de1a657e1 in / 
# Tue, 17 Nov 2020 20:27:37 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:28:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 21:14:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Nov 2020 21:15:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 18 Nov 2020 21:15:01 GMT
ENV KAPACITOR_VERSION=1.4.1
# Wed, 18 Nov 2020 21:15:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Wed, 18 Nov 2020 21:15:07 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Nov 2020 21:15:08 GMT
EXPOSE 9092
# Wed, 18 Nov 2020 21:15:09 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Nov 2020 21:15:09 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Nov 2020 21:15:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 21:15:11 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f99bf631c0ebddf9e32516b47bf6e198efc42d06c3eb86d6f5f5739757b5839c`  
		Last Modified: Tue, 17 Nov 2020 20:34:17 GMT  
		Size: 43.2 MB (43176009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a9b3adbe4ac4ca73818d8b79e94d2ff2b6ceafc1225d7c036ec4d384f0804a`  
		Last Modified: Tue, 17 Nov 2020 22:40:38 GMT  
		Size: 9.7 MB (9702292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052ba804da6ef34fd9dddf0ca298b1e0551ac8cf3ea14fc371fa1fa51cbd7f7c`  
		Last Modified: Tue, 17 Nov 2020 22:40:36 GMT  
		Size: 4.1 MB (4095219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d0115aaf8aea01788d62c5180c53c44f5b525f2a9dddfd2859576f55f219b`  
		Last Modified: Wed, 18 Nov 2020 21:15:45 GMT  
		Size: 12.9 MB (12912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f61bf00eecdaa1ba088593162e6892a588b4bdebc909c2cbf006fe9d2b0332a`  
		Last Modified: Wed, 18 Nov 2020 21:15:42 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c933cf9017283815ffdb326dc7a95075238243af1c7fd53f4c61817e3703dc3`  
		Last Modified: Wed, 18 Nov 2020 21:15:50 GMT  
		Size: 21.3 MB (21307888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d548a97c64cd97d4e4ba9b7d50b22f6f935279941bf7f54c467c5bb34c00cddc`  
		Last Modified: Wed, 18 Nov 2020 21:15:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c4c8e7573c067a188b43422916a291461da80c7cfd0294df4201b42235318b`  
		Last Modified: Wed, 18 Nov 2020 21:15:44 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4.1`

```console
$ docker pull kapacitor@sha256:adfd48bb0308ddfaf4097c457c256a9c870eb058a2e9299e343c8396ee642ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.4.1` - linux; amd64

```console
$ docker pull kapacitor@sha256:9f09b94d08a0d7e4d5bd663c0ae501512c8d20c51966f3705607178e4a5cdf5a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96375452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e282dd1718c5f785db309af503da65dc83b59f32e080d704d086ba58f129833`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:10 GMT
ADD file:373a8875589f170b51fa677a3bf736feeb46ea278c553950a3eb3169a2056c12 in / 
# Tue, 17 Nov 2020 20:24:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:43:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 19 Nov 2020 02:58:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 19 Nov 2020 02:58:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 19 Nov 2020 02:58:11 GMT
ENV KAPACITOR_VERSION=1.4.1
# Thu, 19 Nov 2020 02:58:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Thu, 19 Nov 2020 02:58:15 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 19 Nov 2020 02:58:15 GMT
EXPOSE 9092
# Thu, 19 Nov 2020 02:58:15 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 19 Nov 2020 02:58:15 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 19 Nov 2020 02:58:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Nov 2020 02:58:16 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:7919f5b7d60254cafc73c0d097b8ccffb72e0b6472957ece4dd5b378c5ca7cc1`  
		Last Modified: Tue, 17 Nov 2020 20:30:26 GMT  
		Size: 45.4 MB (45377037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e107167dcc5392ce7b34cb6af6bcfe1cf99f76f9e632d6c321526666558ab50`  
		Last Modified: Wed, 18 Nov 2020 00:54:39 GMT  
		Size: 10.8 MB (10752152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a456bba435b99e4c17dd5da957e63bef2c43ae5291b055ce82bd26d9153259`  
		Last Modified: Wed, 18 Nov 2020 00:54:37 GMT  
		Size: 4.3 MB (4340590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b048cb94809123b7360b06fcf7cdc40f6db32b7e4679612eb80812f9281589cc`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 13.2 MB (13208088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315e803a7acf0a2f7ea0534d3b00789832611a9209e0a52609039a760e3acc5c`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 2.8 KB (2827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecab6aded49c4d7c910b757fbc7ee91f7d4a2473e51bdd467bd86c4099af47f4`  
		Last Modified: Thu, 19 Nov 2020 02:58:50 GMT  
		Size: 22.7 MB (22694300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e746b6caad54a6b61d3b8a7a590882748257976204823ae9fd002cb779e2dfc3`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba68761006b14d29e7cd46a5114f64de970e2b79872c600da4729cd6d3f388b5`  
		Last Modified: Thu, 19 Nov 2020 02:58:44 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4.1` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:86fa5b92eba32671d5c1c210cf6be710cfa680320ce6e9a711436ddf103c7b56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efd75b9bba9f77c5058b6c71b26d9605875feae327ce9c5932cb9f0a8783764c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:06 GMT
ADD file:e74dce76704e3faa6198db5cf4192fd431f5addf55f658277eb5b60d254fee8e in / 
# Fri, 11 Dec 2020 02:28:09 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:35:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:35:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 12 Dec 2020 07:16:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 12 Dec 2020 07:16:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 12 Dec 2020 07:16:40 GMT
ENV KAPACITOR_VERSION=1.4.1
# Sat, 12 Dec 2020 07:16:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Sat, 12 Dec 2020 07:16:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 12 Dec 2020 07:16:48 GMT
EXPOSE 9092
# Sat, 12 Dec 2020 07:16:49 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 12 Dec 2020 07:16:50 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 12 Dec 2020 07:16:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Dec 2020 07:16:52 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:062f5403576d7e3aca1c92115ff0a9ea110b270cb0b61013efa86744515666fb`  
		Last Modified: Fri, 11 Dec 2020 02:36:48 GMT  
		Size: 42.1 MB (42117949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5385e34f58366fad1da017d000782de279c46cc834d767686d02d13a59a570`  
		Last Modified: Fri, 11 Dec 2020 16:47:26 GMT  
		Size: 9.4 MB (9444537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba7ef5d6926f92eb8533178d7f708c2e385991e7d97edb8e2433c518f252af7`  
		Last Modified: Fri, 11 Dec 2020 16:47:24 GMT  
		Size: 3.9 MB (3920019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b78f5775b143974c905677d6d57824a7d9c1df56b0c5beb0b04042bdeee0ed`  
		Last Modified: Sat, 12 Dec 2020 07:17:28 GMT  
		Size: 13.4 MB (13428938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad9b956ce07ac5f129c4adcba522b127cc8c115e2cc3392a4e4f576c99416f6`  
		Last Modified: Sat, 12 Dec 2020 07:17:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293215cc916f1d4cf42444ccbd6cca8a35ff8384f195db76af5950bca67af03f`  
		Last Modified: Sat, 12 Dec 2020 07:17:33 GMT  
		Size: 21.3 MB (21308107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4ce82ef03670997fc776bf4fd4684b8d58f4f764d9728057e3feb2b4ba563d`  
		Last Modified: Sat, 12 Dec 2020 07:17:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a2800a03e7f95087381d5ebb2aa2fb66b43ab9241f422a16e0234371419e1a`  
		Last Modified: Sat, 12 Dec 2020 07:17:25 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.4.1` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:3916c73f5ba4c32ae47bea8722f22af38051805bc8d57326f4a16c78db75522f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91197712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a7d2880c5eb1442b3e42d4a9e2254d4f75bfffd663825f9ecc38b51f0a29b13`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:33 GMT
ADD file:d2e307c3e54ad69dff47f6bdacca7c8ee0957a09346bb21baec02b9de1a657e1 in / 
# Tue, 17 Nov 2020 20:27:37 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:28:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 21:14:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Nov 2020 21:15:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 18 Nov 2020 21:15:01 GMT
ENV KAPACITOR_VERSION=1.4.1
# Wed, 18 Nov 2020 21:15:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}_${ARCH}.deb*
# Wed, 18 Nov 2020 21:15:07 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Nov 2020 21:15:08 GMT
EXPOSE 9092
# Wed, 18 Nov 2020 21:15:09 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Nov 2020 21:15:09 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Nov 2020 21:15:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 21:15:11 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f99bf631c0ebddf9e32516b47bf6e198efc42d06c3eb86d6f5f5739757b5839c`  
		Last Modified: Tue, 17 Nov 2020 20:34:17 GMT  
		Size: 43.2 MB (43176009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a9b3adbe4ac4ca73818d8b79e94d2ff2b6ceafc1225d7c036ec4d384f0804a`  
		Last Modified: Tue, 17 Nov 2020 22:40:38 GMT  
		Size: 9.7 MB (9702292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052ba804da6ef34fd9dddf0ca298b1e0551ac8cf3ea14fc371fa1fa51cbd7f7c`  
		Last Modified: Tue, 17 Nov 2020 22:40:36 GMT  
		Size: 4.1 MB (4095219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d0115aaf8aea01788d62c5180c53c44f5b525f2a9dddfd2859576f55f219b`  
		Last Modified: Wed, 18 Nov 2020 21:15:45 GMT  
		Size: 12.9 MB (12912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f61bf00eecdaa1ba088593162e6892a588b4bdebc909c2cbf006fe9d2b0332a`  
		Last Modified: Wed, 18 Nov 2020 21:15:42 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c933cf9017283815ffdb326dc7a95075238243af1c7fd53f4c61817e3703dc3`  
		Last Modified: Wed, 18 Nov 2020 21:15:50 GMT  
		Size: 21.3 MB (21307888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d548a97c64cd97d4e4ba9b7d50b22f6f935279941bf7f54c467c5bb34c00cddc`  
		Last Modified: Wed, 18 Nov 2020 21:15:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c4c8e7573c067a188b43422916a291461da80c7cfd0294df4201b42235318b`  
		Last Modified: Wed, 18 Nov 2020 21:15:44 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4.1-alpine`

```console
$ docker pull kapacitor@sha256:b071e57116f2be889263c25ee4824ea7a204eb6a8a60c31dbc1b49ba9edcdc07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.4.1-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:9014e51d201f6e4258d66a2587a85a1dc3ae7d9c380b3f00ca1856bda3f6d5cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.7 MB (19676857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6348ce1afff51aabf27e75c63c1c1ff2e82a89ec736891bae08de7383a79e496`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 06:11:13 GMT
ENV KAPACITOR_VERSION=1.4.1
# Fri, 11 Dec 2020 06:11:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 06:11:19 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 11 Dec 2020 06:11:19 GMT
EXPOSE 9092
# Fri, 11 Dec 2020 06:11:19 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 11 Dec 2020 06:11:20 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 11 Dec 2020 06:11:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 06:11:20 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9721c7fda0233566313cc2f6f927d44db357e4aedfcfcb38889dac61f5d57c7`  
		Last Modified: Fri, 11 Dec 2020 06:12:13 GMT  
		Size: 16.6 MB (16598495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e03d6c46795b4a64d7293609c0a883c6cbd4a11133da0c9643494b1603cc57`  
		Last Modified: Fri, 11 Dec 2020 06:12:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddaa751bdfbb7e409fef499ffe41df18a756017f242cfcfd41482f7b309992b`  
		Last Modified: Fri, 11 Dec 2020 06:12:07 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.4-alpine`

```console
$ docker pull kapacitor@sha256:b071e57116f2be889263c25ee4824ea7a204eb6a8a60c31dbc1b49ba9edcdc07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.4-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:9014e51d201f6e4258d66a2587a85a1dc3ae7d9c380b3f00ca1856bda3f6d5cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.7 MB (19676857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6348ce1afff51aabf27e75c63c1c1ff2e82a89ec736891bae08de7383a79e496`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 06:11:13 GMT
ENV KAPACITOR_VERSION=1.4.1
# Fri, 11 Dec 2020 06:11:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 06:11:19 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 11 Dec 2020 06:11:19 GMT
EXPOSE 9092
# Fri, 11 Dec 2020 06:11:19 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 11 Dec 2020 06:11:20 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 11 Dec 2020 06:11:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 06:11:20 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9721c7fda0233566313cc2f6f927d44db357e4aedfcfcb38889dac61f5d57c7`  
		Last Modified: Fri, 11 Dec 2020 06:12:13 GMT  
		Size: 16.6 MB (16598495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e03d6c46795b4a64d7293609c0a883c6cbd4a11133da0c9643494b1603cc57`  
		Last Modified: Fri, 11 Dec 2020 06:12:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddaa751bdfbb7e409fef499ffe41df18a756017f242cfcfd41482f7b309992b`  
		Last Modified: Fri, 11 Dec 2020 06:12:07 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5`

```console
$ docker pull kapacitor@sha256:906900ffc4f43809adbbd8dbad7bfef7e7614bec875eedac99054e83331835b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:c74a3bab564e22ddde955f01f80fa3fbec0537e6c6e4c16a301d5a4e56de0618
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110135763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f21a08569c6640d78425e06df958a9fa5ab393f0c0adb8cf5ded716261bc081`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:10 GMT
ADD file:373a8875589f170b51fa677a3bf736feeb46ea278c553950a3eb3169a2056c12 in / 
# Tue, 17 Nov 2020 20:24:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:43:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 19 Nov 2020 02:58:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 19 Nov 2020 02:58:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 19 Nov 2020 02:58:25 GMT
ENV KAPACITOR_VERSION=1.5.7
# Thu, 19 Nov 2020 02:58:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 19 Nov 2020 02:58:28 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 19 Nov 2020 02:58:28 GMT
EXPOSE 9092
# Thu, 19 Nov 2020 02:58:29 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 19 Nov 2020 02:58:29 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 19 Nov 2020 02:58:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Nov 2020 02:58:29 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:7919f5b7d60254cafc73c0d097b8ccffb72e0b6472957ece4dd5b378c5ca7cc1`  
		Last Modified: Tue, 17 Nov 2020 20:30:26 GMT  
		Size: 45.4 MB (45377037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e107167dcc5392ce7b34cb6af6bcfe1cf99f76f9e632d6c321526666558ab50`  
		Last Modified: Wed, 18 Nov 2020 00:54:39 GMT  
		Size: 10.8 MB (10752152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a456bba435b99e4c17dd5da957e63bef2c43ae5291b055ce82bd26d9153259`  
		Last Modified: Wed, 18 Nov 2020 00:54:37 GMT  
		Size: 4.3 MB (4340590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b048cb94809123b7360b06fcf7cdc40f6db32b7e4679612eb80812f9281589cc`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 13.2 MB (13208088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315e803a7acf0a2f7ea0534d3b00789832611a9209e0a52609039a760e3acc5c`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 2.8 KB (2827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181dddab55b6f4f0dcecbdae29e93640187402d8a80454f5c54d4ee532f420ff`  
		Last Modified: Thu, 19 Nov 2020 02:59:02 GMT  
		Size: 36.5 MB (36454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ecec1461f35bbd680d857fca09f475d8a677cd44131254c462b04a3b706a05`  
		Last Modified: Thu, 19 Nov 2020 02:58:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2311c2cd39e045578d65cfc3a8088c74a0cd0d42f87be7a8b6bba24b8a60`  
		Last Modified: Thu, 19 Nov 2020 02:58:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:445ea39899812f673ea3c836f912d3c3dcd82f2468214879a4c77806f8a26340
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103086821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f17f013dc82dc92614348fe55460014da9b0e2221132bdced2a5cff312d072a2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:06 GMT
ADD file:e74dce76704e3faa6198db5cf4192fd431f5addf55f658277eb5b60d254fee8e in / 
# Fri, 11 Dec 2020 02:28:09 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:35:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:35:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 12 Dec 2020 07:16:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 12 Dec 2020 07:16:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 12 Dec 2020 07:17:00 GMT
ENV KAPACITOR_VERSION=1.5.7
# Sat, 12 Dec 2020 07:17:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 12 Dec 2020 07:17:08 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 12 Dec 2020 07:17:09 GMT
EXPOSE 9092
# Sat, 12 Dec 2020 07:17:10 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 12 Dec 2020 07:17:10 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 12 Dec 2020 07:17:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Dec 2020 07:17:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:062f5403576d7e3aca1c92115ff0a9ea110b270cb0b61013efa86744515666fb`  
		Last Modified: Fri, 11 Dec 2020 02:36:48 GMT  
		Size: 42.1 MB (42117949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5385e34f58366fad1da017d000782de279c46cc834d767686d02d13a59a570`  
		Last Modified: Fri, 11 Dec 2020 16:47:26 GMT  
		Size: 9.4 MB (9444537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba7ef5d6926f92eb8533178d7f708c2e385991e7d97edb8e2433c518f252af7`  
		Last Modified: Fri, 11 Dec 2020 16:47:24 GMT  
		Size: 3.9 MB (3920019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b78f5775b143974c905677d6d57824a7d9c1df56b0c5beb0b04042bdeee0ed`  
		Last Modified: Sat, 12 Dec 2020 07:17:28 GMT  
		Size: 13.4 MB (13428938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad9b956ce07ac5f129c4adcba522b127cc8c115e2cc3392a4e4f576c99416f6`  
		Last Modified: Sat, 12 Dec 2020 07:17:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5950e78e516336c951e2ba47c594235c802d1d2d98ac75fd77ef7a8acccaff09`  
		Last Modified: Sat, 12 Dec 2020 07:17:50 GMT  
		Size: 34.2 MB (34172066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6343946d76835a1ec46a85479f2f960433df020aeafe777c264ad1e22036c3`  
		Last Modified: Sat, 12 Dec 2020 07:17:42 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41fe3ad6b00de9ff7c5c618469aadec71e2ba9f28d378200be558bae3ae0e90`  
		Last Modified: Sat, 12 Dec 2020 07:17:41 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:5b20fed30b4e8c9f89c0dad6d8d172e1d76fad60cf53706bf54fe8b031f81c56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103862482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430779a890d64071bec0487e68fc1ccc6a775930a8edd400d8d3d2c8d58dd693`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:33 GMT
ADD file:d2e307c3e54ad69dff47f6bdacca7c8ee0957a09346bb21baec02b9de1a657e1 in / 
# Tue, 17 Nov 2020 20:27:37 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:28:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 21:14:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Nov 2020 21:15:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 18 Nov 2020 21:15:19 GMT
ENV KAPACITOR_VERSION=1.5.7
# Wed, 18 Nov 2020 21:15:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Nov 2020 21:15:26 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Nov 2020 21:15:27 GMT
EXPOSE 9092
# Wed, 18 Nov 2020 21:15:27 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Nov 2020 21:15:28 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Nov 2020 21:15:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 21:15:29 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f99bf631c0ebddf9e32516b47bf6e198efc42d06c3eb86d6f5f5739757b5839c`  
		Last Modified: Tue, 17 Nov 2020 20:34:17 GMT  
		Size: 43.2 MB (43176009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a9b3adbe4ac4ca73818d8b79e94d2ff2b6ceafc1225d7c036ec4d384f0804a`  
		Last Modified: Tue, 17 Nov 2020 22:40:38 GMT  
		Size: 9.7 MB (9702292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052ba804da6ef34fd9dddf0ca298b1e0551ac8cf3ea14fc371fa1fa51cbd7f7c`  
		Last Modified: Tue, 17 Nov 2020 22:40:36 GMT  
		Size: 4.1 MB (4095219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d0115aaf8aea01788d62c5180c53c44f5b525f2a9dddfd2859576f55f219b`  
		Last Modified: Wed, 18 Nov 2020 21:15:45 GMT  
		Size: 12.9 MB (12912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f61bf00eecdaa1ba088593162e6892a588b4bdebc909c2cbf006fe9d2b0332a`  
		Last Modified: Wed, 18 Nov 2020 21:15:42 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8814f25006190778f6d5c4c287f922d620ed7720f89d70b0be24eb7f1db4f0`  
		Last Modified: Wed, 18 Nov 2020 21:16:05 GMT  
		Size: 34.0 MB (33972658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b1a95a3f1063ac127f86a44a5a9cd8a68d6de59df05c3d9455088ddbceab29`  
		Last Modified: Wed, 18 Nov 2020 21:15:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57e1ccfd78a9919f64e08d48f8712b319bf7c4e2058563501c2aa3e4bc640fb`  
		Last Modified: Wed, 18 Nov 2020 21:15:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.7`

```console
$ docker pull kapacitor@sha256:906900ffc4f43809adbbd8dbad7bfef7e7614bec875eedac99054e83331835b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.7` - linux; amd64

```console
$ docker pull kapacitor@sha256:c74a3bab564e22ddde955f01f80fa3fbec0537e6c6e4c16a301d5a4e56de0618
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110135763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f21a08569c6640d78425e06df958a9fa5ab393f0c0adb8cf5ded716261bc081`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:10 GMT
ADD file:373a8875589f170b51fa677a3bf736feeb46ea278c553950a3eb3169a2056c12 in / 
# Tue, 17 Nov 2020 20:24:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:43:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 19 Nov 2020 02:58:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 19 Nov 2020 02:58:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 19 Nov 2020 02:58:25 GMT
ENV KAPACITOR_VERSION=1.5.7
# Thu, 19 Nov 2020 02:58:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 19 Nov 2020 02:58:28 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 19 Nov 2020 02:58:28 GMT
EXPOSE 9092
# Thu, 19 Nov 2020 02:58:29 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 19 Nov 2020 02:58:29 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 19 Nov 2020 02:58:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Nov 2020 02:58:29 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:7919f5b7d60254cafc73c0d097b8ccffb72e0b6472957ece4dd5b378c5ca7cc1`  
		Last Modified: Tue, 17 Nov 2020 20:30:26 GMT  
		Size: 45.4 MB (45377037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e107167dcc5392ce7b34cb6af6bcfe1cf99f76f9e632d6c321526666558ab50`  
		Last Modified: Wed, 18 Nov 2020 00:54:39 GMT  
		Size: 10.8 MB (10752152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a456bba435b99e4c17dd5da957e63bef2c43ae5291b055ce82bd26d9153259`  
		Last Modified: Wed, 18 Nov 2020 00:54:37 GMT  
		Size: 4.3 MB (4340590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b048cb94809123b7360b06fcf7cdc40f6db32b7e4679612eb80812f9281589cc`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 13.2 MB (13208088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315e803a7acf0a2f7ea0534d3b00789832611a9209e0a52609039a760e3acc5c`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 2.8 KB (2827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181dddab55b6f4f0dcecbdae29e93640187402d8a80454f5c54d4ee532f420ff`  
		Last Modified: Thu, 19 Nov 2020 02:59:02 GMT  
		Size: 36.5 MB (36454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ecec1461f35bbd680d857fca09f475d8a677cd44131254c462b04a3b706a05`  
		Last Modified: Thu, 19 Nov 2020 02:58:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2311c2cd39e045578d65cfc3a8088c74a0cd0d42f87be7a8b6bba24b8a60`  
		Last Modified: Thu, 19 Nov 2020 02:58:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.7` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:445ea39899812f673ea3c836f912d3c3dcd82f2468214879a4c77806f8a26340
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103086821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f17f013dc82dc92614348fe55460014da9b0e2221132bdced2a5cff312d072a2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:06 GMT
ADD file:e74dce76704e3faa6198db5cf4192fd431f5addf55f658277eb5b60d254fee8e in / 
# Fri, 11 Dec 2020 02:28:09 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:35:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:35:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 12 Dec 2020 07:16:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 12 Dec 2020 07:16:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 12 Dec 2020 07:17:00 GMT
ENV KAPACITOR_VERSION=1.5.7
# Sat, 12 Dec 2020 07:17:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 12 Dec 2020 07:17:08 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 12 Dec 2020 07:17:09 GMT
EXPOSE 9092
# Sat, 12 Dec 2020 07:17:10 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 12 Dec 2020 07:17:10 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 12 Dec 2020 07:17:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Dec 2020 07:17:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:062f5403576d7e3aca1c92115ff0a9ea110b270cb0b61013efa86744515666fb`  
		Last Modified: Fri, 11 Dec 2020 02:36:48 GMT  
		Size: 42.1 MB (42117949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5385e34f58366fad1da017d000782de279c46cc834d767686d02d13a59a570`  
		Last Modified: Fri, 11 Dec 2020 16:47:26 GMT  
		Size: 9.4 MB (9444537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba7ef5d6926f92eb8533178d7f708c2e385991e7d97edb8e2433c518f252af7`  
		Last Modified: Fri, 11 Dec 2020 16:47:24 GMT  
		Size: 3.9 MB (3920019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b78f5775b143974c905677d6d57824a7d9c1df56b0c5beb0b04042bdeee0ed`  
		Last Modified: Sat, 12 Dec 2020 07:17:28 GMT  
		Size: 13.4 MB (13428938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad9b956ce07ac5f129c4adcba522b127cc8c115e2cc3392a4e4f576c99416f6`  
		Last Modified: Sat, 12 Dec 2020 07:17:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5950e78e516336c951e2ba47c594235c802d1d2d98ac75fd77ef7a8acccaff09`  
		Last Modified: Sat, 12 Dec 2020 07:17:50 GMT  
		Size: 34.2 MB (34172066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6343946d76835a1ec46a85479f2f960433df020aeafe777c264ad1e22036c3`  
		Last Modified: Sat, 12 Dec 2020 07:17:42 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41fe3ad6b00de9ff7c5c618469aadec71e2ba9f28d378200be558bae3ae0e90`  
		Last Modified: Sat, 12 Dec 2020 07:17:41 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.7` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:5b20fed30b4e8c9f89c0dad6d8d172e1d76fad60cf53706bf54fe8b031f81c56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103862482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430779a890d64071bec0487e68fc1ccc6a775930a8edd400d8d3d2c8d58dd693`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:33 GMT
ADD file:d2e307c3e54ad69dff47f6bdacca7c8ee0957a09346bb21baec02b9de1a657e1 in / 
# Tue, 17 Nov 2020 20:27:37 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:28:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 21:14:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Nov 2020 21:15:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 18 Nov 2020 21:15:19 GMT
ENV KAPACITOR_VERSION=1.5.7
# Wed, 18 Nov 2020 21:15:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Nov 2020 21:15:26 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Nov 2020 21:15:27 GMT
EXPOSE 9092
# Wed, 18 Nov 2020 21:15:27 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Nov 2020 21:15:28 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Nov 2020 21:15:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 21:15:29 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f99bf631c0ebddf9e32516b47bf6e198efc42d06c3eb86d6f5f5739757b5839c`  
		Last Modified: Tue, 17 Nov 2020 20:34:17 GMT  
		Size: 43.2 MB (43176009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a9b3adbe4ac4ca73818d8b79e94d2ff2b6ceafc1225d7c036ec4d384f0804a`  
		Last Modified: Tue, 17 Nov 2020 22:40:38 GMT  
		Size: 9.7 MB (9702292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052ba804da6ef34fd9dddf0ca298b1e0551ac8cf3ea14fc371fa1fa51cbd7f7c`  
		Last Modified: Tue, 17 Nov 2020 22:40:36 GMT  
		Size: 4.1 MB (4095219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d0115aaf8aea01788d62c5180c53c44f5b525f2a9dddfd2859576f55f219b`  
		Last Modified: Wed, 18 Nov 2020 21:15:45 GMT  
		Size: 12.9 MB (12912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f61bf00eecdaa1ba088593162e6892a588b4bdebc909c2cbf006fe9d2b0332a`  
		Last Modified: Wed, 18 Nov 2020 21:15:42 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8814f25006190778f6d5c4c287f922d620ed7720f89d70b0be24eb7f1db4f0`  
		Last Modified: Wed, 18 Nov 2020 21:16:05 GMT  
		Size: 34.0 MB (33972658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b1a95a3f1063ac127f86a44a5a9cd8a68d6de59df05c3d9455088ddbceab29`  
		Last Modified: Wed, 18 Nov 2020 21:15:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57e1ccfd78a9919f64e08d48f8712b319bf7c4e2058563501c2aa3e4bc640fb`  
		Last Modified: Wed, 18 Nov 2020 21:15:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.7-alpine`

```console
$ docker pull kapacitor@sha256:cc96f6817a7592c4ede7e8db7b9e2c55a79be5e6103f88728db5c595a39e24e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.5.7-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:fdf27ead951da5e692d8df31873ef42c82dc2a25c7f0b04176db521aa9d8a159
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.2 MB (23178969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821cc2b89a53d8e4ef0c213eef01cb4716de3fb45e5ac4c7c957e47040bf7c40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 06:11:31 GMT
ENV KAPACITOR_VERSION=1.5.7
# Fri, 11 Dec 2020 06:11:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 06:11:37 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 11 Dec 2020 06:11:37 GMT
EXPOSE 9092
# Fri, 11 Dec 2020 06:11:37 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 11 Dec 2020 06:11:38 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 11 Dec 2020 06:11:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 06:11:38 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae04b5137f000abc8cac383898f3143e57a86644ae27042a5d9aec6291f5476`  
		Last Modified: Fri, 11 Dec 2020 06:12:27 GMT  
		Size: 20.1 MB (20100611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e670b986ae7565da2b6683b0fb385e75fc34e7cb1c37a19ec0921259b68731`  
		Last Modified: Fri, 11 Dec 2020 06:12:21 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b8fc4ea8a40ce61c1f6a6c0501b5787341c9e029ff64de22fbe0a97a55cd45`  
		Last Modified: Fri, 11 Dec 2020 06:12:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:cc96f6817a7592c4ede7e8db7b9e2c55a79be5e6103f88728db5c595a39e24e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:fdf27ead951da5e692d8df31873ef42c82dc2a25c7f0b04176db521aa9d8a159
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.2 MB (23178969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821cc2b89a53d8e4ef0c213eef01cb4716de3fb45e5ac4c7c957e47040bf7c40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 06:11:31 GMT
ENV KAPACITOR_VERSION=1.5.7
# Fri, 11 Dec 2020 06:11:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 06:11:37 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 11 Dec 2020 06:11:37 GMT
EXPOSE 9092
# Fri, 11 Dec 2020 06:11:37 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 11 Dec 2020 06:11:38 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 11 Dec 2020 06:11:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 06:11:38 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae04b5137f000abc8cac383898f3143e57a86644ae27042a5d9aec6291f5476`  
		Last Modified: Fri, 11 Dec 2020 06:12:27 GMT  
		Size: 20.1 MB (20100611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e670b986ae7565da2b6683b0fb385e75fc34e7cb1c37a19ec0921259b68731`  
		Last Modified: Fri, 11 Dec 2020 06:12:21 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b8fc4ea8a40ce61c1f6a6c0501b5787341c9e029ff64de22fbe0a97a55cd45`  
		Last Modified: Fri, 11 Dec 2020 06:12:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:cc96f6817a7592c4ede7e8db7b9e2c55a79be5e6103f88728db5c595a39e24e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:fdf27ead951da5e692d8df31873ef42c82dc2a25c7f0b04176db521aa9d8a159
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.2 MB (23178969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821cc2b89a53d8e4ef0c213eef01cb4716de3fb45e5ac4c7c957e47040bf7c40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:51:45 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:51:47 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 11 Dec 2020 06:11:31 GMT
ENV KAPACITOR_VERSION=1.5.7
# Fri, 11 Dec 2020 06:11:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 11 Dec 2020 06:11:37 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 11 Dec 2020 06:11:37 GMT
EXPOSE 9092
# Fri, 11 Dec 2020 06:11:37 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 11 Dec 2020 06:11:38 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 11 Dec 2020 06:11:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 06:11:38 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9624996f533f5dfa6054365968149298c1183a1202c16061de0fc5093ad633f`  
		Last Modified: Fri, 11 Dec 2020 02:53:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714c102d667de25287e212434b418f887c3297d809db411374920f3d8b36201`  
		Last Modified: Fri, 11 Dec 2020 02:53:53 GMT  
		Size: 280.8 KB (280809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae04b5137f000abc8cac383898f3143e57a86644ae27042a5d9aec6291f5476`  
		Last Modified: Fri, 11 Dec 2020 06:12:27 GMT  
		Size: 20.1 MB (20100611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e670b986ae7565da2b6683b0fb385e75fc34e7cb1c37a19ec0921259b68731`  
		Last Modified: Fri, 11 Dec 2020 06:12:21 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b8fc4ea8a40ce61c1f6a6c0501b5787341c9e029ff64de22fbe0a97a55cd45`  
		Last Modified: Fri, 11 Dec 2020 06:12:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:906900ffc4f43809adbbd8dbad7bfef7e7614bec875eedac99054e83331835b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:c74a3bab564e22ddde955f01f80fa3fbec0537e6c6e4c16a301d5a4e56de0618
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110135763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f21a08569c6640d78425e06df958a9fa5ab393f0c0adb8cf5ded716261bc081`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:10 GMT
ADD file:373a8875589f170b51fa677a3bf736feeb46ea278c553950a3eb3169a2056c12 in / 
# Tue, 17 Nov 2020 20:24:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:43:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 19 Nov 2020 02:58:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Thu, 19 Nov 2020 02:58:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 19 Nov 2020 02:58:25 GMT
ENV KAPACITOR_VERSION=1.5.7
# Thu, 19 Nov 2020 02:58:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Thu, 19 Nov 2020 02:58:28 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 19 Nov 2020 02:58:28 GMT
EXPOSE 9092
# Thu, 19 Nov 2020 02:58:29 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 19 Nov 2020 02:58:29 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Thu, 19 Nov 2020 02:58:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 19 Nov 2020 02:58:29 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:7919f5b7d60254cafc73c0d097b8ccffb72e0b6472957ece4dd5b378c5ca7cc1`  
		Last Modified: Tue, 17 Nov 2020 20:30:26 GMT  
		Size: 45.4 MB (45377037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e107167dcc5392ce7b34cb6af6bcfe1cf99f76f9e632d6c321526666558ab50`  
		Last Modified: Wed, 18 Nov 2020 00:54:39 GMT  
		Size: 10.8 MB (10752152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a456bba435b99e4c17dd5da957e63bef2c43ae5291b055ce82bd26d9153259`  
		Last Modified: Wed, 18 Nov 2020 00:54:37 GMT  
		Size: 4.3 MB (4340590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b048cb94809123b7360b06fcf7cdc40f6db32b7e4679612eb80812f9281589cc`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 13.2 MB (13208088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315e803a7acf0a2f7ea0534d3b00789832611a9209e0a52609039a760e3acc5c`  
		Last Modified: Thu, 19 Nov 2020 02:58:45 GMT  
		Size: 2.8 KB (2827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181dddab55b6f4f0dcecbdae29e93640187402d8a80454f5c54d4ee532f420ff`  
		Last Modified: Thu, 19 Nov 2020 02:59:02 GMT  
		Size: 36.5 MB (36454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ecec1461f35bbd680d857fca09f475d8a677cd44131254c462b04a3b706a05`  
		Last Modified: Thu, 19 Nov 2020 02:58:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2311c2cd39e045578d65cfc3a8088c74a0cd0d42f87be7a8b6bba24b8a60`  
		Last Modified: Thu, 19 Nov 2020 02:58:56 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:445ea39899812f673ea3c836f912d3c3dcd82f2468214879a4c77806f8a26340
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103086821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f17f013dc82dc92614348fe55460014da9b0e2221132bdced2a5cff312d072a2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:06 GMT
ADD file:e74dce76704e3faa6198db5cf4192fd431f5addf55f658277eb5b60d254fee8e in / 
# Fri, 11 Dec 2020 02:28:09 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:35:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:35:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 12 Dec 2020 07:16:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Sat, 12 Dec 2020 07:16:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 12 Dec 2020 07:17:00 GMT
ENV KAPACITOR_VERSION=1.5.7
# Sat, 12 Dec 2020 07:17:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Sat, 12 Dec 2020 07:17:08 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Sat, 12 Dec 2020 07:17:09 GMT
EXPOSE 9092
# Sat, 12 Dec 2020 07:17:10 GMT
VOLUME [/var/lib/kapacitor]
# Sat, 12 Dec 2020 07:17:10 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Sat, 12 Dec 2020 07:17:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Dec 2020 07:17:12 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:062f5403576d7e3aca1c92115ff0a9ea110b270cb0b61013efa86744515666fb`  
		Last Modified: Fri, 11 Dec 2020 02:36:48 GMT  
		Size: 42.1 MB (42117949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5385e34f58366fad1da017d000782de279c46cc834d767686d02d13a59a570`  
		Last Modified: Fri, 11 Dec 2020 16:47:26 GMT  
		Size: 9.4 MB (9444537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba7ef5d6926f92eb8533178d7f708c2e385991e7d97edb8e2433c518f252af7`  
		Last Modified: Fri, 11 Dec 2020 16:47:24 GMT  
		Size: 3.9 MB (3920019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b78f5775b143974c905677d6d57824a7d9c1df56b0c5beb0b04042bdeee0ed`  
		Last Modified: Sat, 12 Dec 2020 07:17:28 GMT  
		Size: 13.4 MB (13428938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad9b956ce07ac5f129c4adcba522b127cc8c115e2cc3392a4e4f576c99416f6`  
		Last Modified: Sat, 12 Dec 2020 07:17:26 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5950e78e516336c951e2ba47c594235c802d1d2d98ac75fd77ef7a8acccaff09`  
		Last Modified: Sat, 12 Dec 2020 07:17:50 GMT  
		Size: 34.2 MB (34172066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6343946d76835a1ec46a85479f2f960433df020aeafe777c264ad1e22036c3`  
		Last Modified: Sat, 12 Dec 2020 07:17:42 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41fe3ad6b00de9ff7c5c618469aadec71e2ba9f28d378200be558bae3ae0e90`  
		Last Modified: Sat, 12 Dec 2020 07:17:41 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:5b20fed30b4e8c9f89c0dad6d8d172e1d76fad60cf53706bf54fe8b031f81c56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.9 MB (103862482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430779a890d64071bec0487e68fc1ccc6a775930a8edd400d8d3d2c8d58dd693`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Nov 2020 20:27:33 GMT
ADD file:d2e307c3e54ad69dff47f6bdacca7c8ee0957a09346bb21baec02b9de1a657e1 in / 
# Tue, 17 Nov 2020 20:27:37 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:28:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 21:14:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Nov 2020 21:15:00 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 18 Nov 2020 21:15:19 GMT
ENV KAPACITOR_VERSION=1.5.7
# Wed, 18 Nov 2020 21:15:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Nov 2020 21:15:26 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Nov 2020 21:15:27 GMT
EXPOSE 9092
# Wed, 18 Nov 2020 21:15:27 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Nov 2020 21:15:28 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Nov 2020 21:15:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 21:15:29 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f99bf631c0ebddf9e32516b47bf6e198efc42d06c3eb86d6f5f5739757b5839c`  
		Last Modified: Tue, 17 Nov 2020 20:34:17 GMT  
		Size: 43.2 MB (43176009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a9b3adbe4ac4ca73818d8b79e94d2ff2b6ceafc1225d7c036ec4d384f0804a`  
		Last Modified: Tue, 17 Nov 2020 22:40:38 GMT  
		Size: 9.7 MB (9702292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052ba804da6ef34fd9dddf0ca298b1e0551ac8cf3ea14fc371fa1fa51cbd7f7c`  
		Last Modified: Tue, 17 Nov 2020 22:40:36 GMT  
		Size: 4.1 MB (4095219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d0115aaf8aea01788d62c5180c53c44f5b525f2a9dddfd2859576f55f219b`  
		Last Modified: Wed, 18 Nov 2020 21:15:45 GMT  
		Size: 12.9 MB (12912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f61bf00eecdaa1ba088593162e6892a588b4bdebc909c2cbf006fe9d2b0332a`  
		Last Modified: Wed, 18 Nov 2020 21:15:42 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8814f25006190778f6d5c4c287f922d620ed7720f89d70b0be24eb7f1db4f0`  
		Last Modified: Wed, 18 Nov 2020 21:16:05 GMT  
		Size: 34.0 MB (33972658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b1a95a3f1063ac127f86a44a5a9cd8a68d6de59df05c3d9455088ddbceab29`  
		Last Modified: Wed, 18 Nov 2020 21:15:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57e1ccfd78a9919f64e08d48f8712b319bf7c4e2058563501c2aa3e4bc640fb`  
		Last Modified: Wed, 18 Nov 2020 21:15:58 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
