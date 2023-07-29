<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.25`](#telegraf125)
-	[`telegraf:1.25-alpine`](#telegraf125-alpine)
-	[`telegraf:1.25.3`](#telegraf1253)
-	[`telegraf:1.25.3-alpine`](#telegraf1253-alpine)
-	[`telegraf:1.26`](#telegraf126)
-	[`telegraf:1.26-alpine`](#telegraf126-alpine)
-	[`telegraf:1.26.3`](#telegraf1263)
-	[`telegraf:1.26.3-alpine`](#telegraf1263-alpine)
-	[`telegraf:1.27`](#telegraf127)
-	[`telegraf:1.27-alpine`](#telegraf127-alpine)
-	[`telegraf:1.27.2`](#telegraf1272)
-	[`telegraf:1.27.2-alpine`](#telegraf1272-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.25`

```console
$ docker pull telegraf@sha256:95bec7e2799898a5a74af7f571fa92a858ba9b225add6e898f3887afc968c941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25` - linux; amd64

```console
$ docker pull telegraf@sha256:fa46591962db79212855884747733e3cc158a637e7d80baf1467776fa73b83ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136154894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e572ac884a7ab26c01df29f3ee818981f6d50a95306258080b9a6ec58ce8e183`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 22:55:48 GMT
ENV TELEGRAF_VERSION=1.25.3
# Fri, 28 Jul 2023 22:55:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 22:55:54 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 22:55:54 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 22:55:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 22:55:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73ccc85cd69e3c3e8eeb927b3ed51cce8e63e067e07b960cd5322c4a9ec4c4f`  
		Last Modified: Fri, 28 Jul 2023 22:56:34 GMT  
		Size: 18.8 MB (18759984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7b7a2e9993ee0093c7cfda4148cf0d6f93907c289799b935b5a441d054fe49`  
		Last Modified: Fri, 28 Jul 2023 22:56:31 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3bcc28d801230e7d731f06b9cf43471f30fd17ccf7d8baa3019e2cf9250b38`  
		Last Modified: Fri, 28 Jul 2023 22:56:38 GMT  
		Size: 46.6 MB (46576603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc23e4a59fc82bbfcab465eb5b57eb74c6aad298ad3f1e6e594c9a14a9edddb`  
		Last Modified: Fri, 28 Jul 2023 22:56:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:e5a3f33d9bbbfb6d6da6ecc6c8dd9b35d4919b05a02e80800e393f98cceee092
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125935273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed4c8ef9b020424b130fc10bfeb0da36b4eea824112c50d4231259492dac6907`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Jul 2023 01:06:10 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 05 Jul 2023 01:06:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 05 Jul 2023 01:06:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 05 Jul 2023 01:06:17 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 05 Jul 2023 01:06:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jul 2023 01:06:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfda8b0f699ac1265b6331ee0cdbdd3173377a290f6015a85356ffedeb1ec20`  
		Last Modified: Wed, 05 Jul 2023 01:06:51 GMT  
		Size: 17.5 MB (17462308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa89b7dae9239a6274f09393d087befeaa77e5fe8911eff9c8943cfb58366b8`  
		Last Modified: Wed, 05 Jul 2023 01:06:48 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9236fbfc5a0d0427ba7302ddf28dfc01e5b3ab57d4d45590b7fb47df2022b7`  
		Last Modified: Wed, 05 Jul 2023 01:06:55 GMT  
		Size: 43.4 MB (43383929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec7f76680fadfcb98709f2c4de5c2fa4ed5cd35f35426bf7aba155c5cbc8aab`  
		Last Modified: Wed, 05 Jul 2023 01:06:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:6fc76550f4e598229945b2ce995d3137ba54b15b5132d619404a3c097f02ceb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130367185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d952547d261083b16a43ece4b0fe4ed98828dd3d416566fe8e8bd6a5e2145a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 15:24:44 GMT
ENV TELEGRAF_VERSION=1.25.3
# Fri, 28 Jul 2023 15:24:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 15:24:50 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 15:24:50 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 15:24:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 15:24:50 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e114cf56dac555e98c33c0683ca11dc1269682de2de4ba50b585a8b524aad1a`  
		Last Modified: Fri, 28 Jul 2023 15:25:27 GMT  
		Size: 18.6 MB (18598482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114687f558ab848257ff5214c9e4fdd8afd35d551630c7ab76d585d3b3e6a904`  
		Last Modified: Fri, 28 Jul 2023 15:25:25 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0435eaa90a8bf8692e57f392fe52ae2d9e6c6a26458347f392d10de8c36e3459`  
		Last Modified: Fri, 28 Jul 2023 15:25:30 GMT  
		Size: 42.3 MB (42315234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60620bcbad3adc39aa711e68462c71118301f03a8c6e12dcea44cb8d3322b43`  
		Last Modified: Fri, 28 Jul 2023 15:25:25 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25-alpine`

```console
$ docker pull telegraf@sha256:0ab1ee27391df8eca074482b539b9aee5d6b2e6d2986e4040675ea1771c24827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4af6029141ed5e65ebb3f5854545be8804f378158d3ea8ca86cc164cd250f7e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52439734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d95ea10154c5b631dc30528e8022d2b8505ffbabc247b69d8a8c68ea22bf16e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 04:23:01 GMT
ENV TELEGRAF_VERSION=1.25.3
# Thu, 15 Jun 2023 04:23:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 04:23:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 04:23:07 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 04:23:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:08 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb243cfb4afaf2eb52159e92f52f16a523278ba3191a2821105f9bc5ab551e1`  
		Last Modified: Thu, 15 Jun 2023 04:23:59 GMT  
		Size: 46.4 MB (46392665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2908126481e9bcbc296e89036faf1af309d7d7d17c50ccf9d5eab2145d52a5`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.3`

```console
$ docker pull telegraf@sha256:95bec7e2799898a5a74af7f571fa92a858ba9b225add6e898f3887afc968c941
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25.3` - linux; amd64

```console
$ docker pull telegraf@sha256:fa46591962db79212855884747733e3cc158a637e7d80baf1467776fa73b83ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136154894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e572ac884a7ab26c01df29f3ee818981f6d50a95306258080b9a6ec58ce8e183`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 22:55:48 GMT
ENV TELEGRAF_VERSION=1.25.3
# Fri, 28 Jul 2023 22:55:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 22:55:54 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 22:55:54 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 22:55:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 22:55:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73ccc85cd69e3c3e8eeb927b3ed51cce8e63e067e07b960cd5322c4a9ec4c4f`  
		Last Modified: Fri, 28 Jul 2023 22:56:34 GMT  
		Size: 18.8 MB (18759984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7b7a2e9993ee0093c7cfda4148cf0d6f93907c289799b935b5a441d054fe49`  
		Last Modified: Fri, 28 Jul 2023 22:56:31 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3bcc28d801230e7d731f06b9cf43471f30fd17ccf7d8baa3019e2cf9250b38`  
		Last Modified: Fri, 28 Jul 2023 22:56:38 GMT  
		Size: 46.6 MB (46576603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc23e4a59fc82bbfcab465eb5b57eb74c6aad298ad3f1e6e594c9a14a9edddb`  
		Last Modified: Fri, 28 Jul 2023 22:56:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:e5a3f33d9bbbfb6d6da6ecc6c8dd9b35d4919b05a02e80800e393f98cceee092
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125935273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed4c8ef9b020424b130fc10bfeb0da36b4eea824112c50d4231259492dac6907`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Jul 2023 01:06:10 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 05 Jul 2023 01:06:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 05 Jul 2023 01:06:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 05 Jul 2023 01:06:17 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 05 Jul 2023 01:06:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jul 2023 01:06:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfda8b0f699ac1265b6331ee0cdbdd3173377a290f6015a85356ffedeb1ec20`  
		Last Modified: Wed, 05 Jul 2023 01:06:51 GMT  
		Size: 17.5 MB (17462308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa89b7dae9239a6274f09393d087befeaa77e5fe8911eff9c8943cfb58366b8`  
		Last Modified: Wed, 05 Jul 2023 01:06:48 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9236fbfc5a0d0427ba7302ddf28dfc01e5b3ab57d4d45590b7fb47df2022b7`  
		Last Modified: Wed, 05 Jul 2023 01:06:55 GMT  
		Size: 43.4 MB (43383929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec7f76680fadfcb98709f2c4de5c2fa4ed5cd35f35426bf7aba155c5cbc8aab`  
		Last Modified: Wed, 05 Jul 2023 01:06:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:6fc76550f4e598229945b2ce995d3137ba54b15b5132d619404a3c097f02ceb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130367185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d952547d261083b16a43ece4b0fe4ed98828dd3d416566fe8e8bd6a5e2145a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 15:24:44 GMT
ENV TELEGRAF_VERSION=1.25.3
# Fri, 28 Jul 2023 15:24:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 15:24:50 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 15:24:50 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 15:24:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 15:24:50 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e114cf56dac555e98c33c0683ca11dc1269682de2de4ba50b585a8b524aad1a`  
		Last Modified: Fri, 28 Jul 2023 15:25:27 GMT  
		Size: 18.6 MB (18598482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114687f558ab848257ff5214c9e4fdd8afd35d551630c7ab76d585d3b3e6a904`  
		Last Modified: Fri, 28 Jul 2023 15:25:25 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0435eaa90a8bf8692e57f392fe52ae2d9e6c6a26458347f392d10de8c36e3459`  
		Last Modified: Fri, 28 Jul 2023 15:25:30 GMT  
		Size: 42.3 MB (42315234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60620bcbad3adc39aa711e68462c71118301f03a8c6e12dcea44cb8d3322b43`  
		Last Modified: Fri, 28 Jul 2023 15:25:25 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.3-alpine`

```console
$ docker pull telegraf@sha256:0ab1ee27391df8eca074482b539b9aee5d6b2e6d2986e4040675ea1771c24827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4af6029141ed5e65ebb3f5854545be8804f378158d3ea8ca86cc164cd250f7e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52439734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d95ea10154c5b631dc30528e8022d2b8505ffbabc247b69d8a8c68ea22bf16e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 04:23:01 GMT
ENV TELEGRAF_VERSION=1.25.3
# Thu, 15 Jun 2023 04:23:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 04:23:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 04:23:07 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 04:23:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:08 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb243cfb4afaf2eb52159e92f52f16a523278ba3191a2821105f9bc5ab551e1`  
		Last Modified: Thu, 15 Jun 2023 04:23:59 GMT  
		Size: 46.4 MB (46392665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2908126481e9bcbc296e89036faf1af309d7d7d17c50ccf9d5eab2145d52a5`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26`

```console
$ docker pull telegraf@sha256:c7a27527fe0f5f29ed61d236d244e09b2825b8ebc1d6eb3ba7fe0810ebeb02f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26` - linux; amd64

```console
$ docker pull telegraf@sha256:ce2e36aa66216d92d916ff241b1a7c7f3497cdfae9759d4dee210f62a6534599
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140130809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc7ef3f03130f039a8cc8f1c08a6a118cdf925e1aa0b301d41dbf18bbeeb0b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 22:55:59 GMT
ENV TELEGRAF_VERSION=1.26.3
# Fri, 28 Jul 2023 22:56:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 22:56:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 22:56:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 22:56:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 22:56:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73ccc85cd69e3c3e8eeb927b3ed51cce8e63e067e07b960cd5322c4a9ec4c4f`  
		Last Modified: Fri, 28 Jul 2023 22:56:34 GMT  
		Size: 18.8 MB (18759984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7b7a2e9993ee0093c7cfda4148cf0d6f93907c289799b935b5a441d054fe49`  
		Last Modified: Fri, 28 Jul 2023 22:56:31 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e525e78f9d5df6389185640d23907e2114bc09480269fa616bb1eaf68ad65f`  
		Last Modified: Fri, 28 Jul 2023 22:56:56 GMT  
		Size: 50.6 MB (50552519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc9f7a88322f5d662e9a87cf7c930bba0fdb93f8c914f7fc11f0b74682ebdd8`  
		Last Modified: Fri, 28 Jul 2023 22:56:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:840606da11b436734ca65c23617fb15843efcea1a01d69a36a4d168a42c8e900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129834037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc382ad6a1f1e57ce767438f592e602529ed91baecb36e4c049631f3b937feec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Jul 2023 01:06:20 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 05 Jul 2023 01:06:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 05 Jul 2023 01:06:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 05 Jul 2023 01:06:27 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 05 Jul 2023 01:06:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jul 2023 01:06:27 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfda8b0f699ac1265b6331ee0cdbdd3173377a290f6015a85356ffedeb1ec20`  
		Last Modified: Wed, 05 Jul 2023 01:06:51 GMT  
		Size: 17.5 MB (17462308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa89b7dae9239a6274f09393d087befeaa77e5fe8911eff9c8943cfb58366b8`  
		Last Modified: Wed, 05 Jul 2023 01:06:48 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b70a869c125fdab55b15096858869aefa7c633f42249561c19f4c42a66ea0c3`  
		Last Modified: Wed, 05 Jul 2023 01:07:13 GMT  
		Size: 47.3 MB (47282695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f4ce765de627e0d65afb049354176352bfc2bf36cffd06e9430dd4876d8ee4`  
		Last Modified: Wed, 05 Jul 2023 01:07:05 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ccecd566b92d49ebf06da721332b971f1d15c7ce21135e699de363ad1bb1e21a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134023817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:039c11b4dea41198805125f4e272c3207b0a4334410f2573a1bf293f5454f52c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 15:24:53 GMT
ENV TELEGRAF_VERSION=1.26.3
# Fri, 28 Jul 2023 15:24:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 15:24:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 15:24:59 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 15:24:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 15:24:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e114cf56dac555e98c33c0683ca11dc1269682de2de4ba50b585a8b524aad1a`  
		Last Modified: Fri, 28 Jul 2023 15:25:27 GMT  
		Size: 18.6 MB (18598482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114687f558ab848257ff5214c9e4fdd8afd35d551630c7ab76d585d3b3e6a904`  
		Last Modified: Fri, 28 Jul 2023 15:25:25 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276468cf5adff7cde1de4359f6c7dd74add83d2682673e4010e96ba5711c18fd`  
		Last Modified: Fri, 28 Jul 2023 15:25:45 GMT  
		Size: 46.0 MB (45971868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fb83a18aaf827751254384f3dc2c48592fa3f7a2c1b97fb67d44da62866126`  
		Last Modified: Fri, 28 Jul 2023 15:25:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26-alpine`

```console
$ docker pull telegraf@sha256:d7670fca45a2fa0c153447618c85b9648ee58b55b0e4c9803ed5ede3ae027160
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4fe69f57d5b57f7419e6120e28b665bcaa4bd1b25e0e29c38ddd44c6219f33af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56439016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b17e2edadcd01dd98f9dcd6f7f9f21fc64ae2cc415a8ea360fdb844ebcd82ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 04:23:13 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 15 Jun 2023 04:23:21 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 04:23:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 04:23:22 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 04:23:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18990458155a92d1fb3fae8eed5615af4d63beeb00fa44a5fbd158977f7ef425`  
		Last Modified: Thu, 15 Jun 2023 04:24:18 GMT  
		Size: 50.4 MB (50391945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4274a4d20dcdf6dd563418735d039dffa8131530660a69c32270923f6c62b9ea`  
		Last Modified: Thu, 15 Jun 2023 04:24:09 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:5de71a2aa2f231e2710b08014fadaece7fae2a0dec3d6deee41269608eef2c55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d87a2fbcaeb6bd28afc599e0c730ea53207fed335061771bd62f9408750015`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 07:08:51 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 07:08:51 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 15 Jun 2023 07:08:58 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 07:08:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 07:08:59 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 07:08:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 07:08:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533040d8d2939a14e08289606aa07e7e8b93b273b0cc9bbdc66c5e5bae7901dd`  
		Last Modified: Thu, 15 Jun 2023 07:09:27 GMT  
		Size: 2.7 MB (2703885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75ae3de250799144d4a3ad82b891ea2058ef091277e638c7c82e4609d815a8e`  
		Last Modified: Thu, 15 Jun 2023 07:09:31 GMT  
		Size: 45.8 MB (45812293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f27b13bf3f7b32f2842c148833f64deb24dead30665ae31f7224f4313ba9872`  
		Last Modified: Thu, 15 Jun 2023 07:09:26 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3`

```console
$ docker pull telegraf@sha256:c7a27527fe0f5f29ed61d236d244e09b2825b8ebc1d6eb3ba7fe0810ebeb02f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26.3` - linux; amd64

```console
$ docker pull telegraf@sha256:ce2e36aa66216d92d916ff241b1a7c7f3497cdfae9759d4dee210f62a6534599
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140130809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc7ef3f03130f039a8cc8f1c08a6a118cdf925e1aa0b301d41dbf18bbeeb0b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 22:55:59 GMT
ENV TELEGRAF_VERSION=1.26.3
# Fri, 28 Jul 2023 22:56:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 22:56:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 22:56:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 22:56:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 22:56:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73ccc85cd69e3c3e8eeb927b3ed51cce8e63e067e07b960cd5322c4a9ec4c4f`  
		Last Modified: Fri, 28 Jul 2023 22:56:34 GMT  
		Size: 18.8 MB (18759984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7b7a2e9993ee0093c7cfda4148cf0d6f93907c289799b935b5a441d054fe49`  
		Last Modified: Fri, 28 Jul 2023 22:56:31 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e525e78f9d5df6389185640d23907e2114bc09480269fa616bb1eaf68ad65f`  
		Last Modified: Fri, 28 Jul 2023 22:56:56 GMT  
		Size: 50.6 MB (50552519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc9f7a88322f5d662e9a87cf7c930bba0fdb93f8c914f7fc11f0b74682ebdd8`  
		Last Modified: Fri, 28 Jul 2023 22:56:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:840606da11b436734ca65c23617fb15843efcea1a01d69a36a4d168a42c8e900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129834037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc382ad6a1f1e57ce767438f592e602529ed91baecb36e4c049631f3b937feec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Jul 2023 01:06:20 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 05 Jul 2023 01:06:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 05 Jul 2023 01:06:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 05 Jul 2023 01:06:27 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 05 Jul 2023 01:06:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Jul 2023 01:06:27 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfda8b0f699ac1265b6331ee0cdbdd3173377a290f6015a85356ffedeb1ec20`  
		Last Modified: Wed, 05 Jul 2023 01:06:51 GMT  
		Size: 17.5 MB (17462308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa89b7dae9239a6274f09393d087befeaa77e5fe8911eff9c8943cfb58366b8`  
		Last Modified: Wed, 05 Jul 2023 01:06:48 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b70a869c125fdab55b15096858869aefa7c633f42249561c19f4c42a66ea0c3`  
		Last Modified: Wed, 05 Jul 2023 01:07:13 GMT  
		Size: 47.3 MB (47282695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f4ce765de627e0d65afb049354176352bfc2bf36cffd06e9430dd4876d8ee4`  
		Last Modified: Wed, 05 Jul 2023 01:07:05 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ccecd566b92d49ebf06da721332b971f1d15c7ce21135e699de363ad1bb1e21a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134023817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:039c11b4dea41198805125f4e272c3207b0a4334410f2573a1bf293f5454f52c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 15:24:53 GMT
ENV TELEGRAF_VERSION=1.26.3
# Fri, 28 Jul 2023 15:24:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 15:24:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 15:24:59 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 15:24:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 15:24:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e114cf56dac555e98c33c0683ca11dc1269682de2de4ba50b585a8b524aad1a`  
		Last Modified: Fri, 28 Jul 2023 15:25:27 GMT  
		Size: 18.6 MB (18598482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114687f558ab848257ff5214c9e4fdd8afd35d551630c7ab76d585d3b3e6a904`  
		Last Modified: Fri, 28 Jul 2023 15:25:25 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276468cf5adff7cde1de4359f6c7dd74add83d2682673e4010e96ba5711c18fd`  
		Last Modified: Fri, 28 Jul 2023 15:25:45 GMT  
		Size: 46.0 MB (45971868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fb83a18aaf827751254384f3dc2c48592fa3f7a2c1b97fb67d44da62866126`  
		Last Modified: Fri, 28 Jul 2023 15:25:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3-alpine`

```console
$ docker pull telegraf@sha256:d7670fca45a2fa0c153447618c85b9648ee58b55b0e4c9803ed5ede3ae027160
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4fe69f57d5b57f7419e6120e28b665bcaa4bd1b25e0e29c38ddd44c6219f33af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56439016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b17e2edadcd01dd98f9dcd6f7f9f21fc64ae2cc415a8ea360fdb844ebcd82ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 04:23:13 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 15 Jun 2023 04:23:21 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 04:23:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 04:23:22 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 04:23:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18990458155a92d1fb3fae8eed5615af4d63beeb00fa44a5fbd158977f7ef425`  
		Last Modified: Thu, 15 Jun 2023 04:24:18 GMT  
		Size: 50.4 MB (50391945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4274a4d20dcdf6dd563418735d039dffa8131530660a69c32270923f6c62b9ea`  
		Last Modified: Thu, 15 Jun 2023 04:24:09 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:5de71a2aa2f231e2710b08014fadaece7fae2a0dec3d6deee41269608eef2c55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d87a2fbcaeb6bd28afc599e0c730ea53207fed335061771bd62f9408750015`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 07:08:51 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 07:08:51 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 15 Jun 2023 07:08:58 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 07:08:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 07:08:59 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 07:08:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 07:08:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533040d8d2939a14e08289606aa07e7e8b93b273b0cc9bbdc66c5e5bae7901dd`  
		Last Modified: Thu, 15 Jun 2023 07:09:27 GMT  
		Size: 2.7 MB (2703885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75ae3de250799144d4a3ad82b891ea2058ef091277e638c7c82e4609d815a8e`  
		Last Modified: Thu, 15 Jun 2023 07:09:31 GMT  
		Size: 45.8 MB (45812293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f27b13bf3f7b32f2842c148833f64deb24dead30665ae31f7224f4313ba9872`  
		Last Modified: Thu, 15 Jun 2023 07:09:26 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27`

```console
$ docker pull telegraf@sha256:27d57ae691d0ba4eadca94fa41ae8d36d9730b40b83e9a3f5aa2534965a8a296
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27` - linux; amd64

```console
$ docker pull telegraf@sha256:eadb41446e53ee0c11d6f63d8cd0b10a27daa9c072b304a3fc99bd6c326114cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.7 MB (144715727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c738368acf9af09b71cbb2e4b940b70c72179ce9ebcc66462243f8946aaa32f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 22:56:09 GMT
ENV TELEGRAF_VERSION=1.27.2
# Fri, 28 Jul 2023 22:56:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 22:56:14 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 22:56:14 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 22:56:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 22:56:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73ccc85cd69e3c3e8eeb927b3ed51cce8e63e067e07b960cd5322c4a9ec4c4f`  
		Last Modified: Fri, 28 Jul 2023 22:56:34 GMT  
		Size: 18.8 MB (18759984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7b7a2e9993ee0093c7cfda4148cf0d6f93907c289799b935b5a441d054fe49`  
		Last Modified: Fri, 28 Jul 2023 22:56:31 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d9d585254805d2a03bdbb6c06fa00b01af9411e4d0d4fbef10a5ca7eed8480`  
		Last Modified: Fri, 28 Jul 2023 22:57:15 GMT  
		Size: 55.1 MB (55137437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bec0b7000b10a29e0ba156f2d61f21f4e2b644b4bfad98a7275927f7f845bf`  
		Last Modified: Fri, 28 Jul 2023 22:57:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:d2365c99798e0b091a62fb4c52f315fd8de1c3f32c998af518033a486d794877
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133858062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5e2d15f505c0b1757b4c80934dbcbe2dd6aa9442491c1d359292f357d0b58e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 11 Jul 2023 05:07:08 GMT
ENV TELEGRAF_VERSION=1.27.2
# Tue, 11 Jul 2023 05:07:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 11 Jul 2023 05:07:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 11 Jul 2023 05:07:16 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 11 Jul 2023 05:07:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 11 Jul 2023 05:07:16 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfda8b0f699ac1265b6331ee0cdbdd3173377a290f6015a85356ffedeb1ec20`  
		Last Modified: Wed, 05 Jul 2023 01:06:51 GMT  
		Size: 17.5 MB (17462308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa89b7dae9239a6274f09393d087befeaa77e5fe8911eff9c8943cfb58366b8`  
		Last Modified: Wed, 05 Jul 2023 01:06:48 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2d4e68d094ea84a9a7c0c91a8d968c3224030d44d7cd71c9f184b63b3380b8`  
		Last Modified: Tue, 11 Jul 2023 05:07:39 GMT  
		Size: 51.3 MB (51306718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ca8f4bbc2e0014446fe7b17e1ea186a797c167651ffca5d83fe05aa36e3a29`  
		Last Modified: Tue, 11 Jul 2023 05:07:30 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:62a7115341793adc0e0050abbd738e96ebfca29f3bc7621413f9c4105989e1e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137832876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:230499293a34269db84b30e560360874b636ccd2b9fbe1f1db7197329bb1d528`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 15:25:03 GMT
ENV TELEGRAF_VERSION=1.27.2
# Fri, 28 Jul 2023 15:25:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 15:25:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 15:25:12 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 15:25:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 15:25:12 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e114cf56dac555e98c33c0683ca11dc1269682de2de4ba50b585a8b524aad1a`  
		Last Modified: Fri, 28 Jul 2023 15:25:27 GMT  
		Size: 18.6 MB (18598482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114687f558ab848257ff5214c9e4fdd8afd35d551630c7ab76d585d3b3e6a904`  
		Last Modified: Fri, 28 Jul 2023 15:25:25 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62165e595008d16238c6a369f73ad5574dc69344c5b1737730fc6acf7e5a94b`  
		Last Modified: Fri, 28 Jul 2023 15:26:01 GMT  
		Size: 49.8 MB (49780926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f453ed256d7785864919a8609b693dbcef325710a895c2009209a893ff0729`  
		Last Modified: Fri, 28 Jul 2023 15:25:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27-alpine`

```console
$ docker pull telegraf@sha256:5e4c2d9bbd259e0328919dc28835e6990d77bc89ab05cbe15a220721533bbed0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.27-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:341a881442b046004f35d3aa6b20d0ee04e8234a81bb86ff9845e36991a241ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61025922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cacf48f1c67211b7cf2cc493b7be0822031b5084da7b852e0009774a0ede478`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 11 Jul 2023 00:00:17 GMT
ENV TELEGRAF_VERSION=1.27.2
# Tue, 11 Jul 2023 00:00:23 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 11 Jul 2023 00:00:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 11 Jul 2023 00:00:23 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 11 Jul 2023 00:00:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 11 Jul 2023 00:00:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89955b5b2cc13736c3a27fd19d504e05265fc851fdae096f124663d5653d97b2`  
		Last Modified: Tue, 11 Jul 2023 00:01:15 GMT  
		Size: 55.0 MB (54978851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0ccdedf6a34a048960749fa035ddd11d0c5311643c3251540034f7d9e331f4`  
		Last Modified: Tue, 11 Jul 2023 00:01:07 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:55624a16b5d87b95d311c43c4c789d823c341b2ce7adf9281b7a6b3793bedb9e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55568046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c9a19a54adce30c1e4b618ac1797919064ed0a5b2b0cdd5cf062de743d671c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 07:08:51 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 11 Jul 2023 01:05:15 GMT
ENV TELEGRAF_VERSION=1.27.2
# Tue, 11 Jul 2023 01:05:21 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 11 Jul 2023 01:05:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 11 Jul 2023 01:05:23 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 11 Jul 2023 01:05:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 11 Jul 2023 01:05:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533040d8d2939a14e08289606aa07e7e8b93b273b0cc9bbdc66c5e5bae7901dd`  
		Last Modified: Thu, 15 Jun 2023 07:09:27 GMT  
		Size: 2.7 MB (2703885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae15e8643d4c4ebb01c83fa7dbf1b92fc0ccbfb87f5d9d71f982ed21a72582`  
		Last Modified: Tue, 11 Jul 2023 01:06:02 GMT  
		Size: 49.6 MB (49602419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3651c1cad2aa1e349408e063be9cc68e454d0cd037574677aaf74078488e94e`  
		Last Modified: Tue, 11 Jul 2023 01:05:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27.2`

```console
$ docker pull telegraf@sha256:27d57ae691d0ba4eadca94fa41ae8d36d9730b40b83e9a3f5aa2534965a8a296
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27.2` - linux; amd64

```console
$ docker pull telegraf@sha256:eadb41446e53ee0c11d6f63d8cd0b10a27daa9c072b304a3fc99bd6c326114cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.7 MB (144715727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c738368acf9af09b71cbb2e4b940b70c72179ce9ebcc66462243f8946aaa32f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 22:56:09 GMT
ENV TELEGRAF_VERSION=1.27.2
# Fri, 28 Jul 2023 22:56:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 22:56:14 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 22:56:14 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 22:56:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 22:56:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73ccc85cd69e3c3e8eeb927b3ed51cce8e63e067e07b960cd5322c4a9ec4c4f`  
		Last Modified: Fri, 28 Jul 2023 22:56:34 GMT  
		Size: 18.8 MB (18759984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7b7a2e9993ee0093c7cfda4148cf0d6f93907c289799b935b5a441d054fe49`  
		Last Modified: Fri, 28 Jul 2023 22:56:31 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d9d585254805d2a03bdbb6c06fa00b01af9411e4d0d4fbef10a5ca7eed8480`  
		Last Modified: Fri, 28 Jul 2023 22:57:15 GMT  
		Size: 55.1 MB (55137437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bec0b7000b10a29e0ba156f2d61f21f4e2b644b4bfad98a7275927f7f845bf`  
		Last Modified: Fri, 28 Jul 2023 22:57:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.2` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:d2365c99798e0b091a62fb4c52f315fd8de1c3f32c998af518033a486d794877
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133858062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5e2d15f505c0b1757b4c80934dbcbe2dd6aa9442491c1d359292f357d0b58e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 11 Jul 2023 05:07:08 GMT
ENV TELEGRAF_VERSION=1.27.2
# Tue, 11 Jul 2023 05:07:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 11 Jul 2023 05:07:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 11 Jul 2023 05:07:16 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 11 Jul 2023 05:07:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 11 Jul 2023 05:07:16 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfda8b0f699ac1265b6331ee0cdbdd3173377a290f6015a85356ffedeb1ec20`  
		Last Modified: Wed, 05 Jul 2023 01:06:51 GMT  
		Size: 17.5 MB (17462308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa89b7dae9239a6274f09393d087befeaa77e5fe8911eff9c8943cfb58366b8`  
		Last Modified: Wed, 05 Jul 2023 01:06:48 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2d4e68d094ea84a9a7c0c91a8d968c3224030d44d7cd71c9f184b63b3380b8`  
		Last Modified: Tue, 11 Jul 2023 05:07:39 GMT  
		Size: 51.3 MB (51306718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ca8f4bbc2e0014446fe7b17e1ea186a797c167651ffca5d83fe05aa36e3a29`  
		Last Modified: Tue, 11 Jul 2023 05:07:30 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.2` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:62a7115341793adc0e0050abbd738e96ebfca29f3bc7621413f9c4105989e1e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137832876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:230499293a34269db84b30e560360874b636ccd2b9fbe1f1db7197329bb1d528`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 15:25:03 GMT
ENV TELEGRAF_VERSION=1.27.2
# Fri, 28 Jul 2023 15:25:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 15:25:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 15:25:12 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 15:25:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 15:25:12 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e114cf56dac555e98c33c0683ca11dc1269682de2de4ba50b585a8b524aad1a`  
		Last Modified: Fri, 28 Jul 2023 15:25:27 GMT  
		Size: 18.6 MB (18598482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114687f558ab848257ff5214c9e4fdd8afd35d551630c7ab76d585d3b3e6a904`  
		Last Modified: Fri, 28 Jul 2023 15:25:25 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62165e595008d16238c6a369f73ad5574dc69344c5b1737730fc6acf7e5a94b`  
		Last Modified: Fri, 28 Jul 2023 15:26:01 GMT  
		Size: 49.8 MB (49780926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f453ed256d7785864919a8609b693dbcef325710a895c2009209a893ff0729`  
		Last Modified: Fri, 28 Jul 2023 15:25:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27.2-alpine`

```console
$ docker pull telegraf@sha256:5e4c2d9bbd259e0328919dc28835e6990d77bc89ab05cbe15a220721533bbed0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.27.2-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:341a881442b046004f35d3aa6b20d0ee04e8234a81bb86ff9845e36991a241ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61025922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cacf48f1c67211b7cf2cc493b7be0822031b5084da7b852e0009774a0ede478`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 11 Jul 2023 00:00:17 GMT
ENV TELEGRAF_VERSION=1.27.2
# Tue, 11 Jul 2023 00:00:23 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 11 Jul 2023 00:00:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 11 Jul 2023 00:00:23 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 11 Jul 2023 00:00:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 11 Jul 2023 00:00:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89955b5b2cc13736c3a27fd19d504e05265fc851fdae096f124663d5653d97b2`  
		Last Modified: Tue, 11 Jul 2023 00:01:15 GMT  
		Size: 55.0 MB (54978851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0ccdedf6a34a048960749fa035ddd11d0c5311643c3251540034f7d9e331f4`  
		Last Modified: Tue, 11 Jul 2023 00:01:07 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.2-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:55624a16b5d87b95d311c43c4c789d823c341b2ce7adf9281b7a6b3793bedb9e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55568046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c9a19a54adce30c1e4b618ac1797919064ed0a5b2b0cdd5cf062de743d671c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 07:08:51 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 11 Jul 2023 01:05:15 GMT
ENV TELEGRAF_VERSION=1.27.2
# Tue, 11 Jul 2023 01:05:21 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 11 Jul 2023 01:05:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 11 Jul 2023 01:05:23 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 11 Jul 2023 01:05:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 11 Jul 2023 01:05:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533040d8d2939a14e08289606aa07e7e8b93b273b0cc9bbdc66c5e5bae7901dd`  
		Last Modified: Thu, 15 Jun 2023 07:09:27 GMT  
		Size: 2.7 MB (2703885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae15e8643d4c4ebb01c83fa7dbf1b92fc0ccbfb87f5d9d71f982ed21a72582`  
		Last Modified: Tue, 11 Jul 2023 01:06:02 GMT  
		Size: 49.6 MB (49602419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3651c1cad2aa1e349408e063be9cc68e454d0cd037574677aaf74078488e94e`  
		Last Modified: Tue, 11 Jul 2023 01:05:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:5e4c2d9bbd259e0328919dc28835e6990d77bc89ab05cbe15a220721533bbed0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:341a881442b046004f35d3aa6b20d0ee04e8234a81bb86ff9845e36991a241ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61025922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cacf48f1c67211b7cf2cc493b7be0822031b5084da7b852e0009774a0ede478`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 11 Jul 2023 00:00:17 GMT
ENV TELEGRAF_VERSION=1.27.2
# Tue, 11 Jul 2023 00:00:23 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 11 Jul 2023 00:00:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 11 Jul 2023 00:00:23 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 11 Jul 2023 00:00:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 11 Jul 2023 00:00:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89955b5b2cc13736c3a27fd19d504e05265fc851fdae096f124663d5653d97b2`  
		Last Modified: Tue, 11 Jul 2023 00:01:15 GMT  
		Size: 55.0 MB (54978851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0ccdedf6a34a048960749fa035ddd11d0c5311643c3251540034f7d9e331f4`  
		Last Modified: Tue, 11 Jul 2023 00:01:07 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:55624a16b5d87b95d311c43c4c789d823c341b2ce7adf9281b7a6b3793bedb9e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55568046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c9a19a54adce30c1e4b618ac1797919064ed0a5b2b0cdd5cf062de743d671c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 07:08:51 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 11 Jul 2023 01:05:15 GMT
ENV TELEGRAF_VERSION=1.27.2
# Tue, 11 Jul 2023 01:05:21 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 11 Jul 2023 01:05:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 11 Jul 2023 01:05:23 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 11 Jul 2023 01:05:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 11 Jul 2023 01:05:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533040d8d2939a14e08289606aa07e7e8b93b273b0cc9bbdc66c5e5bae7901dd`  
		Last Modified: Thu, 15 Jun 2023 07:09:27 GMT  
		Size: 2.7 MB (2703885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae15e8643d4c4ebb01c83fa7dbf1b92fc0ccbfb87f5d9d71f982ed21a72582`  
		Last Modified: Tue, 11 Jul 2023 01:06:02 GMT  
		Size: 49.6 MB (49602419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3651c1cad2aa1e349408e063be9cc68e454d0cd037574677aaf74078488e94e`  
		Last Modified: Tue, 11 Jul 2023 01:05:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:27d57ae691d0ba4eadca94fa41ae8d36d9730b40b83e9a3f5aa2534965a8a296
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:eadb41446e53ee0c11d6f63d8cd0b10a27daa9c072b304a3fc99bd6c326114cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.7 MB (144715727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c738368acf9af09b71cbb2e4b940b70c72179ce9ebcc66462243f8946aaa32f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:47 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 22:55:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 22:56:09 GMT
ENV TELEGRAF_VERSION=1.27.2
# Fri, 28 Jul 2023 22:56:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 22:56:14 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 22:56:14 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 22:56:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 22:56:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73ccc85cd69e3c3e8eeb927b3ed51cce8e63e067e07b960cd5322c4a9ec4c4f`  
		Last Modified: Fri, 28 Jul 2023 22:56:34 GMT  
		Size: 18.8 MB (18759984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7b7a2e9993ee0093c7cfda4148cf0d6f93907c289799b935b5a441d054fe49`  
		Last Modified: Fri, 28 Jul 2023 22:56:31 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d9d585254805d2a03bdbb6c06fa00b01af9411e4d0d4fbef10a5ca7eed8480`  
		Last Modified: Fri, 28 Jul 2023 22:57:15 GMT  
		Size: 55.1 MB (55137437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bec0b7000b10a29e0ba156f2d61f21f4e2b644b4bfad98a7275927f7f845bf`  
		Last Modified: Fri, 28 Jul 2023 22:57:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:d2365c99798e0b091a62fb4c52f315fd8de1c3f32c998af518033a486d794877
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133858062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5e2d15f505c0b1757b4c80934dbcbe2dd6aa9442491c1d359292f357d0b58e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:08 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 01:06:09 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 11 Jul 2023 05:07:08 GMT
ENV TELEGRAF_VERSION=1.27.2
# Tue, 11 Jul 2023 05:07:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 11 Jul 2023 05:07:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 11 Jul 2023 05:07:16 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 11 Jul 2023 05:07:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 11 Jul 2023 05:07:16 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfda8b0f699ac1265b6331ee0cdbdd3173377a290f6015a85356ffedeb1ec20`  
		Last Modified: Wed, 05 Jul 2023 01:06:51 GMT  
		Size: 17.5 MB (17462308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa89b7dae9239a6274f09393d087befeaa77e5fe8911eff9c8943cfb58366b8`  
		Last Modified: Wed, 05 Jul 2023 01:06:48 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2d4e68d094ea84a9a7c0c91a8d968c3224030d44d7cd71c9f184b63b3380b8`  
		Last Modified: Tue, 11 Jul 2023 05:07:39 GMT  
		Size: 51.3 MB (51306718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ca8f4bbc2e0014446fe7b17e1ea186a797c167651ffca5d83fe05aa36e3a29`  
		Last Modified: Tue, 11 Jul 2023 05:07:30 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:62a7115341793adc0e0050abbd738e96ebfca29f3bc7621413f9c4105989e1e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137832876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:230499293a34269db84b30e560360874b636ccd2b9fbe1f1db7197329bb1d528`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:43 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:24:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 28 Jul 2023 15:25:03 GMT
ENV TELEGRAF_VERSION=1.27.2
# Fri, 28 Jul 2023 15:25:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 28 Jul 2023 15:25:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 28 Jul 2023 15:25:12 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 28 Jul 2023 15:25:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Jul 2023 15:25:12 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e114cf56dac555e98c33c0683ca11dc1269682de2de4ba50b585a8b524aad1a`  
		Last Modified: Fri, 28 Jul 2023 15:25:27 GMT  
		Size: 18.6 MB (18598482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114687f558ab848257ff5214c9e4fdd8afd35d551630c7ab76d585d3b3e6a904`  
		Last Modified: Fri, 28 Jul 2023 15:25:25 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62165e595008d16238c6a369f73ad5574dc69344c5b1737730fc6acf7e5a94b`  
		Last Modified: Fri, 28 Jul 2023 15:26:01 GMT  
		Size: 49.8 MB (49780926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f453ed256d7785864919a8609b693dbcef325710a895c2009209a893ff0729`  
		Last Modified: Fri, 28 Jul 2023 15:25:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
