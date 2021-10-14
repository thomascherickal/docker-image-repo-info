## `telegraf:latest`

```console
$ docker pull telegraf@sha256:e627603c8fbf01b26faa5fd832c9ce5fd12a423d5a90df7f7c4d2143eeeb7d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:d7de36f6c04825144b45189eba7c0b363ecb08e63a3a7c8572d8dcf1b4eca73d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120438552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36bdd348ca3bd084087c93bbb35ece214e69dcd1e17d86389e9a9950e6ba4c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:44:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:44:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 10:25:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 10:25:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 10:26:24 GMT
ENV TELEGRAF_VERSION=1.20.2
# Wed, 13 Oct 2021 10:26:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 10:26:28 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 10:26:29 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 10:26:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 10:26:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cef1aa2170c001b320769bf8b018ed82d2c94a673e3010ea1ffe152e107419`  
		Last Modified: Tue, 12 Oct 2021 15:54:16 GMT  
		Size: 7.8 MB (7833862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a51f13be8e69cfc526b671d0bbf621b985b0932acd1523050e2995777b5926`  
		Last Modified: Tue, 12 Oct 2021 15:54:17 GMT  
		Size: 10.0 MB (9997204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91a466291d423e3faad6a8be6ae82e4a4d0550acb67989ac71c98f900e74d41`  
		Last Modified: Wed, 13 Oct 2021 10:26:55 GMT  
		Size: 17.4 MB (17415387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77934da0dce5bef46b239a3871787c2962a08cf1c8b1e629282f0c617b46426`  
		Last Modified: Wed, 13 Oct 2021 10:26:52 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fe40b78b74cb29485f43d826630febe77421a130fc3a60e984efee2d0cacca`  
		Last Modified: Wed, 13 Oct 2021 10:27:32 GMT  
		Size: 34.8 MB (34752317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b39af786583bce9560759a1517b19efa4b4d9a1a5a9f2613af7358365db368`  
		Last Modified: Wed, 13 Oct 2021 10:27:26 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:1095e724ff8b62ca04c45c86c617eb7fda3a1949be4a31a97f3a3d6871b5695d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110968719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6367f3beba90bfac51b16bf4bd246bf3117f537226d643b0ee0267b158a791eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:06 GMT
ADD file:b1857dc4fe4fbc4af220829cc6af7169c4555d3f63a3a304db6fa0146b1d5539 in / 
# Tue, 12 Oct 2021 01:29:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:39:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 15:31:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 15:31:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 15:31:57 GMT
ENV TELEGRAF_VERSION=1.20.2
# Wed, 13 Oct 2021 15:32:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 15:32:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 15:32:10 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 15:32:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 15:32:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:139a906e9407e96c50669130c30fe8fba2681b14aa838a3e52f8753b566ef1c8`  
		Last Modified: Tue, 12 Oct 2021 01:45:13 GMT  
		Size: 45.9 MB (45917899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3907051e2154d5bd4ad15141b8938bc09674039787512494a99b93fd4ebc088d`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 7.1 MB (7125242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8651d4793d5f4d465002213d2d462c964aaf8665a87d5f9cc0de7384f10eeb10`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 9.3 MB (9343819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e659684a04aace7b984a69bccde2a720cb53304f8905d65b9068605177b2a4b6`  
		Last Modified: Wed, 13 Oct 2021 15:33:06 GMT  
		Size: 16.2 MB (16161376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc86d346babddcb58c40b9188fc289d120a16518eed1782662459497e55f179`  
		Last Modified: Wed, 13 Oct 2021 15:32:54 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ab61c37e049992dec37a6aba62a2046c0218ac8e88f196d8f297335e469910`  
		Last Modified: Wed, 13 Oct 2021 15:34:22 GMT  
		Size: 32.4 MB (32417295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7392c9c96023c85c1c1c8747fddf4b44295a00702e98de30a55891277c55c92`  
		Last Modified: Wed, 13 Oct 2021 15:33:59 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ede9cc91f56999d79f7ade2f368a7f54834f1ec53fdc06bb814a769dd0e97e7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115595211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef51bd0a527d8c746e852ef6bb675fa3e73024901101a53babc07979e925cbc2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:11:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:11:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 19:45:40 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 01:08:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 14 Oct 2021 01:09:01 GMT
ENV TELEGRAF_VERSION=1.20.2
# Thu, 14 Oct 2021 01:09:11 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 14 Oct 2021 01:09:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 14 Oct 2021 01:09:13 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 14 Oct 2021 01:09:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 Oct 2021 01:09:14 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bebdb41abf00ce2793427be3560666b324dbc582685d67cbd222fd9a96c780`  
		Last Modified: Tue, 12 Oct 2021 02:20:12 GMT  
		Size: 7.7 MB (7696033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67efbd5f352709c5700a9d20834d4ba77810ddf79e37c3802037f213ffc2d375`  
		Last Modified: Tue, 12 Oct 2021 02:20:12 GMT  
		Size: 10.0 MB (9984354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f511852f4dee84af3adfeba8528e62a31fd9b3622a82e8abc2fb978220886a`  
		Last Modified: Thu, 14 Oct 2021 01:09:42 GMT  
		Size: 17.1 MB (17058979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd486e63e91bfb1f2430bd3b78d815b753e87b1671702287d76ee574c452b056`  
		Last Modified: Thu, 14 Oct 2021 01:09:38 GMT  
		Size: 2.9 KB (2876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec860f43c6efe7cdeded8f3ac86050da3f62188c8dc2967f8a29a36a2d7c9e4`  
		Last Modified: Thu, 14 Oct 2021 01:10:16 GMT  
		Size: 31.6 MB (31630028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2239e9294b066de186434c8361531c5dd846cdff3f509d9f81a99c2721d22fc6`  
		Last Modified: Thu, 14 Oct 2021 01:10:10 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
