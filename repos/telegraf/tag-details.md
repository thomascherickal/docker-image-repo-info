<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.15`](#telegraf115)
-	[`telegraf:1.15.4`](#telegraf1154)
-	[`telegraf:1.15.4-alpine`](#telegraf1154-alpine)
-	[`telegraf:1.15-alpine`](#telegraf115-alpine)
-	[`telegraf:1.16`](#telegraf116)
-	[`telegraf:1.16.3`](#telegraf1163)
-	[`telegraf:1.16.3-alpine`](#telegraf1163-alpine)
-	[`telegraf:1.16-alpine`](#telegraf116-alpine)
-	[`telegraf:1.17`](#telegraf117)
-	[`telegraf:1.17.2`](#telegraf1172)
-	[`telegraf:1.17.2-alpine`](#telegraf1172-alpine)
-	[`telegraf:1.17-alpine`](#telegraf117-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.15`

```console
$ docker pull telegraf@sha256:af17bcce03bff81bb604119ff9ebc48c38394bea919ec4d2c424eb8eb5025448
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.15` - linux; amd64

```console
$ docker pull telegraf@sha256:b45e10c2edc0fadd80d8cb7c881172965de9079bda18b79155c5afa2222af69e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2facf48002d0f6b6caa1dba97a060e6a9f8d3a37682726512b8409dd90ff4c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jan 2021 04:53:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Jan 2021 04:53:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 Jan 2021 04:53:37 GMT
ENV TELEGRAF_VERSION=1.15.4
# Wed, 13 Jan 2021 04:53:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Jan 2021 04:53:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Jan 2021 04:53:41 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Jan 2021 04:53:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 04:53:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b1b9836397a1f6a8bcceaf48114f9358677f022f0872b44f5446fe6ac98590`  
		Last Modified: Wed, 13 Jan 2021 04:54:38 GMT  
		Size: 17.4 MB (17412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481d0989b3180f85249175a536a5497daf377815101a00b80ac6f3df31ba200`  
		Last Modified: Wed, 13 Jan 2021 04:54:32 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8937b536072bdb280c76ca44b45533d63e95dc833838804dd01480f2bacc473`  
		Last Modified: Wed, 13 Jan 2021 04:54:39 GMT  
		Size: 21.7 MB (21669635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b0a16e385243accc34c766360195c83ea2dd0b9c6cbe2fcdc37caa963da799`  
		Last Modified: Wed, 13 Jan 2021 04:54:32 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.15` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:587dfc078472c3c2588da1d1384ba552aa35bb5b3cb9ee577bd43e42667f480d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98882189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82fd8f104502d98d6c9dc1c6744894bb592c68fc287e3b831c744c71faab3897`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:00:37 GMT
ADD file:216371f6fe8c803a0191f84e555c809a3301d1344c62b831dddb5e0c595fe0ef in / 
# Tue, 12 Jan 2021 00:00:46 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:14:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:04:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 21:04:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 21:04:51 GMT
ENV TELEGRAF_VERSION=1.15.4
# Tue, 12 Jan 2021 21:04:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Jan 2021 21:04:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Jan 2021 21:04:58 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 12 Jan 2021 21:04:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 21:04:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d8925d905dadf63fa0ff74be912443a1cf8cd72ea5543317b0e22067d39ef948`  
		Last Modified: Tue, 12 Jan 2021 00:10:42 GMT  
		Size: 45.9 MB (45870031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd9c5a6d77413d17345fcf1f89b9dde2f3d9d6157bd070d4093cfef30107add`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 7.1 MB (7099141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e1f8e87a65e3a71764ea79b951f915c90a885dfd516f61e57d81745acaf272`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 9.3 MB (9343447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ec62dff3056e70cc453ec4b2d4db22debd86a42ddeaa47252e4672774bf7a8`  
		Last Modified: Tue, 12 Jan 2021 21:06:02 GMT  
		Size: 16.2 MB (16158602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7e36c129df27747aced5a1d50e367b06ee3dbdd9dcdb8ac6eb7c4e7e5132bd`  
		Last Modified: Tue, 12 Jan 2021 21:05:55 GMT  
		Size: 2.9 KB (2912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a5a53e7b905105171664dd638a14e271d7b8aefe796d9921cf908f30509627`  
		Last Modified: Tue, 12 Jan 2021 21:06:02 GMT  
		Size: 20.4 MB (20407873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f5d833ff7ccde0bc6a167c4a9f54f55109276c044665f19e82e68775cbb24`  
		Last Modified: Tue, 12 Jan 2021 21:05:56 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.15` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:b23a4015177f778c63f62a4b0c291867a45e1da0317386c3b0c8a61dccf8d51c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104141752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c32ac88797c1d77c3a2969ababb3b493aef8d6e13466d46ab5288ff63613b89`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:40:39 GMT
ADD file:849d424ecc8572facb3ca68eff836dce211bc677cb32d3c3eaa129d364d33878 in / 
# Tue, 12 Jan 2021 00:40:43 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:34:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:34:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 23:34:31 GMT
ENV TELEGRAF_VERSION=1.15.4
# Tue, 12 Jan 2021 23:34:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Jan 2021 23:34:40 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Jan 2021 23:34:41 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 12 Jan 2021 23:34:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 23:34:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:6e5587ff5efa4e647ae927194fac9b961a68d46b23b68a3119c90016e58f17aa`  
		Last Modified: Tue, 12 Jan 2021 00:51:18 GMT  
		Size: 49.2 MB (49183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439dbbb05ea0aa8484ae8a51d0fbb1c7609176a1b0d3f15dad69d52e9a83af66`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 7.7 MB (7682325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b89c8b4e5b232c040d5905808ee62cdfcc9d697de10183d6bc4767468859d92`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 10.0 MB (9984327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc23f43b0bc1dd7f18ad8d9c699e4f57a322ad66aeb71996e6e8c9d2020abea`  
		Last Modified: Tue, 12 Jan 2021 23:35:36 GMT  
		Size: 17.3 MB (17269787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9c730332453078e166b4df31247ee7882c51ff0125356dab99e3a9dcc73661`  
		Last Modified: Tue, 12 Jan 2021 23:35:33 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467f513a28502825248b93776c150c2edac773b0a8deda5782ac26aacb6c8fda`  
		Last Modified: Tue, 12 Jan 2021 23:35:37 GMT  
		Size: 20.0 MB (20018497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5940454ec4499351669b0d9643b805223b801aeeae35aad1c8f4c505e6c8293`  
		Last Modified: Tue, 12 Jan 2021 23:35:32 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.15.4`

```console
$ docker pull telegraf@sha256:af17bcce03bff81bb604119ff9ebc48c38394bea919ec4d2c424eb8eb5025448
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.15.4` - linux; amd64

```console
$ docker pull telegraf@sha256:b45e10c2edc0fadd80d8cb7c881172965de9079bda18b79155c5afa2222af69e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2facf48002d0f6b6caa1dba97a060e6a9f8d3a37682726512b8409dd90ff4c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jan 2021 04:53:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Jan 2021 04:53:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 Jan 2021 04:53:37 GMT
ENV TELEGRAF_VERSION=1.15.4
# Wed, 13 Jan 2021 04:53:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Jan 2021 04:53:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Jan 2021 04:53:41 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Jan 2021 04:53:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 04:53:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b1b9836397a1f6a8bcceaf48114f9358677f022f0872b44f5446fe6ac98590`  
		Last Modified: Wed, 13 Jan 2021 04:54:38 GMT  
		Size: 17.4 MB (17412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481d0989b3180f85249175a536a5497daf377815101a00b80ac6f3df31ba200`  
		Last Modified: Wed, 13 Jan 2021 04:54:32 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8937b536072bdb280c76ca44b45533d63e95dc833838804dd01480f2bacc473`  
		Last Modified: Wed, 13 Jan 2021 04:54:39 GMT  
		Size: 21.7 MB (21669635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b0a16e385243accc34c766360195c83ea2dd0b9c6cbe2fcdc37caa963da799`  
		Last Modified: Wed, 13 Jan 2021 04:54:32 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.15.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:587dfc078472c3c2588da1d1384ba552aa35bb5b3cb9ee577bd43e42667f480d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98882189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82fd8f104502d98d6c9dc1c6744894bb592c68fc287e3b831c744c71faab3897`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:00:37 GMT
ADD file:216371f6fe8c803a0191f84e555c809a3301d1344c62b831dddb5e0c595fe0ef in / 
# Tue, 12 Jan 2021 00:00:46 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:14:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:04:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 21:04:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 21:04:51 GMT
ENV TELEGRAF_VERSION=1.15.4
# Tue, 12 Jan 2021 21:04:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Jan 2021 21:04:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Jan 2021 21:04:58 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 12 Jan 2021 21:04:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 21:04:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d8925d905dadf63fa0ff74be912443a1cf8cd72ea5543317b0e22067d39ef948`  
		Last Modified: Tue, 12 Jan 2021 00:10:42 GMT  
		Size: 45.9 MB (45870031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd9c5a6d77413d17345fcf1f89b9dde2f3d9d6157bd070d4093cfef30107add`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 7.1 MB (7099141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e1f8e87a65e3a71764ea79b951f915c90a885dfd516f61e57d81745acaf272`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 9.3 MB (9343447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ec62dff3056e70cc453ec4b2d4db22debd86a42ddeaa47252e4672774bf7a8`  
		Last Modified: Tue, 12 Jan 2021 21:06:02 GMT  
		Size: 16.2 MB (16158602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7e36c129df27747aced5a1d50e367b06ee3dbdd9dcdb8ac6eb7c4e7e5132bd`  
		Last Modified: Tue, 12 Jan 2021 21:05:55 GMT  
		Size: 2.9 KB (2912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a5a53e7b905105171664dd638a14e271d7b8aefe796d9921cf908f30509627`  
		Last Modified: Tue, 12 Jan 2021 21:06:02 GMT  
		Size: 20.4 MB (20407873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f5d833ff7ccde0bc6a167c4a9f54f55109276c044665f19e82e68775cbb24`  
		Last Modified: Tue, 12 Jan 2021 21:05:56 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.15.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:b23a4015177f778c63f62a4b0c291867a45e1da0317386c3b0c8a61dccf8d51c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104141752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c32ac88797c1d77c3a2969ababb3b493aef8d6e13466d46ab5288ff63613b89`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:40:39 GMT
ADD file:849d424ecc8572facb3ca68eff836dce211bc677cb32d3c3eaa129d364d33878 in / 
# Tue, 12 Jan 2021 00:40:43 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:34:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:34:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 23:34:31 GMT
ENV TELEGRAF_VERSION=1.15.4
# Tue, 12 Jan 2021 23:34:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Jan 2021 23:34:40 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Jan 2021 23:34:41 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 12 Jan 2021 23:34:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 23:34:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:6e5587ff5efa4e647ae927194fac9b961a68d46b23b68a3119c90016e58f17aa`  
		Last Modified: Tue, 12 Jan 2021 00:51:18 GMT  
		Size: 49.2 MB (49183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439dbbb05ea0aa8484ae8a51d0fbb1c7609176a1b0d3f15dad69d52e9a83af66`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 7.7 MB (7682325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b89c8b4e5b232c040d5905808ee62cdfcc9d697de10183d6bc4767468859d92`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 10.0 MB (9984327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc23f43b0bc1dd7f18ad8d9c699e4f57a322ad66aeb71996e6e8c9d2020abea`  
		Last Modified: Tue, 12 Jan 2021 23:35:36 GMT  
		Size: 17.3 MB (17269787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9c730332453078e166b4df31247ee7882c51ff0125356dab99e3a9dcc73661`  
		Last Modified: Tue, 12 Jan 2021 23:35:33 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467f513a28502825248b93776c150c2edac773b0a8deda5782ac26aacb6c8fda`  
		Last Modified: Tue, 12 Jan 2021 23:35:37 GMT  
		Size: 20.0 MB (20018497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5940454ec4499351669b0d9643b805223b801aeeae35aad1c8f4c505e6c8293`  
		Last Modified: Tue, 12 Jan 2021 23:35:32 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.15.4-alpine`

```console
$ docker pull telegraf@sha256:96ce9fc299ea4d2104226c69853925d5673213163d5b2ecd6c7608b8eb00dcf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.15.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:c62a89ed97872452cda722a9ba02c729a9fa8fe26576f4fc0226e0f3a54193c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27691802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19fc471fb0bc3c32b15eb8759d1a74f0ae35b9cb62ed5086317c2d81884bc65b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 04:32:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 29 Jan 2021 04:32:02 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 29 Jan 2021 04:32:02 GMT
ENV TELEGRAF_VERSION=1.15.4
# Fri, 29 Jan 2021 04:32:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 29 Jan 2021 04:32:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:32:07 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 29 Jan 2021 04:32:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:32:08 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8515c94ec9ad91ba3918826ef5b2ba1b7c93b4a38e742e74de299fb04e480b`  
		Last Modified: Fri, 29 Jan 2021 04:32:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2175f2277d79b6affe0726e5980e9af728b6e63f502812d8d76b1a6ec54f9dab`  
		Last Modified: Fri, 29 Jan 2021 04:32:57 GMT  
		Size: 3.3 MB (3339388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e468de6e594e2e20f6f7c9ba2ed5e528bf8792319c1a80c7ec9b4d253a85fa3`  
		Last Modified: Fri, 29 Jan 2021 04:33:01 GMT  
		Size: 21.5 MB (21540756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276e92457975f4fc56124c9d6c22830a9aa3c05781a5c1b70223189e170a7e83`  
		Last Modified: Fri, 29 Jan 2021 04:32:56 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.15-alpine`

```console
$ docker pull telegraf@sha256:96ce9fc299ea4d2104226c69853925d5673213163d5b2ecd6c7608b8eb00dcf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.15-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:c62a89ed97872452cda722a9ba02c729a9fa8fe26576f4fc0226e0f3a54193c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27691802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19fc471fb0bc3c32b15eb8759d1a74f0ae35b9cb62ed5086317c2d81884bc65b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 04:32:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 29 Jan 2021 04:32:02 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 29 Jan 2021 04:32:02 GMT
ENV TELEGRAF_VERSION=1.15.4
# Fri, 29 Jan 2021 04:32:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 29 Jan 2021 04:32:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:32:07 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 29 Jan 2021 04:32:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:32:08 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8515c94ec9ad91ba3918826ef5b2ba1b7c93b4a38e742e74de299fb04e480b`  
		Last Modified: Fri, 29 Jan 2021 04:32:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2175f2277d79b6affe0726e5980e9af728b6e63f502812d8d76b1a6ec54f9dab`  
		Last Modified: Fri, 29 Jan 2021 04:32:57 GMT  
		Size: 3.3 MB (3339388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e468de6e594e2e20f6f7c9ba2ed5e528bf8792319c1a80c7ec9b4d253a85fa3`  
		Last Modified: Fri, 29 Jan 2021 04:33:01 GMT  
		Size: 21.5 MB (21540756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276e92457975f4fc56124c9d6c22830a9aa3c05781a5c1b70223189e170a7e83`  
		Last Modified: Fri, 29 Jan 2021 04:32:56 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.16`

```console
$ docker pull telegraf@sha256:9992ebc551d2da0dade165a7900c7170517edca6271f80dd08cbadf63ed592d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.16` - linux; amd64

```console
$ docker pull telegraf@sha256:cfd86535105a3db65ee9376dc616188d7079312729e85ebcccd2361f6836e15d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107979992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d7c6bb6fbe6511ef8785e95770e7875a9c4695ef8db1c62c79348509a7e4dd3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jan 2021 04:53:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Jan 2021 04:53:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 Jan 2021 04:53:50 GMT
ENV TELEGRAF_VERSION=1.16.3
# Wed, 13 Jan 2021 04:53:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Jan 2021 04:53:54 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Jan 2021 04:53:54 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Jan 2021 04:53:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 04:53:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b1b9836397a1f6a8bcceaf48114f9358677f022f0872b44f5446fe6ac98590`  
		Last Modified: Wed, 13 Jan 2021 04:54:38 GMT  
		Size: 17.4 MB (17412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481d0989b3180f85249175a536a5497daf377815101a00b80ac6f3df31ba200`  
		Last Modified: Wed, 13 Jan 2021 04:54:32 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2022883ef76fd2042f2c9a1361ef5f1ea7039b1f8f177ea90fb5cada08aa9934`  
		Last Modified: Wed, 13 Jan 2021 04:54:53 GMT  
		Size: 22.4 MB (22357213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc3f56198ff41fcf7b780a82bfa12b23a3c612cd2431f2b5849536512b6ab0`  
		Last Modified: Wed, 13 Jan 2021 04:54:47 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.16` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c12c38f3ea1ce718149b1fbbe91b49ecc614745d82eb5fb9446b9e3872b667c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac5b0df4a786757ae9568b84facbfe72b33d585dd56f9198fc4c3a978a15689c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:00:37 GMT
ADD file:216371f6fe8c803a0191f84e555c809a3301d1344c62b831dddb5e0c595fe0ef in / 
# Tue, 12 Jan 2021 00:00:46 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:14:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:04:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 21:04:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 21:05:07 GMT
ENV TELEGRAF_VERSION=1.16.3
# Tue, 12 Jan 2021 21:05:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Jan 2021 21:05:13 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Jan 2021 21:05:17 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 12 Jan 2021 21:05:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 21:05:18 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d8925d905dadf63fa0ff74be912443a1cf8cd72ea5543317b0e22067d39ef948`  
		Last Modified: Tue, 12 Jan 2021 00:10:42 GMT  
		Size: 45.9 MB (45870031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd9c5a6d77413d17345fcf1f89b9dde2f3d9d6157bd070d4093cfef30107add`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 7.1 MB (7099141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e1f8e87a65e3a71764ea79b951f915c90a885dfd516f61e57d81745acaf272`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 9.3 MB (9343447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ec62dff3056e70cc453ec4b2d4db22debd86a42ddeaa47252e4672774bf7a8`  
		Last Modified: Tue, 12 Jan 2021 21:06:02 GMT  
		Size: 16.2 MB (16158602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7e36c129df27747aced5a1d50e367b06ee3dbdd9dcdb8ac6eb7c4e7e5132bd`  
		Last Modified: Tue, 12 Jan 2021 21:05:55 GMT  
		Size: 2.9 KB (2912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6351ac1e619db0b33a7984032acd52a3395879ecd293d235b758652251e80ed8`  
		Last Modified: Tue, 12 Jan 2021 21:06:24 GMT  
		Size: 20.9 MB (20889993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83deaf35291b5567f3444d93f6d5b4f3e87bc2f79b03a03cdc14cc2b3a1c792f`  
		Last Modified: Tue, 12 Jan 2021 21:06:17 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.16` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:1faba2fb159d06347c32bbacd8c260d4e7360f5a5e8cb3d7b5006f0cbc582744
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104617593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8497330190e6ed0cc29c85cf75354ecd675638f19dcba5e99a329e00b67fc8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:40:39 GMT
ADD file:849d424ecc8572facb3ca68eff836dce211bc677cb32d3c3eaa129d364d33878 in / 
# Tue, 12 Jan 2021 00:40:43 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:34:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:34:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 23:34:51 GMT
ENV TELEGRAF_VERSION=1.16.3
# Tue, 12 Jan 2021 23:34:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Jan 2021 23:34:56 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Jan 2021 23:34:57 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 12 Jan 2021 23:34:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 23:34:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:6e5587ff5efa4e647ae927194fac9b961a68d46b23b68a3119c90016e58f17aa`  
		Last Modified: Tue, 12 Jan 2021 00:51:18 GMT  
		Size: 49.2 MB (49183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439dbbb05ea0aa8484ae8a51d0fbb1c7609176a1b0d3f15dad69d52e9a83af66`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 7.7 MB (7682325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b89c8b4e5b232c040d5905808ee62cdfcc9d697de10183d6bc4767468859d92`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 10.0 MB (9984327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc23f43b0bc1dd7f18ad8d9c699e4f57a322ad66aeb71996e6e8c9d2020abea`  
		Last Modified: Tue, 12 Jan 2021 23:35:36 GMT  
		Size: 17.3 MB (17269787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9c730332453078e166b4df31247ee7882c51ff0125356dab99e3a9dcc73661`  
		Last Modified: Tue, 12 Jan 2021 23:35:33 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477c13ac3a95f511d0a0bb48dfc528a2e27b607f43c8dd5fc19e487c57850068`  
		Last Modified: Tue, 12 Jan 2021 23:35:52 GMT  
		Size: 20.5 MB (20494336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d41fa77d9b8d393ba80fdc5d52eb689cace7ef12603e5247c5ed899c476d91`  
		Last Modified: Tue, 12 Jan 2021 23:35:45 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.16.3`

```console
$ docker pull telegraf@sha256:9992ebc551d2da0dade165a7900c7170517edca6271f80dd08cbadf63ed592d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.16.3` - linux; amd64

```console
$ docker pull telegraf@sha256:cfd86535105a3db65ee9376dc616188d7079312729e85ebcccd2361f6836e15d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107979992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d7c6bb6fbe6511ef8785e95770e7875a9c4695ef8db1c62c79348509a7e4dd3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jan 2021 04:53:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Jan 2021 04:53:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 13 Jan 2021 04:53:50 GMT
ENV TELEGRAF_VERSION=1.16.3
# Wed, 13 Jan 2021 04:53:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Jan 2021 04:53:54 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Jan 2021 04:53:54 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Jan 2021 04:53:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 04:53:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b1b9836397a1f6a8bcceaf48114f9358677f022f0872b44f5446fe6ac98590`  
		Last Modified: Wed, 13 Jan 2021 04:54:38 GMT  
		Size: 17.4 MB (17412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481d0989b3180f85249175a536a5497daf377815101a00b80ac6f3df31ba200`  
		Last Modified: Wed, 13 Jan 2021 04:54:32 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2022883ef76fd2042f2c9a1361ef5f1ea7039b1f8f177ea90fb5cada08aa9934`  
		Last Modified: Wed, 13 Jan 2021 04:54:53 GMT  
		Size: 22.4 MB (22357213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc3f56198ff41fcf7b780a82bfa12b23a3c612cd2431f2b5849536512b6ab0`  
		Last Modified: Wed, 13 Jan 2021 04:54:47 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.16.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c12c38f3ea1ce718149b1fbbe91b49ecc614745d82eb5fb9446b9e3872b667c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac5b0df4a786757ae9568b84facbfe72b33d585dd56f9198fc4c3a978a15689c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:00:37 GMT
ADD file:216371f6fe8c803a0191f84e555c809a3301d1344c62b831dddb5e0c595fe0ef in / 
# Tue, 12 Jan 2021 00:00:46 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:14:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:04:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 21:04:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 21:05:07 GMT
ENV TELEGRAF_VERSION=1.16.3
# Tue, 12 Jan 2021 21:05:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Jan 2021 21:05:13 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Jan 2021 21:05:17 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 12 Jan 2021 21:05:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 21:05:18 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d8925d905dadf63fa0ff74be912443a1cf8cd72ea5543317b0e22067d39ef948`  
		Last Modified: Tue, 12 Jan 2021 00:10:42 GMT  
		Size: 45.9 MB (45870031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd9c5a6d77413d17345fcf1f89b9dde2f3d9d6157bd070d4093cfef30107add`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 7.1 MB (7099141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e1f8e87a65e3a71764ea79b951f915c90a885dfd516f61e57d81745acaf272`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 9.3 MB (9343447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ec62dff3056e70cc453ec4b2d4db22debd86a42ddeaa47252e4672774bf7a8`  
		Last Modified: Tue, 12 Jan 2021 21:06:02 GMT  
		Size: 16.2 MB (16158602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7e36c129df27747aced5a1d50e367b06ee3dbdd9dcdb8ac6eb7c4e7e5132bd`  
		Last Modified: Tue, 12 Jan 2021 21:05:55 GMT  
		Size: 2.9 KB (2912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6351ac1e619db0b33a7984032acd52a3395879ecd293d235b758652251e80ed8`  
		Last Modified: Tue, 12 Jan 2021 21:06:24 GMT  
		Size: 20.9 MB (20889993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83deaf35291b5567f3444d93f6d5b4f3e87bc2f79b03a03cdc14cc2b3a1c792f`  
		Last Modified: Tue, 12 Jan 2021 21:06:17 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.16.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:1faba2fb159d06347c32bbacd8c260d4e7360f5a5e8cb3d7b5006f0cbc582744
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104617593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8497330190e6ed0cc29c85cf75354ecd675638f19dcba5e99a329e00b67fc8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:40:39 GMT
ADD file:849d424ecc8572facb3ca68eff836dce211bc677cb32d3c3eaa129d364d33878 in / 
# Tue, 12 Jan 2021 00:40:43 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:34:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:34:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 12 Jan 2021 23:34:51 GMT
ENV TELEGRAF_VERSION=1.16.3
# Tue, 12 Jan 2021 23:34:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Jan 2021 23:34:56 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Jan 2021 23:34:57 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 12 Jan 2021 23:34:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Jan 2021 23:34:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:6e5587ff5efa4e647ae927194fac9b961a68d46b23b68a3119c90016e58f17aa`  
		Last Modified: Tue, 12 Jan 2021 00:51:18 GMT  
		Size: 49.2 MB (49183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439dbbb05ea0aa8484ae8a51d0fbb1c7609176a1b0d3f15dad69d52e9a83af66`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 7.7 MB (7682325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b89c8b4e5b232c040d5905808ee62cdfcc9d697de10183d6bc4767468859d92`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 10.0 MB (9984327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc23f43b0bc1dd7f18ad8d9c699e4f57a322ad66aeb71996e6e8c9d2020abea`  
		Last Modified: Tue, 12 Jan 2021 23:35:36 GMT  
		Size: 17.3 MB (17269787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9c730332453078e166b4df31247ee7882c51ff0125356dab99e3a9dcc73661`  
		Last Modified: Tue, 12 Jan 2021 23:35:33 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477c13ac3a95f511d0a0bb48dfc528a2e27b607f43c8dd5fc19e487c57850068`  
		Last Modified: Tue, 12 Jan 2021 23:35:52 GMT  
		Size: 20.5 MB (20494336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d41fa77d9b8d393ba80fdc5d52eb689cace7ef12603e5247c5ed899c476d91`  
		Last Modified: Tue, 12 Jan 2021 23:35:45 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.16.3-alpine`

```console
$ docker pull telegraf@sha256:6debe89a07f21f9f56b3f5fd7b04274c80bbdb7d1991927446785aa3990c3bc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.16.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7b696fe9e0c50a90d80c8649fc50ff48c4ab3e25995dd190a74be403d477c4e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28311927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95bd7e02fd4b6f4b5140c8c3bbe55789d20ca60684039940e5c7dcce9acd9c50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:12:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Thu, 17 Dec 2020 13:12:29 GMT
ENV TELEGRAF_VERSION=1.16.3
# Thu, 17 Dec 2020 13:12:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:12:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 17 Dec 2020 13:12:34 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Thu, 17 Dec 2020 13:12:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:12:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc126952e49fc432899db0576349c89a04f3ecbe722480dbcad6a332a82e5ff5`  
		Last Modified: Thu, 17 Dec 2020 13:12:59 GMT  
		Size: 3.3 MB (3298140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ec745bfd9cb880e27194c1eba0c4801c3c1ec611ac789733bab345573c8b77`  
		Last Modified: Thu, 17 Dec 2020 13:13:31 GMT  
		Size: 22.2 MB (22214386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d23340ef6fea8bbbec68e8c8fb6ccb725fa2a0dfea62991899d4d3d25c414f4`  
		Last Modified: Thu, 17 Dec 2020 13:13:26 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.16-alpine`

```console
$ docker pull telegraf@sha256:6debe89a07f21f9f56b3f5fd7b04274c80bbdb7d1991927446785aa3990c3bc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.16-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7b696fe9e0c50a90d80c8649fc50ff48c4ab3e25995dd190a74be403d477c4e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.3 MB (28311927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95bd7e02fd4b6f4b5140c8c3bbe55789d20ca60684039940e5c7dcce9acd9c50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:12:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Thu, 17 Dec 2020 13:12:29 GMT
ENV TELEGRAF_VERSION=1.16.3
# Thu, 17 Dec 2020 13:12:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 17 Dec 2020 13:12:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 17 Dec 2020 13:12:34 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Thu, 17 Dec 2020 13:12:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:12:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc126952e49fc432899db0576349c89a04f3ecbe722480dbcad6a332a82e5ff5`  
		Last Modified: Thu, 17 Dec 2020 13:12:59 GMT  
		Size: 3.3 MB (3298140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ec745bfd9cb880e27194c1eba0c4801c3c1ec611ac789733bab345573c8b77`  
		Last Modified: Thu, 17 Dec 2020 13:13:31 GMT  
		Size: 22.2 MB (22214386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d23340ef6fea8bbbec68e8c8fb6ccb725fa2a0dfea62991899d4d3d25c414f4`  
		Last Modified: Thu, 17 Dec 2020 13:13:26 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.17`

```console
$ docker pull telegraf@sha256:c9703aa340e2c28306c93c3b0eff87e0760f20cf8f299ad577220a62b61cbb0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.17` - linux; amd64

```console
$ docker pull telegraf@sha256:a05a950f2d426641b1f549806943ee1f7f862522a004aa5a1ff91bd0d662ee84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108348187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fe56be3a20fc85dc845c8c73e677bb9c51a4757cb632af00f18c63b27a3ce05`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jan 2021 04:53:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Jan 2021 04:53:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 29 Jan 2021 04:32:20 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:32:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jan 2021 04:32:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:32:24 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 29 Jan 2021 04:32:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:32:25 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b1b9836397a1f6a8bcceaf48114f9358677f022f0872b44f5446fe6ac98590`  
		Last Modified: Wed, 13 Jan 2021 04:54:38 GMT  
		Size: 17.4 MB (17412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481d0989b3180f85249175a536a5497daf377815101a00b80ac6f3df31ba200`  
		Last Modified: Wed, 13 Jan 2021 04:54:32 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b755b74a2742266b814d5b3f189f8e1763c5138ddd24a6b2179e019925a4378`  
		Last Modified: Fri, 29 Jan 2021 04:33:11 GMT  
		Size: 22.7 MB (22725409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395a1e47e5e9b6e8ad986cfc21c216a8c86294cc0d34e0b13b0681af187bc85c`  
		Last Modified: Fri, 29 Jan 2021 04:33:06 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:7e0d8987bebc8d24153705131c229a5274dcedc4ee2ff9de098de4c7e6f96e1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.7 MB (99708947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523df42dd23af807a491666f653b94fd3064f358c3544aac180091a4af4b569b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:00:37 GMT
ADD file:216371f6fe8c803a0191f84e555c809a3301d1344c62b831dddb5e0c595fe0ef in / 
# Tue, 12 Jan 2021 00:00:46 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:14:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:04:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 21:04:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 29 Jan 2021 04:16:37 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:16:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jan 2021 04:16:54 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:16:54 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 29 Jan 2021 04:16:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:16:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d8925d905dadf63fa0ff74be912443a1cf8cd72ea5543317b0e22067d39ef948`  
		Last Modified: Tue, 12 Jan 2021 00:10:42 GMT  
		Size: 45.9 MB (45870031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd9c5a6d77413d17345fcf1f89b9dde2f3d9d6157bd070d4093cfef30107add`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 7.1 MB (7099141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e1f8e87a65e3a71764ea79b951f915c90a885dfd516f61e57d81745acaf272`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 9.3 MB (9343447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ec62dff3056e70cc453ec4b2d4db22debd86a42ddeaa47252e4672774bf7a8`  
		Last Modified: Tue, 12 Jan 2021 21:06:02 GMT  
		Size: 16.2 MB (16158602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7e36c129df27747aced5a1d50e367b06ee3dbdd9dcdb8ac6eb7c4e7e5132bd`  
		Last Modified: Tue, 12 Jan 2021 21:05:55 GMT  
		Size: 2.9 KB (2912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f6e296701c348c1a4d28fb053edb46058edf5feb68997a6b2f0552a67a10d`  
		Last Modified: Fri, 29 Jan 2021 04:17:25 GMT  
		Size: 21.2 MB (21234629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bfeb9de72b585eed2cb391ccfc0ac5f473624e9009c1514549e901189d0670`  
		Last Modified: Fri, 29 Jan 2021 04:17:17 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:651938aebe1d3b6accbe82c69ec5d8bbc98d084f5dd9b9cfd18caae88444dfd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104952179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38f0051c6073a114822ef9eb096346a7656a0afeaf89bd69fe975e09134985b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:40:39 GMT
ADD file:849d424ecc8572facb3ca68eff836dce211bc677cb32d3c3eaa129d364d33878 in / 
# Tue, 12 Jan 2021 00:40:43 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:34:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:34:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 29 Jan 2021 04:13:54 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:13:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jan 2021 04:14:00 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:14:01 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 29 Jan 2021 04:14:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:14:03 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:6e5587ff5efa4e647ae927194fac9b961a68d46b23b68a3119c90016e58f17aa`  
		Last Modified: Tue, 12 Jan 2021 00:51:18 GMT  
		Size: 49.2 MB (49183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439dbbb05ea0aa8484ae8a51d0fbb1c7609176a1b0d3f15dad69d52e9a83af66`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 7.7 MB (7682325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b89c8b4e5b232c040d5905808ee62cdfcc9d697de10183d6bc4767468859d92`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 10.0 MB (9984327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc23f43b0bc1dd7f18ad8d9c699e4f57a322ad66aeb71996e6e8c9d2020abea`  
		Last Modified: Tue, 12 Jan 2021 23:35:36 GMT  
		Size: 17.3 MB (17269787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9c730332453078e166b4df31247ee7882c51ff0125356dab99e3a9dcc73661`  
		Last Modified: Tue, 12 Jan 2021 23:35:33 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b744ede9fee749f06d0138e246498a252f7df3d72235125aba8f193973aa51`  
		Last Modified: Fri, 29 Jan 2021 04:14:25 GMT  
		Size: 20.8 MB (20828925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58647fe3c3c17ecc0faba5068f12ffd2765aac0c065816a6865bb42875d25d3e`  
		Last Modified: Fri, 29 Jan 2021 04:14:18 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.17.2`

```console
$ docker pull telegraf@sha256:c9703aa340e2c28306c93c3b0eff87e0760f20cf8f299ad577220a62b61cbb0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.17.2` - linux; amd64

```console
$ docker pull telegraf@sha256:a05a950f2d426641b1f549806943ee1f7f862522a004aa5a1ff91bd0d662ee84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108348187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fe56be3a20fc85dc845c8c73e677bb9c51a4757cb632af00f18c63b27a3ce05`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jan 2021 04:53:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Jan 2021 04:53:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 29 Jan 2021 04:32:20 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:32:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jan 2021 04:32:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:32:24 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 29 Jan 2021 04:32:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:32:25 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b1b9836397a1f6a8bcceaf48114f9358677f022f0872b44f5446fe6ac98590`  
		Last Modified: Wed, 13 Jan 2021 04:54:38 GMT  
		Size: 17.4 MB (17412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481d0989b3180f85249175a536a5497daf377815101a00b80ac6f3df31ba200`  
		Last Modified: Wed, 13 Jan 2021 04:54:32 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b755b74a2742266b814d5b3f189f8e1763c5138ddd24a6b2179e019925a4378`  
		Last Modified: Fri, 29 Jan 2021 04:33:11 GMT  
		Size: 22.7 MB (22725409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395a1e47e5e9b6e8ad986cfc21c216a8c86294cc0d34e0b13b0681af187bc85c`  
		Last Modified: Fri, 29 Jan 2021 04:33:06 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17.2` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:7e0d8987bebc8d24153705131c229a5274dcedc4ee2ff9de098de4c7e6f96e1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.7 MB (99708947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523df42dd23af807a491666f653b94fd3064f358c3544aac180091a4af4b569b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:00:37 GMT
ADD file:216371f6fe8c803a0191f84e555c809a3301d1344c62b831dddb5e0c595fe0ef in / 
# Tue, 12 Jan 2021 00:00:46 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:14:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:04:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 21:04:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 29 Jan 2021 04:16:37 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:16:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jan 2021 04:16:54 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:16:54 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 29 Jan 2021 04:16:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:16:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d8925d905dadf63fa0ff74be912443a1cf8cd72ea5543317b0e22067d39ef948`  
		Last Modified: Tue, 12 Jan 2021 00:10:42 GMT  
		Size: 45.9 MB (45870031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd9c5a6d77413d17345fcf1f89b9dde2f3d9d6157bd070d4093cfef30107add`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 7.1 MB (7099141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e1f8e87a65e3a71764ea79b951f915c90a885dfd516f61e57d81745acaf272`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 9.3 MB (9343447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ec62dff3056e70cc453ec4b2d4db22debd86a42ddeaa47252e4672774bf7a8`  
		Last Modified: Tue, 12 Jan 2021 21:06:02 GMT  
		Size: 16.2 MB (16158602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7e36c129df27747aced5a1d50e367b06ee3dbdd9dcdb8ac6eb7c4e7e5132bd`  
		Last Modified: Tue, 12 Jan 2021 21:05:55 GMT  
		Size: 2.9 KB (2912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f6e296701c348c1a4d28fb053edb46058edf5feb68997a6b2f0552a67a10d`  
		Last Modified: Fri, 29 Jan 2021 04:17:25 GMT  
		Size: 21.2 MB (21234629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bfeb9de72b585eed2cb391ccfc0ac5f473624e9009c1514549e901189d0670`  
		Last Modified: Fri, 29 Jan 2021 04:17:17 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17.2` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:651938aebe1d3b6accbe82c69ec5d8bbc98d084f5dd9b9cfd18caae88444dfd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104952179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38f0051c6073a114822ef9eb096346a7656a0afeaf89bd69fe975e09134985b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:40:39 GMT
ADD file:849d424ecc8572facb3ca68eff836dce211bc677cb32d3c3eaa129d364d33878 in / 
# Tue, 12 Jan 2021 00:40:43 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:34:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:34:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 29 Jan 2021 04:13:54 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:13:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jan 2021 04:14:00 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:14:01 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 29 Jan 2021 04:14:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:14:03 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:6e5587ff5efa4e647ae927194fac9b961a68d46b23b68a3119c90016e58f17aa`  
		Last Modified: Tue, 12 Jan 2021 00:51:18 GMT  
		Size: 49.2 MB (49183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439dbbb05ea0aa8484ae8a51d0fbb1c7609176a1b0d3f15dad69d52e9a83af66`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 7.7 MB (7682325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b89c8b4e5b232c040d5905808ee62cdfcc9d697de10183d6bc4767468859d92`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 10.0 MB (9984327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc23f43b0bc1dd7f18ad8d9c699e4f57a322ad66aeb71996e6e8c9d2020abea`  
		Last Modified: Tue, 12 Jan 2021 23:35:36 GMT  
		Size: 17.3 MB (17269787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9c730332453078e166b4df31247ee7882c51ff0125356dab99e3a9dcc73661`  
		Last Modified: Tue, 12 Jan 2021 23:35:33 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b744ede9fee749f06d0138e246498a252f7df3d72235125aba8f193973aa51`  
		Last Modified: Fri, 29 Jan 2021 04:14:25 GMT  
		Size: 20.8 MB (20828925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58647fe3c3c17ecc0faba5068f12ffd2765aac0c065816a6865bb42875d25d3e`  
		Last Modified: Fri, 29 Jan 2021 04:14:18 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.17.2-alpine`

```console
$ docker pull telegraf@sha256:c487479e3aec32e8fd29433a61c2d3a8d18ca32d468e827144eda8a23b303090
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.17.2-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:d2f192af79ad1d2a33be626b0d38cc3a8f877671224c44c3a25d935481d64113
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28688307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9859a8cdeedb56f85d812ba6a95a1ec3c0430c8a8424f8f7db56c705026bd3ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:12:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 29 Jan 2021 04:32:30 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:32:34 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 29 Jan 2021 04:32:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:32:34 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 29 Jan 2021 04:32:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:32:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc126952e49fc432899db0576349c89a04f3ecbe722480dbcad6a332a82e5ff5`  
		Last Modified: Thu, 17 Dec 2020 13:12:59 GMT  
		Size: 3.3 MB (3298140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3752da50fd464657ab29f7440867850025ad4b1bf2ea24c221e01dca0a6e3352`  
		Last Modified: Fri, 29 Jan 2021 04:33:21 GMT  
		Size: 22.6 MB (22590765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763ba331b899fb53992b81c5b159b98d56cb292177445c9b1ae0f9789824d295`  
		Last Modified: Fri, 29 Jan 2021 04:33:16 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.17-alpine`

```console
$ docker pull telegraf@sha256:c487479e3aec32e8fd29433a61c2d3a8d18ca32d468e827144eda8a23b303090
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.17-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:d2f192af79ad1d2a33be626b0d38cc3a8f877671224c44c3a25d935481d64113
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28688307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9859a8cdeedb56f85d812ba6a95a1ec3c0430c8a8424f8f7db56c705026bd3ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:12:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 29 Jan 2021 04:32:30 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:32:34 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 29 Jan 2021 04:32:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:32:34 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 29 Jan 2021 04:32:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:32:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc126952e49fc432899db0576349c89a04f3ecbe722480dbcad6a332a82e5ff5`  
		Last Modified: Thu, 17 Dec 2020 13:12:59 GMT  
		Size: 3.3 MB (3298140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3752da50fd464657ab29f7440867850025ad4b1bf2ea24c221e01dca0a6e3352`  
		Last Modified: Fri, 29 Jan 2021 04:33:21 GMT  
		Size: 22.6 MB (22590765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763ba331b899fb53992b81c5b159b98d56cb292177445c9b1ae0f9789824d295`  
		Last Modified: Fri, 29 Jan 2021 04:33:16 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:c487479e3aec32e8fd29433a61c2d3a8d18ca32d468e827144eda8a23b303090
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:d2f192af79ad1d2a33be626b0d38cc3a8f877671224c44c3a25d935481d64113
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.7 MB (28688307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9859a8cdeedb56f85d812ba6a95a1ec3c0430c8a8424f8f7db56c705026bd3ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:07:52 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 17 Dec 2020 13:12:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 29 Jan 2021 04:32:30 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:32:34 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 29 Jan 2021 04:32:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:32:34 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 29 Jan 2021 04:32:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:32:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac210e4df99beaffbde65dfe580e9923c2bef3b5dd07f0ac7d364e47dc2fac52`  
		Last Modified: Thu, 17 Dec 2020 13:09:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc126952e49fc432899db0576349c89a04f3ecbe722480dbcad6a332a82e5ff5`  
		Last Modified: Thu, 17 Dec 2020 13:12:59 GMT  
		Size: 3.3 MB (3298140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3752da50fd464657ab29f7440867850025ad4b1bf2ea24c221e01dca0a6e3352`  
		Last Modified: Fri, 29 Jan 2021 04:33:21 GMT  
		Size: 22.6 MB (22590765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763ba331b899fb53992b81c5b159b98d56cb292177445c9b1ae0f9789824d295`  
		Last Modified: Fri, 29 Jan 2021 04:33:16 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:c9703aa340e2c28306c93c3b0eff87e0760f20cf8f299ad577220a62b61cbb0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:a05a950f2d426641b1f549806943ee1f7f862522a004aa5a1ff91bd0d662ee84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108348187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fe56be3a20fc85dc845c8c73e677bb9c51a4757cb632af00f18c63b27a3ce05`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jan 2021 04:53:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Jan 2021 04:53:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 29 Jan 2021 04:32:20 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:32:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jan 2021 04:32:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:32:24 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 29 Jan 2021 04:32:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:32:25 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b1b9836397a1f6a8bcceaf48114f9358677f022f0872b44f5446fe6ac98590`  
		Last Modified: Wed, 13 Jan 2021 04:54:38 GMT  
		Size: 17.4 MB (17412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481d0989b3180f85249175a536a5497daf377815101a00b80ac6f3df31ba200`  
		Last Modified: Wed, 13 Jan 2021 04:54:32 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b755b74a2742266b814d5b3f189f8e1763c5138ddd24a6b2179e019925a4378`  
		Last Modified: Fri, 29 Jan 2021 04:33:11 GMT  
		Size: 22.7 MB (22725409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395a1e47e5e9b6e8ad986cfc21c216a8c86294cc0d34e0b13b0681af187bc85c`  
		Last Modified: Fri, 29 Jan 2021 04:33:06 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:7e0d8987bebc8d24153705131c229a5274dcedc4ee2ff9de098de4c7e6f96e1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.7 MB (99708947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523df42dd23af807a491666f653b94fd3064f358c3544aac180091a4af4b569b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:00:37 GMT
ADD file:216371f6fe8c803a0191f84e555c809a3301d1344c62b831dddb5e0c595fe0ef in / 
# Tue, 12 Jan 2021 00:00:46 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:14:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 21:04:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 21:04:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 29 Jan 2021 04:16:37 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:16:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jan 2021 04:16:54 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:16:54 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 29 Jan 2021 04:16:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:16:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d8925d905dadf63fa0ff74be912443a1cf8cd72ea5543317b0e22067d39ef948`  
		Last Modified: Tue, 12 Jan 2021 00:10:42 GMT  
		Size: 45.9 MB (45870031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd9c5a6d77413d17345fcf1f89b9dde2f3d9d6157bd070d4093cfef30107add`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 7.1 MB (7099141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e1f8e87a65e3a71764ea79b951f915c90a885dfd516f61e57d81745acaf272`  
		Last Modified: Tue, 12 Jan 2021 01:29:46 GMT  
		Size: 9.3 MB (9343447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ec62dff3056e70cc453ec4b2d4db22debd86a42ddeaa47252e4672774bf7a8`  
		Last Modified: Tue, 12 Jan 2021 21:06:02 GMT  
		Size: 16.2 MB (16158602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7e36c129df27747aced5a1d50e367b06ee3dbdd9dcdb8ac6eb7c4e7e5132bd`  
		Last Modified: Tue, 12 Jan 2021 21:05:55 GMT  
		Size: 2.9 KB (2912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f6e296701c348c1a4d28fb053edb46058edf5feb68997a6b2f0552a67a10d`  
		Last Modified: Fri, 29 Jan 2021 04:17:25 GMT  
		Size: 21.2 MB (21234629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bfeb9de72b585eed2cb391ccfc0ac5f473624e9009c1514549e901189d0670`  
		Last Modified: Fri, 29 Jan 2021 04:17:17 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:651938aebe1d3b6accbe82c69ec5d8bbc98d084f5dd9b9cfd18caae88444dfd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104952179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38f0051c6073a114822ef9eb096346a7656a0afeaf89bd69fe975e09134985b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:40:39 GMT
ADD file:849d424ecc8572facb3ca68eff836dce211bc677cb32d3c3eaa129d364d33878 in / 
# Tue, 12 Jan 2021 00:40:43 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 23:34:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:34:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 29 Jan 2021 04:13:54 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:13:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jan 2021 04:14:00 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:14:01 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 29 Jan 2021 04:14:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:14:03 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:6e5587ff5efa4e647ae927194fac9b961a68d46b23b68a3119c90016e58f17aa`  
		Last Modified: Tue, 12 Jan 2021 00:51:18 GMT  
		Size: 49.2 MB (49183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439dbbb05ea0aa8484ae8a51d0fbb1c7609176a1b0d3f15dad69d52e9a83af66`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 7.7 MB (7682325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b89c8b4e5b232c040d5905808ee62cdfcc9d697de10183d6bc4767468859d92`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 10.0 MB (9984327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc23f43b0bc1dd7f18ad8d9c699e4f57a322ad66aeb71996e6e8c9d2020abea`  
		Last Modified: Tue, 12 Jan 2021 23:35:36 GMT  
		Size: 17.3 MB (17269787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9c730332453078e166b4df31247ee7882c51ff0125356dab99e3a9dcc73661`  
		Last Modified: Tue, 12 Jan 2021 23:35:33 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b744ede9fee749f06d0138e246498a252f7df3d72235125aba8f193973aa51`  
		Last Modified: Fri, 29 Jan 2021 04:14:25 GMT  
		Size: 20.8 MB (20828925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58647fe3c3c17ecc0faba5068f12ffd2765aac0c065816a6865bb42875d25d3e`  
		Last Modified: Fri, 29 Jan 2021 04:14:18 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
