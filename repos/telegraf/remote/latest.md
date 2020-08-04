## `telegraf:latest`

```console
$ docker pull telegraf@sha256:d235b1bdbaba90c9c42748527dc7c91969d23223c452aa64b235a91b3d659492
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:85020ace531bcb4ec4892e972f9e0349c502cc4c76081b1f8cd5bc4db47c1f16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107267784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8615e48698154c5b16a3d15fde9e6ea4f47833e9850ba6e0ba02467df4117847`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:16 GMT
ADD file:89dfd7d3ed77fd5e05f20a0ab631142207ae462f5bbd877f8745d3930c751d87 in / 
# Wed, 22 Jul 2020 02:03:16 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 03:00:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 03:00:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jul 2020 05:21:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 05:21:58 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Jul 2020 05:21:58 GMT
ENV TELEGRAF_VERSION=1.15.1
# Thu, 23 Jul 2020 05:22:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Jul 2020 05:22:02 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Jul 2020 05:22:03 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Jul 2020 05:22:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jul 2020 05:22:03 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31dd5ebca5efc5e96a425402fa85e492b02c8fe757dfd3edfdea2a7c67322909`  
		Last Modified: Wed, 22 Jul 2020 02:09:37 GMT  
		Size: 50.4 MB (50390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed641c4ae9821ca3c399071ea82ae667237acbcaad1e367c3e1e87fc967834c`  
		Last Modified: Wed, 22 Jul 2020 03:16:28 GMT  
		Size: 7.8 MB (7811702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd57146431eae70720cf24877e818256ae1a30b9c1c9e7d0ad093c945ca0af2`  
		Last Modified: Wed, 22 Jul 2020 03:16:28 GMT  
		Size: 10.0 MB (9996319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35a3bf5005f2ba43705c5cdad5759f5548bb8f51f54681215828ae4c610e37c`  
		Last Modified: Thu, 23 Jul 2020 05:23:02 GMT  
		Size: 17.4 MB (17407722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0cbfd5a95f5a442fe3af04c1ef56b23a875ba2c6a46e01cb21eff8ba5c930a`  
		Last Modified: Thu, 23 Jul 2020 05:22:58 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad3d77312c2d9cfe9bdb4a5423284b93e29003228eb9dc575336e935963f785`  
		Last Modified: Thu, 23 Jul 2020 05:23:04 GMT  
		Size: 21.7 MB (21658710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7f48a85e66fa3102ad9b1deaa27ac6e9c94083a84b9aefc76e98424f7e3995`  
		Last Modified: Thu, 23 Jul 2020 05:22:58 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:8964d5c1ecf0efb5c8d5e3cc649310042d92a9ca50988c94193c0114dc6985e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98877270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76b880897b8099c01be02bcf328ff33e0156c13f75ab8d14ca14560428e616e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 22 Jul 2020 01:18:19 GMT
ADD file:38965defa0df84392a8ff562c2fa6393fe8d42f65f85591c07a581d694eebc30 in / 
# Wed, 22 Jul 2020 01:18:24 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:27:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:27:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jul 2020 08:21:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 08:21:16 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 04 Aug 2020 04:51:26 GMT
ENV TELEGRAF_VERSION=1.15.2
# Tue, 04 Aug 2020 04:52:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Aug 2020 04:52:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Aug 2020 04:52:43 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 04 Aug 2020 04:52:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 04:52:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:f890282b0ef00faf11d62374bcdfc54ca574d085127c66977d9a08ab80978a98`  
		Last Modified: Wed, 22 Jul 2020 01:40:13 GMT  
		Size: 45.9 MB (45868714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fda9a2c24b0e12476aa415979e2be070c1cb51f060e0af97ed46ee44de7a3be`  
		Last Modified: Wed, 22 Jul 2020 06:01:56 GMT  
		Size: 7.1 MB (7097816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792d650db03400aa008d695ec7474d63c2c2d0463789209a45254c5499c8e301`  
		Last Modified: Wed, 22 Jul 2020 06:01:54 GMT  
		Size: 9.3 MB (9343320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef85cb8be5c6eab5adac2aa4bf837bd540e68151717ff15245d4d7e28783a2d`  
		Last Modified: Thu, 23 Jul 2020 08:22:02 GMT  
		Size: 16.2 MB (16161298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557343f785fe61732ac9de21e1d1ccfa6847719755fab731fb0ac979ba193240`  
		Last Modified: Thu, 23 Jul 2020 08:21:55 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de00718f543c5237649033ed7a7f8a53975a61ec688ca2a356265bcc6d5e036d`  
		Last Modified: Tue, 04 Aug 2020 04:53:34 GMT  
		Size: 20.4 MB (20403082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0370a4f0d6e7dd4ab384848b39323a20682737f62980ca9e0aff4826f6b9c630`  
		Last Modified: Tue, 04 Aug 2020 04:53:29 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ecfa0fdd53c3e63b781d5a2a0c0a7d1333d397f30c2c9cf4e9dcdb7bfa732d37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104123322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa5587b3b4ebfafe0660ed7f899dbc149f2668949f39bf48ba5e6871fc4eb69`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 22 Jul 2020 00:40:37 GMT
ADD file:14b8dca0bc0e6dae2f0bdb018a3a4e6d8d041abd03d118ae27cf7a72668f4970 in / 
# Wed, 22 Jul 2020 00:40:41 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:16:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 01:17:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jul 2020 05:32:05 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 05:32:08 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 04 Aug 2020 06:50:59 GMT
ENV TELEGRAF_VERSION=1.15.2
# Tue, 04 Aug 2020 06:51:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Aug 2020 06:51:28 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Aug 2020 06:51:30 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 04 Aug 2020 06:51:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 06:51:33 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:e2b2cb832ad58353bcc4edbdd16023beb64ec7856b469d202975f8de836c6906`  
		Last Modified: Wed, 22 Jul 2020 00:47:20 GMT  
		Size: 49.2 MB (49168473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d6493ea016bd1aa68fa88d01d53cd305f67bae5fa500592c76c466808bf221`  
		Last Modified: Wed, 22 Jul 2020 01:35:25 GMT  
		Size: 7.7 MB (7681419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33779eed82f6ae65801a87fd1278e902bbab0f609f0c6a0232d8ef0b37112127`  
		Last Modified: Wed, 22 Jul 2020 01:35:25 GMT  
		Size: 10.0 MB (9983891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb0004e285ff938a41c29e6da2d82c2b52254d4f5c46779a8b11c601f46594b`  
		Last Modified: Thu, 23 Jul 2020 05:32:46 GMT  
		Size: 17.3 MB (17268053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba546e131bbdc82be633120c68d90294110daef59587fb00a005b68d39078d03`  
		Last Modified: Thu, 23 Jul 2020 05:32:41 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ec47ac5f02e999796f7cefe918a6cec35f5f044efbcd6ab50c72eb14d64e36`  
		Last Modified: Tue, 04 Aug 2020 06:51:57 GMT  
		Size: 20.0 MB (20018451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d155c9630ca385cc1e60762dc20d50d48e795671abf5d83f242dd0bbacfdcfb3`  
		Last Modified: Tue, 04 Aug 2020 06:51:50 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
