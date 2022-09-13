<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.22`](#telegraf122)
-	[`telegraf:1.22-alpine`](#telegraf122-alpine)
-	[`telegraf:1.22.4`](#telegraf1224)
-	[`telegraf:1.22.4-alpine`](#telegraf1224-alpine)
-	[`telegraf:1.23`](#telegraf123)
-	[`telegraf:1.23-alpine`](#telegraf123-alpine)
-	[`telegraf:1.23.4`](#telegraf1234)
-	[`telegraf:1.23.4-alpine`](#telegraf1234-alpine)
-	[`telegraf:1.24`](#telegraf124)
-	[`telegraf:1.24-alpine`](#telegraf124-alpine)
-	[`telegraf:1.24.0`](#telegraf1240)
-	[`telegraf:1.24.0-alpine`](#telegraf1240-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.22`

```console
$ docker pull telegraf@sha256:0df3bf31135553c300910593f3acfa2836b21cffd52d53631edb74dac35d6d9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.22` - linux; amd64

```console
$ docker pull telegraf@sha256:a0316cb0fdb6a261137a44cccf0b77843b48dd78d37cb5e9e40d2f23dbfca22b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.3 MB (130331150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84506e8647eb7b289c4c6ea8b03c412e8f17cba29f6b06ed0eaa29a7c01d1d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:43:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 17:35:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 17:35:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 17:35:46 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 13 Sep 2022 17:35:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 17:35:51 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 17:35:51 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 17:35:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:35:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f452ade5c33097eba4ba88a24bd77a93a3d994d4dc39b936482655e664857`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 5.2 MB (5163200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42821cd14fb31c4aa253203e7f8e34fc3b15d69ce370f1223fbbe4252a64202`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 10.9 MB (10876384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfb39d3f3786c76fffb986ff0092bf7e14fa947dc58edade563c2ab950276ee`  
		Last Modified: Tue, 13 Sep 2022 17:36:37 GMT  
		Size: 18.8 MB (18759844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34ca274d85bef3e27c3994985878b4a4442fae094ba9739c90d86dc894ce0fe`  
		Last Modified: Tue, 13 Sep 2022 17:36:34 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f75842cae1640a33108f5ededb2125644b71afa3de6d5c0611a4191ede3c75f`  
		Last Modified: Tue, 13 Sep 2022 17:36:41 GMT  
		Size: 40.5 MB (40498750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef7cd5e85e017d234183834eb5a92ee7d08b4e718c367ea3e3e1e8bae9add4b`  
		Last Modified: Tue, 13 Sep 2022 17:36:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c5032ca887c62a6c39660f064d007987020f3dbabdc0f6f8db42a0c687ea0338
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120740832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a6bd0f2aa522d544fb76f1d38ae1f53bd82c1b15a81daf66d23f727bdfbd19`
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
# Wed, 24 Aug 2022 17:14:24 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 24 Aug 2022 17:14:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 24 Aug 2022 17:14:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 24 Aug 2022 17:14:30 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 24 Aug 2022 17:14:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Aug 2022 17:14:30 GMT
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
	-	`sha256:c544fef23fe2e946cb72d0a32732e5bfa8f5dfefaf81df81418f85d02e0414e9`  
		Last Modified: Wed, 24 Aug 2022 17:15:33 GMT  
		Size: 37.9 MB (37921671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070b8eae645d69f668b884fcb3600d73cd55841693ae96de8137e7189911b6a3`  
		Last Modified: Wed, 24 Aug 2022 17:15:26 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:9bb1b5af476c6cda44c6de45fd7437cedd8e05bedcf6e5546222bb4e6c361438
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124694766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa6f6414965a403e46e9c95b815253501b6e120f7a94c2cf5ee66a5b70de41bf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:01:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:01:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 18:07:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 18:07:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 18:07:25 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 13 Sep 2022 18:07:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 18:07:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 18:07:32 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 18:07:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 18:07:33 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9f2bf6f4deeb7ed2acd14f7997ec0a0cdf45b5b314051ddaab1911e22d997d`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 5.1 MB (5148962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa25dbffbabb85498e5d2c2d270f81ca67f9679617c9611bf18faf6ed4a09a0`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 10.7 MB (10657461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865179fd5e4418698353c9c0b184dc2f2287d8bdcd53256359563341622818df`  
		Last Modified: Tue, 13 Sep 2022 18:08:27 GMT  
		Size: 18.4 MB (18382801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26c9d0ca7779ffc9446d76ed999981c37950b65e809a3c77001c5b37399e196`  
		Last Modified: Tue, 13 Sep 2022 18:08:24 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91e2d78eb3f869020c5b5ebd6de4d1bcd23aa886526ef3db6951eaeabdc226f`  
		Last Modified: Tue, 13 Sep 2022 18:08:29 GMT  
		Size: 36.8 MB (36810960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af8cd0c1d10e46ae7577aac083e817479b171f4205ef5910b83db70d55adda1`  
		Last Modified: Tue, 13 Sep 2022 18:08:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22-alpine`

```console
$ docker pull telegraf@sha256:a279af3355355d24d17254cb5449c26398dc1f8c8654dccdd7fd4510c095a32c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.22-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:6c51dd921fc0e34e4b617220425783e8857b1da3782f3fe4a696c6130dbb9c06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46468333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705231ea9213ee2eab5c3d24ac68ecaf3337dfe7fb8873eaa3e3676b5f8ffdfc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 24 Aug 2022 19:32:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 13 Sep 2022 00:50:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 13 Sep 2022 00:50:34 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 13 Sep 2022 00:50:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 13 Sep 2022 00:50:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 00:50:41 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 13 Sep 2022 00:50:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 00:50:41 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8decf7e163fc13e474b783cc63da7c74fa93277afae73355cd03b1102adcc3`  
		Last Modified: Wed, 24 Aug 2022 19:33:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ce451dc5a0d29791fad6cba4e6a7b11245a7ac2571e62993f92412ea15863`  
		Last Modified: Tue, 13 Sep 2022 00:51:36 GMT  
		Size: 3.3 MB (3310222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da52bc5f4c9ecaa7d02be65730360754f9f98ae550b13cd02ebb55332a6cca8`  
		Last Modified: Tue, 13 Sep 2022 00:51:42 GMT  
		Size: 40.4 MB (40351579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498f71587107c838000873175d4522be271130574f8e44729d5ebad06ce30d2f`  
		Last Modified: Tue, 13 Sep 2022 00:51:35 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22.4`

```console
$ docker pull telegraf@sha256:0df3bf31135553c300910593f3acfa2836b21cffd52d53631edb74dac35d6d9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.22.4` - linux; amd64

```console
$ docker pull telegraf@sha256:a0316cb0fdb6a261137a44cccf0b77843b48dd78d37cb5e9e40d2f23dbfca22b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.3 MB (130331150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84506e8647eb7b289c4c6ea8b03c412e8f17cba29f6b06ed0eaa29a7c01d1d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:43:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 17:35:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 17:35:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 17:35:46 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 13 Sep 2022 17:35:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 17:35:51 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 17:35:51 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 17:35:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:35:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f452ade5c33097eba4ba88a24bd77a93a3d994d4dc39b936482655e664857`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 5.2 MB (5163200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42821cd14fb31c4aa253203e7f8e34fc3b15d69ce370f1223fbbe4252a64202`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 10.9 MB (10876384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfb39d3f3786c76fffb986ff0092bf7e14fa947dc58edade563c2ab950276ee`  
		Last Modified: Tue, 13 Sep 2022 17:36:37 GMT  
		Size: 18.8 MB (18759844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34ca274d85bef3e27c3994985878b4a4442fae094ba9739c90d86dc894ce0fe`  
		Last Modified: Tue, 13 Sep 2022 17:36:34 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f75842cae1640a33108f5ededb2125644b71afa3de6d5c0611a4191ede3c75f`  
		Last Modified: Tue, 13 Sep 2022 17:36:41 GMT  
		Size: 40.5 MB (40498750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef7cd5e85e017d234183834eb5a92ee7d08b4e718c367ea3e3e1e8bae9add4b`  
		Last Modified: Tue, 13 Sep 2022 17:36:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c5032ca887c62a6c39660f064d007987020f3dbabdc0f6f8db42a0c687ea0338
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120740832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a6bd0f2aa522d544fb76f1d38ae1f53bd82c1b15a81daf66d23f727bdfbd19`
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
# Wed, 24 Aug 2022 17:14:24 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 24 Aug 2022 17:14:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 24 Aug 2022 17:14:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 24 Aug 2022 17:14:30 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 24 Aug 2022 17:14:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Aug 2022 17:14:30 GMT
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
	-	`sha256:c544fef23fe2e946cb72d0a32732e5bfa8f5dfefaf81df81418f85d02e0414e9`  
		Last Modified: Wed, 24 Aug 2022 17:15:33 GMT  
		Size: 37.9 MB (37921671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070b8eae645d69f668b884fcb3600d73cd55841693ae96de8137e7189911b6a3`  
		Last Modified: Wed, 24 Aug 2022 17:15:26 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:9bb1b5af476c6cda44c6de45fd7437cedd8e05bedcf6e5546222bb4e6c361438
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124694766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa6f6414965a403e46e9c95b815253501b6e120f7a94c2cf5ee66a5b70de41bf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:01:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:01:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 18:07:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 18:07:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 18:07:25 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 13 Sep 2022 18:07:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 18:07:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 18:07:32 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 18:07:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 18:07:33 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9f2bf6f4deeb7ed2acd14f7997ec0a0cdf45b5b314051ddaab1911e22d997d`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 5.1 MB (5148962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa25dbffbabb85498e5d2c2d270f81ca67f9679617c9611bf18faf6ed4a09a0`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 10.7 MB (10657461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865179fd5e4418698353c9c0b184dc2f2287d8bdcd53256359563341622818df`  
		Last Modified: Tue, 13 Sep 2022 18:08:27 GMT  
		Size: 18.4 MB (18382801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26c9d0ca7779ffc9446d76ed999981c37950b65e809a3c77001c5b37399e196`  
		Last Modified: Tue, 13 Sep 2022 18:08:24 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91e2d78eb3f869020c5b5ebd6de4d1bcd23aa886526ef3db6951eaeabdc226f`  
		Last Modified: Tue, 13 Sep 2022 18:08:29 GMT  
		Size: 36.8 MB (36810960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af8cd0c1d10e46ae7577aac083e817479b171f4205ef5910b83db70d55adda1`  
		Last Modified: Tue, 13 Sep 2022 18:08:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22.4-alpine`

```console
$ docker pull telegraf@sha256:a279af3355355d24d17254cb5449c26398dc1f8c8654dccdd7fd4510c095a32c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.22.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:6c51dd921fc0e34e4b617220425783e8857b1da3782f3fe4a696c6130dbb9c06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46468333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705231ea9213ee2eab5c3d24ac68ecaf3337dfe7fb8873eaa3e3676b5f8ffdfc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 24 Aug 2022 19:32:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 13 Sep 2022 00:50:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 13 Sep 2022 00:50:34 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 13 Sep 2022 00:50:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 13 Sep 2022 00:50:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 00:50:41 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 13 Sep 2022 00:50:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 00:50:41 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8decf7e163fc13e474b783cc63da7c74fa93277afae73355cd03b1102adcc3`  
		Last Modified: Wed, 24 Aug 2022 19:33:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ce451dc5a0d29791fad6cba4e6a7b11245a7ac2571e62993f92412ea15863`  
		Last Modified: Tue, 13 Sep 2022 00:51:36 GMT  
		Size: 3.3 MB (3310222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da52bc5f4c9ecaa7d02be65730360754f9f98ae550b13cd02ebb55332a6cca8`  
		Last Modified: Tue, 13 Sep 2022 00:51:42 GMT  
		Size: 40.4 MB (40351579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498f71587107c838000873175d4522be271130574f8e44729d5ebad06ce30d2f`  
		Last Modified: Tue, 13 Sep 2022 00:51:35 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23`

```console
$ docker pull telegraf@sha256:ca3b00a8875af1617eabb69edd38f63eadee04cf263116ab767e14e7338306ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23` - linux; amd64

```console
$ docker pull telegraf@sha256:d7edb0e5cf8171f0b38335c3cfd665689685d24c46ea054acff380d92407a227
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131681590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51f189b9b4015a8aedd541305c62603c999ba025b5f9b49f4a7221371c69c0eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:43:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 17:35:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 17:35:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 17:35:58 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 13 Sep 2022 17:36:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 17:36:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 17:36:03 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 17:36:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:36:03 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f452ade5c33097eba4ba88a24bd77a93a3d994d4dc39b936482655e664857`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 5.2 MB (5163200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42821cd14fb31c4aa253203e7f8e34fc3b15d69ce370f1223fbbe4252a64202`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 10.9 MB (10876384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfb39d3f3786c76fffb986ff0092bf7e14fa947dc58edade563c2ab950276ee`  
		Last Modified: Tue, 13 Sep 2022 17:36:37 GMT  
		Size: 18.8 MB (18759844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34ca274d85bef3e27c3994985878b4a4442fae094ba9739c90d86dc894ce0fe`  
		Last Modified: Tue, 13 Sep 2022 17:36:34 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dad369ea22bd32c0ec43ec27067700b05e934a7e968a727ee965e3031aabb39`  
		Last Modified: Tue, 13 Sep 2022 17:36:59 GMT  
		Size: 41.8 MB (41849189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92084af31a2690cf629c3ddbc256e1b7b13e0b8f409b9fdbcebf1f8d4137c916`  
		Last Modified: Tue, 13 Sep 2022 17:36:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:f36be7242e755524990f0674ad2b66a7dc0124ab88af04d030a583e5f92c7754
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121925706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:745c4039868708153fbdf9e81a24218fa03d09a03a402c3ece548b1bdbb4c561`
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
# Wed, 24 Aug 2022 17:14:34 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 24 Aug 2022 17:14:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 24 Aug 2022 17:14:40 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 24 Aug 2022 17:14:40 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 24 Aug 2022 17:14:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Aug 2022 17:14:40 GMT
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
	-	`sha256:16cf92227e9efb3763f04d95fc8533d16d44f5e9ff62208aae4f9e523a4ecde4`  
		Last Modified: Wed, 24 Aug 2022 17:15:51 GMT  
		Size: 39.1 MB (39106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9db4b7aa12e76db182caeb235e71cf186e75e64e6aab4f475cf324cc43b61d`  
		Last Modified: Wed, 24 Aug 2022 17:15:44 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:aadf3df5a2ba7010b1e227d0932091db68aa21a7c95a2ce2f4ffb0da6eb0a09a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125914034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd41501f4f53a92842524a74405f4de6de586b51a1e2451ba71dcb2e2f90606`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:01:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:01:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 18:07:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 18:07:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 18:07:39 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 13 Sep 2022 18:07:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 18:07:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 18:07:46 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 18:07:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 18:07:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9f2bf6f4deeb7ed2acd14f7997ec0a0cdf45b5b314051ddaab1911e22d997d`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 5.1 MB (5148962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa25dbffbabb85498e5d2c2d270f81ca67f9679617c9611bf18faf6ed4a09a0`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 10.7 MB (10657461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865179fd5e4418698353c9c0b184dc2f2287d8bdcd53256359563341622818df`  
		Last Modified: Tue, 13 Sep 2022 18:08:27 GMT  
		Size: 18.4 MB (18382801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26c9d0ca7779ffc9446d76ed999981c37950b65e809a3c77001c5b37399e196`  
		Last Modified: Tue, 13 Sep 2022 18:08:24 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413e44698a625c1d0ca0335dc01ba389e099727b7f3557c998022d12cce79618`  
		Last Modified: Tue, 13 Sep 2022 18:08:47 GMT  
		Size: 38.0 MB (38030226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369240e5130c3043050161529c35d98e8fb93e1f197273f0b1d46bc6f93eb34f`  
		Last Modified: Tue, 13 Sep 2022 18:08:41 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23-alpine`

```console
$ docker pull telegraf@sha256:9bf178d64a12d9a290789a139477f1c04842e0111eade5f28e89e7fc4af950d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:8aa8f02d8151e6080989f24fd0c0a2535932f7957735ec9164b43efb9570d4b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47802160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5234da6e46926c3ca880c50fd822627d9bc403011a9a2dddf9a6548381d72597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 24 Aug 2022 19:32:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 13 Sep 2022 00:50:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 13 Sep 2022 00:50:46 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 13 Sep 2022 00:50:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 13 Sep 2022 00:50:52 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 00:50:52 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 13 Sep 2022 00:50:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 00:50:53 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8decf7e163fc13e474b783cc63da7c74fa93277afae73355cd03b1102adcc3`  
		Last Modified: Wed, 24 Aug 2022 19:33:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ce451dc5a0d29791fad6cba4e6a7b11245a7ac2571e62993f92412ea15863`  
		Last Modified: Tue, 13 Sep 2022 00:51:36 GMT  
		Size: 3.3 MB (3310222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07235f531f957d2e24caa5ac4efbd259ec785c92086d122a46d20bc0d646749`  
		Last Modified: Tue, 13 Sep 2022 00:52:00 GMT  
		Size: 41.7 MB (41685403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189922a71089594de911aefb4673a808f138777adf6d886a31f36475cb1b6b27`  
		Last Modified: Tue, 13 Sep 2022 00:51:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.4`

```console
$ docker pull telegraf@sha256:ca3b00a8875af1617eabb69edd38f63eadee04cf263116ab767e14e7338306ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23.4` - linux; amd64

```console
$ docker pull telegraf@sha256:d7edb0e5cf8171f0b38335c3cfd665689685d24c46ea054acff380d92407a227
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131681590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51f189b9b4015a8aedd541305c62603c999ba025b5f9b49f4a7221371c69c0eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:43:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 17:35:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 17:35:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 17:35:58 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 13 Sep 2022 17:36:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 17:36:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 17:36:03 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 17:36:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:36:03 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f452ade5c33097eba4ba88a24bd77a93a3d994d4dc39b936482655e664857`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 5.2 MB (5163200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42821cd14fb31c4aa253203e7f8e34fc3b15d69ce370f1223fbbe4252a64202`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 10.9 MB (10876384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfb39d3f3786c76fffb986ff0092bf7e14fa947dc58edade563c2ab950276ee`  
		Last Modified: Tue, 13 Sep 2022 17:36:37 GMT  
		Size: 18.8 MB (18759844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34ca274d85bef3e27c3994985878b4a4442fae094ba9739c90d86dc894ce0fe`  
		Last Modified: Tue, 13 Sep 2022 17:36:34 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dad369ea22bd32c0ec43ec27067700b05e934a7e968a727ee965e3031aabb39`  
		Last Modified: Tue, 13 Sep 2022 17:36:59 GMT  
		Size: 41.8 MB (41849189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92084af31a2690cf629c3ddbc256e1b7b13e0b8f409b9fdbcebf1f8d4137c916`  
		Last Modified: Tue, 13 Sep 2022 17:36:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:f36be7242e755524990f0674ad2b66a7dc0124ab88af04d030a583e5f92c7754
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121925706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:745c4039868708153fbdf9e81a24218fa03d09a03a402c3ece548b1bdbb4c561`
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
# Wed, 24 Aug 2022 17:14:34 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 24 Aug 2022 17:14:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 24 Aug 2022 17:14:40 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 24 Aug 2022 17:14:40 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 24 Aug 2022 17:14:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Aug 2022 17:14:40 GMT
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
	-	`sha256:16cf92227e9efb3763f04d95fc8533d16d44f5e9ff62208aae4f9e523a4ecde4`  
		Last Modified: Wed, 24 Aug 2022 17:15:51 GMT  
		Size: 39.1 MB (39106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9db4b7aa12e76db182caeb235e71cf186e75e64e6aab4f475cf324cc43b61d`  
		Last Modified: Wed, 24 Aug 2022 17:15:44 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:aadf3df5a2ba7010b1e227d0932091db68aa21a7c95a2ce2f4ffb0da6eb0a09a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125914034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd41501f4f53a92842524a74405f4de6de586b51a1e2451ba71dcb2e2f90606`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:01:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:01:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 18:07:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 18:07:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 18:07:39 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 13 Sep 2022 18:07:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 18:07:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 18:07:46 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 18:07:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 18:07:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9f2bf6f4deeb7ed2acd14f7997ec0a0cdf45b5b314051ddaab1911e22d997d`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 5.1 MB (5148962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa25dbffbabb85498e5d2c2d270f81ca67f9679617c9611bf18faf6ed4a09a0`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 10.7 MB (10657461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865179fd5e4418698353c9c0b184dc2f2287d8bdcd53256359563341622818df`  
		Last Modified: Tue, 13 Sep 2022 18:08:27 GMT  
		Size: 18.4 MB (18382801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26c9d0ca7779ffc9446d76ed999981c37950b65e809a3c77001c5b37399e196`  
		Last Modified: Tue, 13 Sep 2022 18:08:24 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413e44698a625c1d0ca0335dc01ba389e099727b7f3557c998022d12cce79618`  
		Last Modified: Tue, 13 Sep 2022 18:08:47 GMT  
		Size: 38.0 MB (38030226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369240e5130c3043050161529c35d98e8fb93e1f197273f0b1d46bc6f93eb34f`  
		Last Modified: Tue, 13 Sep 2022 18:08:41 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.4-alpine`

```console
$ docker pull telegraf@sha256:9bf178d64a12d9a290789a139477f1c04842e0111eade5f28e89e7fc4af950d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:8aa8f02d8151e6080989f24fd0c0a2535932f7957735ec9164b43efb9570d4b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47802160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5234da6e46926c3ca880c50fd822627d9bc403011a9a2dddf9a6548381d72597`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 24 Aug 2022 19:32:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 13 Sep 2022 00:50:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 13 Sep 2022 00:50:46 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 13 Sep 2022 00:50:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 13 Sep 2022 00:50:52 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 00:50:52 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 13 Sep 2022 00:50:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 00:50:53 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8decf7e163fc13e474b783cc63da7c74fa93277afae73355cd03b1102adcc3`  
		Last Modified: Wed, 24 Aug 2022 19:33:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ce451dc5a0d29791fad6cba4e6a7b11245a7ac2571e62993f92412ea15863`  
		Last Modified: Tue, 13 Sep 2022 00:51:36 GMT  
		Size: 3.3 MB (3310222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07235f531f957d2e24caa5ac4efbd259ec785c92086d122a46d20bc0d646749`  
		Last Modified: Tue, 13 Sep 2022 00:52:00 GMT  
		Size: 41.7 MB (41685403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189922a71089594de911aefb4673a808f138777adf6d886a31f36475cb1b6b27`  
		Last Modified: Tue, 13 Sep 2022 00:51:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24`

```console
$ docker pull telegraf@sha256:9bb85fde12870bfd6010be6927f877056f918205c690a349c7061af80752d1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24` - linux; amd64

```console
$ docker pull telegraf@sha256:2267cb76c1361e4a187de501e8ec2b5061b30efb208a9027156d013cf3ffca38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133736905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d07df4761d9c1d0354867b9a45df2b25909780c755022b87d4b89d01a20bb2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:43:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 17:35:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 17:35:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 17:36:07 GMT
ENV TELEGRAF_VERSION=1.24.0
# Tue, 13 Sep 2022 17:36:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 17:36:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 17:36:12 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 17:36:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:36:12 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f452ade5c33097eba4ba88a24bd77a93a3d994d4dc39b936482655e664857`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 5.2 MB (5163200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42821cd14fb31c4aa253203e7f8e34fc3b15d69ce370f1223fbbe4252a64202`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 10.9 MB (10876384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfb39d3f3786c76fffb986ff0092bf7e14fa947dc58edade563c2ab950276ee`  
		Last Modified: Tue, 13 Sep 2022 17:36:37 GMT  
		Size: 18.8 MB (18759844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34ca274d85bef3e27c3994985878b4a4442fae094ba9739c90d86dc894ce0fe`  
		Last Modified: Tue, 13 Sep 2022 17:36:34 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132322691b7dc5684ca1e40878845d5360c1688779c5bd6bb8a0d5b5ce947c80`  
		Last Modified: Tue, 13 Sep 2022 17:37:16 GMT  
		Size: 43.9 MB (43904504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfddddf032e58d20bdc8bf3f89a41e67f8cd92cbe1066fede84020f63682ec1d`  
		Last Modified: Tue, 13 Sep 2022 17:37:09 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24` - linux; arm variant v7

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

### `telegraf:1.24` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:0a9d503775a5865892f040347539f09ba06626106a219e7e36e75caf7623df4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127675094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80993d45a30d1103c9b5834e22672381ae4fcd0466faff22aeac9456937e837`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:01:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:01:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 18:07:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 18:07:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 18:07:53 GMT
ENV TELEGRAF_VERSION=1.24.0
# Tue, 13 Sep 2022 18:07:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 18:07:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 18:08:00 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 18:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 18:08:01 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9f2bf6f4deeb7ed2acd14f7997ec0a0cdf45b5b314051ddaab1911e22d997d`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 5.1 MB (5148962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa25dbffbabb85498e5d2c2d270f81ca67f9679617c9611bf18faf6ed4a09a0`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 10.7 MB (10657461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865179fd5e4418698353c9c0b184dc2f2287d8bdcd53256359563341622818df`  
		Last Modified: Tue, 13 Sep 2022 18:08:27 GMT  
		Size: 18.4 MB (18382801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26c9d0ca7779ffc9446d76ed999981c37950b65e809a3c77001c5b37399e196`  
		Last Modified: Tue, 13 Sep 2022 18:08:24 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f32e509bdac0e10716031dba90cda45d96e26abcfecb67aa5150edb0862510`  
		Last Modified: Tue, 13 Sep 2022 18:09:05 GMT  
		Size: 39.8 MB (39791290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486711c8fcbe7fcb273da9d3599748031c206e41567c3019ccae06f0a23e1ac1`  
		Last Modified: Tue, 13 Sep 2022 18:08:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24-alpine`

```console
$ docker pull telegraf@sha256:6b2a9509b62e04e70f1249bf4e245cbd7f2edbcd286d49da5fce2372c609e6d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:6b1b6839ef217a1f804da774bbcec16df05a385c3a3f553ebe02d397d3b63677
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49860906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68f844a82b14bc7770e56f053b2d153e20f8bb013e1f0bce64d61f787178b75`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 24 Aug 2022 19:32:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 13 Sep 2022 00:50:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 13 Sep 2022 00:51:03 GMT
ENV TELEGRAF_VERSION=1.24.0
# Tue, 13 Sep 2022 00:51:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 13 Sep 2022 00:51:14 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 00:51:15 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 13 Sep 2022 00:51:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 00:51:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8decf7e163fc13e474b783cc63da7c74fa93277afae73355cd03b1102adcc3`  
		Last Modified: Wed, 24 Aug 2022 19:33:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ce451dc5a0d29791fad6cba4e6a7b11245a7ac2571e62993f92412ea15863`  
		Last Modified: Tue, 13 Sep 2022 00:51:36 GMT  
		Size: 3.3 MB (3310222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65aec5f38706f9f34576653ae6a99868e109b73fb9ea7bfa661717ea5ca1651`  
		Last Modified: Tue, 13 Sep 2022 00:52:35 GMT  
		Size: 43.7 MB (43744149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb2428e0684d34edd8c2ae8f60aa28e7168761f240daece13ab17a0e5216813`  
		Last Modified: Tue, 13 Sep 2022 00:52:28 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.0`

```console
$ docker pull telegraf@sha256:9bb85fde12870bfd6010be6927f877056f918205c690a349c7061af80752d1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24.0` - linux; amd64

```console
$ docker pull telegraf@sha256:2267cb76c1361e4a187de501e8ec2b5061b30efb208a9027156d013cf3ffca38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133736905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d07df4761d9c1d0354867b9a45df2b25909780c755022b87d4b89d01a20bb2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:43:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 17:35:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 17:35:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 17:36:07 GMT
ENV TELEGRAF_VERSION=1.24.0
# Tue, 13 Sep 2022 17:36:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 17:36:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 17:36:12 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 17:36:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:36:12 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f452ade5c33097eba4ba88a24bd77a93a3d994d4dc39b936482655e664857`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 5.2 MB (5163200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42821cd14fb31c4aa253203e7f8e34fc3b15d69ce370f1223fbbe4252a64202`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 10.9 MB (10876384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfb39d3f3786c76fffb986ff0092bf7e14fa947dc58edade563c2ab950276ee`  
		Last Modified: Tue, 13 Sep 2022 17:36:37 GMT  
		Size: 18.8 MB (18759844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34ca274d85bef3e27c3994985878b4a4442fae094ba9739c90d86dc894ce0fe`  
		Last Modified: Tue, 13 Sep 2022 17:36:34 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132322691b7dc5684ca1e40878845d5360c1688779c5bd6bb8a0d5b5ce947c80`  
		Last Modified: Tue, 13 Sep 2022 17:37:16 GMT  
		Size: 43.9 MB (43904504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfddddf032e58d20bdc8bf3f89a41e67f8cd92cbe1066fede84020f63682ec1d`  
		Last Modified: Tue, 13 Sep 2022 17:37:09 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24.0` - linux; arm variant v7

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

### `telegraf:1.24.0` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:0a9d503775a5865892f040347539f09ba06626106a219e7e36e75caf7623df4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127675094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80993d45a30d1103c9b5834e22672381ae4fcd0466faff22aeac9456937e837`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:01:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:01:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 18:07:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 18:07:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 18:07:53 GMT
ENV TELEGRAF_VERSION=1.24.0
# Tue, 13 Sep 2022 18:07:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 18:07:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 18:08:00 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 18:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 18:08:01 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9f2bf6f4deeb7ed2acd14f7997ec0a0cdf45b5b314051ddaab1911e22d997d`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 5.1 MB (5148962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa25dbffbabb85498e5d2c2d270f81ca67f9679617c9611bf18faf6ed4a09a0`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 10.7 MB (10657461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865179fd5e4418698353c9c0b184dc2f2287d8bdcd53256359563341622818df`  
		Last Modified: Tue, 13 Sep 2022 18:08:27 GMT  
		Size: 18.4 MB (18382801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26c9d0ca7779ffc9446d76ed999981c37950b65e809a3c77001c5b37399e196`  
		Last Modified: Tue, 13 Sep 2022 18:08:24 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f32e509bdac0e10716031dba90cda45d96e26abcfecb67aa5150edb0862510`  
		Last Modified: Tue, 13 Sep 2022 18:09:05 GMT  
		Size: 39.8 MB (39791290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486711c8fcbe7fcb273da9d3599748031c206e41567c3019ccae06f0a23e1ac1`  
		Last Modified: Tue, 13 Sep 2022 18:08:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.0-alpine`

```console
$ docker pull telegraf@sha256:6b2a9509b62e04e70f1249bf4e245cbd7f2edbcd286d49da5fce2372c609e6d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24.0-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:6b1b6839ef217a1f804da774bbcec16df05a385c3a3f553ebe02d397d3b63677
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49860906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68f844a82b14bc7770e56f053b2d153e20f8bb013e1f0bce64d61f787178b75`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 24 Aug 2022 19:32:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 13 Sep 2022 00:50:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 13 Sep 2022 00:51:03 GMT
ENV TELEGRAF_VERSION=1.24.0
# Tue, 13 Sep 2022 00:51:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 13 Sep 2022 00:51:14 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 00:51:15 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 13 Sep 2022 00:51:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 00:51:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8decf7e163fc13e474b783cc63da7c74fa93277afae73355cd03b1102adcc3`  
		Last Modified: Wed, 24 Aug 2022 19:33:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ce451dc5a0d29791fad6cba4e6a7b11245a7ac2571e62993f92412ea15863`  
		Last Modified: Tue, 13 Sep 2022 00:51:36 GMT  
		Size: 3.3 MB (3310222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65aec5f38706f9f34576653ae6a99868e109b73fb9ea7bfa661717ea5ca1651`  
		Last Modified: Tue, 13 Sep 2022 00:52:35 GMT  
		Size: 43.7 MB (43744149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb2428e0684d34edd8c2ae8f60aa28e7168761f240daece13ab17a0e5216813`  
		Last Modified: Tue, 13 Sep 2022 00:52:28 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:6b2a9509b62e04e70f1249bf4e245cbd7f2edbcd286d49da5fce2372c609e6d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:6b1b6839ef217a1f804da774bbcec16df05a385c3a3f553ebe02d397d3b63677
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49860906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68f844a82b14bc7770e56f053b2d153e20f8bb013e1f0bce64d61f787178b75`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 24 Aug 2022 19:32:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 13 Sep 2022 00:50:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 13 Sep 2022 00:51:03 GMT
ENV TELEGRAF_VERSION=1.24.0
# Tue, 13 Sep 2022 00:51:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 13 Sep 2022 00:51:14 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 00:51:15 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 13 Sep 2022 00:51:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 00:51:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8decf7e163fc13e474b783cc63da7c74fa93277afae73355cd03b1102adcc3`  
		Last Modified: Wed, 24 Aug 2022 19:33:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ce451dc5a0d29791fad6cba4e6a7b11245a7ac2571e62993f92412ea15863`  
		Last Modified: Tue, 13 Sep 2022 00:51:36 GMT  
		Size: 3.3 MB (3310222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65aec5f38706f9f34576653ae6a99868e109b73fb9ea7bfa661717ea5ca1651`  
		Last Modified: Tue, 13 Sep 2022 00:52:35 GMT  
		Size: 43.7 MB (43744149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb2428e0684d34edd8c2ae8f60aa28e7168761f240daece13ab17a0e5216813`  
		Last Modified: Tue, 13 Sep 2022 00:52:28 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:9bb85fde12870bfd6010be6927f877056f918205c690a349c7061af80752d1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:2267cb76c1361e4a187de501e8ec2b5061b30efb208a9027156d013cf3ffca38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133736905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d07df4761d9c1d0354867b9a45df2b25909780c755022b87d4b89d01a20bb2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:43:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 17:35:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 17:35:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 17:36:07 GMT
ENV TELEGRAF_VERSION=1.24.0
# Tue, 13 Sep 2022 17:36:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 17:36:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 17:36:12 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 17:36:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:36:12 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f452ade5c33097eba4ba88a24bd77a93a3d994d4dc39b936482655e664857`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 5.2 MB (5163200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42821cd14fb31c4aa253203e7f8e34fc3b15d69ce370f1223fbbe4252a64202`  
		Last Modified: Tue, 13 Sep 2022 03:50:03 GMT  
		Size: 10.9 MB (10876384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfb39d3f3786c76fffb986ff0092bf7e14fa947dc58edade563c2ab950276ee`  
		Last Modified: Tue, 13 Sep 2022 17:36:37 GMT  
		Size: 18.8 MB (18759844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34ca274d85bef3e27c3994985878b4a4442fae094ba9739c90d86dc894ce0fe`  
		Last Modified: Tue, 13 Sep 2022 17:36:34 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132322691b7dc5684ca1e40878845d5360c1688779c5bd6bb8a0d5b5ce947c80`  
		Last Modified: Tue, 13 Sep 2022 17:37:16 GMT  
		Size: 43.9 MB (43904504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfddddf032e58d20bdc8bf3f89a41e67f8cd92cbe1066fede84020f63682ec1d`  
		Last Modified: Tue, 13 Sep 2022 17:37:09 GMT  
		Size: 343.0 B  
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
$ docker pull telegraf@sha256:0a9d503775a5865892f040347539f09ba06626106a219e7e36e75caf7623df4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127675094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a80993d45a30d1103c9b5834e22672381ae4fcd0466faff22aeac9456937e837`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:01:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:01:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 18:07:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 18:07:24 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Sep 2022 18:07:53 GMT
ENV TELEGRAF_VERSION=1.24.0
# Tue, 13 Sep 2022 18:07:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Sep 2022 18:07:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Sep 2022 18:08:00 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Sep 2022 18:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 18:08:01 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9f2bf6f4deeb7ed2acd14f7997ec0a0cdf45b5b314051ddaab1911e22d997d`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 5.1 MB (5148962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa25dbffbabb85498e5d2c2d270f81ca67f9679617c9611bf18faf6ed4a09a0`  
		Last Modified: Tue, 13 Sep 2022 05:09:57 GMT  
		Size: 10.7 MB (10657461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865179fd5e4418698353c9c0b184dc2f2287d8bdcd53256359563341622818df`  
		Last Modified: Tue, 13 Sep 2022 18:08:27 GMT  
		Size: 18.4 MB (18382801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26c9d0ca7779ffc9446d76ed999981c37950b65e809a3c77001c5b37399e196`  
		Last Modified: Tue, 13 Sep 2022 18:08:24 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f32e509bdac0e10716031dba90cda45d96e26abcfecb67aa5150edb0862510`  
		Last Modified: Tue, 13 Sep 2022 18:09:05 GMT  
		Size: 39.8 MB (39791290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486711c8fcbe7fcb273da9d3599748031c206e41567c3019ccae06f0a23e1ac1`  
		Last Modified: Tue, 13 Sep 2022 18:08:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
