## `telegraf:latest`

```console
$ docker pull telegraf@sha256:85b0133f0a2bd09be596901315d5ec40263f2188738312e473c1b830957623c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:cc43a1e734b27b8f76992888ef40c1b6770d716af45083494683b0f45bd0c48d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134296629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf0e9f35af354b67ccddf5073e75bf91bcf5d476d9952aa39807ad7b43b745da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:23:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Oct 2022 05:04:28 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:04:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 02 Nov 2022 17:21:29 GMT
ENV TELEGRAF_VERSION=1.24.3
# Wed, 02 Nov 2022 17:21:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 02 Nov 2022 17:21:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 02 Nov 2022 17:21:35 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 02 Nov 2022 17:21:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 02 Nov 2022 17:21:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4a4c6caea8801bb0b7377e10220a914da403bc93fa79663cbf2dcf1800b6f1`  
		Last Modified: Tue, 25 Oct 2022 09:47:36 GMT  
		Size: 5.2 MB (5164775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4edced8587e6c18412817019074f5e04a8ede4e2fc89d06af13df3f80d78a70d`  
		Last Modified: Tue, 25 Oct 2022 09:47:36 GMT  
		Size: 10.9 MB (10877322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351dbe0337c2dc42d06f34ca09fd880237614b4b994e56fc4c685e2bbe24a3e8`  
		Last Modified: Wed, 26 Oct 2022 05:05:19 GMT  
		Size: 18.8 MB (18760466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b698d0487ff3ce144a0979269d7e6cb907a6128452ba4a69346c5dceb9251a0`  
		Last Modified: Wed, 26 Oct 2022 05:05:15 GMT  
		Size: 2.9 KB (2902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08581c18604c1799caf0bc3328cd9083e9de7c523bca67ad9f991a3d18a0e47`  
		Last Modified: Wed, 02 Nov 2022 17:22:19 GMT  
		Size: 44.4 MB (44444490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a870e65bbcdbc3ecd5bb40ec604422000968d303af280eeceb6e1dc4c849e6`  
		Last Modified: Wed, 02 Nov 2022 17:22:11 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:7ecf62dde91252600647b331bffa1d1bd0a1802dc144d25c8b46810edfaefaf1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123884873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4211f09a78d4c9660a08e958bd708ac51aeeea46cafc2fa8c15f977bb725d8ff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:06 GMT
ADD file:94d6b607b174c11c18753fac156b0ca5ecda941da3d456e136b8b14457810d37 in / 
# Tue, 25 Oct 2022 03:14:06 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 04:36:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 04:36:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 Oct 2022 05:37:40 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 27 Oct 2022 05:37:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 27 Oct 2022 05:38:08 GMT
ENV TELEGRAF_VERSION=1.24.2
# Thu, 27 Oct 2022 05:38:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 27 Oct 2022 05:38:15 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 27 Oct 2022 05:38:15 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 27 Oct 2022 05:38:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Oct 2022 05:38:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a9bec1cbb822a75428a679c01f232b1af10cce0bdc1bf6507d26e8d79ad54300`  
		Last Modified: Tue, 25 Oct 2022 03:20:41 GMT  
		Size: 50.2 MB (50209987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9e47cd2446328779ff30de254793eaf539fec260638990e7d8dd3d29342fca`  
		Last Modified: Wed, 26 Oct 2022 05:10:38 GMT  
		Size: 4.9 MB (4932764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8deb44fa055f393de7346c484ab2ff3ef90e7efc4ebb018f932b377361e3b45`  
		Last Modified: Wed, 26 Oct 2022 05:10:38 GMT  
		Size: 10.2 MB (10218474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7d4d8c8252047f1f66a946398cc78695bd771d319cf2a47fc4cd902f3a639a`  
		Last Modified: Thu, 27 Oct 2022 05:38:48 GMT  
		Size: 17.5 MB (17463010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4129073eba9303dca85935840502913bc2a8f0a9bc8edc73bdad70b804dcc8ee`  
		Last Modified: Thu, 27 Oct 2022 05:38:45 GMT  
		Size: 2.9 KB (2869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15ed156705b473c17463eb71576a33b6ca30942809cd6751954746ede741f1e`  
		Last Modified: Thu, 27 Oct 2022 05:39:32 GMT  
		Size: 41.1 MB (41057425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34eb2d5915fb2afc92b4f023b853797d58c766a324c65a27e1d2236b6a8d0d6f`  
		Last Modified: Thu, 27 Oct 2022 05:39:24 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:922f422f6a6b94fc910f5f3624b7f09ef1617d2c0118f3b4d64bf789c2a1b70a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128224856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbee798a356199f5a27224f5b9f844378ef2c035bd50ea3524c861a8ce50280d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:58:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Oct 2022 09:48:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 09:48:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Oct 2022 09:49:14 GMT
ENV TELEGRAF_VERSION=1.24.2
# Wed, 26 Oct 2022 09:49:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 26 Oct 2022 09:49:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 26 Oct 2022 09:49:19 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 26 Oct 2022 09:49:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Oct 2022 09:49:19 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eadbf427bb41b3e329a95935c65b09c6d3b7a9c2fa8e08417e497df02ed996`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 5.2 MB (5151506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9731f4e3bc3680179c10cece663cf0cfe0488918d6795406f4b76f07b787de`  
		Last Modified: Tue, 25 Oct 2022 08:30:22 GMT  
		Size: 10.9 MB (10874174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c72ea8b63e6f16d43f4d9af4c4c9a85eb32f68ef197070617899ae1176d417`  
		Last Modified: Wed, 26 Oct 2022 09:49:35 GMT  
		Size: 18.6 MB (18599385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c29547de93132c9eb465c23c293e46309e2a89380d99f318ef96001ad9bf2f`  
		Last Modified: Wed, 26 Oct 2022 09:49:32 GMT  
		Size: 2.9 KB (2896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ffd99181aec67f1ca5156935e97da41f79483769352f4122af087fae80b358`  
		Last Modified: Wed, 26 Oct 2022 09:50:06 GMT  
		Size: 39.9 MB (39894584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf475a09f2256d104a9f19ca8fe17790ff30122f4fa818c91b8eae29e9752ef7`  
		Last Modified: Wed, 26 Oct 2022 09:50:00 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
