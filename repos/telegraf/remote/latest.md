## `telegraf:latest`

```console
$ docker pull telegraf@sha256:54333b1de0fcc60dff902253cd2966f570af856bd6552250a907ec331671f88e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:fea6a5a2de228200998d1c26b3402ac540032701886742fe93de001e11964694
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97901849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c7e1d8146dafeaa12324d2d1cf8bd7a56b02edbd5ff5258b7a3bcb1cc75e619`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 31 Mar 2020 01:23:50 GMT
ADD file:774b5e2033bb42ad97daa64267a5f041124cc0b05ec0198f1b5578ceea5a48e4 in / 
# Tue, 31 Mar 2020 01:23:51 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 02:06:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 02:06:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Apr 2020 01:52:18 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 01:52:22 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 14 Apr 2020 23:20:15 GMT
ENV TELEGRAF_VERSION=1.14.1
# Tue, 14 Apr 2020 23:20:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 14 Apr 2020 23:20:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Apr 2020 23:20:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 14 Apr 2020 23:20:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Apr 2020 23:20:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:56da78ce36e97a8ba1f860575bb1422d1cb6ab4dade70b06ddf1651302dde955`  
		Last Modified: Tue, 31 Mar 2020 01:29:15 GMT  
		Size: 45.4 MB (45375928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfe0f13ac4531fb6d077fda0e94ced4b9ed8a354c54b4efced9b7755d3f39d1`  
		Last Modified: Tue, 31 Mar 2020 02:12:44 GMT  
		Size: 10.8 MB (10797329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6254ff6d0e6052b7bead70e37703002eda28ac40f9a1167ea9bf813bf9c17d7f`  
		Last Modified: Tue, 31 Mar 2020 02:12:43 GMT  
		Size: 4.3 MB (4340113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63dbfcc845ec6d72a1f05fee7ccacfb3d35c82227a0f9b4722adba887bcc265`  
		Last Modified: Wed, 01 Apr 2020 01:53:30 GMT  
		Size: 16.0 MB (15964762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102ba7649ad438ec1c9d3ded01ee6af566205ecccf1c4973f924b6885eca4181`  
		Last Modified: Wed, 01 Apr 2020 01:53:23 GMT  
		Size: 2.8 KB (2772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77391693d159d8e6524fcbb95f07532f537e791ccc4d788d2d864243dc5b7c4b`  
		Last Modified: Tue, 14 Apr 2020 23:20:44 GMT  
		Size: 21.4 MB (21420761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ec9e33c246e6faec7a55a5a8e4488dbc5fe111c6a364512df337c7046424fb`  
		Last Modified: Tue, 14 Apr 2020 23:20:39 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:bd91ead79670fe0ca8e5295ec6d7a56ef27bd9a43306c89815ee1e7306939f7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90489101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aa811877da59a0b5ba189d9fe5637f27495b6f19a370b9863e286ff39c75c13`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 31 Mar 2020 01:52:24 GMT
ADD file:b047b0c4dbfbcc048385195e807283b9386c4aac13a4841112cb3f76cd932b06 in / 
# Tue, 31 Mar 2020 01:52:26 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:53:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:53:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 23:30:58 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 23:31:04 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 14 Apr 2020 23:51:45 GMT
ENV TELEGRAF_VERSION=1.14.1
# Tue, 14 Apr 2020 23:51:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 14 Apr 2020 23:51:53 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Apr 2020 23:51:54 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 14 Apr 2020 23:51:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Apr 2020 23:51:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:eb3768893937e6b455f98cd8db65949a6aa5c54ebd94fca3039af9833187ce10`  
		Last Modified: Tue, 31 Mar 2020 01:59:52 GMT  
		Size: 42.1 MB (42100090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69eb68590923b075c8f49c4470341451f9d874afc84c5fc916278815a1064243`  
		Last Modified: Tue, 31 Mar 2020 04:04:43 GMT  
		Size: 9.5 MB (9498284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743981b4cf60d4ed8ddd6610e4d1d75256ddb63a7d83d540a96e1faf8ba8a315`  
		Last Modified: Tue, 31 Mar 2020 04:04:42 GMT  
		Size: 3.9 MB (3918805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb75ed2b05b42b1ba79f7dfbdd884e4e69a449d955524c9fe20a4197f9624719`  
		Last Modified: Tue, 31 Mar 2020 23:32:09 GMT  
		Size: 14.8 MB (14839149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9583861939392eaca0886e7ab00fda5ef8f622ad05bd48712b55c623bac5fbf7`  
		Last Modified: Tue, 31 Mar 2020 23:32:04 GMT  
		Size: 2.8 KB (2800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52cecdf1cab698a77e8c11aafa293553711d7510cda25bf2398fd43b8c9a442`  
		Last Modified: Tue, 14 Apr 2020 23:52:13 GMT  
		Size: 20.1 MB (20129788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704f7281ba7ef12f957c89911ede388d0db510c3ba403fa284f707874d1cccf9`  
		Last Modified: Tue, 14 Apr 2020 23:52:06 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:c9bd10679eb475e1632ed71de0c780cc04a442631ea64e10f4fb89359d7cbb14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92255313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614b828fcff4ad5eef8cfede2fe6709c7c336fae340de286bc39cf9170879a08`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 31 Mar 2020 02:08:11 GMT
ADD file:ab80e35f9496440fac439083c9c9c18cd80521039d4bc4f4082e8e84a5e9fcda in / 
# Tue, 31 Mar 2020 02:08:15 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 04:41:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 04:41:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Apr 2020 00:12:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 00:12:44 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 14 Apr 2020 22:45:08 GMT
ENV TELEGRAF_VERSION=1.14.1
# Tue, 14 Apr 2020 22:45:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 14 Apr 2020 22:45:20 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Apr 2020 22:45:20 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 14 Apr 2020 22:45:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Apr 2020 22:45:26 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:84582781a9f06ad84225307f9cf89d5f77f6e5610281e6ca088fc8c2e9a1d027`  
		Last Modified: Tue, 31 Mar 2020 02:14:13 GMT  
		Size: 43.2 MB (43158116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaedfc9896782bd00cfcf104ca392d0b85363b41be4ecedd7c058c1c183ac01`  
		Last Modified: Tue, 31 Mar 2020 04:49:39 GMT  
		Size: 9.7 MB (9748484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa6bb03021f1e64553e2c40a904ffe7c70a0112c00ba9bf44f67ad27162f2b0`  
		Last Modified: Tue, 31 Mar 2020 04:49:38 GMT  
		Size: 4.1 MB (4094373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107b3cd097a2df228bfaca5e7da60c3cad508fe1174a335b5c3a04176a7a6424`  
		Last Modified: Wed, 01 Apr 2020 00:13:38 GMT  
		Size: 15.5 MB (15529462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67412f3a7a311a019187de482f8f8de65c51f53853a9ff154c107e95821a0106`  
		Last Modified: Wed, 01 Apr 2020 00:13:33 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea0b6d8ea998fe90b61d9d7911dff2048963e9deb778570c192c6f8fe39a9e9`  
		Last Modified: Tue, 14 Apr 2020 22:45:58 GMT  
		Size: 19.7 MB (19721893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ab3f9a68cb72dbcd5da99d37fafe137ed8bfa5ed39898672b4054899457c04`  
		Last Modified: Tue, 14 Apr 2020 22:45:51 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
