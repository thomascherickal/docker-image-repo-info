## `telegraf:latest`

```console
$ docker pull telegraf@sha256:6790fa19556e4a19408a5adbabccc635fef46979d0fdf529fb0ad35e1c0fe979
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:f626169475804c556ff35e418032b7b79619b4b4f339d59146cd23bbaf2619e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148059998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a20206efc41d51f99c85aef67693dd56e35789aac484d7af1afbef27ffc44f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 07 Sep 2023 00:20:39 GMT
ADD file:8415eb847ca46ed1aa1695965af86f1a0f09e8859a7b3c07b2f719404b665102 in / 
# Thu, 07 Sep 2023 00:20:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:56:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 22:44:17 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 22:44:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 22:44:18 GMT
ENV TELEGRAF_VERSION=1.27.4
# Thu, 07 Sep 2023 22:44:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 07 Sep 2023 22:44:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 07 Sep 2023 22:44:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 07 Sep 2023 22:44:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 22:44:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:012c0b3e998c1a0c0bedcf712eaaafb188580529dd026a04aa1ce13fdb39e42b`  
		Last Modified: Thu, 07 Sep 2023 00:24:59 GMT  
		Size: 49.6 MB (49557216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00046d1e755ea94fa55a700ca9a10597e4fac7c47be19d970a359b0267a51fbf`  
		Last Modified: Thu, 07 Sep 2023 03:04:41 GMT  
		Size: 24.0 MB (24030451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb6a885cf05af87b03dc0760c49315846a46a14e40307838388402c787ac5b`  
		Last Modified: Thu, 07 Sep 2023 22:45:17 GMT  
		Size: 19.1 MB (19143468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef685fa60eef2ecb32de1be898cc22426d5074884e2334991558e776a5be1f2c`  
		Last Modified: Thu, 07 Sep 2023 22:45:14 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9471341e94f43a39a61050ae0453e6f4dbc9930d0b68a22bd946d80c50a35d0d`  
		Last Modified: Thu, 07 Sep 2023 22:45:23 GMT  
		Size: 55.3 MB (55326715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147bddd4e1d39b201cfdc11a9bfc11c01c51b042768339f3f9fd6b11fe26ab9f`  
		Last Modified: Thu, 07 Sep 2023 22:45:14 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:85ccb0d09b7d7648a1c730ce35a6f607916347d65936f4ceae5c6b1d14e006e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136667192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32e9b9dddf311c9a365cffe6c22e08cd33fae7db4f67120bd9a408b3cb2f17e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:31 GMT
ADD file:33a39c01d7e209fab46b54083ee271e3bdd3d4dccc3a6e8635cbe0989c92c53e in / 
# Thu, 07 Sep 2023 00:57:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:33:35 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:33:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 19:33:36 GMT
ENV TELEGRAF_VERSION=1.27.4
# Thu, 07 Sep 2023 19:33:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 07 Sep 2023 19:33:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 07 Sep 2023 19:33:44 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 07 Sep 2023 19:33:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 19:33:45 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4e1ef44b7a1dc38ec98ec01f961a48844fdf07e1ff182d55daae1c01406302a9`  
		Last Modified: Thu, 07 Sep 2023 01:02:04 GMT  
		Size: 45.2 MB (45233200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c71aa39a4f5a50ddeb9942b08a954d6892177b5409397b1e948e88ac7f6575a`  
		Last Modified: Thu, 07 Sep 2023 01:44:56 GMT  
		Size: 21.9 MB (21936900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7478dca3d662e96d838b4be3ec8d69a5207bc88ec0e58fc729e20efc92c6b314`  
		Last Modified: Thu, 07 Sep 2023 19:34:44 GMT  
		Size: 18.0 MB (17989213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf6e8baa84204d932b09bd493be5742abf6ac0c77352d7e55044f79ad2d06d5`  
		Last Modified: Thu, 07 Sep 2023 19:34:39 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f5a8d73f44292228850dd7f7d90554affa09c6ebcd831fdeb38a01bf63c2c7`  
		Last Modified: Thu, 07 Sep 2023 19:34:51 GMT  
		Size: 51.5 MB (51505731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4307f61b87ea98d7e7603a9ff8940c00ad08f6ec3991cc654ba23da82865ed`  
		Last Modified: Thu, 07 Sep 2023 19:34:39 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:5ab22bb85a71606d23150cef3beff84b9d4ce347c8abbb53f497de15f46bb4e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142198860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b643f547eceab158f3542624c60b7cc716e41da222e79181020c4b3fa5a3cd1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:31 GMT
ADD file:f9dd2b1cc0ba261acd8a3e500c54f6b6e0a46131a32988bfd71cf3c6fc5a7d13 in / 
# Thu, 07 Sep 2023 00:39:32 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:51:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:38:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:38:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 19:38:21 GMT
ENV TELEGRAF_VERSION=1.27.4
# Thu, 07 Sep 2023 19:38:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 07 Sep 2023 19:38:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 07 Sep 2023 19:38:28 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 07 Sep 2023 19:38:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 19:38:28 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fa34261389f3dee2ecffe9bfe38ae7fd05a1908e98a7486354905aee0f648a6e`  
		Last Modified: Thu, 07 Sep 2023 00:42:39 GMT  
		Size: 49.6 MB (49590783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993525952a483617183655b735562fd3eee4b3a85a472e3dc3c79a258adca100`  
		Last Modified: Thu, 07 Sep 2023 06:59:20 GMT  
		Size: 23.6 MB (23570086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72451c72e989c3737872403fa80ba26c9c18121690e8fc4bf54784bb55f7618`  
		Last Modified: Thu, 07 Sep 2023 19:39:15 GMT  
		Size: 19.1 MB (19077240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8be5dd722b46de02a012c0f6aae92ffa934c2f8d52fd5485345ab0eed03a2b`  
		Last Modified: Thu, 07 Sep 2023 19:39:13 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a7f9b1e0715f72c067711c0b7457fa91550881a5c58f5f10cbe9f99808777d`  
		Last Modified: Thu, 07 Sep 2023 19:39:18 GMT  
		Size: 50.0 MB (49958593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374fc6167827df8dc077719573d8a7a6c354783cebd145e2963c82f63efcca65`  
		Last Modified: Thu, 07 Sep 2023 19:39:13 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
