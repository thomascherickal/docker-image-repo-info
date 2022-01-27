<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.19`](#telegraf119)
-	[`telegraf:1.19-alpine`](#telegraf119-alpine)
-	[`telegraf:1.19.3`](#telegraf1193)
-	[`telegraf:1.19.3-alpine`](#telegraf1193-alpine)
-	[`telegraf:1.20`](#telegraf120)
-	[`telegraf:1.20-alpine`](#telegraf120-alpine)
-	[`telegraf:1.20.4`](#telegraf1204)
-	[`telegraf:1.20.4-alpine`](#telegraf1204-alpine)
-	[`telegraf:1.21`](#telegraf121)
-	[`telegraf:1.21-alpine`](#telegraf121-alpine)
-	[`telegraf:1.21.2`](#telegraf1212)
-	[`telegraf:1.21.2-alpine`](#telegraf1212-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.19`

```console
$ docker pull telegraf@sha256:11ab5ba49d7a8ed1ba07341343e527d611595dac2deff511d7e86003a8703b84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.19` - linux; amd64

```console
$ docker pull telegraf@sha256:2de0e3240e699c6ace781a9d3b4c519408cb3d334967ef3df3990839b64c830b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119874555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86fab08f9fddb9cd1c8ad99521ebadabfedb68bf1209a87314c600f33fa4c23c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 Jan 2022 11:28:42 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 11:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 27 Jan 2022 11:29:15 GMT
ENV TELEGRAF_VERSION=1.19.3
# Thu, 27 Jan 2022 11:29:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 27 Jan 2022 11:29:21 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 27 Jan 2022 11:29:21 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Thu, 27 Jan 2022 11:29:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jan 2022 11:29:21 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2c7a10ef219c322572998db3b37e08fb7c0a71b5767641e82de694ea2f50a`  
		Last Modified: Thu, 27 Jan 2022 11:30:14 GMT  
		Size: 17.4 MB (17415400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d2ffb6435ae10f04900e1da7a08dd941b27c5e1174abbfc597c77a8e078f8`  
		Last Modified: Thu, 27 Jan 2022 11:30:10 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9947ac50c95836d7f1b47f4560e397c9e98dc752ddb4a06a601db1fbe71181`  
		Last Modified: Thu, 27 Jan 2022 11:30:17 GMT  
		Size: 34.2 MB (34187825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fee0ef996e11c787971eed6599c9e0bccce38f7ea7736be9c5773d309611ce`  
		Last Modified: Thu, 27 Jan 2022 11:30:10 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:dbf951cf1130b7a648bf615bcb4d458b913b55455f4389931aeb9eb1c95ab82c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110245902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034401455f8bfd763177e6eca2a9504b13b5431ff2aed20c95530514f358cb32`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 18:05:01 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 18:05:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 18:05:12 GMT
ENV TELEGRAF_VERSION=1.19.3
# Wed, 22 Dec 2021 18:05:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Dec 2021 18:05:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Dec 2021 18:05:23 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 22 Dec 2021 18:05:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 18:05:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607f3d7f4404cb0dc06799b481c25dde452fc6d23f2bea8b69cdea4043e51b15`  
		Last Modified: Wed, 22 Dec 2021 18:07:16 GMT  
		Size: 16.2 MB (16161072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd5e4e2470e79658cef7e65784eaa20c4e4b5b4a24240bb9b4057d9066947ea`  
		Last Modified: Wed, 22 Dec 2021 18:07:05 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5be178c2e674eb44029864a15818a2514fbd0eeb43f473ee21da138b69572f`  
		Last Modified: Wed, 22 Dec 2021 18:07:26 GMT  
		Size: 31.7 MB (31694539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fc153ed4716d1e086b616794d4672b79ab4c6f6ba87662d906b6ba68fcf6a7`  
		Last Modified: Wed, 22 Dec 2021 18:07:05 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:c837a8d3ca250ed8290af7f833c75ecf3b2168aff6ec1b67ad10c9d8575da454
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114714186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af44fe9756d2aefc50ad001fec2b24e311898bef1030bb01bcdbde6f5423c4f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 20:03:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 20:04:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 20:04:29 GMT
ENV TELEGRAF_VERSION=1.19.3
# Wed, 26 Jan 2022 20:04:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 26 Jan 2022 20:04:39 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 26 Jan 2022 20:04:41 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 26 Jan 2022 20:04:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 20:04:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34ec0624fdce392c92171379a77f7d018e7fac8f2e39c8f6bbb2579cc93de47`  
		Last Modified: Wed, 26 Jan 2022 20:05:40 GMT  
		Size: 17.1 MB (17059033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520feaefcdd19ed3e79b582d65947eb00d949353436959210a4c685ea9bd660b`  
		Last Modified: Wed, 26 Jan 2022 20:05:36 GMT  
		Size: 2.9 KB (2875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a94809ba03eccbf2ce723c9f24f4788605d9138f89d3b72b49da733d60b77a7`  
		Last Modified: Wed, 26 Jan 2022 20:05:42 GMT  
		Size: 31.0 MB (30966516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b386439618cf01e687352650e2870a58beab9f4faf5e72d4bbe59a7eeef517c`  
		Last Modified: Wed, 26 Jan 2022 20:05:36 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19-alpine`

```console
$ docker pull telegraf@sha256:205891b655b4552ee18a8f73a8ba56b3a8e82529d9e3681337f50396d43985fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.19-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:27f0741fe4e358f1dcab0908c35fc85d749a7dec06c14d0dfa26ae3880d8ee90
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40241427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90de7eb4b0f8db88ba670178245f5795dae4b6de18b02240ce1f76b3b952733b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 17 Dec 2021 02:20:31 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 17 Dec 2021 02:20:32 GMT
ENV TELEGRAF_VERSION=1.19.3
# Fri, 17 Dec 2021 02:20:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 17 Dec 2021 02:20:42 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 17 Dec 2021 02:20:43 GMT
COPY file:84034863b49a281750ea7e176a1957ded02179a42503f45931a6770e9517a763 in /entrypoint.sh 
# Fri, 17 Dec 2021 02:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Dec 2021 02:20:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8116ffcf4b23c813aa4315dc15470c986de61b6f13f6a82d80bb928b952193ac`  
		Last Modified: Fri, 17 Dec 2021 02:21:59 GMT  
		Size: 3.4 MB (3371639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b756b34f098dfccf85ef4d349792362c784cee693e1ad5a07835334a8bdf93`  
		Last Modified: Fri, 17 Dec 2021 02:22:05 GMT  
		Size: 34.0 MB (34046360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d809607691ab69c23e71b223f24cc33e3d7e2979d30385f1a3a9285222cfd2d`  
		Last Modified: Fri, 17 Dec 2021 02:21:59 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19.3`

```console
$ docker pull telegraf@sha256:11ab5ba49d7a8ed1ba07341343e527d611595dac2deff511d7e86003a8703b84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.19.3` - linux; amd64

```console
$ docker pull telegraf@sha256:2de0e3240e699c6ace781a9d3b4c519408cb3d334967ef3df3990839b64c830b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119874555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86fab08f9fddb9cd1c8ad99521ebadabfedb68bf1209a87314c600f33fa4c23c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 Jan 2022 11:28:42 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 11:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 27 Jan 2022 11:29:15 GMT
ENV TELEGRAF_VERSION=1.19.3
# Thu, 27 Jan 2022 11:29:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 27 Jan 2022 11:29:21 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 27 Jan 2022 11:29:21 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Thu, 27 Jan 2022 11:29:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jan 2022 11:29:21 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2c7a10ef219c322572998db3b37e08fb7c0a71b5767641e82de694ea2f50a`  
		Last Modified: Thu, 27 Jan 2022 11:30:14 GMT  
		Size: 17.4 MB (17415400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d2ffb6435ae10f04900e1da7a08dd941b27c5e1174abbfc597c77a8e078f8`  
		Last Modified: Thu, 27 Jan 2022 11:30:10 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9947ac50c95836d7f1b47f4560e397c9e98dc752ddb4a06a601db1fbe71181`  
		Last Modified: Thu, 27 Jan 2022 11:30:17 GMT  
		Size: 34.2 MB (34187825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fee0ef996e11c787971eed6599c9e0bccce38f7ea7736be9c5773d309611ce`  
		Last Modified: Thu, 27 Jan 2022 11:30:10 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:dbf951cf1130b7a648bf615bcb4d458b913b55455f4389931aeb9eb1c95ab82c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110245902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034401455f8bfd763177e6eca2a9504b13b5431ff2aed20c95530514f358cb32`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 18:05:01 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 18:05:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 18:05:12 GMT
ENV TELEGRAF_VERSION=1.19.3
# Wed, 22 Dec 2021 18:05:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Dec 2021 18:05:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Dec 2021 18:05:23 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 22 Dec 2021 18:05:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 18:05:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607f3d7f4404cb0dc06799b481c25dde452fc6d23f2bea8b69cdea4043e51b15`  
		Last Modified: Wed, 22 Dec 2021 18:07:16 GMT  
		Size: 16.2 MB (16161072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd5e4e2470e79658cef7e65784eaa20c4e4b5b4a24240bb9b4057d9066947ea`  
		Last Modified: Wed, 22 Dec 2021 18:07:05 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5be178c2e674eb44029864a15818a2514fbd0eeb43f473ee21da138b69572f`  
		Last Modified: Wed, 22 Dec 2021 18:07:26 GMT  
		Size: 31.7 MB (31694539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fc153ed4716d1e086b616794d4672b79ab4c6f6ba87662d906b6ba68fcf6a7`  
		Last Modified: Wed, 22 Dec 2021 18:07:05 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:c837a8d3ca250ed8290af7f833c75ecf3b2168aff6ec1b67ad10c9d8575da454
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114714186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af44fe9756d2aefc50ad001fec2b24e311898bef1030bb01bcdbde6f5423c4f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 20:03:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 20:04:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 20:04:29 GMT
ENV TELEGRAF_VERSION=1.19.3
# Wed, 26 Jan 2022 20:04:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 26 Jan 2022 20:04:39 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 26 Jan 2022 20:04:41 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 26 Jan 2022 20:04:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 20:04:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34ec0624fdce392c92171379a77f7d018e7fac8f2e39c8f6bbb2579cc93de47`  
		Last Modified: Wed, 26 Jan 2022 20:05:40 GMT  
		Size: 17.1 MB (17059033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520feaefcdd19ed3e79b582d65947eb00d949353436959210a4c685ea9bd660b`  
		Last Modified: Wed, 26 Jan 2022 20:05:36 GMT  
		Size: 2.9 KB (2875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a94809ba03eccbf2ce723c9f24f4788605d9138f89d3b72b49da733d60b77a7`  
		Last Modified: Wed, 26 Jan 2022 20:05:42 GMT  
		Size: 31.0 MB (30966516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b386439618cf01e687352650e2870a58beab9f4faf5e72d4bbe59a7eeef517c`  
		Last Modified: Wed, 26 Jan 2022 20:05:36 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19.3-alpine`

```console
$ docker pull telegraf@sha256:205891b655b4552ee18a8f73a8ba56b3a8e82529d9e3681337f50396d43985fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.19.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:27f0741fe4e358f1dcab0908c35fc85d749a7dec06c14d0dfa26ae3880d8ee90
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40241427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90de7eb4b0f8db88ba670178245f5795dae4b6de18b02240ce1f76b3b952733b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 17 Dec 2021 02:20:31 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 17 Dec 2021 02:20:32 GMT
ENV TELEGRAF_VERSION=1.19.3
# Fri, 17 Dec 2021 02:20:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 17 Dec 2021 02:20:42 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 17 Dec 2021 02:20:43 GMT
COPY file:84034863b49a281750ea7e176a1957ded02179a42503f45931a6770e9517a763 in /entrypoint.sh 
# Fri, 17 Dec 2021 02:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Dec 2021 02:20:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8116ffcf4b23c813aa4315dc15470c986de61b6f13f6a82d80bb928b952193ac`  
		Last Modified: Fri, 17 Dec 2021 02:21:59 GMT  
		Size: 3.4 MB (3371639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b756b34f098dfccf85ef4d349792362c784cee693e1ad5a07835334a8bdf93`  
		Last Modified: Fri, 17 Dec 2021 02:22:05 GMT  
		Size: 34.0 MB (34046360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d809607691ab69c23e71b223f24cc33e3d7e2979d30385f1a3a9285222cfd2d`  
		Last Modified: Fri, 17 Dec 2021 02:21:59 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20`

```console
$ docker pull telegraf@sha256:3499a11e5cad4779c6ed6698456f0e0981a1a6f61123cb1d5c14040021085491
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.20` - linux; amd64

```console
$ docker pull telegraf@sha256:f0a8a238b2e2595d3ebd0e3c17704720eb7414dcf05efb4f3058248010d211ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121320407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7afeae39f6dd45887e3337ae718ab17aad32bfec199305734450175dadac8f08`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 Jan 2022 11:28:42 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 11:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 27 Jan 2022 11:29:30 GMT
ENV TELEGRAF_VERSION=1.20.4
# Thu, 27 Jan 2022 11:29:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 27 Jan 2022 11:29:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 27 Jan 2022 11:29:36 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Thu, 27 Jan 2022 11:29:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jan 2022 11:29:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2c7a10ef219c322572998db3b37e08fb7c0a71b5767641e82de694ea2f50a`  
		Last Modified: Thu, 27 Jan 2022 11:30:14 GMT  
		Size: 17.4 MB (17415400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d2ffb6435ae10f04900e1da7a08dd941b27c5e1174abbfc597c77a8e078f8`  
		Last Modified: Thu, 27 Jan 2022 11:30:10 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3fd955de8ce5c7a744d68fcef5a241fa37faa0daabd4d1a6780600a8e145cd`  
		Last Modified: Thu, 27 Jan 2022 11:30:35 GMT  
		Size: 35.6 MB (35633677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5564208a66c3ea434297e1b7d2a3ee2bdfde1a34b762dd71c4c4e0775c77a5ca`  
		Last Modified: Thu, 27 Jan 2022 11:30:28 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:d367028487c8b669fb436a7e308ab46e7f5b8f5d50d90e96635315e9d46682db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111646509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1e5959fd9f3a873e4db4db35e25e79b2b760ff436549cf87e4abbdd107cefcd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 18:05:01 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 18:05:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 18:05:40 GMT
ENV TELEGRAF_VERSION=1.20.4
# Wed, 22 Dec 2021 18:05:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Dec 2021 18:05:53 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Dec 2021 18:05:54 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 22 Dec 2021 18:05:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 18:05:54 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607f3d7f4404cb0dc06799b481c25dde452fc6d23f2bea8b69cdea4043e51b15`  
		Last Modified: Wed, 22 Dec 2021 18:07:16 GMT  
		Size: 16.2 MB (16161072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd5e4e2470e79658cef7e65784eaa20c4e4b5b4a24240bb9b4057d9066947ea`  
		Last Modified: Wed, 22 Dec 2021 18:07:05 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cece7b521c2de3ca3fb3074e280128cd61dd5b24197447df3bdde86979a9c828`  
		Last Modified: Wed, 22 Dec 2021 18:08:03 GMT  
		Size: 33.1 MB (33095147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7de0597b85dd84b01acd78aa63fc098565849ca376e8410ff852f8c6a54d225`  
		Last Modified: Wed, 22 Dec 2021 18:07:41 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a44bd482a69d894358742c137d520c3b381262d224b0abcea2d3246d2276224f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.1 MB (116117309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74998c1cc71b56523b6d935440763dfe200dcb0938d073dcac2b6f3b1911e784`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 20:03:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 20:04:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 20:04:51 GMT
ENV TELEGRAF_VERSION=1.20.4
# Wed, 26 Jan 2022 20:04:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 26 Jan 2022 20:04:56 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 26 Jan 2022 20:04:58 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 26 Jan 2022 20:04:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 20:04:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34ec0624fdce392c92171379a77f7d018e7fac8f2e39c8f6bbb2579cc93de47`  
		Last Modified: Wed, 26 Jan 2022 20:05:40 GMT  
		Size: 17.1 MB (17059033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520feaefcdd19ed3e79b582d65947eb00d949353436959210a4c685ea9bd660b`  
		Last Modified: Wed, 26 Jan 2022 20:05:36 GMT  
		Size: 2.9 KB (2875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5379fd74af03f4f35ac1692412f222d0a5550d6fa671d204e1034ed0d159bc14`  
		Last Modified: Wed, 26 Jan 2022 20:05:58 GMT  
		Size: 32.4 MB (32369639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b788e9b007e8d0809536fba7801365e3d7aa35847ddd91f3ad4e65af9842f761`  
		Last Modified: Wed, 26 Jan 2022 20:05:53 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20-alpine`

```console
$ docker pull telegraf@sha256:c456aa3dce27771929fee5ef056d6d15e9a246a8e7667e91432bcc8d9daacfff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.20-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ae4f8bc4ae97e81ad3321ef9547a17223c1f5360de9ff68b3f86e1a53244406f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41665196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad29bda657eb5e7894bd3adae6fabecaacb27b4a37296a5637ce14256683a30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 17 Dec 2021 02:20:31 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 17 Dec 2021 02:20:54 GMT
ENV TELEGRAF_VERSION=1.20.4
# Fri, 17 Dec 2021 02:21:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 17 Dec 2021 02:21:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 17 Dec 2021 02:21:05 GMT
COPY file:84034863b49a281750ea7e176a1957ded02179a42503f45931a6770e9517a763 in /entrypoint.sh 
# Fri, 17 Dec 2021 02:21:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Dec 2021 02:21:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8116ffcf4b23c813aa4315dc15470c986de61b6f13f6a82d80bb928b952193ac`  
		Last Modified: Fri, 17 Dec 2021 02:21:59 GMT  
		Size: 3.4 MB (3371639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55559b77a85076ea7f0cb2546de89a8f132f252614b893cf7a346563510aae4e`  
		Last Modified: Fri, 17 Dec 2021 02:22:38 GMT  
		Size: 35.5 MB (35470129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656fa61b3541bd9e624ce0a521df6fcd2a6bc725f4d423cb054f712fa98d429f`  
		Last Modified: Fri, 17 Dec 2021 02:22:31 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20.4`

```console
$ docker pull telegraf@sha256:3499a11e5cad4779c6ed6698456f0e0981a1a6f61123cb1d5c14040021085491
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.20.4` - linux; amd64

```console
$ docker pull telegraf@sha256:f0a8a238b2e2595d3ebd0e3c17704720eb7414dcf05efb4f3058248010d211ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121320407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7afeae39f6dd45887e3337ae718ab17aad32bfec199305734450175dadac8f08`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 Jan 2022 11:28:42 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 11:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 27 Jan 2022 11:29:30 GMT
ENV TELEGRAF_VERSION=1.20.4
# Thu, 27 Jan 2022 11:29:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 27 Jan 2022 11:29:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 27 Jan 2022 11:29:36 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Thu, 27 Jan 2022 11:29:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jan 2022 11:29:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2c7a10ef219c322572998db3b37e08fb7c0a71b5767641e82de694ea2f50a`  
		Last Modified: Thu, 27 Jan 2022 11:30:14 GMT  
		Size: 17.4 MB (17415400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d2ffb6435ae10f04900e1da7a08dd941b27c5e1174abbfc597c77a8e078f8`  
		Last Modified: Thu, 27 Jan 2022 11:30:10 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3fd955de8ce5c7a744d68fcef5a241fa37faa0daabd4d1a6780600a8e145cd`  
		Last Modified: Thu, 27 Jan 2022 11:30:35 GMT  
		Size: 35.6 MB (35633677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5564208a66c3ea434297e1b7d2a3ee2bdfde1a34b762dd71c4c4e0775c77a5ca`  
		Last Modified: Thu, 27 Jan 2022 11:30:28 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:d367028487c8b669fb436a7e308ab46e7f5b8f5d50d90e96635315e9d46682db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111646509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1e5959fd9f3a873e4db4db35e25e79b2b760ff436549cf87e4abbdd107cefcd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 18:05:01 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 18:05:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Dec 2021 18:05:40 GMT
ENV TELEGRAF_VERSION=1.20.4
# Wed, 22 Dec 2021 18:05:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Dec 2021 18:05:53 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Dec 2021 18:05:54 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 22 Dec 2021 18:05:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Dec 2021 18:05:54 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607f3d7f4404cb0dc06799b481c25dde452fc6d23f2bea8b69cdea4043e51b15`  
		Last Modified: Wed, 22 Dec 2021 18:07:16 GMT  
		Size: 16.2 MB (16161072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd5e4e2470e79658cef7e65784eaa20c4e4b5b4a24240bb9b4057d9066947ea`  
		Last Modified: Wed, 22 Dec 2021 18:07:05 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cece7b521c2de3ca3fb3074e280128cd61dd5b24197447df3bdde86979a9c828`  
		Last Modified: Wed, 22 Dec 2021 18:08:03 GMT  
		Size: 33.1 MB (33095147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7de0597b85dd84b01acd78aa63fc098565849ca376e8410ff852f8c6a54d225`  
		Last Modified: Wed, 22 Dec 2021 18:07:41 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a44bd482a69d894358742c137d520c3b381262d224b0abcea2d3246d2276224f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.1 MB (116117309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74998c1cc71b56523b6d935440763dfe200dcb0938d073dcac2b6f3b1911e784`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 20:03:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 20:04:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 20:04:51 GMT
ENV TELEGRAF_VERSION=1.20.4
# Wed, 26 Jan 2022 20:04:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 26 Jan 2022 20:04:56 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 26 Jan 2022 20:04:58 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 26 Jan 2022 20:04:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 20:04:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34ec0624fdce392c92171379a77f7d018e7fac8f2e39c8f6bbb2579cc93de47`  
		Last Modified: Wed, 26 Jan 2022 20:05:40 GMT  
		Size: 17.1 MB (17059033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520feaefcdd19ed3e79b582d65947eb00d949353436959210a4c685ea9bd660b`  
		Last Modified: Wed, 26 Jan 2022 20:05:36 GMT  
		Size: 2.9 KB (2875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5379fd74af03f4f35ac1692412f222d0a5550d6fa671d204e1034ed0d159bc14`  
		Last Modified: Wed, 26 Jan 2022 20:05:58 GMT  
		Size: 32.4 MB (32369639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b788e9b007e8d0809536fba7801365e3d7aa35847ddd91f3ad4e65af9842f761`  
		Last Modified: Wed, 26 Jan 2022 20:05:53 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20.4-alpine`

```console
$ docker pull telegraf@sha256:c456aa3dce27771929fee5ef056d6d15e9a246a8e7667e91432bcc8d9daacfff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.20.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ae4f8bc4ae97e81ad3321ef9547a17223c1f5360de9ff68b3f86e1a53244406f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41665196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad29bda657eb5e7894bd3adae6fabecaacb27b4a37296a5637ce14256683a30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 17 Dec 2021 02:20:31 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 17 Dec 2021 02:20:54 GMT
ENV TELEGRAF_VERSION=1.20.4
# Fri, 17 Dec 2021 02:21:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 17 Dec 2021 02:21:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 17 Dec 2021 02:21:05 GMT
COPY file:84034863b49a281750ea7e176a1957ded02179a42503f45931a6770e9517a763 in /entrypoint.sh 
# Fri, 17 Dec 2021 02:21:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Dec 2021 02:21:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8116ffcf4b23c813aa4315dc15470c986de61b6f13f6a82d80bb928b952193ac`  
		Last Modified: Fri, 17 Dec 2021 02:21:59 GMT  
		Size: 3.4 MB (3371639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55559b77a85076ea7f0cb2546de89a8f132f252614b893cf7a346563510aae4e`  
		Last Modified: Fri, 17 Dec 2021 02:22:38 GMT  
		Size: 35.5 MB (35470129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656fa61b3541bd9e624ce0a521df6fcd2a6bc725f4d423cb054f712fa98d429f`  
		Last Modified: Fri, 17 Dec 2021 02:22:31 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21`

```console
$ docker pull telegraf@sha256:38d789523a0c960f77d564b997b53378e508d4c34338a0a7e586bc32cf24675c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.21` - linux; amd64

```console
$ docker pull telegraf@sha256:e1c81bcb6d24903fb4e6cbb524861096aa36b25c5ff82f58aa1ff13f24b3c510
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122088989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630d6edf6e4fbfa62eb4ba24fa6ccb21311936416a634a9b586201ea8ac85120`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 Jan 2022 11:28:42 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 11:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 27 Jan 2022 11:29:41 GMT
ENV TELEGRAF_VERSION=1.21.2
# Thu, 27 Jan 2022 11:29:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 27 Jan 2022 11:29:47 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 27 Jan 2022 11:29:47 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Thu, 27 Jan 2022 11:29:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jan 2022 11:29:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2c7a10ef219c322572998db3b37e08fb7c0a71b5767641e82de694ea2f50a`  
		Last Modified: Thu, 27 Jan 2022 11:30:14 GMT  
		Size: 17.4 MB (17415400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d2ffb6435ae10f04900e1da7a08dd941b27c5e1174abbfc597c77a8e078f8`  
		Last Modified: Thu, 27 Jan 2022 11:30:10 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe30861de9a72b92a45baa97ac1754b3ebf3c3c0c31895605a8a6909d05fcfe`  
		Last Modified: Thu, 27 Jan 2022 11:30:52 GMT  
		Size: 36.4 MB (36402259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93455755b871f26bd429ad71cc614fa2ca934dbd2410ee7c1094bbcf40b2e686`  
		Last Modified: Thu, 27 Jan 2022 11:30:45 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c64a796754527940aa16ec69b304014487a344b8a1903981629e1a695097755d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112303821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38108ae4f8a16556619ed2ff7aa1b4630dba9b0723cb98ac2881ab2351a6cf2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 18:05:01 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 18:05:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Jan 2022 19:58:29 GMT
ENV TELEGRAF_VERSION=1.21.2
# Wed, 05 Jan 2022 19:58:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 05 Jan 2022 19:58:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 05 Jan 2022 19:58:42 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 05 Jan 2022 19:58:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jan 2022 19:58:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607f3d7f4404cb0dc06799b481c25dde452fc6d23f2bea8b69cdea4043e51b15`  
		Last Modified: Wed, 22 Dec 2021 18:07:16 GMT  
		Size: 16.2 MB (16161072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd5e4e2470e79658cef7e65784eaa20c4e4b5b4a24240bb9b4057d9066947ea`  
		Last Modified: Wed, 22 Dec 2021 18:07:05 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f14aa6436095875eef055bca633575b10cf6f0107c2c50cd8f996965245af93`  
		Last Modified: Wed, 05 Jan 2022 19:59:55 GMT  
		Size: 33.8 MB (33752459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd50a26b965184e3fa25457d318b0fd44504880085c76ba55500c1614bc5b8ae`  
		Last Modified: Wed, 05 Jan 2022 19:59:31 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:96e416fca6c247244a48bb35aa19ac77a772536405be101b9708c9691a616bf3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116775561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7e05be85c1200a070dd12c0a4ae7a2f64a7bbc9334bb4ee91b877d73b0a4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 20:03:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 20:04:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 20:05:05 GMT
ENV TELEGRAF_VERSION=1.21.2
# Wed, 26 Jan 2022 20:05:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 26 Jan 2022 20:05:11 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 26 Jan 2022 20:05:13 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 26 Jan 2022 20:05:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 20:05:14 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34ec0624fdce392c92171379a77f7d018e7fac8f2e39c8f6bbb2579cc93de47`  
		Last Modified: Wed, 26 Jan 2022 20:05:40 GMT  
		Size: 17.1 MB (17059033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520feaefcdd19ed3e79b582d65947eb00d949353436959210a4c685ea9bd660b`  
		Last Modified: Wed, 26 Jan 2022 20:05:36 GMT  
		Size: 2.9 KB (2875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d44ca63f7c7c2de2ca79a29f286f52c640f52b7e103f121afc224921b779c18`  
		Last Modified: Wed, 26 Jan 2022 20:06:17 GMT  
		Size: 33.0 MB (33027889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22adfe43dff7fe8f5fa544c1a836152222b7b1874dec3ec030c57c6327fa063d`  
		Last Modified: Wed, 26 Jan 2022 20:06:10 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21-alpine`

```console
$ docker pull telegraf@sha256:89344ae0b98954194ba3e9d21100f979798ef41698b4b1ee0a2f7a64b31e0cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.21-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:2005f8a5972be4b1259735cb2890b5b321c70a9fea671fc2d856a4aeb7ced2a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42440729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c105adf7541cfb62e32c299b8adf87bfb2ff9f213356df20407909bc954254d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 17 Dec 2021 02:20:31 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 05 Jan 2022 20:20:15 GMT
ENV TELEGRAF_VERSION=1.21.2
# Wed, 05 Jan 2022 20:20:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 05 Jan 2022 20:20:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 05 Jan 2022 20:20:27 GMT
COPY file:84034863b49a281750ea7e176a1957ded02179a42503f45931a6770e9517a763 in /entrypoint.sh 
# Wed, 05 Jan 2022 20:20:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jan 2022 20:20:27 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8116ffcf4b23c813aa4315dc15470c986de61b6f13f6a82d80bb928b952193ac`  
		Last Modified: Fri, 17 Dec 2021 02:21:59 GMT  
		Size: 3.4 MB (3371639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cbe132eb0f2210fedf8a29048a735ea5cfa9749cb7edef2a28e6acc822083d`  
		Last Modified: Wed, 05 Jan 2022 20:21:15 GMT  
		Size: 36.2 MB (36245663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a24ac945d8b53b29d49759fa78eb0a765f8786430a946800318037266e7fead`  
		Last Modified: Wed, 05 Jan 2022 20:21:08 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21.2`

```console
$ docker pull telegraf@sha256:38d789523a0c960f77d564b997b53378e508d4c34338a0a7e586bc32cf24675c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.21.2` - linux; amd64

```console
$ docker pull telegraf@sha256:e1c81bcb6d24903fb4e6cbb524861096aa36b25c5ff82f58aa1ff13f24b3c510
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122088989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630d6edf6e4fbfa62eb4ba24fa6ccb21311936416a634a9b586201ea8ac85120`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 Jan 2022 11:28:42 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 11:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 27 Jan 2022 11:29:41 GMT
ENV TELEGRAF_VERSION=1.21.2
# Thu, 27 Jan 2022 11:29:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 27 Jan 2022 11:29:47 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 27 Jan 2022 11:29:47 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Thu, 27 Jan 2022 11:29:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jan 2022 11:29:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2c7a10ef219c322572998db3b37e08fb7c0a71b5767641e82de694ea2f50a`  
		Last Modified: Thu, 27 Jan 2022 11:30:14 GMT  
		Size: 17.4 MB (17415400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d2ffb6435ae10f04900e1da7a08dd941b27c5e1174abbfc597c77a8e078f8`  
		Last Modified: Thu, 27 Jan 2022 11:30:10 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe30861de9a72b92a45baa97ac1754b3ebf3c3c0c31895605a8a6909d05fcfe`  
		Last Modified: Thu, 27 Jan 2022 11:30:52 GMT  
		Size: 36.4 MB (36402259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93455755b871f26bd429ad71cc614fa2ca934dbd2410ee7c1094bbcf40b2e686`  
		Last Modified: Thu, 27 Jan 2022 11:30:45 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21.2` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c64a796754527940aa16ec69b304014487a344b8a1903981629e1a695097755d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112303821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38108ae4f8a16556619ed2ff7aa1b4630dba9b0723cb98ac2881ab2351a6cf2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 18:05:01 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 18:05:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Jan 2022 19:58:29 GMT
ENV TELEGRAF_VERSION=1.21.2
# Wed, 05 Jan 2022 19:58:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 05 Jan 2022 19:58:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 05 Jan 2022 19:58:42 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 05 Jan 2022 19:58:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jan 2022 19:58:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607f3d7f4404cb0dc06799b481c25dde452fc6d23f2bea8b69cdea4043e51b15`  
		Last Modified: Wed, 22 Dec 2021 18:07:16 GMT  
		Size: 16.2 MB (16161072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd5e4e2470e79658cef7e65784eaa20c4e4b5b4a24240bb9b4057d9066947ea`  
		Last Modified: Wed, 22 Dec 2021 18:07:05 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f14aa6436095875eef055bca633575b10cf6f0107c2c50cd8f996965245af93`  
		Last Modified: Wed, 05 Jan 2022 19:59:55 GMT  
		Size: 33.8 MB (33752459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd50a26b965184e3fa25457d318b0fd44504880085c76ba55500c1614bc5b8ae`  
		Last Modified: Wed, 05 Jan 2022 19:59:31 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21.2` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:96e416fca6c247244a48bb35aa19ac77a772536405be101b9708c9691a616bf3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116775561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7e05be85c1200a070dd12c0a4ae7a2f64a7bbc9334bb4ee91b877d73b0a4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 20:03:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 20:04:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 20:05:05 GMT
ENV TELEGRAF_VERSION=1.21.2
# Wed, 26 Jan 2022 20:05:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 26 Jan 2022 20:05:11 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 26 Jan 2022 20:05:13 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 26 Jan 2022 20:05:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 20:05:14 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34ec0624fdce392c92171379a77f7d018e7fac8f2e39c8f6bbb2579cc93de47`  
		Last Modified: Wed, 26 Jan 2022 20:05:40 GMT  
		Size: 17.1 MB (17059033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520feaefcdd19ed3e79b582d65947eb00d949353436959210a4c685ea9bd660b`  
		Last Modified: Wed, 26 Jan 2022 20:05:36 GMT  
		Size: 2.9 KB (2875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d44ca63f7c7c2de2ca79a29f286f52c640f52b7e103f121afc224921b779c18`  
		Last Modified: Wed, 26 Jan 2022 20:06:17 GMT  
		Size: 33.0 MB (33027889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22adfe43dff7fe8f5fa544c1a836152222b7b1874dec3ec030c57c6327fa063d`  
		Last Modified: Wed, 26 Jan 2022 20:06:10 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21.2-alpine`

```console
$ docker pull telegraf@sha256:89344ae0b98954194ba3e9d21100f979798ef41698b4b1ee0a2f7a64b31e0cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.21.2-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:2005f8a5972be4b1259735cb2890b5b321c70a9fea671fc2d856a4aeb7ced2a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42440729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c105adf7541cfb62e32c299b8adf87bfb2ff9f213356df20407909bc954254d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 17 Dec 2021 02:20:31 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 05 Jan 2022 20:20:15 GMT
ENV TELEGRAF_VERSION=1.21.2
# Wed, 05 Jan 2022 20:20:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 05 Jan 2022 20:20:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 05 Jan 2022 20:20:27 GMT
COPY file:84034863b49a281750ea7e176a1957ded02179a42503f45931a6770e9517a763 in /entrypoint.sh 
# Wed, 05 Jan 2022 20:20:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jan 2022 20:20:27 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8116ffcf4b23c813aa4315dc15470c986de61b6f13f6a82d80bb928b952193ac`  
		Last Modified: Fri, 17 Dec 2021 02:21:59 GMT  
		Size: 3.4 MB (3371639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cbe132eb0f2210fedf8a29048a735ea5cfa9749cb7edef2a28e6acc822083d`  
		Last Modified: Wed, 05 Jan 2022 20:21:15 GMT  
		Size: 36.2 MB (36245663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a24ac945d8b53b29d49759fa78eb0a765f8786430a946800318037266e7fead`  
		Last Modified: Wed, 05 Jan 2022 20:21:08 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:89344ae0b98954194ba3e9d21100f979798ef41698b4b1ee0a2f7a64b31e0cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:2005f8a5972be4b1259735cb2890b5b321c70a9fea671fc2d856a4aeb7ced2a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42440729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c105adf7541cfb62e32c299b8adf87bfb2ff9f213356df20407909bc954254d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:55:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 17 Dec 2021 02:20:31 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 05 Jan 2022 20:20:15 GMT
ENV TELEGRAF_VERSION=1.21.2
# Wed, 05 Jan 2022 20:20:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 05 Jan 2022 20:20:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 05 Jan 2022 20:20:27 GMT
COPY file:84034863b49a281750ea7e176a1957ded02179a42503f45931a6770e9517a763 in /entrypoint.sh 
# Wed, 05 Jan 2022 20:20:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jan 2022 20:20:27 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f199b43e46c5dfea12dfa8b92b7811e74b4d3812ff99c8368e4d2af803e7`  
		Last Modified: Fri, 12 Nov 2021 21:56:45 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8116ffcf4b23c813aa4315dc15470c986de61b6f13f6a82d80bb928b952193ac`  
		Last Modified: Fri, 17 Dec 2021 02:21:59 GMT  
		Size: 3.4 MB (3371639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cbe132eb0f2210fedf8a29048a735ea5cfa9749cb7edef2a28e6acc822083d`  
		Last Modified: Wed, 05 Jan 2022 20:21:15 GMT  
		Size: 36.2 MB (36245663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a24ac945d8b53b29d49759fa78eb0a765f8786430a946800318037266e7fead`  
		Last Modified: Wed, 05 Jan 2022 20:21:08 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:38d789523a0c960f77d564b997b53378e508d4c34338a0a7e586bc32cf24675c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:e1c81bcb6d24903fb4e6cbb524861096aa36b25c5ff82f58aa1ff13f24b3c510
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122088989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630d6edf6e4fbfa62eb4ba24fa6ccb21311936416a634a9b586201ea8ac85120`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 Jan 2022 11:28:42 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 11:29:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 27 Jan 2022 11:29:41 GMT
ENV TELEGRAF_VERSION=1.21.2
# Thu, 27 Jan 2022 11:29:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 27 Jan 2022 11:29:47 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 27 Jan 2022 11:29:47 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Thu, 27 Jan 2022 11:29:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Jan 2022 11:29:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2c7a10ef219c322572998db3b37e08fb7c0a71b5767641e82de694ea2f50a`  
		Last Modified: Thu, 27 Jan 2022 11:30:14 GMT  
		Size: 17.4 MB (17415400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d2ffb6435ae10f04900e1da7a08dd941b27c5e1174abbfc597c77a8e078f8`  
		Last Modified: Thu, 27 Jan 2022 11:30:10 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe30861de9a72b92a45baa97ac1754b3ebf3c3c0c31895605a8a6909d05fcfe`  
		Last Modified: Thu, 27 Jan 2022 11:30:52 GMT  
		Size: 36.4 MB (36402259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93455755b871f26bd429ad71cc614fa2ca934dbd2410ee7c1094bbcf40b2e686`  
		Last Modified: Thu, 27 Jan 2022 11:30:45 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c64a796754527940aa16ec69b304014487a344b8a1903981629e1a695097755d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112303821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38108ae4f8a16556619ed2ff7aa1b4630dba9b0723cb98ac2881ab2351a6cf2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Dec 2021 18:05:01 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 18:05:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Jan 2022 19:58:29 GMT
ENV TELEGRAF_VERSION=1.21.2
# Wed, 05 Jan 2022 19:58:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 05 Jan 2022 19:58:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 05 Jan 2022 19:58:42 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 05 Jan 2022 19:58:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jan 2022 19:58:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607f3d7f4404cb0dc06799b481c25dde452fc6d23f2bea8b69cdea4043e51b15`  
		Last Modified: Wed, 22 Dec 2021 18:07:16 GMT  
		Size: 16.2 MB (16161072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd5e4e2470e79658cef7e65784eaa20c4e4b5b4a24240bb9b4057d9066947ea`  
		Last Modified: Wed, 22 Dec 2021 18:07:05 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f14aa6436095875eef055bca633575b10cf6f0107c2c50cd8f996965245af93`  
		Last Modified: Wed, 05 Jan 2022 19:59:55 GMT  
		Size: 33.8 MB (33752459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd50a26b965184e3fa25457d318b0fd44504880085c76ba55500c1614bc5b8ae`  
		Last Modified: Wed, 05 Jan 2022 19:59:31 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:96e416fca6c247244a48bb35aa19ac77a772536405be101b9708c9691a616bf3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116775561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7e05be85c1200a070dd12c0a4ae7a2f64a7bbc9334bb4ee91b877d73b0a4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 20:03:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 20:04:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 26 Jan 2022 20:05:05 GMT
ENV TELEGRAF_VERSION=1.21.2
# Wed, 26 Jan 2022 20:05:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 26 Jan 2022 20:05:11 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 26 Jan 2022 20:05:13 GMT
COPY file:0ef29f50667596ea844399ecdebe09cc173891df00d5bf1ad2403422b2b2db39 in /entrypoint.sh 
# Wed, 26 Jan 2022 20:05:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Jan 2022 20:05:14 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34ec0624fdce392c92171379a77f7d018e7fac8f2e39c8f6bbb2579cc93de47`  
		Last Modified: Wed, 26 Jan 2022 20:05:40 GMT  
		Size: 17.1 MB (17059033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520feaefcdd19ed3e79b582d65947eb00d949353436959210a4c685ea9bd660b`  
		Last Modified: Wed, 26 Jan 2022 20:05:36 GMT  
		Size: 2.9 KB (2875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d44ca63f7c7c2de2ca79a29f286f52c640f52b7e103f121afc224921b779c18`  
		Last Modified: Wed, 26 Jan 2022 20:06:17 GMT  
		Size: 33.0 MB (33027889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22adfe43dff7fe8f5fa544c1a836152222b7b1874dec3ec030c57c6327fa063d`  
		Last Modified: Wed, 26 Jan 2022 20:06:10 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
