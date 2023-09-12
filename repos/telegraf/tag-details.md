<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.26`](#telegraf126)
-	[`telegraf:1.26-alpine`](#telegraf126-alpine)
-	[`telegraf:1.26.3`](#telegraf1263)
-	[`telegraf:1.26.3-alpine`](#telegraf1263-alpine)
-	[`telegraf:1.27`](#telegraf127)
-	[`telegraf:1.27-alpine`](#telegraf127-alpine)
-	[`telegraf:1.27.4`](#telegraf1274)
-	[`telegraf:1.27.4-alpine`](#telegraf1274-alpine)
-	[`telegraf:1.28`](#telegraf128)
-	[`telegraf:1.28-alpine`](#telegraf128-alpine)
-	[`telegraf:1.28.1`](#telegraf1281)
-	[`telegraf:1.28.1-alpine`](#telegraf1281-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.26`

```console
$ docker pull telegraf@sha256:5aa3b18a95a7e623ab659dad1fd0be5cb2fd9c86fcd7b9effcd188d569c50041
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26` - linux; amd64

```console
$ docker pull telegraf@sha256:191a896a4976dee1341e338bf9f8d07a40ef0948d4142831bae0443106303fad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140131237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92c74dde92bc453fd0c87f780ab3f68b1968ec8c9c3d31eba0fcfee9a127d483`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:57:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 22:43:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 22:43:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 22:43:58 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 07 Sep 2023 22:44:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 07 Sep 2023 22:44:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 07 Sep 2023 22:44:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 07 Sep 2023 22:44:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 22:44:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d190df514e96e82a9048dff1406b65e853dbdfbfc0d8474b85ef6bf37bfea62a`  
		Last Modified: Thu, 07 Sep 2023 03:05:52 GMT  
		Size: 15.8 MB (15760386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf7913915e7433b80616c449c855eeb4543e3c1fe3ec748352ed2f3502352ba`  
		Last Modified: Thu, 07 Sep 2023 22:44:43 GMT  
		Size: 18.8 MB (18759934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7af63480ddc5b6ac2fb706dac722b779125c67e2e0fde620d5f9b425c8c83d7`  
		Last Modified: Thu, 07 Sep 2023 22:44:40 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff2007c9ecc6acb62b88af18ac63c5a356b44f3806a1efa01983a7f8b362cf4`  
		Last Modified: Thu, 07 Sep 2023 22:45:04 GMT  
		Size: 50.6 MB (50552510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc8261edc3166c2b3a1f725071790e36231b2ffbe5abf4ac201f13daff75bb2`  
		Last Modified: Thu, 07 Sep 2023 22:44:56 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:f857538676deb374bf9625240b97f5cb4c2737b25f864afec505268e6a526100
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129835168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3b8d0f53180004143f1746e3a9c802168da407a9c49ae74adbc6a638bd6ef2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:33:01 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:33:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 19:33:14 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 07 Sep 2023 19:33:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 07 Sep 2023 19:33:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 07 Sep 2023 19:33:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 07 Sep 2023 19:33:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 19:33:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a3e40045b60de87bd316fc81bad3ca642a31ef598e190c09841e07788e602b`  
		Last Modified: Thu, 07 Sep 2023 01:46:10 GMT  
		Size: 14.9 MB (14868694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f934a49cef7866826ade423c670213165beb2d443dab3b667250f9a0550386b3`  
		Last Modified: Thu, 07 Sep 2023 19:34:06 GMT  
		Size: 17.5 MB (17462349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230ddd7d94a3faaeb06c3930eaa4a48aa48539489c28c705513c90391260fdcd`  
		Last Modified: Thu, 07 Sep 2023 19:34:00 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f840c0b480e572d583e569d8034d6677e0f61e26bc04376a1221c1f96c6a7bb9`  
		Last Modified: Thu, 07 Sep 2023 19:34:30 GMT  
		Size: 47.3 MB (47282730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c39c8abeee4094bcfe6eec50fc06ee4c896743978176dfff23d2b2f2ba7b192`  
		Last Modified: Thu, 07 Sep 2023 19:34:20 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:da778ed26a2b437a15204cf8b59f6191325d2f6e2762c94f1afc27a3fc314ec5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134023681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18583cedf956cd5c51e624275aea272ca6b89c462e2dd9ffa42dbcc6274dea78`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:52:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:37:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:37:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 19:38:03 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 07 Sep 2023 19:38:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 07 Sep 2023 19:38:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 07 Sep 2023 19:38:09 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 07 Sep 2023 19:38:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 19:38:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b3f92a99188e47f7b0b8d38aff11fd0ad90510e0d26506aec007d24fe539b6`  
		Last Modified: Thu, 07 Sep 2023 07:00:19 GMT  
		Size: 15.7 MB (15746623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb55859439f997f32e05748735103343b467a25cef7272af904815533cbebd17`  
		Last Modified: Thu, 07 Sep 2023 19:38:46 GMT  
		Size: 18.6 MB (18598350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0856c0a2fce875f1607d59f328edc7ded871f09431ac6b813bda01486265f14b`  
		Last Modified: Thu, 07 Sep 2023 19:38:43 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c58d20122648b5147c493b75db78bb49410cb06aa7c61dd9d88328a879f7c14`  
		Last Modified: Thu, 07 Sep 2023 19:39:02 GMT  
		Size: 46.0 MB (45971847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30a31e244a86e30cadf0caf8f7b5c2b874b2d93ed101883d2d4c475d6f8b9be`  
		Last Modified: Thu, 07 Sep 2023 19:38:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26-alpine`

```console
$ docker pull telegraf@sha256:6324054ecb1955be213e63944c66a84a8fd98972aa93f95d116dc8c4524e5c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:78f7670b9bcd3a4aad80c6ebbee49cf7335f6a5d2d859c953bfa64f8006f38e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56442923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c98ff0b99b251029050997eaa7c7f4781b917a79b8bed512a729e69982f7c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:04:25 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:04:40 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 09 Aug 2023 04:04:52 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:04:52 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:04:52 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:04:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:04:52 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81f19a7d917a9734911b177e41983aa98776e1138b57753de6adba42dd022ba`  
		Last Modified: Wed, 09 Aug 2023 04:05:25 GMT  
		Size: 2.7 MB (2671751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ffe32ffc35ea9bbf469c7313d2e28eb55dce4def6d7921b4a8ed64d5065827`  
		Last Modified: Wed, 09 Aug 2023 04:05:49 GMT  
		Size: 50.4 MB (50391957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae69b2b52e8bf419120908053a720d3c85e1cd6eee473ce91f75e98b516a`  
		Last Modified: Wed, 09 Aug 2023 04:05:41 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:e663774ce831002c89534e1f287e55d3bd316713b618e67701db26fbe5d8028d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51774942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8375fdb742f718828f27c8a87bcacfe958d4efe3802049d8e0f2db47b8b63653`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:46:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:25:36 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:25:36 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 09 Aug 2023 04:25:43 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:25:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:25:44 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:25:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:25:44 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd1799839c258f2f362340c258c49aa080e354fd0e137266f54d413ef004a1b`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47f27f99383dfe7b1872c5a815d6081f46d86eeaa05a1cb0fef13827b0fe766`  
		Last Modified: Wed, 09 Aug 2023 04:26:17 GMT  
		Size: 2.7 MB (2703763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014a294016445a25dbb6ffc116ee7cabe334d80ec4a227196a4109180dbe204b`  
		Last Modified: Wed, 09 Aug 2023 04:26:22 GMT  
		Size: 45.8 MB (45812279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8399f752cf89525b188eb16e83df90ab39e25524c9308c289d2f748445fca4`  
		Last Modified: Wed, 09 Aug 2023 04:26:16 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3`

```console
$ docker pull telegraf@sha256:5aa3b18a95a7e623ab659dad1fd0be5cb2fd9c86fcd7b9effcd188d569c50041
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26.3` - linux; amd64

```console
$ docker pull telegraf@sha256:191a896a4976dee1341e338bf9f8d07a40ef0948d4142831bae0443106303fad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140131237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92c74dde92bc453fd0c87f780ab3f68b1968ec8c9c3d31eba0fcfee9a127d483`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:57:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 22:43:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 22:43:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 22:43:58 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 07 Sep 2023 22:44:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 07 Sep 2023 22:44:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 07 Sep 2023 22:44:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 07 Sep 2023 22:44:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 22:44:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d190df514e96e82a9048dff1406b65e853dbdfbfc0d8474b85ef6bf37bfea62a`  
		Last Modified: Thu, 07 Sep 2023 03:05:52 GMT  
		Size: 15.8 MB (15760386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf7913915e7433b80616c449c855eeb4543e3c1fe3ec748352ed2f3502352ba`  
		Last Modified: Thu, 07 Sep 2023 22:44:43 GMT  
		Size: 18.8 MB (18759934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7af63480ddc5b6ac2fb706dac722b779125c67e2e0fde620d5f9b425c8c83d7`  
		Last Modified: Thu, 07 Sep 2023 22:44:40 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff2007c9ecc6acb62b88af18ac63c5a356b44f3806a1efa01983a7f8b362cf4`  
		Last Modified: Thu, 07 Sep 2023 22:45:04 GMT  
		Size: 50.6 MB (50552510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc8261edc3166c2b3a1f725071790e36231b2ffbe5abf4ac201f13daff75bb2`  
		Last Modified: Thu, 07 Sep 2023 22:44:56 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:f857538676deb374bf9625240b97f5cb4c2737b25f864afec505268e6a526100
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129835168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3b8d0f53180004143f1746e3a9c802168da407a9c49ae74adbc6a638bd6ef2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:33:01 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:33:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 19:33:14 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 07 Sep 2023 19:33:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 07 Sep 2023 19:33:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 07 Sep 2023 19:33:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 07 Sep 2023 19:33:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 19:33:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a3e40045b60de87bd316fc81bad3ca642a31ef598e190c09841e07788e602b`  
		Last Modified: Thu, 07 Sep 2023 01:46:10 GMT  
		Size: 14.9 MB (14868694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f934a49cef7866826ade423c670213165beb2d443dab3b667250f9a0550386b3`  
		Last Modified: Thu, 07 Sep 2023 19:34:06 GMT  
		Size: 17.5 MB (17462349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230ddd7d94a3faaeb06c3930eaa4a48aa48539489c28c705513c90391260fdcd`  
		Last Modified: Thu, 07 Sep 2023 19:34:00 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f840c0b480e572d583e569d8034d6677e0f61e26bc04376a1221c1f96c6a7bb9`  
		Last Modified: Thu, 07 Sep 2023 19:34:30 GMT  
		Size: 47.3 MB (47282730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c39c8abeee4094bcfe6eec50fc06ee4c896743978176dfff23d2b2f2ba7b192`  
		Last Modified: Thu, 07 Sep 2023 19:34:20 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:da778ed26a2b437a15204cf8b59f6191325d2f6e2762c94f1afc27a3fc314ec5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134023681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18583cedf956cd5c51e624275aea272ca6b89c462e2dd9ffa42dbcc6274dea78`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:52:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:37:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:37:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 19:38:03 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 07 Sep 2023 19:38:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 07 Sep 2023 19:38:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 07 Sep 2023 19:38:09 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 07 Sep 2023 19:38:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 19:38:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b3f92a99188e47f7b0b8d38aff11fd0ad90510e0d26506aec007d24fe539b6`  
		Last Modified: Thu, 07 Sep 2023 07:00:19 GMT  
		Size: 15.7 MB (15746623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb55859439f997f32e05748735103343b467a25cef7272af904815533cbebd17`  
		Last Modified: Thu, 07 Sep 2023 19:38:46 GMT  
		Size: 18.6 MB (18598350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0856c0a2fce875f1607d59f328edc7ded871f09431ac6b813bda01486265f14b`  
		Last Modified: Thu, 07 Sep 2023 19:38:43 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c58d20122648b5147c493b75db78bb49410cb06aa7c61dd9d88328a879f7c14`  
		Last Modified: Thu, 07 Sep 2023 19:39:02 GMT  
		Size: 46.0 MB (45971847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30a31e244a86e30cadf0caf8f7b5c2b874b2d93ed101883d2d4c475d6f8b9be`  
		Last Modified: Thu, 07 Sep 2023 19:38:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3-alpine`

```console
$ docker pull telegraf@sha256:6324054ecb1955be213e63944c66a84a8fd98972aa93f95d116dc8c4524e5c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:78f7670b9bcd3a4aad80c6ebbee49cf7335f6a5d2d859c953bfa64f8006f38e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56442923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c98ff0b99b251029050997eaa7c7f4781b917a79b8bed512a729e69982f7c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:04:25 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:04:40 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 09 Aug 2023 04:04:52 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:04:52 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:04:52 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:04:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:04:52 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81f19a7d917a9734911b177e41983aa98776e1138b57753de6adba42dd022ba`  
		Last Modified: Wed, 09 Aug 2023 04:05:25 GMT  
		Size: 2.7 MB (2671751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ffe32ffc35ea9bbf469c7313d2e28eb55dce4def6d7921b4a8ed64d5065827`  
		Last Modified: Wed, 09 Aug 2023 04:05:49 GMT  
		Size: 50.4 MB (50391957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae69b2b52e8bf419120908053a720d3c85e1cd6eee473ce91f75e98b516a`  
		Last Modified: Wed, 09 Aug 2023 04:05:41 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:e663774ce831002c89534e1f287e55d3bd316713b618e67701db26fbe5d8028d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51774942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8375fdb742f718828f27c8a87bcacfe958d4efe3802049d8e0f2db47b8b63653`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:46:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:25:36 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:25:36 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 09 Aug 2023 04:25:43 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:25:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:25:44 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:25:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:25:44 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd1799839c258f2f362340c258c49aa080e354fd0e137266f54d413ef004a1b`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47f27f99383dfe7b1872c5a815d6081f46d86eeaa05a1cb0fef13827b0fe766`  
		Last Modified: Wed, 09 Aug 2023 04:26:17 GMT  
		Size: 2.7 MB (2703763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014a294016445a25dbb6ffc116ee7cabe334d80ec4a227196a4109180dbe204b`  
		Last Modified: Wed, 09 Aug 2023 04:26:22 GMT  
		Size: 45.8 MB (45812279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8399f752cf89525b188eb16e83df90ab39e25524c9308c289d2f748445fca4`  
		Last Modified: Wed, 09 Aug 2023 04:26:16 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27`

```console
$ docker pull telegraf@sha256:6790fa19556e4a19408a5adbabccc635fef46979d0fdf529fb0ad35e1c0fe979
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27` - linux; amd64

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

### `telegraf:1.27` - linux; arm variant v7

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

### `telegraf:1.27` - linux; arm64 variant v8

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

## `telegraf:1.27-alpine`

```console
$ docker pull telegraf@sha256:d7f88f8c45549c846d12660dc014e189fc7b65caa2b0660a02c6b27d12add7f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.27-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:6c266d120abb95bb0b38bb87cd2c0f101f689b0ea9f7be209dd94093dd286434
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61198147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dcc393fe5d6fd8f0b245d47830dfd65184688351e3979468a65a64628050ed7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:05:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:05:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 21 Aug 2023 22:32:49 GMT
ENV TELEGRAF_VERSION=1.27.4
# Mon, 21 Aug 2023 22:32:55 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 21 Aug 2023 22:32:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 21 Aug 2023 22:32:55 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 21 Aug 2023 22:32:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 21 Aug 2023 22:32:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039529048aa7cd46b974231fd34d48f954eb067994d5f425569af914e7de0ef6`  
		Last Modified: Wed, 09 Aug 2023 04:05:58 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96767576f65551b43cd2f308297af5090afedffb7eb547e395c8c2e02d848397`  
		Last Modified: Wed, 09 Aug 2023 04:05:59 GMT  
		Size: 2.6 MB (2643772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c47c26b900f637b175da03d0c775cc6991379c642c37877043d59c55000e00`  
		Last Modified: Mon, 21 Aug 2023 22:33:40 GMT  
		Size: 55.2 MB (55152152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a508c965f21fa20f5f00e0597af4911e73f902502883aeeeeae9a88665c6766`  
		Last Modified: Mon, 21 Aug 2023 22:33:31 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:01f0fd973316b62349c85e4f4db9478e3ebb20f599c1127e7c8a0a3169104838
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55797753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11da62082aa70cbeff7459f646e214b10d0054819ae2c276bb98af38cab8fdc9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:25:48 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:25:50 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 21 Aug 2023 23:16:27 GMT
ENV TELEGRAF_VERSION=1.27.4
# Mon, 21 Aug 2023 23:16:32 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 21 Aug 2023 23:16:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 21 Aug 2023 23:16:34 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 21 Aug 2023 23:16:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 21 Aug 2023 23:16:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d4096012e5a9408aedb4891d96f73d6678d25354afc929941aa2338446c730`  
		Last Modified: Wed, 09 Aug 2023 04:26:31 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a312960d045953e25342cafbc53ced993bfc32dfe9e0cebfaf28769e1b2f481`  
		Last Modified: Wed, 09 Aug 2023 04:26:32 GMT  
		Size: 2.7 MB (2671154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4132af2555da52279d3986a9d2d451b879af36c3461a3d8b2c080bf6444fb5b8`  
		Last Modified: Mon, 21 Aug 2023 23:17:14 GMT  
		Size: 49.8 MB (49795224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8ddd0d8124213492a8030ded57d56f2a477224f7298811e3db99120b2b1731`  
		Last Modified: Mon, 21 Aug 2023 23:17:08 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27.4`

```console
$ docker pull telegraf@sha256:6790fa19556e4a19408a5adbabccc635fef46979d0fdf529fb0ad35e1c0fe979
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27.4` - linux; amd64

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

### `telegraf:1.27.4` - linux; arm variant v7

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

### `telegraf:1.27.4` - linux; arm64 variant v8

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

## `telegraf:1.27.4-alpine`

```console
$ docker pull telegraf@sha256:d7f88f8c45549c846d12660dc014e189fc7b65caa2b0660a02c6b27d12add7f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.27.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:6c266d120abb95bb0b38bb87cd2c0f101f689b0ea9f7be209dd94093dd286434
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61198147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dcc393fe5d6fd8f0b245d47830dfd65184688351e3979468a65a64628050ed7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:05:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:05:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 21 Aug 2023 22:32:49 GMT
ENV TELEGRAF_VERSION=1.27.4
# Mon, 21 Aug 2023 22:32:55 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 21 Aug 2023 22:32:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 21 Aug 2023 22:32:55 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 21 Aug 2023 22:32:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 21 Aug 2023 22:32:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039529048aa7cd46b974231fd34d48f954eb067994d5f425569af914e7de0ef6`  
		Last Modified: Wed, 09 Aug 2023 04:05:58 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96767576f65551b43cd2f308297af5090afedffb7eb547e395c8c2e02d848397`  
		Last Modified: Wed, 09 Aug 2023 04:05:59 GMT  
		Size: 2.6 MB (2643772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c47c26b900f637b175da03d0c775cc6991379c642c37877043d59c55000e00`  
		Last Modified: Mon, 21 Aug 2023 22:33:40 GMT  
		Size: 55.2 MB (55152152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a508c965f21fa20f5f00e0597af4911e73f902502883aeeeeae9a88665c6766`  
		Last Modified: Mon, 21 Aug 2023 22:33:31 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.4-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:01f0fd973316b62349c85e4f4db9478e3ebb20f599c1127e7c8a0a3169104838
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55797753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11da62082aa70cbeff7459f646e214b10d0054819ae2c276bb98af38cab8fdc9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:25:48 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:25:50 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 21 Aug 2023 23:16:27 GMT
ENV TELEGRAF_VERSION=1.27.4
# Mon, 21 Aug 2023 23:16:32 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 21 Aug 2023 23:16:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 21 Aug 2023 23:16:34 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 21 Aug 2023 23:16:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 21 Aug 2023 23:16:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d4096012e5a9408aedb4891d96f73d6678d25354afc929941aa2338446c730`  
		Last Modified: Wed, 09 Aug 2023 04:26:31 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a312960d045953e25342cafbc53ced993bfc32dfe9e0cebfaf28769e1b2f481`  
		Last Modified: Wed, 09 Aug 2023 04:26:32 GMT  
		Size: 2.7 MB (2671154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4132af2555da52279d3986a9d2d451b879af36c3461a3d8b2c080bf6444fb5b8`  
		Last Modified: Mon, 21 Aug 2023 23:17:14 GMT  
		Size: 49.8 MB (49795224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8ddd0d8124213492a8030ded57d56f2a477224f7298811e3db99120b2b1731`  
		Last Modified: Mon, 21 Aug 2023 23:17:08 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.28`

```console
$ docker pull telegraf@sha256:509c325b9fedc290f1221dc862727717846b164b1a0404cb36860eef09191d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.28` - linux; amd64

```console
$ docker pull telegraf@sha256:895c34566cae9ed5cf8dfee7be642b495b60b0047ba11f75c5e548ee7ee87683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.4 MB (148376015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f4a1cc74046ce48cd918693cd6bf4b2683f4ce0d7be3f7148a21df9f06f5b5f`
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
# Tue, 12 Sep 2023 20:20:20 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 20:20:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Sep 2023 20:20:25 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 20:20:26 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 12 Sep 2023 20:20:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 20:20:26 GMT
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
	-	`sha256:078fa832f61ddbb425b2e6ffa993c446e23bbcee3609ceaf00239d7c6f76a28d`  
		Last Modified: Tue, 12 Sep 2023 20:21:09 GMT  
		Size: 55.6 MB (55642734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8303e0f4db2e6c371a897d344690e13d031c9a23f3a9a324f7fde80536b7fbb7`  
		Last Modified: Tue, 12 Sep 2023 20:21:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:0009c5790c1d556e9a74c08973229ff99e31c2705d142f225e0f8a0c0413a084
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136571729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21b7ddc4f1e8b1033a3c16e99904c0e40dba1df148cb9b57fb806b5c42efa3eb`
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
# Tue, 12 Sep 2023 20:13:22 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 20:13:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Sep 2023 20:13:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 20:13:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 12 Sep 2023 20:13:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 20:13:31 GMT
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
	-	`sha256:bef637acc01d98376f12d71b0233f0f17296570d001aa568bcaa8119d1e8f575`  
		Last Modified: Tue, 12 Sep 2023 20:13:56 GMT  
		Size: 51.4 MB (51410269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ec5b8ee30bd2429cf3c4dcd020e5474cf3e258d7edcda91f6fc27c42c77d68`  
		Last Modified: Tue, 12 Sep 2023 20:13:46 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:826b15a58f5f8cbef47f6f4572117c0adcd3525ad88a24a92e5afaf3e7ccaf04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142611542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11af0d4fc12a2d6546f86895f4060509c89cbcdbc2a3abd9d3f096d55a5262c3`
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
# Tue, 12 Sep 2023 19:50:40 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 19:50:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Sep 2023 19:50:46 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 19:50:46 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 12 Sep 2023 19:50:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 19:50:46 GMT
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
	-	`sha256:47a4d556bfbb6598277863ecd661e1ef882670ded7b3ae208ef460352e79234b`  
		Last Modified: Tue, 12 Sep 2023 19:51:24 GMT  
		Size: 50.4 MB (50371277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2074b9263f7c85a359ddff83a230784ab67051111dfa32aacd5df8899fb9c1f`  
		Last Modified: Tue, 12 Sep 2023 19:51:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.28-alpine`

```console
$ docker pull telegraf@sha256:7c4f7caddfe0a7872e0534d609439e9730b0ccba10cd48b7c84933cc1eb9d9fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.28-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:2442b46f9b9ae54212126db217695efa442819d18814d9a005280baaf91944b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61517663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2508d88f446b86b3ca9721940e5f34e484b735def5c1b5b8e4294b46f9ac474`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:05:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:05:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 12 Sep 2023 20:20:29 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 20:20:36 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 12 Sep 2023 20:20:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 20:20:36 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 12 Sep 2023 20:20:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 20:20:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039529048aa7cd46b974231fd34d48f954eb067994d5f425569af914e7de0ef6`  
		Last Modified: Wed, 09 Aug 2023 04:05:58 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96767576f65551b43cd2f308297af5090afedffb7eb547e395c8c2e02d848397`  
		Last Modified: Wed, 09 Aug 2023 04:05:59 GMT  
		Size: 2.6 MB (2643772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ea743fa0e9a480c9d7126221166681d41459674d1118d0a19021b03ab16e69`  
		Last Modified: Tue, 12 Sep 2023 20:21:30 GMT  
		Size: 55.5 MB (55471669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3da6562d5a4d538628be0e8be63953126f894dc87c9a8a8cdbc2a0fac959513`  
		Last Modified: Tue, 12 Sep 2023 20:21:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:bb20d0afcc4dba9923cdbed640e7ff54252164da3180385b76937a7d6b73302b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56205539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00c4963377892ef4587d24642488aef39b6df6a53cb3cf1c0dcfa3eaee20ae4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:25:48 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:25:50 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 12 Sep 2023 19:50:49 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 19:50:57 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 12 Sep 2023 19:50:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 19:50:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 12 Sep 2023 19:50:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 19:50:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d4096012e5a9408aedb4891d96f73d6678d25354afc929941aa2338446c730`  
		Last Modified: Wed, 09 Aug 2023 04:26:31 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a312960d045953e25342cafbc53ced993bfc32dfe9e0cebfaf28769e1b2f481`  
		Last Modified: Wed, 09 Aug 2023 04:26:32 GMT  
		Size: 2.7 MB (2671154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02617d155741999eabb62c33f15a25a82f1cb82a07d48f2fac1ed6a5110caf52`  
		Last Modified: Tue, 12 Sep 2023 19:51:41 GMT  
		Size: 50.2 MB (50203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bab5c7e080f54e5a9276168addb328de30c38441b222ef218041de5b42c6fcc`  
		Last Modified: Tue, 12 Sep 2023 19:51:35 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.28.1`

```console
$ docker pull telegraf@sha256:509c325b9fedc290f1221dc862727717846b164b1a0404cb36860eef09191d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.28.1` - linux; amd64

```console
$ docker pull telegraf@sha256:895c34566cae9ed5cf8dfee7be642b495b60b0047ba11f75c5e548ee7ee87683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.4 MB (148376015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f4a1cc74046ce48cd918693cd6bf4b2683f4ce0d7be3f7148a21df9f06f5b5f`
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
# Tue, 12 Sep 2023 20:20:20 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 20:20:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Sep 2023 20:20:25 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 20:20:26 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 12 Sep 2023 20:20:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 20:20:26 GMT
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
	-	`sha256:078fa832f61ddbb425b2e6ffa993c446e23bbcee3609ceaf00239d7c6f76a28d`  
		Last Modified: Tue, 12 Sep 2023 20:21:09 GMT  
		Size: 55.6 MB (55642734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8303e0f4db2e6c371a897d344690e13d031c9a23f3a9a324f7fde80536b7fbb7`  
		Last Modified: Tue, 12 Sep 2023 20:21:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28.1` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:0009c5790c1d556e9a74c08973229ff99e31c2705d142f225e0f8a0c0413a084
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136571729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21b7ddc4f1e8b1033a3c16e99904c0e40dba1df148cb9b57fb806b5c42efa3eb`
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
# Tue, 12 Sep 2023 20:13:22 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 20:13:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Sep 2023 20:13:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 20:13:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 12 Sep 2023 20:13:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 20:13:31 GMT
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
	-	`sha256:bef637acc01d98376f12d71b0233f0f17296570d001aa568bcaa8119d1e8f575`  
		Last Modified: Tue, 12 Sep 2023 20:13:56 GMT  
		Size: 51.4 MB (51410269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ec5b8ee30bd2429cf3c4dcd020e5474cf3e258d7edcda91f6fc27c42c77d68`  
		Last Modified: Tue, 12 Sep 2023 20:13:46 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28.1` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:826b15a58f5f8cbef47f6f4572117c0adcd3525ad88a24a92e5afaf3e7ccaf04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142611542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11af0d4fc12a2d6546f86895f4060509c89cbcdbc2a3abd9d3f096d55a5262c3`
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
# Tue, 12 Sep 2023 19:50:40 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 19:50:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Sep 2023 19:50:46 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 19:50:46 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 12 Sep 2023 19:50:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 19:50:46 GMT
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
	-	`sha256:47a4d556bfbb6598277863ecd661e1ef882670ded7b3ae208ef460352e79234b`  
		Last Modified: Tue, 12 Sep 2023 19:51:24 GMT  
		Size: 50.4 MB (50371277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2074b9263f7c85a359ddff83a230784ab67051111dfa32aacd5df8899fb9c1f`  
		Last Modified: Tue, 12 Sep 2023 19:51:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.28.1-alpine`

```console
$ docker pull telegraf@sha256:7c4f7caddfe0a7872e0534d609439e9730b0ccba10cd48b7c84933cc1eb9d9fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.28.1-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:2442b46f9b9ae54212126db217695efa442819d18814d9a005280baaf91944b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61517663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2508d88f446b86b3ca9721940e5f34e484b735def5c1b5b8e4294b46f9ac474`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:05:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:05:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 12 Sep 2023 20:20:29 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 20:20:36 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 12 Sep 2023 20:20:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 20:20:36 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 12 Sep 2023 20:20:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 20:20:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039529048aa7cd46b974231fd34d48f954eb067994d5f425569af914e7de0ef6`  
		Last Modified: Wed, 09 Aug 2023 04:05:58 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96767576f65551b43cd2f308297af5090afedffb7eb547e395c8c2e02d848397`  
		Last Modified: Wed, 09 Aug 2023 04:05:59 GMT  
		Size: 2.6 MB (2643772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ea743fa0e9a480c9d7126221166681d41459674d1118d0a19021b03ab16e69`  
		Last Modified: Tue, 12 Sep 2023 20:21:30 GMT  
		Size: 55.5 MB (55471669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3da6562d5a4d538628be0e8be63953126f894dc87c9a8a8cdbc2a0fac959513`  
		Last Modified: Tue, 12 Sep 2023 20:21:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28.1-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:bb20d0afcc4dba9923cdbed640e7ff54252164da3180385b76937a7d6b73302b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56205539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00c4963377892ef4587d24642488aef39b6df6a53cb3cf1c0dcfa3eaee20ae4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:25:48 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:25:50 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 12 Sep 2023 19:50:49 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 19:50:57 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 12 Sep 2023 19:50:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 19:50:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 12 Sep 2023 19:50:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 19:50:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d4096012e5a9408aedb4891d96f73d6678d25354afc929941aa2338446c730`  
		Last Modified: Wed, 09 Aug 2023 04:26:31 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a312960d045953e25342cafbc53ced993bfc32dfe9e0cebfaf28769e1b2f481`  
		Last Modified: Wed, 09 Aug 2023 04:26:32 GMT  
		Size: 2.7 MB (2671154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02617d155741999eabb62c33f15a25a82f1cb82a07d48f2fac1ed6a5110caf52`  
		Last Modified: Tue, 12 Sep 2023 19:51:41 GMT  
		Size: 50.2 MB (50203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bab5c7e080f54e5a9276168addb328de30c38441b222ef218041de5b42c6fcc`  
		Last Modified: Tue, 12 Sep 2023 19:51:35 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:7c4f7caddfe0a7872e0534d609439e9730b0ccba10cd48b7c84933cc1eb9d9fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:2442b46f9b9ae54212126db217695efa442819d18814d9a005280baaf91944b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61517663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2508d88f446b86b3ca9721940e5f34e484b735def5c1b5b8e4294b46f9ac474`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:05:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:05:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 12 Sep 2023 20:20:29 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 20:20:36 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 12 Sep 2023 20:20:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 20:20:36 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 12 Sep 2023 20:20:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 20:20:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039529048aa7cd46b974231fd34d48f954eb067994d5f425569af914e7de0ef6`  
		Last Modified: Wed, 09 Aug 2023 04:05:58 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96767576f65551b43cd2f308297af5090afedffb7eb547e395c8c2e02d848397`  
		Last Modified: Wed, 09 Aug 2023 04:05:59 GMT  
		Size: 2.6 MB (2643772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ea743fa0e9a480c9d7126221166681d41459674d1118d0a19021b03ab16e69`  
		Last Modified: Tue, 12 Sep 2023 20:21:30 GMT  
		Size: 55.5 MB (55471669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3da6562d5a4d538628be0e8be63953126f894dc87c9a8a8cdbc2a0fac959513`  
		Last Modified: Tue, 12 Sep 2023 20:21:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:bb20d0afcc4dba9923cdbed640e7ff54252164da3180385b76937a7d6b73302b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56205539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00c4963377892ef4587d24642488aef39b6df6a53cb3cf1c0dcfa3eaee20ae4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:25:48 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:25:50 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 12 Sep 2023 19:50:49 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 19:50:57 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 12 Sep 2023 19:50:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 19:50:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 12 Sep 2023 19:50:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 19:50:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d4096012e5a9408aedb4891d96f73d6678d25354afc929941aa2338446c730`  
		Last Modified: Wed, 09 Aug 2023 04:26:31 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a312960d045953e25342cafbc53ced993bfc32dfe9e0cebfaf28769e1b2f481`  
		Last Modified: Wed, 09 Aug 2023 04:26:32 GMT  
		Size: 2.7 MB (2671154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02617d155741999eabb62c33f15a25a82f1cb82a07d48f2fac1ed6a5110caf52`  
		Last Modified: Tue, 12 Sep 2023 19:51:41 GMT  
		Size: 50.2 MB (50203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bab5c7e080f54e5a9276168addb328de30c38441b222ef218041de5b42c6fcc`  
		Last Modified: Tue, 12 Sep 2023 19:51:35 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:509c325b9fedc290f1221dc862727717846b164b1a0404cb36860eef09191d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:895c34566cae9ed5cf8dfee7be642b495b60b0047ba11f75c5e548ee7ee87683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.4 MB (148376015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f4a1cc74046ce48cd918693cd6bf4b2683f4ce0d7be3f7148a21df9f06f5b5f`
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
# Tue, 12 Sep 2023 20:20:20 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 20:20:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Sep 2023 20:20:25 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 20:20:26 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 12 Sep 2023 20:20:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 20:20:26 GMT
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
	-	`sha256:078fa832f61ddbb425b2e6ffa993c446e23bbcee3609ceaf00239d7c6f76a28d`  
		Last Modified: Tue, 12 Sep 2023 20:21:09 GMT  
		Size: 55.6 MB (55642734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8303e0f4db2e6c371a897d344690e13d031c9a23f3a9a324f7fde80536b7fbb7`  
		Last Modified: Tue, 12 Sep 2023 20:21:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:0009c5790c1d556e9a74c08973229ff99e31c2705d142f225e0f8a0c0413a084
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136571729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21b7ddc4f1e8b1033a3c16e99904c0e40dba1df148cb9b57fb806b5c42efa3eb`
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
# Tue, 12 Sep 2023 20:13:22 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 20:13:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Sep 2023 20:13:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 20:13:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 12 Sep 2023 20:13:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 20:13:31 GMT
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
	-	`sha256:bef637acc01d98376f12d71b0233f0f17296570d001aa568bcaa8119d1e8f575`  
		Last Modified: Tue, 12 Sep 2023 20:13:56 GMT  
		Size: 51.4 MB (51410269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ec5b8ee30bd2429cf3c4dcd020e5474cf3e258d7edcda91f6fc27c42c77d68`  
		Last Modified: Tue, 12 Sep 2023 20:13:46 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:826b15a58f5f8cbef47f6f4572117c0adcd3525ad88a24a92e5afaf3e7ccaf04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142611542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11af0d4fc12a2d6546f86895f4060509c89cbcdbc2a3abd9d3f096d55a5262c3`
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
# Tue, 12 Sep 2023 19:50:40 GMT
ENV TELEGRAF_VERSION=1.28.1
# Tue, 12 Sep 2023 19:50:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 12 Sep 2023 19:50:46 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 12 Sep 2023 19:50:46 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 12 Sep 2023 19:50:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Sep 2023 19:50:46 GMT
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
	-	`sha256:47a4d556bfbb6598277863ecd661e1ef882670ded7b3ae208ef460352e79234b`  
		Last Modified: Tue, 12 Sep 2023 19:51:24 GMT  
		Size: 50.4 MB (50371277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2074b9263f7c85a359ddff83a230784ab67051111dfa32aacd5df8899fb9c1f`  
		Last Modified: Tue, 12 Sep 2023 19:51:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
