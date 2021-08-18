## `telegraf:latest`

```console
$ docker pull telegraf@sha256:266487732596eb1df84950eac64b92193f0a625d7eb49ccef536e9c86785719e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:64c3815ff8f322d42c23ab79ec202666c138f997d97dc1dd8fce08f909c17d74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119756205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce7ed2cfbcd391a1ca51fad18d7af4e2575895a88c6c1ca15131537fb8173e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:20:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 09:25:15 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 09:25:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 09:25:50 GMT
ENV TELEGRAF_VERSION=1.19.2
# Wed, 18 Aug 2021 09:25:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 09:25:56 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 18 Aug 2021 09:25:56 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 18 Aug 2021 09:25:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 09:25:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4099a935a96edef1e9378de34e314d07fb3aea1b7205774055a1fa44a3819f4`  
		Last Modified: Tue, 17 Aug 2021 09:30:37 GMT  
		Size: 7.8 MB (7833079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e2960d83651b1494b4da6c97686e79cc760aa90a75948eed56786726f86928`  
		Last Modified: Tue, 17 Aug 2021 09:30:38 GMT  
		Size: 10.0 MB (9997209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5cf88f7c51344a5e065d720bae41c86894f30c85badd7d2572fba22c652727`  
		Last Modified: Wed, 18 Aug 2021 09:26:22 GMT  
		Size: 17.4 MB (17415111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e4ada2757ad6e9ea2c0620ac9edfa023899d82c48c547c9239ebe6a48b6b0a`  
		Last Modified: Wed, 18 Aug 2021 09:26:19 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d197c0f2b16ad3ade89195675008bc337acb41547b2e489f014437fd16da2`  
		Last Modified: Wed, 18 Aug 2021 09:26:59 GMT  
		Size: 34.1 MB (34071515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bcb12e8f8a342ec5313b940dc34fed483e60297de510224c9a8003b5fbb299`  
		Last Modified: Wed, 18 Aug 2021 09:26:53 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:62ff41061b6321337e883b8e4f42d6709a44820e62130291b15dac131b77990c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110131231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59ecacc78142a6cf4d81df0466ac8b3fc4a04d30b3f25fafd37e2cbcd43bee2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:13 GMT
ADD file:c33137dc0d277fe210ea6387a8be105c625fdf777a541a6392896766df9919d4 in / 
# Thu, 22 Jul 2021 02:03:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:14:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 11:03:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:03:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 29 Jul 2021 23:51:17 GMT
ENV TELEGRAF_VERSION=1.19.2
# Thu, 29 Jul 2021 23:51:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 29 Jul 2021 23:51:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 29 Jul 2021 23:51:30 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 29 Jul 2021 23:51:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 29 Jul 2021 23:51:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ff16e408fd8b8191145782047ebc0c76176550d844743a679143d53a164bea21`  
		Last Modified: Thu, 22 Jul 2021 02:15:33 GMT  
		Size: 45.9 MB (45917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701a3a4dc54422c371762f5416afea6835e02e9db10fd686f73159ec84ec2f7`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 7.1 MB (7124233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8651c1854c791264fe60acc8ab39e9b914dc3258a9aa42509f1c35ce32a880d`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 9.3 MB (9343793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2503b0beae04002464d92392e6fec2e284562e61a808159dca26a3b1fd759e35`  
		Last Modified: Fri, 23 Jul 2021 11:05:22 GMT  
		Size: 16.2 MB (16160458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc38ed3cb27fb443f2917c5bdc8189fa8831a0ae153b7c740183fc14c7c43ee`  
		Last Modified: Fri, 23 Jul 2021 11:05:10 GMT  
		Size: 2.9 KB (2892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904212545166c39935a87d5761d96757d92fc88956b16a3d2fe01989ff473799`  
		Last Modified: Thu, 29 Jul 2021 23:52:42 GMT  
		Size: 31.6 MB (31582420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84adccc3c7b8c3c1c6d00a502eed47b0fdc0ab12af045f044c9df3ac0e3f1ae`  
		Last Modified: Thu, 29 Jul 2021 23:52:19 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:164f8965f22c281c4e301661847efcd5d79453e00a16449314e623098721cb4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115031849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3674daa4ad68474b5ec27f5688b784a882b860b4e19c8bc303ea3faef0c8119e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 05:06:02 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 05:06:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 05:06:24 GMT
ENV TELEGRAF_VERSION=1.19.2
# Wed, 18 Aug 2021 05:06:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 05:06:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 18 Aug 2021 05:06:29 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 18 Aug 2021 05:06:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 05:06:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565d34c87c364517d34ad3b0cc55cc5ba5228ed3d524e7349b620cb41ed599a6`  
		Last Modified: Wed, 18 Aug 2021 05:06:56 GMT  
		Size: 17.3 MB (17268562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba78e60bcb30e04825f9773196e1cb82065b234a76f0a78f95741f5ddb78315`  
		Last Modified: Wed, 18 Aug 2021 05:06:53 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c5efe21cd4049fd7b1fc94194543068ecfda406c6c2ab4d2bafd9665867630`  
		Last Modified: Wed, 18 Aug 2021 05:07:32 GMT  
		Size: 30.9 MB (30858291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0788055a9f36567d5d60243c75950f44211329862c0fde806fcd2bccd588690c`  
		Last Modified: Wed, 18 Aug 2021 05:07:26 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
