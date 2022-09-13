## `telegraf:latest`

```console
$ docker pull telegraf@sha256:939b54479270bcde7684f4e9fe540f952a4a97afc7f6729526dd42648b13e3d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:6579540446d8b48a68ee70a5d00aec0180a394b390f5c274192c125498befe80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131659359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7b77eb6d0523c0d58a999fb389e9023a81544aa60e91cd318e6d8d8d48240d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 20:18:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 20:18:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 20:18:59 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 23 Aug 2022 20:19:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 20:19:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 20:19:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 20:19:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 20:19:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bf78e724b533506c47d613e8c51e7756df404678ac937fb012ecd677818fe8`  
		Last Modified: Tue, 23 Aug 2022 20:19:29 GMT  
		Size: 18.8 MB (18759919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320b93d95aa1cf3f1430c41fd73db6dbce1a9555be411bdc7b8beb2ccd712412`  
		Last Modified: Tue, 23 Aug 2022 20:19:25 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afae3dc366acd2e94f54c7ed688bad5b07e398c1d0b98d1c3397adbc3d1b55c`  
		Last Modified: Tue, 23 Aug 2022 20:20:07 GMT  
		Size: 41.8 MB (41849146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c6f4c95ed83df0120941707276fe29656a520a3f740d6ec95b730fb3232927`  
		Last Modified: Tue, 23 Aug 2022 20:20:00 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:edab75903a420533e2a8e640b3ea09d5fe3136acd032cffab9709525182fda03
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123769808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b366cbcc0a98de891775fed7f4be758083183a6c38dc93e5f74902a9d2414a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 24 Aug 2022 17:14:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 17:14:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 12 Sep 2022 23:03:53 GMT
ENV TELEGRAF_VERSION=1.24.0
# Mon, 12 Sep 2022 23:04:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 12 Sep 2022 23:04:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Sep 2022 23:04:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 12 Sep 2022 23:04:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Sep 2022 23:04:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28127e82dbad78eb691a0fb5e5374c2f1c2c7d4f9826ef923493608b5b98fb3c`  
		Last Modified: Wed, 24 Aug 2022 17:15:12 GMT  
		Size: 17.5 MB (17462272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a8e2427f6ebb3290b16701a3683670b1b092f3fb657747570316664b57f8e0`  
		Last Modified: Wed, 24 Aug 2022 17:15:08 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b76fc4f664cb73e224ff9a62594464ceea48098c16c5d6abc1f25c20e4ea34`  
		Last Modified: Mon, 12 Sep 2022 23:04:52 GMT  
		Size: 41.0 MB (40950649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628bd3dc6e40f60f19069b944a009c1e45f57c2b85a72578d38e95799f0b9e95`  
		Last Modified: Mon, 12 Sep 2022 23:04:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a8ddacdc65a521e49f009f6771d55db2193e00f99ff5cba645e5c71ca0b50578
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125708649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66153c6da3e29fe92c650407126babd7a3446c9379a0f807b70d3693ebcb156d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 21:31:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:32:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 21:32:29 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 23 Aug 2022 21:32:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 21:32:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 21:32:37 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 21:32:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 21:32:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23840b45319a569927bb1e754dbbc4a1cd2644adaf7e32337156a0d803b491`  
		Last Modified: Tue, 23 Aug 2022 21:33:03 GMT  
		Size: 18.4 MB (18382761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8209f5a5eb7e11a25b57321f7e44a027d4c987c6abce3e24edf37b2184eb729`  
		Last Modified: Tue, 23 Aug 2022 21:33:00 GMT  
		Size: 2.9 KB (2858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e18d77d74c012eeac46b242bc3673fc10630818bb08c4fdef95a6ecb2b33767`  
		Last Modified: Tue, 23 Aug 2022 21:33:39 GMT  
		Size: 38.0 MB (38030233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e9a4598baf2ed832676e49bb46f60f62fe677ce35e2a18ce5cb976566e3863`  
		Last Modified: Tue, 23 Aug 2022 21:33:33 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
