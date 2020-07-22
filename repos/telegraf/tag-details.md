<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.12`](#telegraf112)
-	[`telegraf:1.12.6`](#telegraf1126)
-	[`telegraf:1.12.6-alpine`](#telegraf1126-alpine)
-	[`telegraf:1.12-alpine`](#telegraf112-alpine)
-	[`telegraf:1.13`](#telegraf113)
-	[`telegraf:1.13.4`](#telegraf1134)
-	[`telegraf:1.13.4-alpine`](#telegraf1134-alpine)
-	[`telegraf:1.13-alpine`](#telegraf113-alpine)
-	[`telegraf:1.14`](#telegraf114)
-	[`telegraf:1.14.5`](#telegraf1145)
-	[`telegraf:1.14.5-alpine`](#telegraf1145-alpine)
-	[`telegraf:1.14-alpine`](#telegraf114-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.12`

```console
$ docker pull telegraf@sha256:c0c3c9a321611549f48d8aa3623441f6e660bad0dd381e5b93a7c1f3a25a2316
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.12` - linux; amd64

```console
$ docker pull telegraf@sha256:d6b18c6a463dd4f3bc24687d91dc71e77895b05b6bf6e5f3788a850ef5d2ab6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97800621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b6d302ca3cbc786857a3d39f5ce97e055d407caf07febd68e41e10e80e2db7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:47:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 02:47:07 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:47:07 GMT
ENV TELEGRAF_VERSION=1.12.6
# Wed, 10 Jun 2020 02:47:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 10 Jun 2020 02:47:11 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 10 Jun 2020 02:47:11 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:47:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:47:12 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b69ee1aa5fd2053c60bb7876c57cccda6bb9f6e767638a73cd3a29f9df3016a`  
		Last Modified: Wed, 10 Jun 2020 02:47:58 GMT  
		Size: 16.0 MB (15964407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5666e6b82a727d7af99bf2df78a19e9756471cecc4e7e4d92502b7ed418643`  
		Last Modified: Wed, 10 Jun 2020 02:47:55 GMT  
		Size: 2.8 KB (2772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1420c188d305fdf0a34bc77c4b129ab2be99b53c38d7a02725252fa13649be05`  
		Last Modified: Wed, 10 Jun 2020 02:47:59 GMT  
		Size: 21.4 MB (21368551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cdcbf5ee97b220d1d39fa37d47f4271d414392635f5e13727de03d3f50802a`  
		Last Modified: Wed, 10 Jun 2020 02:47:54 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.12` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:a357b64c4dd9a9c65f4b12480180371ba989987132d4b305d6e4dfb25ca628a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90472694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009bd4c26a41c4921b00b47591043c8387a8ba97370be2b8cab11cf100db819a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 22 Jul 2020 01:32:02 GMT
ADD file:762e52a5e1d8ff2daa22c3bec2cfdfe4cbcf224deb1e73d7db3af0cbf5658785 in / 
# Wed, 22 Jul 2020 01:32:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:50:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 20:50:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:50:25 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 22 Jul 2020 20:50:26 GMT
ENV TELEGRAF_VERSION=1.12.6
# Wed, 22 Jul 2020 20:50:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Jul 2020 20:50:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Jul 2020 20:50:34 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 22 Jul 2020 20:50:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 20:50:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:05dc12a0df610a09562914533797508b791bbd115ae17b6a1b75666ec90263da`  
		Last Modified: Wed, 22 Jul 2020 01:44:04 GMT  
		Size: 42.1 MB (42107480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b998b2d4ee2005b0f51e94b6fc7467091e54a910491e7873b9e0d6f59aabd98`  
		Last Modified: Wed, 22 Jul 2020 06:06:37 GMT  
		Size: 9.4 MB (9444083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15230f55c10a543d54564a792784b1d2e133d4edeadd58978682d9bf02d1425a`  
		Last Modified: Wed, 22 Jul 2020 06:06:34 GMT  
		Size: 3.9 MB (3918506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8ed6da9c9a9b6a83c45713f25bc874233a2ed8a57ffdd0fcdfd8fc3b70c41`  
		Last Modified: Wed, 22 Jul 2020 20:51:39 GMT  
		Size: 14.8 MB (14838306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d146b77fdedc3c75ccf0db81330d0afb9d3a27da887066550bfba1f169358f`  
		Last Modified: Wed, 22 Jul 2020 20:51:34 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1466e1f68da061cf9662ffb310d9f5cc70ab897e6de058081f6b9b49aff675dd`  
		Last Modified: Wed, 22 Jul 2020 20:51:43 GMT  
		Size: 20.2 MB (20161332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a4a9983bf8a7b8a5cb1e82f0c1489baea79ff588c93736401212670135f550`  
		Last Modified: Wed, 22 Jul 2020 20:51:34 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.12` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:dc5f3484ca7aa461bb7b7f615c95adc699aa27cec37b8aa5be4314c1542c66ad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92219835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5314d0537bb82aba353bd70ab5fbaf97947f9e8c0b62b96efbc24b1bcc72bb0c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 22:28:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 22:28:59 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 22:29:00 GMT
ENV TELEGRAF_VERSION=1.12.6
# Tue, 09 Jun 2020 22:29:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 09 Jun 2020 22:29:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 09 Jun 2020 22:29:06 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 09 Jun 2020 22:29:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 22:29:07 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a373e9cf9ef79f55bd10fc3f195dc6b5087ab63fbff958f993f128f050a1d5`  
		Last Modified: Tue, 09 Jun 2020 22:30:07 GMT  
		Size: 15.5 MB (15529632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838987d1084e45c5cfc56c78edf137c89d5460b702b72d1cccdbdb5d6cf1424`  
		Last Modified: Tue, 09 Jun 2020 22:30:02 GMT  
		Size: 2.8 KB (2807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e9a57abb9fbaf186e999de617b0d561354d3d8919f979ccce9bcb2570dfec5`  
		Last Modified: Tue, 09 Jun 2020 22:30:10 GMT  
		Size: 19.7 MB (19732549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6a395ee3a85e52887efe6b8416cbfe2b8083f30526c0c89628924750084cc4`  
		Last Modified: Tue, 09 Jun 2020 22:30:02 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.12.6`

```console
$ docker pull telegraf@sha256:c0c3c9a321611549f48d8aa3623441f6e660bad0dd381e5b93a7c1f3a25a2316
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.12.6` - linux; amd64

```console
$ docker pull telegraf@sha256:d6b18c6a463dd4f3bc24687d91dc71e77895b05b6bf6e5f3788a850ef5d2ab6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97800621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b6d302ca3cbc786857a3d39f5ce97e055d407caf07febd68e41e10e80e2db7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:47:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 02:47:07 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:47:07 GMT
ENV TELEGRAF_VERSION=1.12.6
# Wed, 10 Jun 2020 02:47:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 10 Jun 2020 02:47:11 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 10 Jun 2020 02:47:11 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:47:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:47:12 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b69ee1aa5fd2053c60bb7876c57cccda6bb9f6e767638a73cd3a29f9df3016a`  
		Last Modified: Wed, 10 Jun 2020 02:47:58 GMT  
		Size: 16.0 MB (15964407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5666e6b82a727d7af99bf2df78a19e9756471cecc4e7e4d92502b7ed418643`  
		Last Modified: Wed, 10 Jun 2020 02:47:55 GMT  
		Size: 2.8 KB (2772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1420c188d305fdf0a34bc77c4b129ab2be99b53c38d7a02725252fa13649be05`  
		Last Modified: Wed, 10 Jun 2020 02:47:59 GMT  
		Size: 21.4 MB (21368551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cdcbf5ee97b220d1d39fa37d47f4271d414392635f5e13727de03d3f50802a`  
		Last Modified: Wed, 10 Jun 2020 02:47:54 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.12.6` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:a357b64c4dd9a9c65f4b12480180371ba989987132d4b305d6e4dfb25ca628a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90472694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009bd4c26a41c4921b00b47591043c8387a8ba97370be2b8cab11cf100db819a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 22 Jul 2020 01:32:02 GMT
ADD file:762e52a5e1d8ff2daa22c3bec2cfdfe4cbcf224deb1e73d7db3af0cbf5658785 in / 
# Wed, 22 Jul 2020 01:32:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:50:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 20:50:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:50:25 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 22 Jul 2020 20:50:26 GMT
ENV TELEGRAF_VERSION=1.12.6
# Wed, 22 Jul 2020 20:50:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Jul 2020 20:50:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Jul 2020 20:50:34 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 22 Jul 2020 20:50:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 20:50:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:05dc12a0df610a09562914533797508b791bbd115ae17b6a1b75666ec90263da`  
		Last Modified: Wed, 22 Jul 2020 01:44:04 GMT  
		Size: 42.1 MB (42107480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b998b2d4ee2005b0f51e94b6fc7467091e54a910491e7873b9e0d6f59aabd98`  
		Last Modified: Wed, 22 Jul 2020 06:06:37 GMT  
		Size: 9.4 MB (9444083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15230f55c10a543d54564a792784b1d2e133d4edeadd58978682d9bf02d1425a`  
		Last Modified: Wed, 22 Jul 2020 06:06:34 GMT  
		Size: 3.9 MB (3918506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8ed6da9c9a9b6a83c45713f25bc874233a2ed8a57ffdd0fcdfd8fc3b70c41`  
		Last Modified: Wed, 22 Jul 2020 20:51:39 GMT  
		Size: 14.8 MB (14838306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d146b77fdedc3c75ccf0db81330d0afb9d3a27da887066550bfba1f169358f`  
		Last Modified: Wed, 22 Jul 2020 20:51:34 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1466e1f68da061cf9662ffb310d9f5cc70ab897e6de058081f6b9b49aff675dd`  
		Last Modified: Wed, 22 Jul 2020 20:51:43 GMT  
		Size: 20.2 MB (20161332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a4a9983bf8a7b8a5cb1e82f0c1489baea79ff588c93736401212670135f550`  
		Last Modified: Wed, 22 Jul 2020 20:51:34 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.12.6` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:dc5f3484ca7aa461bb7b7f615c95adc699aa27cec37b8aa5be4314c1542c66ad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92219835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5314d0537bb82aba353bd70ab5fbaf97947f9e8c0b62b96efbc24b1bcc72bb0c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 22:28:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 22:28:59 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 22:29:00 GMT
ENV TELEGRAF_VERSION=1.12.6
# Tue, 09 Jun 2020 22:29:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 09 Jun 2020 22:29:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 09 Jun 2020 22:29:06 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 09 Jun 2020 22:29:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 22:29:07 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a373e9cf9ef79f55bd10fc3f195dc6b5087ab63fbff958f993f128f050a1d5`  
		Last Modified: Tue, 09 Jun 2020 22:30:07 GMT  
		Size: 15.5 MB (15529632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838987d1084e45c5cfc56c78edf137c89d5460b702b72d1cccdbdb5d6cf1424`  
		Last Modified: Tue, 09 Jun 2020 22:30:02 GMT  
		Size: 2.8 KB (2807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e9a57abb9fbaf186e999de617b0d561354d3d8919f979ccce9bcb2570dfec5`  
		Last Modified: Tue, 09 Jun 2020 22:30:10 GMT  
		Size: 19.7 MB (19732549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6a395ee3a85e52887efe6b8416cbfe2b8083f30526c0c89628924750084cc4`  
		Last Modified: Tue, 09 Jun 2020 22:30:02 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.12.6-alpine`

```console
$ docker pull telegraf@sha256:88f59aacd3dbef010bdd5cb6527e852e933a1b79a2e907e61666bb0f8e92013a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.12.6-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7b0c8a6d7cd0a4ba7646b3c5926ef44a490a3a8d4e9f89cca2889a928d70a822
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27854316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2e6a0fe70f163b3ba1c3df5c28d7f0dbdda50ae967cf10b79e5b28a28623082`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 24 Apr 2020 14:24:06 GMT
ENV TELEGRAF_VERSION=1.12.6
# Fri, 24 Apr 2020 14:24:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:24:10 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 24 Apr 2020 14:24:10 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 24 Apr 2020 14:24:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:24:11 GMT
CMD ["telegraf"]
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
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d142ff75baa0a44652c2874af91eb8b22457112d6f9a3ccabc2199ba2d97c99`  
		Last Modified: Fri, 24 Apr 2020 14:24:52 GMT  
		Size: 21.4 MB (21360269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce28b0bfe86cf8633862376618d78142310380ab980d43015959151806e28958`  
		Last Modified: Fri, 24 Apr 2020 14:24:48 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.12-alpine`

```console
$ docker pull telegraf@sha256:88f59aacd3dbef010bdd5cb6527e852e933a1b79a2e907e61666bb0f8e92013a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.12-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7b0c8a6d7cd0a4ba7646b3c5926ef44a490a3a8d4e9f89cca2889a928d70a822
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27854316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2e6a0fe70f163b3ba1c3df5c28d7f0dbdda50ae967cf10b79e5b28a28623082`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 24 Apr 2020 14:24:06 GMT
ENV TELEGRAF_VERSION=1.12.6
# Fri, 24 Apr 2020 14:24:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:24:10 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 24 Apr 2020 14:24:10 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 24 Apr 2020 14:24:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:24:11 GMT
CMD ["telegraf"]
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
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d142ff75baa0a44652c2874af91eb8b22457112d6f9a3ccabc2199ba2d97c99`  
		Last Modified: Fri, 24 Apr 2020 14:24:52 GMT  
		Size: 21.4 MB (21360269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce28b0bfe86cf8633862376618d78142310380ab980d43015959151806e28958`  
		Last Modified: Fri, 24 Apr 2020 14:24:48 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.13`

```console
$ docker pull telegraf@sha256:af0ebd18bcefdf61ffd18818ace9833b768702aa95c8d044fb8998a375adc4bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.13` - linux; amd64

```console
$ docker pull telegraf@sha256:153cc69d000d5dfe7c7289d5cf4e1afc747bd0acc3455add8352a05990950280
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96743847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:964e3109d3780d9341e57ad616ad0da82d4a2d86b7e259760822c2bb2609a25e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:47:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 02:47:07 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:47:20 GMT
ENV TELEGRAF_VERSION=1.13.4
# Wed, 10 Jun 2020 02:47:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 10 Jun 2020 02:47:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 10 Jun 2020 02:47:23 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:47:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:47:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b69ee1aa5fd2053c60bb7876c57cccda6bb9f6e767638a73cd3a29f9df3016a`  
		Last Modified: Wed, 10 Jun 2020 02:47:58 GMT  
		Size: 16.0 MB (15964407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5666e6b82a727d7af99bf2df78a19e9756471cecc4e7e4d92502b7ed418643`  
		Last Modified: Wed, 10 Jun 2020 02:47:55 GMT  
		Size: 2.8 KB (2772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ee3991d8d9d61efaf09a444e63633d183077f58c955d267e2df91936f08cc7`  
		Last Modified: Wed, 10 Jun 2020 02:48:07 GMT  
		Size: 20.3 MB (20311776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d97d8975b5d5b4032df55d3b2165a9c5364600f5483e4c0ee5f12e1d243fb1`  
		Last Modified: Wed, 10 Jun 2020 02:48:03 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.13` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:9d395b855ac92448cdab3c99b4e0d288e08e2b693c755ecb41d4628b7082e172
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89364441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ffe3fcad0972f1f525e37908f79e117ade897520b3a49f95fbfbe03c6832e66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 22 Jul 2020 01:32:02 GMT
ADD file:762e52a5e1d8ff2daa22c3bec2cfdfe4cbcf224deb1e73d7db3af0cbf5658785 in / 
# Wed, 22 Jul 2020 01:32:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:50:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 20:50:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:50:25 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 22 Jul 2020 20:50:47 GMT
ENV TELEGRAF_VERSION=1.13.4
# Wed, 22 Jul 2020 20:50:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Jul 2020 20:50:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Jul 2020 20:50:58 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 22 Jul 2020 20:50:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 20:51:00 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:05dc12a0df610a09562914533797508b791bbd115ae17b6a1b75666ec90263da`  
		Last Modified: Wed, 22 Jul 2020 01:44:04 GMT  
		Size: 42.1 MB (42107480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b998b2d4ee2005b0f51e94b6fc7467091e54a910491e7873b9e0d6f59aabd98`  
		Last Modified: Wed, 22 Jul 2020 06:06:37 GMT  
		Size: 9.4 MB (9444083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15230f55c10a543d54564a792784b1d2e133d4edeadd58978682d9bf02d1425a`  
		Last Modified: Wed, 22 Jul 2020 06:06:34 GMT  
		Size: 3.9 MB (3918506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8ed6da9c9a9b6a83c45713f25bc874233a2ed8a57ffdd0fcdfd8fc3b70c41`  
		Last Modified: Wed, 22 Jul 2020 20:51:39 GMT  
		Size: 14.8 MB (14838306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d146b77fdedc3c75ccf0db81330d0afb9d3a27da887066550bfba1f169358f`  
		Last Modified: Wed, 22 Jul 2020 20:51:34 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e011113c8eb3432f71b37f3b45b9d71587a8f7bcd0ce2f4d29b11abe98caf0d1`  
		Last Modified: Wed, 22 Jul 2020 20:51:56 GMT  
		Size: 19.1 MB (19053078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996b5866cf403c6caea5ae153451bfbbca735a3a08a8d003e2829803906b3ca5`  
		Last Modified: Wed, 22 Jul 2020 20:51:49 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.13` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:095be161b1df8840c1f19b9c5058e49d424960eb96ee32e46c961217e95b8d08
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91192648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0f8fadd48eaf66168cce9e6c6714ed5c842fbf652a0a1338ab763f87b22da9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 22:28:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 22:28:59 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 22:29:18 GMT
ENV TELEGRAF_VERSION=1.13.4
# Tue, 09 Jun 2020 22:29:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 09 Jun 2020 22:29:25 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 09 Jun 2020 22:29:27 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 09 Jun 2020 22:29:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 22:29:32 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a373e9cf9ef79f55bd10fc3f195dc6b5087ab63fbff958f993f128f050a1d5`  
		Last Modified: Tue, 09 Jun 2020 22:30:07 GMT  
		Size: 15.5 MB (15529632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838987d1084e45c5cfc56c78edf137c89d5460b702b72d1cccdbdb5d6cf1424`  
		Last Modified: Tue, 09 Jun 2020 22:30:02 GMT  
		Size: 2.8 KB (2807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d269a5f98de4a6d295730377457d3b8f4f4264e05ba830c70df1f5740ea250a`  
		Last Modified: Tue, 09 Jun 2020 22:30:22 GMT  
		Size: 18.7 MB (18705361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a022f171f9f17f38caef4287ebaca3a0e0387ff5577d66ac732af4f2349f7765`  
		Last Modified: Tue, 09 Jun 2020 22:30:15 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.13.4`

```console
$ docker pull telegraf@sha256:af0ebd18bcefdf61ffd18818ace9833b768702aa95c8d044fb8998a375adc4bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.13.4` - linux; amd64

```console
$ docker pull telegraf@sha256:153cc69d000d5dfe7c7289d5cf4e1afc747bd0acc3455add8352a05990950280
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96743847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:964e3109d3780d9341e57ad616ad0da82d4a2d86b7e259760822c2bb2609a25e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:47:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 02:47:07 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Jun 2020 02:47:20 GMT
ENV TELEGRAF_VERSION=1.13.4
# Wed, 10 Jun 2020 02:47:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 10 Jun 2020 02:47:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 10 Jun 2020 02:47:23 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 10 Jun 2020 02:47:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Jun 2020 02:47:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b69ee1aa5fd2053c60bb7876c57cccda6bb9f6e767638a73cd3a29f9df3016a`  
		Last Modified: Wed, 10 Jun 2020 02:47:58 GMT  
		Size: 16.0 MB (15964407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5666e6b82a727d7af99bf2df78a19e9756471cecc4e7e4d92502b7ed418643`  
		Last Modified: Wed, 10 Jun 2020 02:47:55 GMT  
		Size: 2.8 KB (2772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ee3991d8d9d61efaf09a444e63633d183077f58c955d267e2df91936f08cc7`  
		Last Modified: Wed, 10 Jun 2020 02:48:07 GMT  
		Size: 20.3 MB (20311776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d97d8975b5d5b4032df55d3b2165a9c5364600f5483e4c0ee5f12e1d243fb1`  
		Last Modified: Wed, 10 Jun 2020 02:48:03 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.13.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:9d395b855ac92448cdab3c99b4e0d288e08e2b693c755ecb41d4628b7082e172
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89364441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ffe3fcad0972f1f525e37908f79e117ade897520b3a49f95fbfbe03c6832e66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 22 Jul 2020 01:32:02 GMT
ADD file:762e52a5e1d8ff2daa22c3bec2cfdfe4cbcf224deb1e73d7db3af0cbf5658785 in / 
# Wed, 22 Jul 2020 01:32:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:50:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 20:50:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:50:25 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 22 Jul 2020 20:50:47 GMT
ENV TELEGRAF_VERSION=1.13.4
# Wed, 22 Jul 2020 20:50:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Jul 2020 20:50:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Jul 2020 20:50:58 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 22 Jul 2020 20:50:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 20:51:00 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:05dc12a0df610a09562914533797508b791bbd115ae17b6a1b75666ec90263da`  
		Last Modified: Wed, 22 Jul 2020 01:44:04 GMT  
		Size: 42.1 MB (42107480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b998b2d4ee2005b0f51e94b6fc7467091e54a910491e7873b9e0d6f59aabd98`  
		Last Modified: Wed, 22 Jul 2020 06:06:37 GMT  
		Size: 9.4 MB (9444083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15230f55c10a543d54564a792784b1d2e133d4edeadd58978682d9bf02d1425a`  
		Last Modified: Wed, 22 Jul 2020 06:06:34 GMT  
		Size: 3.9 MB (3918506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8ed6da9c9a9b6a83c45713f25bc874233a2ed8a57ffdd0fcdfd8fc3b70c41`  
		Last Modified: Wed, 22 Jul 2020 20:51:39 GMT  
		Size: 14.8 MB (14838306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d146b77fdedc3c75ccf0db81330d0afb9d3a27da887066550bfba1f169358f`  
		Last Modified: Wed, 22 Jul 2020 20:51:34 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e011113c8eb3432f71b37f3b45b9d71587a8f7bcd0ce2f4d29b11abe98caf0d1`  
		Last Modified: Wed, 22 Jul 2020 20:51:56 GMT  
		Size: 19.1 MB (19053078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996b5866cf403c6caea5ae153451bfbbca735a3a08a8d003e2829803906b3ca5`  
		Last Modified: Wed, 22 Jul 2020 20:51:49 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.13.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:095be161b1df8840c1f19b9c5058e49d424960eb96ee32e46c961217e95b8d08
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91192648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0f8fadd48eaf66168cce9e6c6714ed5c842fbf652a0a1338ab763f87b22da9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 22:28:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 22:28:59 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Jun 2020 22:29:18 GMT
ENV TELEGRAF_VERSION=1.13.4
# Tue, 09 Jun 2020 22:29:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 09 Jun 2020 22:29:25 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 09 Jun 2020 22:29:27 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 09 Jun 2020 22:29:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 22:29:32 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a373e9cf9ef79f55bd10fc3f195dc6b5087ab63fbff958f993f128f050a1d5`  
		Last Modified: Tue, 09 Jun 2020 22:30:07 GMT  
		Size: 15.5 MB (15529632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838987d1084e45c5cfc56c78edf137c89d5460b702b72d1cccdbdb5d6cf1424`  
		Last Modified: Tue, 09 Jun 2020 22:30:02 GMT  
		Size: 2.8 KB (2807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d269a5f98de4a6d295730377457d3b8f4f4264e05ba830c70df1f5740ea250a`  
		Last Modified: Tue, 09 Jun 2020 22:30:22 GMT  
		Size: 18.7 MB (18705361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a022f171f9f17f38caef4287ebaca3a0e0387ff5577d66ac732af4f2349f7765`  
		Last Modified: Tue, 09 Jun 2020 22:30:15 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.13.4-alpine`

```console
$ docker pull telegraf@sha256:69b94db3382157ac83f038c214ed6ff6e45d66d98674729a77bdf61aae3ed24c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.13.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:b63949253dc27196cc56d2c4b37725ee788f75e275ade9d313843c57aa77a628
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26785588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48c9cb07cabc64d9937b921e995328bea356ab7f7c78ad2604199b5809a29d07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 24 Apr 2020 14:24:18 GMT
ENV TELEGRAF_VERSION=1.13.4
# Fri, 24 Apr 2020 14:24:22 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:24:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 24 Apr 2020 14:24:22 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 24 Apr 2020 14:24:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:24:23 GMT
CMD ["telegraf"]
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
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf519af12b10fd075a5f8db5b1c74f3c911ecd7bb59aa1ffddfbb11da4573d7`  
		Last Modified: Fri, 24 Apr 2020 14:25:00 GMT  
		Size: 20.3 MB (20291543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd64901ca1cf1ed9041856bd9403f3a0a4e3d6f5ece8d5d96a79dd24bf7fc18`  
		Last Modified: Fri, 24 Apr 2020 14:24:56 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.13-alpine`

```console
$ docker pull telegraf@sha256:69b94db3382157ac83f038c214ed6ff6e45d66d98674729a77bdf61aae3ed24c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.13-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:b63949253dc27196cc56d2c4b37725ee788f75e275ade9d313843c57aa77a628
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26785588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48c9cb07cabc64d9937b921e995328bea356ab7f7c78ad2604199b5809a29d07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 24 Apr 2020 14:24:18 GMT
ENV TELEGRAF_VERSION=1.13.4
# Fri, 24 Apr 2020 14:24:22 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:24:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 24 Apr 2020 14:24:22 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 24 Apr 2020 14:24:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:24:23 GMT
CMD ["telegraf"]
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
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf519af12b10fd075a5f8db5b1c74f3c911ecd7bb59aa1ffddfbb11da4573d7`  
		Last Modified: Fri, 24 Apr 2020 14:25:00 GMT  
		Size: 20.3 MB (20291543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd64901ca1cf1ed9041856bd9403f3a0a4e3d6f5ece8d5d96a79dd24bf7fc18`  
		Last Modified: Fri, 24 Apr 2020 14:24:56 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.14`

```console
$ docker pull telegraf@sha256:15011deb692f672b03123f41d5324082510deb838d61d6359ba34a50cb943f04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.14` - linux; amd64

```console
$ docker pull telegraf@sha256:ca0b45710ba1a2717dd10f29e09df054e295b1a84a3759178e5505532da13ae9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97849438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e17c44e0083a3daa08f894d665fb4988a556ee2138f1e57f16352b38933216a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:47:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 02:47:07 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Jun 2020 22:40:17 GMT
ENV TELEGRAF_VERSION=1.14.5
# Tue, 30 Jun 2020 22:40:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 30 Jun 2020 22:40:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 30 Jun 2020 22:40:23 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 30 Jun 2020 22:40:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Jun 2020 22:40:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b69ee1aa5fd2053c60bb7876c57cccda6bb9f6e767638a73cd3a29f9df3016a`  
		Last Modified: Wed, 10 Jun 2020 02:47:58 GMT  
		Size: 16.0 MB (15964407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5666e6b82a727d7af99bf2df78a19e9756471cecc4e7e4d92502b7ed418643`  
		Last Modified: Wed, 10 Jun 2020 02:47:55 GMT  
		Size: 2.8 KB (2772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adb1d49497466a9ac1700ef10289b4fac71bf94829ea9fff645b77254a11599`  
		Last Modified: Tue, 30 Jun 2020 22:40:50 GMT  
		Size: 21.4 MB (21417367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65c41811d1257a895a07ce66ff0c7453125a6d3927d16f03b323bb3ead7c6c5`  
		Last Modified: Tue, 30 Jun 2020 22:40:45 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.14` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:95c9fa3f85a8874303bb11da10b6192e9e6d81d2d149083ab0cadb8f35ad4705
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.4 MB (90441629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4e98e7d280480217ace773fb2a885ad0421b3e2f1da44d8ce96962da3c201f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 22 Jul 2020 01:32:02 GMT
ADD file:762e52a5e1d8ff2daa22c3bec2cfdfe4cbcf224deb1e73d7db3af0cbf5658785 in / 
# Wed, 22 Jul 2020 01:32:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:50:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 20:50:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:50:25 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 22 Jul 2020 20:51:08 GMT
ENV TELEGRAF_VERSION=1.14.5
# Wed, 22 Jul 2020 20:51:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Jul 2020 20:51:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Jul 2020 20:51:18 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 22 Jul 2020 20:51:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 20:51:21 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:05dc12a0df610a09562914533797508b791bbd115ae17b6a1b75666ec90263da`  
		Last Modified: Wed, 22 Jul 2020 01:44:04 GMT  
		Size: 42.1 MB (42107480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b998b2d4ee2005b0f51e94b6fc7467091e54a910491e7873b9e0d6f59aabd98`  
		Last Modified: Wed, 22 Jul 2020 06:06:37 GMT  
		Size: 9.4 MB (9444083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15230f55c10a543d54564a792784b1d2e133d4edeadd58978682d9bf02d1425a`  
		Last Modified: Wed, 22 Jul 2020 06:06:34 GMT  
		Size: 3.9 MB (3918506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8ed6da9c9a9b6a83c45713f25bc874233a2ed8a57ffdd0fcdfd8fc3b70c41`  
		Last Modified: Wed, 22 Jul 2020 20:51:39 GMT  
		Size: 14.8 MB (14838306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d146b77fdedc3c75ccf0db81330d0afb9d3a27da887066550bfba1f169358f`  
		Last Modified: Wed, 22 Jul 2020 20:51:34 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06269392053c963d7de9bfc92e721fbe21b0cb6eb12abf438f2ecd1611e9243e`  
		Last Modified: Wed, 22 Jul 2020 20:52:11 GMT  
		Size: 20.1 MB (20130267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240d798fa970c843b5c02d460d39b77ef0309a0d16d115f03362e6ce48312bc9`  
		Last Modified: Wed, 22 Jul 2020 20:52:03 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.14` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3946fc04c28cb082335a63387dbb568d9f5e4865400725a93372c84881f2c455
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92208967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d0f738ec1cee6f867e9a7fbfc8c588e0410c53ab3c70fdb4d66da9289d41b77`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 22:28:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 22:28:59 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Jun 2020 23:36:00 GMT
ENV TELEGRAF_VERSION=1.14.5
# Tue, 30 Jun 2020 23:36:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 30 Jun 2020 23:36:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 30 Jun 2020 23:36:10 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 30 Jun 2020 23:36:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Jun 2020 23:36:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a373e9cf9ef79f55bd10fc3f195dc6b5087ab63fbff958f993f128f050a1d5`  
		Last Modified: Tue, 09 Jun 2020 22:30:07 GMT  
		Size: 15.5 MB (15529632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838987d1084e45c5cfc56c78edf137c89d5460b702b72d1cccdbdb5d6cf1424`  
		Last Modified: Tue, 09 Jun 2020 22:30:02 GMT  
		Size: 2.8 KB (2807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3693eac47b7554033c1fc1e19695f322160ead83fbea70b0c65de7719350d035`  
		Last Modified: Tue, 30 Jun 2020 23:36:29 GMT  
		Size: 19.7 MB (19721680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609d9a680458710b9b57c0cf686d9f0a5b374020b56ab3ea7afcae15989adcec`  
		Last Modified: Tue, 30 Jun 2020 23:36:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.14.5`

```console
$ docker pull telegraf@sha256:15011deb692f672b03123f41d5324082510deb838d61d6359ba34a50cb943f04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.14.5` - linux; amd64

```console
$ docker pull telegraf@sha256:ca0b45710ba1a2717dd10f29e09df054e295b1a84a3759178e5505532da13ae9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97849438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e17c44e0083a3daa08f894d665fb4988a556ee2138f1e57f16352b38933216a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:47:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 02:47:07 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Jun 2020 22:40:17 GMT
ENV TELEGRAF_VERSION=1.14.5
# Tue, 30 Jun 2020 22:40:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 30 Jun 2020 22:40:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 30 Jun 2020 22:40:23 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 30 Jun 2020 22:40:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Jun 2020 22:40:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b69ee1aa5fd2053c60bb7876c57cccda6bb9f6e767638a73cd3a29f9df3016a`  
		Last Modified: Wed, 10 Jun 2020 02:47:58 GMT  
		Size: 16.0 MB (15964407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5666e6b82a727d7af99bf2df78a19e9756471cecc4e7e4d92502b7ed418643`  
		Last Modified: Wed, 10 Jun 2020 02:47:55 GMT  
		Size: 2.8 KB (2772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adb1d49497466a9ac1700ef10289b4fac71bf94829ea9fff645b77254a11599`  
		Last Modified: Tue, 30 Jun 2020 22:40:50 GMT  
		Size: 21.4 MB (21417367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65c41811d1257a895a07ce66ff0c7453125a6d3927d16f03b323bb3ead7c6c5`  
		Last Modified: Tue, 30 Jun 2020 22:40:45 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.14.5` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:95c9fa3f85a8874303bb11da10b6192e9e6d81d2d149083ab0cadb8f35ad4705
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.4 MB (90441629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4e98e7d280480217ace773fb2a885ad0421b3e2f1da44d8ce96962da3c201f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 22 Jul 2020 01:32:02 GMT
ADD file:762e52a5e1d8ff2daa22c3bec2cfdfe4cbcf224deb1e73d7db3af0cbf5658785 in / 
# Wed, 22 Jul 2020 01:32:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:50:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 20:50:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:50:25 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 22 Jul 2020 20:51:08 GMT
ENV TELEGRAF_VERSION=1.14.5
# Wed, 22 Jul 2020 20:51:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Jul 2020 20:51:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Jul 2020 20:51:18 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 22 Jul 2020 20:51:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 20:51:21 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:05dc12a0df610a09562914533797508b791bbd115ae17b6a1b75666ec90263da`  
		Last Modified: Wed, 22 Jul 2020 01:44:04 GMT  
		Size: 42.1 MB (42107480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b998b2d4ee2005b0f51e94b6fc7467091e54a910491e7873b9e0d6f59aabd98`  
		Last Modified: Wed, 22 Jul 2020 06:06:37 GMT  
		Size: 9.4 MB (9444083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15230f55c10a543d54564a792784b1d2e133d4edeadd58978682d9bf02d1425a`  
		Last Modified: Wed, 22 Jul 2020 06:06:34 GMT  
		Size: 3.9 MB (3918506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8ed6da9c9a9b6a83c45713f25bc874233a2ed8a57ffdd0fcdfd8fc3b70c41`  
		Last Modified: Wed, 22 Jul 2020 20:51:39 GMT  
		Size: 14.8 MB (14838306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d146b77fdedc3c75ccf0db81330d0afb9d3a27da887066550bfba1f169358f`  
		Last Modified: Wed, 22 Jul 2020 20:51:34 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06269392053c963d7de9bfc92e721fbe21b0cb6eb12abf438f2ecd1611e9243e`  
		Last Modified: Wed, 22 Jul 2020 20:52:11 GMT  
		Size: 20.1 MB (20130267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240d798fa970c843b5c02d460d39b77ef0309a0d16d115f03362e6ce48312bc9`  
		Last Modified: Wed, 22 Jul 2020 20:52:03 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.14.5` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3946fc04c28cb082335a63387dbb568d9f5e4865400725a93372c84881f2c455
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92208967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d0f738ec1cee6f867e9a7fbfc8c588e0410c53ab3c70fdb4d66da9289d41b77`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 22:28:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 22:28:59 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Jun 2020 23:36:00 GMT
ENV TELEGRAF_VERSION=1.14.5
# Tue, 30 Jun 2020 23:36:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 30 Jun 2020 23:36:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 30 Jun 2020 23:36:10 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 30 Jun 2020 23:36:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Jun 2020 23:36:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a373e9cf9ef79f55bd10fc3f195dc6b5087ab63fbff958f993f128f050a1d5`  
		Last Modified: Tue, 09 Jun 2020 22:30:07 GMT  
		Size: 15.5 MB (15529632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838987d1084e45c5cfc56c78edf137c89d5460b702b72d1cccdbdb5d6cf1424`  
		Last Modified: Tue, 09 Jun 2020 22:30:02 GMT  
		Size: 2.8 KB (2807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3693eac47b7554033c1fc1e19695f322160ead83fbea70b0c65de7719350d035`  
		Last Modified: Tue, 30 Jun 2020 23:36:29 GMT  
		Size: 19.7 MB (19721680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609d9a680458710b9b57c0cf686d9f0a5b374020b56ab3ea7afcae15989adcec`  
		Last Modified: Tue, 30 Jun 2020 23:36:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.14.5-alpine`

```console
$ docker pull telegraf@sha256:bdf5a80d7d08557dcdde2c2197404e7a9b55c3e27f553d23b031eac5aa01bf47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.14.5-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:db058965ced42292a23ce44124fc35a2ebb61ea9a238f2e56d16f332700c2a39
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27908230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4b57af3f33e8451291c131d9558a37f1ba043ba1da553a16fa198a998df07e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Tue, 30 Jun 2020 22:40:28 GMT
ENV TELEGRAF_VERSION=1.14.5
# Tue, 30 Jun 2020 22:40:32 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 30 Jun 2020 22:40:32 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 30 Jun 2020 22:40:33 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Tue, 30 Jun 2020 22:40:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Jun 2020 22:40:33 GMT
CMD ["telegraf"]
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
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f33ffac2604796a23fa50e501180e138cbf5f558871bd42b829f16c712ac6`  
		Last Modified: Tue, 30 Jun 2020 22:41:00 GMT  
		Size: 21.4 MB (21414185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96eb74783ee1172ca3384f4e179d3e3da908c693df321b1f53b1a9f544af02b2`  
		Last Modified: Tue, 30 Jun 2020 22:40:56 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.14-alpine`

```console
$ docker pull telegraf@sha256:bdf5a80d7d08557dcdde2c2197404e7a9b55c3e27f553d23b031eac5aa01bf47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.14-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:db058965ced42292a23ce44124fc35a2ebb61ea9a238f2e56d16f332700c2a39
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27908230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4b57af3f33e8451291c131d9558a37f1ba043ba1da553a16fa198a998df07e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Tue, 30 Jun 2020 22:40:28 GMT
ENV TELEGRAF_VERSION=1.14.5
# Tue, 30 Jun 2020 22:40:32 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 30 Jun 2020 22:40:32 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 30 Jun 2020 22:40:33 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Tue, 30 Jun 2020 22:40:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Jun 2020 22:40:33 GMT
CMD ["telegraf"]
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
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f33ffac2604796a23fa50e501180e138cbf5f558871bd42b829f16c712ac6`  
		Last Modified: Tue, 30 Jun 2020 22:41:00 GMT  
		Size: 21.4 MB (21414185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96eb74783ee1172ca3384f4e179d3e3da908c693df321b1f53b1a9f544af02b2`  
		Last Modified: Tue, 30 Jun 2020 22:40:56 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:bdf5a80d7d08557dcdde2c2197404e7a9b55c3e27f553d23b031eac5aa01bf47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:db058965ced42292a23ce44124fc35a2ebb61ea9a238f2e56d16f332700c2a39
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27908230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4b57af3f33e8451291c131d9558a37f1ba043ba1da553a16fa198a998df07e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Tue, 30 Jun 2020 22:40:28 GMT
ENV TELEGRAF_VERSION=1.14.5
# Tue, 30 Jun 2020 22:40:32 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Tue, 30 Jun 2020 22:40:32 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 30 Jun 2020 22:40:33 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Tue, 30 Jun 2020 22:40:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Jun 2020 22:40:33 GMT
CMD ["telegraf"]
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
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f33ffac2604796a23fa50e501180e138cbf5f558871bd42b829f16c712ac6`  
		Last Modified: Tue, 30 Jun 2020 22:41:00 GMT  
		Size: 21.4 MB (21414185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96eb74783ee1172ca3384f4e179d3e3da908c693df321b1f53b1a9f544af02b2`  
		Last Modified: Tue, 30 Jun 2020 22:40:56 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:15011deb692f672b03123f41d5324082510deb838d61d6359ba34a50cb943f04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:ca0b45710ba1a2717dd10f29e09df054e295b1a84a3759178e5505532da13ae9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97849438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e17c44e0083a3daa08f894d665fb4988a556ee2138f1e57f16352b38933216a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Jun 2020 02:47:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 10 Jun 2020 02:47:07 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Jun 2020 22:40:17 GMT
ENV TELEGRAF_VERSION=1.14.5
# Tue, 30 Jun 2020 22:40:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 30 Jun 2020 22:40:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 30 Jun 2020 22:40:23 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 30 Jun 2020 22:40:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Jun 2020 22:40:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b69ee1aa5fd2053c60bb7876c57cccda6bb9f6e767638a73cd3a29f9df3016a`  
		Last Modified: Wed, 10 Jun 2020 02:47:58 GMT  
		Size: 16.0 MB (15964407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5666e6b82a727d7af99bf2df78a19e9756471cecc4e7e4d92502b7ed418643`  
		Last Modified: Wed, 10 Jun 2020 02:47:55 GMT  
		Size: 2.8 KB (2772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adb1d49497466a9ac1700ef10289b4fac71bf94829ea9fff645b77254a11599`  
		Last Modified: Tue, 30 Jun 2020 22:40:50 GMT  
		Size: 21.4 MB (21417367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65c41811d1257a895a07ce66ff0c7453125a6d3927d16f03b323bb3ead7c6c5`  
		Last Modified: Tue, 30 Jun 2020 22:40:45 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:95c9fa3f85a8874303bb11da10b6192e9e6d81d2d149083ab0cadb8f35ad4705
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.4 MB (90441629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4e98e7d280480217ace773fb2a885ad0421b3e2f1da44d8ce96962da3c201f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 22 Jul 2020 01:32:02 GMT
ADD file:762e52a5e1d8ff2daa22c3bec2cfdfe4cbcf224deb1e73d7db3af0cbf5658785 in / 
# Wed, 22 Jul 2020 01:32:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:50:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 20:50:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:50:25 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 22 Jul 2020 20:51:08 GMT
ENV TELEGRAF_VERSION=1.14.5
# Wed, 22 Jul 2020 20:51:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Jul 2020 20:51:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Jul 2020 20:51:18 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 22 Jul 2020 20:51:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 20:51:21 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:05dc12a0df610a09562914533797508b791bbd115ae17b6a1b75666ec90263da`  
		Last Modified: Wed, 22 Jul 2020 01:44:04 GMT  
		Size: 42.1 MB (42107480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b998b2d4ee2005b0f51e94b6fc7467091e54a910491e7873b9e0d6f59aabd98`  
		Last Modified: Wed, 22 Jul 2020 06:06:37 GMT  
		Size: 9.4 MB (9444083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15230f55c10a543d54564a792784b1d2e133d4edeadd58978682d9bf02d1425a`  
		Last Modified: Wed, 22 Jul 2020 06:06:34 GMT  
		Size: 3.9 MB (3918506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8ed6da9c9a9b6a83c45713f25bc874233a2ed8a57ffdd0fcdfd8fc3b70c41`  
		Last Modified: Wed, 22 Jul 2020 20:51:39 GMT  
		Size: 14.8 MB (14838306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d146b77fdedc3c75ccf0db81330d0afb9d3a27da887066550bfba1f169358f`  
		Last Modified: Wed, 22 Jul 2020 20:51:34 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06269392053c963d7de9bfc92e721fbe21b0cb6eb12abf438f2ecd1611e9243e`  
		Last Modified: Wed, 22 Jul 2020 20:52:11 GMT  
		Size: 20.1 MB (20130267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240d798fa970c843b5c02d460d39b77ef0309a0d16d115f03362e6ce48312bc9`  
		Last Modified: Wed, 22 Jul 2020 20:52:03 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3946fc04c28cb082335a63387dbb568d9f5e4865400725a93372c84881f2c455
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92208967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d0f738ec1cee6f867e9a7fbfc8c588e0410c53ab3c70fdb4d66da9289d41b77`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 22:28:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 22:28:59 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 30 Jun 2020 23:36:00 GMT
ENV TELEGRAF_VERSION=1.14.5
# Tue, 30 Jun 2020 23:36:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 30 Jun 2020 23:36:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 30 Jun 2020 23:36:10 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 30 Jun 2020 23:36:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Jun 2020 23:36:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a373e9cf9ef79f55bd10fc3f195dc6b5087ab63fbff958f993f128f050a1d5`  
		Last Modified: Tue, 09 Jun 2020 22:30:07 GMT  
		Size: 15.5 MB (15529632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838987d1084e45c5cfc56c78edf137c89d5460b702b72d1cccdbdb5d6cf1424`  
		Last Modified: Tue, 09 Jun 2020 22:30:02 GMT  
		Size: 2.8 KB (2807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3693eac47b7554033c1fc1e19695f322160ead83fbea70b0c65de7719350d035`  
		Last Modified: Tue, 30 Jun 2020 23:36:29 GMT  
		Size: 19.7 MB (19721680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609d9a680458710b9b57c0cf686d9f0a5b374020b56ab3ea7afcae15989adcec`  
		Last Modified: Tue, 30 Jun 2020 23:36:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
