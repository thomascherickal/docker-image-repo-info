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
