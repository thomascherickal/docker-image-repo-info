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
-	[`telegraf:1.24.4`](#telegraf1244)
-	[`telegraf:1.24.4-alpine`](#telegraf1244-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.22`

```console
$ docker pull telegraf@sha256:b6746734234b98a6f63c89f199b455ebabe14d9f26f8faf817cc341ae49aea0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.22` - linux; amd64

```console
$ docker pull telegraf@sha256:3b89defc8ee32cc10a31ef53539b92ded5c4177205ffdb22b55f253efc92391a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.3 MB (130343293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b578a132fb7c5731506c5afe7a9694c96424f5af2292092c43bf802bb541e191`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 00:11:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:11:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 00:11:25 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 16 Nov 2022 00:11:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Nov 2022 00:11:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Nov 2022 00:11:29 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Nov 2022 00:11:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 00:11:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e470c46ca228512e8b187d5fe846c93c976f72bcd54b96c870855e69877e02a`  
		Last Modified: Wed, 16 Nov 2022 00:12:11 GMT  
		Size: 18.8 MB (18760393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e66d445937565d68a5f8be7023f158f0d5cdcc333af3c70c5124dfda50802`  
		Last Modified: Wed, 16 Nov 2022 00:12:07 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca1275b1586a9c86899e01025d0f711c58a9258b0dcdeee454eef4a9a6eeedc`  
		Last Modified: Wed, 16 Nov 2022 00:12:14 GMT  
		Size: 40.5 MB (40498769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3326c2c351e3b695d656eae1d861686840f5f0c73f64391360207defbbbb6686`  
		Last Modified: Wed, 16 Nov 2022 00:12:07 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:003cddf83cec6d33071f7098137de539de9e2614132a53d1b7ad3badaafb73ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120745628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd7ea5cf16fbd044355c64f458b59a6fbb3592ead2e56626e8246db8c21eede1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 19:59:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:59:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 19:59:45 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 15 Nov 2022 19:59:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 15 Nov 2022 19:59:50 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 15 Nov 2022 19:59:50 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 15 Nov 2022 19:59:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 19:59:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a09dc2ad5d15708c33af827818a7920afcc85c714ad1e377cbce9a7f0f286f`  
		Last Modified: Tue, 15 Nov 2022 20:00:53 GMT  
		Size: 17.5 MB (17463030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef14a56e15e24420180503745c2e9604ad396f53801ed3f4ab7d28ab86318d28`  
		Last Modified: Tue, 15 Nov 2022 20:00:49 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1b8ad183b9694a7505f8925edfd5c60607e02621f93d92c4e3bdee68421c42`  
		Last Modified: Tue, 15 Nov 2022 20:00:57 GMT  
		Size: 37.9 MB (37921678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f19cd31a1e4f9ff9007fa75976b324c02b652bd87f5dc9c2d7826f1522522b0`  
		Last Modified: Tue, 15 Nov 2022 20:00:49 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:380908caf38ce028189ae05332df4f437c24df967e5fad2bb879cf95e5134f6b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125139203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3ab629262dc93c9dac4b3f324517188fb17a036b5ca1d5272d53ae48a1d048`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:29:30 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 22:29:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 22:29:31 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 15 Nov 2022 22:29:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 15 Nov 2022 22:29:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 15 Nov 2022 22:29:36 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 15 Nov 2022 22:29:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:29:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dacffc09706b3a7717b5dc24201989950028c356bbc321c851f61ffbff3917d`  
		Last Modified: Tue, 15 Nov 2022 22:30:09 GMT  
		Size: 18.6 MB (18599319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a956f65aaa93f41831e7e91c5c19af3d879ae834730e3ec7385859fde285337`  
		Last Modified: Tue, 15 Nov 2022 22:30:06 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ffcf770fc99ade1fd9033a5696ac3731aef24ed5c897b5662f6d99fae3a145`  
		Last Modified: Tue, 15 Nov 2022 22:30:10 GMT  
		Size: 36.8 MB (36811199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdc5b1d405e2100eaebab48507c4054bf0dd7dfec09733fb8ac3987dc0c039f`  
		Last Modified: Tue, 15 Nov 2022 22:30:06 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22-alpine`

```console
$ docker pull telegraf@sha256:99e5bd30bbae2e2b162f520c9c6093c4fae49702e0eac90d978562c3be0be1ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.22-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:76d7cdfba581ed5f830b811cb042e37f2f620e685d38792219d05dd479472574
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46455648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e381325e9726ae4bfaefc67c9d2f5a16a57148325e6863fc5345b1dc66b317`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Sat, 12 Nov 2022 10:02:29 GMT
ENV TELEGRAF_VERSION=1.22.4
# Sat, 12 Nov 2022 10:02:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Sat, 12 Nov 2022 10:02:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 12 Nov 2022 10:02:36 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Sat, 12 Nov 2022 10:02:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 10:02:37 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d5e4b4e27929ea8353ce35e1f88bab2b13cb958f9a9bc13ac6d453a86c5c1`  
		Last Modified: Sat, 12 Nov 2022 10:03:33 GMT  
		Size: 40.4 MB (40350707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649531614e809567a4674e4427415e457c880b210e5853af0804846a083df593`  
		Last Modified: Sat, 12 Nov 2022 10:03:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22.4`

```console
$ docker pull telegraf@sha256:b6746734234b98a6f63c89f199b455ebabe14d9f26f8faf817cc341ae49aea0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.22.4` - linux; amd64

```console
$ docker pull telegraf@sha256:3b89defc8ee32cc10a31ef53539b92ded5c4177205ffdb22b55f253efc92391a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.3 MB (130343293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b578a132fb7c5731506c5afe7a9694c96424f5af2292092c43bf802bb541e191`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 00:11:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:11:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 00:11:25 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 16 Nov 2022 00:11:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Nov 2022 00:11:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Nov 2022 00:11:29 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Nov 2022 00:11:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 00:11:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e470c46ca228512e8b187d5fe846c93c976f72bcd54b96c870855e69877e02a`  
		Last Modified: Wed, 16 Nov 2022 00:12:11 GMT  
		Size: 18.8 MB (18760393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e66d445937565d68a5f8be7023f158f0d5cdcc333af3c70c5124dfda50802`  
		Last Modified: Wed, 16 Nov 2022 00:12:07 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca1275b1586a9c86899e01025d0f711c58a9258b0dcdeee454eef4a9a6eeedc`  
		Last Modified: Wed, 16 Nov 2022 00:12:14 GMT  
		Size: 40.5 MB (40498769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3326c2c351e3b695d656eae1d861686840f5f0c73f64391360207defbbbb6686`  
		Last Modified: Wed, 16 Nov 2022 00:12:07 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:003cddf83cec6d33071f7098137de539de9e2614132a53d1b7ad3badaafb73ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120745628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd7ea5cf16fbd044355c64f458b59a6fbb3592ead2e56626e8246db8c21eede1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 19:59:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:59:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 19:59:45 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 15 Nov 2022 19:59:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 15 Nov 2022 19:59:50 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 15 Nov 2022 19:59:50 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 15 Nov 2022 19:59:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 19:59:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a09dc2ad5d15708c33af827818a7920afcc85c714ad1e377cbce9a7f0f286f`  
		Last Modified: Tue, 15 Nov 2022 20:00:53 GMT  
		Size: 17.5 MB (17463030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef14a56e15e24420180503745c2e9604ad396f53801ed3f4ab7d28ab86318d28`  
		Last Modified: Tue, 15 Nov 2022 20:00:49 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1b8ad183b9694a7505f8925edfd5c60607e02621f93d92c4e3bdee68421c42`  
		Last Modified: Tue, 15 Nov 2022 20:00:57 GMT  
		Size: 37.9 MB (37921678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f19cd31a1e4f9ff9007fa75976b324c02b652bd87f5dc9c2d7826f1522522b0`  
		Last Modified: Tue, 15 Nov 2022 20:00:49 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:380908caf38ce028189ae05332df4f437c24df967e5fad2bb879cf95e5134f6b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125139203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3ab629262dc93c9dac4b3f324517188fb17a036b5ca1d5272d53ae48a1d048`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:29:30 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 22:29:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 22:29:31 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 15 Nov 2022 22:29:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 15 Nov 2022 22:29:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 15 Nov 2022 22:29:36 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 15 Nov 2022 22:29:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:29:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dacffc09706b3a7717b5dc24201989950028c356bbc321c851f61ffbff3917d`  
		Last Modified: Tue, 15 Nov 2022 22:30:09 GMT  
		Size: 18.6 MB (18599319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a956f65aaa93f41831e7e91c5c19af3d879ae834730e3ec7385859fde285337`  
		Last Modified: Tue, 15 Nov 2022 22:30:06 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ffcf770fc99ade1fd9033a5696ac3731aef24ed5c897b5662f6d99fae3a145`  
		Last Modified: Tue, 15 Nov 2022 22:30:10 GMT  
		Size: 36.8 MB (36811199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdc5b1d405e2100eaebab48507c4054bf0dd7dfec09733fb8ac3987dc0c039f`  
		Last Modified: Tue, 15 Nov 2022 22:30:06 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22.4-alpine`

```console
$ docker pull telegraf@sha256:99e5bd30bbae2e2b162f520c9c6093c4fae49702e0eac90d978562c3be0be1ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.22.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:76d7cdfba581ed5f830b811cb042e37f2f620e685d38792219d05dd479472574
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46455648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e381325e9726ae4bfaefc67c9d2f5a16a57148325e6863fc5345b1dc66b317`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Sat, 12 Nov 2022 10:02:29 GMT
ENV TELEGRAF_VERSION=1.22.4
# Sat, 12 Nov 2022 10:02:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Sat, 12 Nov 2022 10:02:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 12 Nov 2022 10:02:36 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Sat, 12 Nov 2022 10:02:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 10:02:37 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d5e4b4e27929ea8353ce35e1f88bab2b13cb958f9a9bc13ac6d453a86c5c1`  
		Last Modified: Sat, 12 Nov 2022 10:03:33 GMT  
		Size: 40.4 MB (40350707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649531614e809567a4674e4427415e457c880b210e5853af0804846a083df593`  
		Last Modified: Sat, 12 Nov 2022 10:03:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23`

```console
$ docker pull telegraf@sha256:740c7e132e08d3061ee60858ddd1e84c82fb5039de976f6e5263e90a0a5b433e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23` - linux; amd64

```console
$ docker pull telegraf@sha256:edd06a36cb2ed4e3be16ec314118e38d3e941e0b0cc33c5d484c7e10269b7c29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131693758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ad2b196197068ba4ee36f7dffac80e82705c8ad90e2aab2a172d5b279efb67`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 00:11:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:11:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 00:11:34 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 16 Nov 2022 00:11:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Nov 2022 00:11:38 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Nov 2022 00:11:38 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Nov 2022 00:11:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 00:11:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e470c46ca228512e8b187d5fe846c93c976f72bcd54b96c870855e69877e02a`  
		Last Modified: Wed, 16 Nov 2022 00:12:11 GMT  
		Size: 18.8 MB (18760393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e66d445937565d68a5f8be7023f158f0d5cdcc333af3c70c5124dfda50802`  
		Last Modified: Wed, 16 Nov 2022 00:12:07 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52869644ddd23d79ab9f23dac586467f42bb025079d39669f1f1117205e54e1`  
		Last Modified: Wed, 16 Nov 2022 00:12:31 GMT  
		Size: 41.8 MB (41849237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b31e3312ab583b76dccf0bd96607b40c34e12f96bc6bf743799760084c00395`  
		Last Modified: Wed, 16 Nov 2022 00:12:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:1846989295399612ea7efe28bd79a981e5a73d1cabc44a9bb1535f16525b7dd7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121930505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88b6bd98fb53404d3a55b9cf2d6885b9848c4c8e9834df8c3a25d987c5e1a40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 19:59:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:59:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 19:59:58 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 15 Nov 2022 20:00:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 15 Nov 2022 20:00:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 15 Nov 2022 20:00:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 15 Nov 2022 20:00:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 20:00:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a09dc2ad5d15708c33af827818a7920afcc85c714ad1e377cbce9a7f0f286f`  
		Last Modified: Tue, 15 Nov 2022 20:00:53 GMT  
		Size: 17.5 MB (17463030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef14a56e15e24420180503745c2e9604ad396f53801ed3f4ab7d28ab86318d28`  
		Last Modified: Tue, 15 Nov 2022 20:00:49 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d44e76c2066051aad83e5c1de3a4cb624e67e65354c69a5d9b3e2bc7a6c55cb`  
		Last Modified: Tue, 15 Nov 2022 20:01:15 GMT  
		Size: 39.1 MB (39106556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605d06414bd46ad40d5f38ced24f3ba0da96a21ce751c1a4964ba2d823d61113`  
		Last Modified: Tue, 15 Nov 2022 20:01:08 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:1528cd7750f219dda0d4f73c98162aa645db7e28828fbfb81ec8fd3c7a30964b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126359295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a916e0a6e6ba0de10285c81d3bce51851d93bc7fc7b7956d79f485948b7d2bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:29:30 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 22:29:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 22:29:40 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 15 Nov 2022 22:29:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 15 Nov 2022 22:29:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 15 Nov 2022 22:29:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 15 Nov 2022 22:29:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:29:44 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dacffc09706b3a7717b5dc24201989950028c356bbc321c851f61ffbff3917d`  
		Last Modified: Tue, 15 Nov 2022 22:30:09 GMT  
		Size: 18.6 MB (18599319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a956f65aaa93f41831e7e91c5c19af3d879ae834730e3ec7385859fde285337`  
		Last Modified: Tue, 15 Nov 2022 22:30:06 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab5737119a2be66c56be7207ccb91bd7644e311086ec8a75bc3ca0b479cbb10`  
		Last Modified: Tue, 15 Nov 2022 22:30:23 GMT  
		Size: 38.0 MB (38031292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911494be15187e3b9407fd23c5ade35d63c65c2e1c881e7ea6ae3a07fefde92a`  
		Last Modified: Tue, 15 Nov 2022 22:30:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23-alpine`

```console
$ docker pull telegraf@sha256:deada02a4669f60913770b54e538e7c4ef1f3596b69425a1ae17fec155050d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:acca0f662ea434da10739c21ee6c94a3af210baab442528013e20b251649a9ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47790772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cb5b879e6101df5e177d87eb1ebf9b5da0c90fab88d3a03479bf6b075bda2ae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Sat, 12 Nov 2022 10:02:41 GMT
ENV TELEGRAF_VERSION=1.23.4
# Sat, 12 Nov 2022 10:02:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Sat, 12 Nov 2022 10:02:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 12 Nov 2022 10:02:49 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Sat, 12 Nov 2022 10:02:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 10:02:49 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e702c89f92384b863c431a1780fe1eb6cb2051d840892639c41ab668017ae0`  
		Last Modified: Sat, 12 Nov 2022 10:03:50 GMT  
		Size: 41.7 MB (41685831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d62792d26ded35216d918492be7c49a9d8bff2da01169e4a3f362fa409cb365`  
		Last Modified: Sat, 12 Nov 2022 10:03:43 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.4`

```console
$ docker pull telegraf@sha256:740c7e132e08d3061ee60858ddd1e84c82fb5039de976f6e5263e90a0a5b433e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23.4` - linux; amd64

```console
$ docker pull telegraf@sha256:edd06a36cb2ed4e3be16ec314118e38d3e941e0b0cc33c5d484c7e10269b7c29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131693758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ad2b196197068ba4ee36f7dffac80e82705c8ad90e2aab2a172d5b279efb67`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 00:11:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:11:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Nov 2022 00:11:34 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 16 Nov 2022 00:11:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Nov 2022 00:11:38 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Nov 2022 00:11:38 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Nov 2022 00:11:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Nov 2022 00:11:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e470c46ca228512e8b187d5fe846c93c976f72bcd54b96c870855e69877e02a`  
		Last Modified: Wed, 16 Nov 2022 00:12:11 GMT  
		Size: 18.8 MB (18760393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e66d445937565d68a5f8be7023f158f0d5cdcc333af3c70c5124dfda50802`  
		Last Modified: Wed, 16 Nov 2022 00:12:07 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52869644ddd23d79ab9f23dac586467f42bb025079d39669f1f1117205e54e1`  
		Last Modified: Wed, 16 Nov 2022 00:12:31 GMT  
		Size: 41.8 MB (41849237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b31e3312ab583b76dccf0bd96607b40c34e12f96bc6bf743799760084c00395`  
		Last Modified: Wed, 16 Nov 2022 00:12:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:1846989295399612ea7efe28bd79a981e5a73d1cabc44a9bb1535f16525b7dd7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121930505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88b6bd98fb53404d3a55b9cf2d6885b9848c4c8e9834df8c3a25d987c5e1a40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 19:59:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:59:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 19:59:58 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 15 Nov 2022 20:00:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 15 Nov 2022 20:00:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 15 Nov 2022 20:00:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 15 Nov 2022 20:00:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 20:00:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a09dc2ad5d15708c33af827818a7920afcc85c714ad1e377cbce9a7f0f286f`  
		Last Modified: Tue, 15 Nov 2022 20:00:53 GMT  
		Size: 17.5 MB (17463030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef14a56e15e24420180503745c2e9604ad396f53801ed3f4ab7d28ab86318d28`  
		Last Modified: Tue, 15 Nov 2022 20:00:49 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d44e76c2066051aad83e5c1de3a4cb624e67e65354c69a5d9b3e2bc7a6c55cb`  
		Last Modified: Tue, 15 Nov 2022 20:01:15 GMT  
		Size: 39.1 MB (39106556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605d06414bd46ad40d5f38ced24f3ba0da96a21ce751c1a4964ba2d823d61113`  
		Last Modified: Tue, 15 Nov 2022 20:01:08 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:1528cd7750f219dda0d4f73c98162aa645db7e28828fbfb81ec8fd3c7a30964b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126359295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a916e0a6e6ba0de10285c81d3bce51851d93bc7fc7b7956d79f485948b7d2bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:29:30 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 22:29:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 22:29:40 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 15 Nov 2022 22:29:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 15 Nov 2022 22:29:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 15 Nov 2022 22:29:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 15 Nov 2022 22:29:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 22:29:44 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dacffc09706b3a7717b5dc24201989950028c356bbc321c851f61ffbff3917d`  
		Last Modified: Tue, 15 Nov 2022 22:30:09 GMT  
		Size: 18.6 MB (18599319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a956f65aaa93f41831e7e91c5c19af3d879ae834730e3ec7385859fde285337`  
		Last Modified: Tue, 15 Nov 2022 22:30:06 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab5737119a2be66c56be7207ccb91bd7644e311086ec8a75bc3ca0b479cbb10`  
		Last Modified: Tue, 15 Nov 2022 22:30:23 GMT  
		Size: 38.0 MB (38031292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911494be15187e3b9407fd23c5ade35d63c65c2e1c881e7ea6ae3a07fefde92a`  
		Last Modified: Tue, 15 Nov 2022 22:30:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.4-alpine`

```console
$ docker pull telegraf@sha256:deada02a4669f60913770b54e538e7c4ef1f3596b69425a1ae17fec155050d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:acca0f662ea434da10739c21ee6c94a3af210baab442528013e20b251649a9ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47790772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cb5b879e6101df5e177d87eb1ebf9b5da0c90fab88d3a03479bf6b075bda2ae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Sat, 12 Nov 2022 10:02:41 GMT
ENV TELEGRAF_VERSION=1.23.4
# Sat, 12 Nov 2022 10:02:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Sat, 12 Nov 2022 10:02:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 12 Nov 2022 10:02:49 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Sat, 12 Nov 2022 10:02:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 12 Nov 2022 10:02:49 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e702c89f92384b863c431a1780fe1eb6cb2051d840892639c41ab668017ae0`  
		Last Modified: Sat, 12 Nov 2022 10:03:50 GMT  
		Size: 41.7 MB (41685831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d62792d26ded35216d918492be7c49a9d8bff2da01169e4a3f362fa409cb365`  
		Last Modified: Sat, 12 Nov 2022 10:03:43 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24`

```console
$ docker pull telegraf@sha256:686e0ba054be4546a2b2b438f35d1b19c4446194004e5417021d4c0975d6a095
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24` - linux; amd64

```console
$ docker pull telegraf@sha256:4dbce0dbae67d46c8081fe515c759af78524e6223643ead2bf15ee6083547562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134311920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7bdc8f60c977b9047f325b4bd6e36b14b468e1e4e461ecd787d4418a3214dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 00:11:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:11:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Nov 2022 21:43:29 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 21:43:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 29 Nov 2022 21:43:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 21:43:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 29 Nov 2022 21:43:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 21:43:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e470c46ca228512e8b187d5fe846c93c976f72bcd54b96c870855e69877e02a`  
		Last Modified: Wed, 16 Nov 2022 00:12:11 GMT  
		Size: 18.8 MB (18760393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e66d445937565d68a5f8be7023f158f0d5cdcc333af3c70c5124dfda50802`  
		Last Modified: Wed, 16 Nov 2022 00:12:07 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595c504662bc3db0fde2d0afff831d0b323c2b64ce4c4db33a0116c494732320`  
		Last Modified: Tue, 29 Nov 2022 21:44:15 GMT  
		Size: 44.5 MB (44467397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39997058afeb22b92e0d92132062b33142d5fd89cba9b7422faddf45d8991c52`  
		Last Modified: Tue, 29 Nov 2022 21:44:08 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:302d3da852d75f374f8f0e02cc4b200de8243b0132bebf13c501c6f2259a1f81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124330998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f98e4795d47aae4a0b175c651d2fafce2842c03fe6ac8ebfc77a0f75f9e5e5a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 19:59:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:59:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Nov 2022 22:54:45 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 22:54:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 29 Nov 2022 22:54:51 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 22:54:51 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 29 Nov 2022 22:54:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 22:54:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a09dc2ad5d15708c33af827818a7920afcc85c714ad1e377cbce9a7f0f286f`  
		Last Modified: Tue, 15 Nov 2022 20:00:53 GMT  
		Size: 17.5 MB (17463030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef14a56e15e24420180503745c2e9604ad396f53801ed3f4ab7d28ab86318d28`  
		Last Modified: Tue, 15 Nov 2022 20:00:49 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c515068a56c48dbc192d09d02bee1b5a6820cf6a376580baaec1e9369b41d1`  
		Last Modified: Tue, 29 Nov 2022 22:55:32 GMT  
		Size: 41.5 MB (41507051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc153a20965409d3ee9cd1848938a903e3dff7d3b3ceb0bb19bde699b2009f42`  
		Last Modified: Tue, 29 Nov 2022 22:55:23 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:6c8ba769760fc5e33723fb09e1d0138d531a0350b31c0828f0103a40040e613a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128633435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48b7505b57eba2c6cbf64efdd90c695fbb600cda7d992e54decc9fc4ee4bbb0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:29:30 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 22:29:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Nov 2022 21:59:19 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 21:59:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 29 Nov 2022 21:59:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 21:59:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 29 Nov 2022 21:59:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 21:59:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dacffc09706b3a7717b5dc24201989950028c356bbc321c851f61ffbff3917d`  
		Last Modified: Tue, 15 Nov 2022 22:30:09 GMT  
		Size: 18.6 MB (18599319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a956f65aaa93f41831e7e91c5c19af3d879ae834730e3ec7385859fde285337`  
		Last Modified: Tue, 15 Nov 2022 22:30:06 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff47b4708fb2dabe14d9ef693d8383c7c3e02b0f77a1f2f5f93740f125ef5a5`  
		Last Modified: Tue, 29 Nov 2022 21:59:44 GMT  
		Size: 40.3 MB (40305435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a1268e88baba8c01a3ded599de98179cfc248c98a0f6cd2bea764de3ff76b5`  
		Last Modified: Tue, 29 Nov 2022 21:59:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24-alpine`

```console
$ docker pull telegraf@sha256:931837fcc2fffee2e4c49a26d7f5d1661f1b9110f48e0a88487359480b997acb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:a9ced3bb7e97d9934af64190a43e4bc3070ac4de3eb78d7436f26bfca8393b75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50402774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d62aa8f8aab76d62ea53a6ea5df86b36262fc8aa85199d59b8df57070168216b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Nov 2022 21:43:37 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 21:43:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 29 Nov 2022 21:43:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 21:43:43 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 29 Nov 2022 21:43:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 21:43:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742b2df39f6a27cbf7a4ad7f41349ba8273b8d75e3e353ee528d2318b420621`  
		Last Modified: Tue, 29 Nov 2022 21:44:33 GMT  
		Size: 44.3 MB (44297833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c12c991a997bd8392e8ad217b7f28e72804f920abefa588ed594646b7facdea`  
		Last Modified: Tue, 29 Nov 2022 21:44:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.4`

```console
$ docker pull telegraf@sha256:686e0ba054be4546a2b2b438f35d1b19c4446194004e5417021d4c0975d6a095
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24.4` - linux; amd64

```console
$ docker pull telegraf@sha256:4dbce0dbae67d46c8081fe515c759af78524e6223643ead2bf15ee6083547562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134311920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7bdc8f60c977b9047f325b4bd6e36b14b468e1e4e461ecd787d4418a3214dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 00:11:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:11:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Nov 2022 21:43:29 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 21:43:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 29 Nov 2022 21:43:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 21:43:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 29 Nov 2022 21:43:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 21:43:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e470c46ca228512e8b187d5fe846c93c976f72bcd54b96c870855e69877e02a`  
		Last Modified: Wed, 16 Nov 2022 00:12:11 GMT  
		Size: 18.8 MB (18760393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e66d445937565d68a5f8be7023f158f0d5cdcc333af3c70c5124dfda50802`  
		Last Modified: Wed, 16 Nov 2022 00:12:07 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595c504662bc3db0fde2d0afff831d0b323c2b64ce4c4db33a0116c494732320`  
		Last Modified: Tue, 29 Nov 2022 21:44:15 GMT  
		Size: 44.5 MB (44467397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39997058afeb22b92e0d92132062b33142d5fd89cba9b7422faddf45d8991c52`  
		Last Modified: Tue, 29 Nov 2022 21:44:08 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:302d3da852d75f374f8f0e02cc4b200de8243b0132bebf13c501c6f2259a1f81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124330998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f98e4795d47aae4a0b175c651d2fafce2842c03fe6ac8ebfc77a0f75f9e5e5a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 19:59:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:59:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Nov 2022 22:54:45 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 22:54:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 29 Nov 2022 22:54:51 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 22:54:51 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 29 Nov 2022 22:54:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 22:54:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a09dc2ad5d15708c33af827818a7920afcc85c714ad1e377cbce9a7f0f286f`  
		Last Modified: Tue, 15 Nov 2022 20:00:53 GMT  
		Size: 17.5 MB (17463030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef14a56e15e24420180503745c2e9604ad396f53801ed3f4ab7d28ab86318d28`  
		Last Modified: Tue, 15 Nov 2022 20:00:49 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c515068a56c48dbc192d09d02bee1b5a6820cf6a376580baaec1e9369b41d1`  
		Last Modified: Tue, 29 Nov 2022 22:55:32 GMT  
		Size: 41.5 MB (41507051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc153a20965409d3ee9cd1848938a903e3dff7d3b3ceb0bb19bde699b2009f42`  
		Last Modified: Tue, 29 Nov 2022 22:55:23 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:6c8ba769760fc5e33723fb09e1d0138d531a0350b31c0828f0103a40040e613a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128633435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48b7505b57eba2c6cbf64efdd90c695fbb600cda7d992e54decc9fc4ee4bbb0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:29:30 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 22:29:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Nov 2022 21:59:19 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 21:59:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 29 Nov 2022 21:59:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 21:59:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 29 Nov 2022 21:59:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 21:59:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dacffc09706b3a7717b5dc24201989950028c356bbc321c851f61ffbff3917d`  
		Last Modified: Tue, 15 Nov 2022 22:30:09 GMT  
		Size: 18.6 MB (18599319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a956f65aaa93f41831e7e91c5c19af3d879ae834730e3ec7385859fde285337`  
		Last Modified: Tue, 15 Nov 2022 22:30:06 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff47b4708fb2dabe14d9ef693d8383c7c3e02b0f77a1f2f5f93740f125ef5a5`  
		Last Modified: Tue, 29 Nov 2022 21:59:44 GMT  
		Size: 40.3 MB (40305435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a1268e88baba8c01a3ded599de98179cfc248c98a0f6cd2bea764de3ff76b5`  
		Last Modified: Tue, 29 Nov 2022 21:59:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.4-alpine`

```console
$ docker pull telegraf@sha256:931837fcc2fffee2e4c49a26d7f5d1661f1b9110f48e0a88487359480b997acb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:a9ced3bb7e97d9934af64190a43e4bc3070ac4de3eb78d7436f26bfca8393b75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50402774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d62aa8f8aab76d62ea53a6ea5df86b36262fc8aa85199d59b8df57070168216b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Nov 2022 21:43:37 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 21:43:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 29 Nov 2022 21:43:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 21:43:43 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 29 Nov 2022 21:43:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 21:43:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742b2df39f6a27cbf7a4ad7f41349ba8273b8d75e3e353ee528d2318b420621`  
		Last Modified: Tue, 29 Nov 2022 21:44:33 GMT  
		Size: 44.3 MB (44297833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c12c991a997bd8392e8ad217b7f28e72804f920abefa588ed594646b7facdea`  
		Last Modified: Tue, 29 Nov 2022 21:44:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:931837fcc2fffee2e4c49a26d7f5d1661f1b9110f48e0a88487359480b997acb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:a9ced3bb7e97d9934af64190a43e4bc3070ac4de3eb78d7436f26bfca8393b75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50402774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d62aa8f8aab76d62ea53a6ea5df86b36262fc8aa85199d59b8df57070168216b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Nov 2022 21:43:37 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 21:43:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 29 Nov 2022 21:43:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 21:43:43 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 29 Nov 2022 21:43:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 21:43:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742b2df39f6a27cbf7a4ad7f41349ba8273b8d75e3e353ee528d2318b420621`  
		Last Modified: Tue, 29 Nov 2022 21:44:33 GMT  
		Size: 44.3 MB (44297833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c12c991a997bd8392e8ad217b7f28e72804f920abefa588ed594646b7facdea`  
		Last Modified: Tue, 29 Nov 2022 21:44:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:686e0ba054be4546a2b2b438f35d1b19c4446194004e5417021d4c0975d6a095
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:4dbce0dbae67d46c8081fe515c759af78524e6223643ead2bf15ee6083547562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134311920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7bdc8f60c977b9047f325b4bd6e36b14b468e1e4e461ecd787d4418a3214dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:43 GMT
ADD file:abc6873c98339a3c496cb75ec2528e65ebe1f20d2cea777033f86dcd55d73da5 in / 
# Tue, 15 Nov 2022 04:04:43 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:23:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 00:11:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:11:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Nov 2022 21:43:29 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 21:43:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 29 Nov 2022 21:43:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 21:43:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 29 Nov 2022 21:43:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 21:43:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8ca11554fce00d9177da2d76307bdc06df7faeb84529755c648ac4886192ed1`  
		Last Modified: Tue, 15 Nov 2022 04:08:24 GMT  
		Size: 55.0 MB (55038615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e46864aba2e62ba7c75965e4aa33ec856ee1b1074dda6b478101c577b63abd`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 5.2 MB (5164893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85a0be79bfba309d1f05dc40b447aa82b604593531fed1e7e12e4bef63483a5`  
		Last Modified: Tue, 15 Nov 2022 10:31:37 GMT  
		Size: 10.9 MB (10877392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e470c46ca228512e8b187d5fe846c93c976f72bcd54b96c870855e69877e02a`  
		Last Modified: Wed, 16 Nov 2022 00:12:11 GMT  
		Size: 18.8 MB (18760393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e66d445937565d68a5f8be7023f158f0d5cdcc333af3c70c5124dfda50802`  
		Last Modified: Wed, 16 Nov 2022 00:12:07 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595c504662bc3db0fde2d0afff831d0b323c2b64ce4c4db33a0116c494732320`  
		Last Modified: Tue, 29 Nov 2022 21:44:15 GMT  
		Size: 44.5 MB (44467397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39997058afeb22b92e0d92132062b33142d5fd89cba9b7422faddf45d8991c52`  
		Last Modified: Tue, 29 Nov 2022 21:44:08 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:302d3da852d75f374f8f0e02cc4b200de8243b0132bebf13c501c6f2259a1f81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124330998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f98e4795d47aae4a0b175c651d2fafce2842c03fe6ac8ebfc77a0f75f9e5e5a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:06 GMT
ADD file:b9aa70e61b1fbe181b8c48785afc4ef75e7b075b3bc2bc6c329b8397f141efdb in / 
# Tue, 15 Nov 2022 03:43:07 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:18:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:18:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 19:59:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 19:59:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Nov 2022 22:54:45 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 22:54:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 29 Nov 2022 22:54:51 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 22:54:51 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 29 Nov 2022 22:54:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 22:54:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ee6e2ee12efd45cd8105de9bf53619cb3c28867c3974dc5e0137fc0efeb0f577`  
		Last Modified: Tue, 15 Nov 2022 03:49:41 GMT  
		Size: 50.2 MB (50206360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e57b390d8cdf8398d64b2fe40ea3ba6adaff3fd6f221428b28eab7babf88f4`  
		Last Modified: Tue, 15 Nov 2022 12:28:30 GMT  
		Size: 4.9 MB (4932799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6e3dceb24a7026a68b789a939899dc5b68bdfd8bef46052a5a176eca4c76b2`  
		Last Modified: Tue, 15 Nov 2022 12:28:31 GMT  
		Size: 10.2 MB (10218556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a09dc2ad5d15708c33af827818a7920afcc85c714ad1e377cbce9a7f0f286f`  
		Last Modified: Tue, 15 Nov 2022 20:00:53 GMT  
		Size: 17.5 MB (17463030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef14a56e15e24420180503745c2e9604ad396f53801ed3f4ab7d28ab86318d28`  
		Last Modified: Tue, 15 Nov 2022 20:00:49 GMT  
		Size: 2.9 KB (2860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c515068a56c48dbc192d09d02bee1b5a6820cf6a376580baaec1e9369b41d1`  
		Last Modified: Tue, 29 Nov 2022 22:55:32 GMT  
		Size: 41.5 MB (41507051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc153a20965409d3ee9cd1848938a903e3dff7d3b3ceb0bb19bde699b2009f42`  
		Last Modified: Tue, 29 Nov 2022 22:55:23 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:6c8ba769760fc5e33723fb09e1d0138d531a0350b31c0828f0103a40040e613a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128633435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48b7505b57eba2c6cbf64efdd90c695fbb600cda7d992e54decc9fc4ee4bbb0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:12 GMT
ADD file:1f3a7177f64e1adda3e7a541c93dd4322c6ecb4f00f7b015665df2c0c08b59a5 in / 
# Tue, 15 Nov 2022 01:41:12 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:36:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 22:29:30 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 22:29:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 29 Nov 2022 21:59:19 GMT
ENV TELEGRAF_VERSION=1.24.4
# Tue, 29 Nov 2022 21:59:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 29 Nov 2022 21:59:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Nov 2022 21:59:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 29 Nov 2022 21:59:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Nov 2022 21:59:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:077c13527d405646e2f6bb426e04716ae4f8dd2fdd8966dcb0194564a2b57896`  
		Last Modified: Tue, 15 Nov 2022 01:44:12 GMT  
		Size: 53.7 MB (53699862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e29af4daf3531efcc63588162e8bdcf3434aa5d72df4eabeb5e20c6695e303`  
		Last Modified: Tue, 15 Nov 2022 05:42:56 GMT  
		Size: 5.2 MB (5151439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b1480fa4dae5cbbb7d091c46ae0ae52f501418d4cfeb849b87023364e2564`  
		Last Modified: Tue, 15 Nov 2022 05:42:57 GMT  
		Size: 10.9 MB (10874142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dacffc09706b3a7717b5dc24201989950028c356bbc321c851f61ffbff3917d`  
		Last Modified: Tue, 15 Nov 2022 22:30:09 GMT  
		Size: 18.6 MB (18599319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a956f65aaa93f41831e7e91c5c19af3d879ae834730e3ec7385859fde285337`  
		Last Modified: Tue, 15 Nov 2022 22:30:06 GMT  
		Size: 2.9 KB (2897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff47b4708fb2dabe14d9ef693d8383c7c3e02b0f77a1f2f5f93740f125ef5a5`  
		Last Modified: Tue, 29 Nov 2022 21:59:44 GMT  
		Size: 40.3 MB (40305435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a1268e88baba8c01a3ded599de98179cfc248c98a0f6cd2bea764de3ff76b5`  
		Last Modified: Tue, 29 Nov 2022 21:59:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
