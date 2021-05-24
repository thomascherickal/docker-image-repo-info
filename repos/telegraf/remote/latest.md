## `telegraf:latest`

```console
$ docker pull telegraf@sha256:1dc03cb51f8a998b0ddfd369f93bcbccceaa4ac0af679423bb50b1f994511f31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:a7cd5ce39fe3285b2fcb40b84919d9556319d5caceab5945e7fca1fb1316938f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115488527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:870ee38129f8445492e28f0bcab38e1b212de617e813dac5645ab81f510dd435`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 13 May 2021 01:53:29 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 13 May 2021 01:53:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Mon, 24 May 2021 19:45:45 GMT
ENV TELEGRAF_VERSION=1.18.3
# Mon, 24 May 2021 19:45:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 24 May 2021 19:45:50 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 24 May 2021 19:45:51 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Mon, 24 May 2021 19:45:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 May 2021 19:45:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a673b7ce359ffba067166d571714630151228ab4091c835a238a9f7a115fdb2e`  
		Last Modified: Thu, 13 May 2021 01:54:21 GMT  
		Size: 17.4 MB (17414412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b810804dad08ec7b108bac304d8ed669a376f34ba6f13f02cdc33ddbb7ba5687`  
		Last Modified: Thu, 13 May 2021 01:54:18 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e979ae447c6193b2ba6c1d636d4096abe6b0c02e6bfc9e8042a6b5f8a9773bd4`  
		Last Modified: Mon, 24 May 2021 19:46:31 GMT  
		Size: 29.8 MB (29807698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe315ae1e3a6df546cd07b837168e37d47d0c1e9dbc144d3e2d9c2d570ea88`  
		Last Modified: Mon, 24 May 2021 19:46:24 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:8ceae0f513b459ad9c6faf80f4a70cd83ad4aa91ae1f1817aef7bac94922ec34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102322235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9004c1a7d157ad73be0ce83beba1ef6bd374c8a6f76664560ea62bec2f09db5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 May 2021 01:02:10 GMT
ADD file:51a0472692adf18117444dc1f35d6eb3b4d6d672f28a7f6631f9d5d269b0b85d in / 
# Wed, 12 May 2021 01:02:15 GMT
CMD ["bash"]
# Wed, 12 May 2021 03:44:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 03:44:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 13 May 2021 04:00:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 13 May 2021 04:00:26 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 13 May 2021 04:01:09 GMT
ENV TELEGRAF_VERSION=1.18.2
# Thu, 13 May 2021 04:01:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 13 May 2021 04:01:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 13 May 2021 04:01:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 13 May 2021 04:01:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 13 May 2021 04:01:21 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:89475607b1df9fc7eec7efe2fa845738a16cee3e92c1bb864c1f5a93b8303bc6`  
		Last Modified: Wed, 12 May 2021 01:18:49 GMT  
		Size: 45.9 MB (45916922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60b392acef5d5734279504aa16b720c25b67a3e59b224c69c0cc9ac9772919f`  
		Last Modified: Wed, 12 May 2021 04:01:04 GMT  
		Size: 7.1 MB (7124103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf29c9b0911c9aaa2561392012c561157f1029b7078a0f62be5c13b4a8711f6`  
		Last Modified: Wed, 12 May 2021 04:01:04 GMT  
		Size: 9.3 MB (9343805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a242445aeb590a52c8febe4ebf6e9b77f3cb1a5c1cc63f4071ad511305d30316`  
		Last Modified: Thu, 13 May 2021 04:01:45 GMT  
		Size: 16.2 MB (16159119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eeef6cb10d57085d6117e2e85c7abe805b3e90a8e231b67f1b7f04e519e43f`  
		Last Modified: Thu, 13 May 2021 04:01:40 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee75ea67044dff548affc8e7c753bdccdad46d36e07679a15e1a616128290b29`  
		Last Modified: Thu, 13 May 2021 04:02:15 GMT  
		Size: 23.8 MB (23775198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819619127f72b39ae67788dfdaba46d7d8dd23deaeb81ed896e74915ec5754ac`  
		Last Modified: Thu, 13 May 2021 04:02:07 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:6b7dec78773d41eedbcaf33a6f3a700e0f006ba9210ae7aec2fdee4de4b5648c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.5 MB (107495557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48917cbf5d592ae6dfae0656501e41e0047103b7b1876a667d3f156f2142fa78`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 May 2021 00:50:48 GMT
ADD file:ff9983cd659b3fc32ddfbbdeda76a971afd7d399e6d8b98faea3a9ead0e598f6 in / 
# Wed, 12 May 2021 00:50:52 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:34:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:34:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 13 May 2021 00:40:15 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 13 May 2021 00:40:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 13 May 2021 00:40:57 GMT
ENV TELEGRAF_VERSION=1.18.2
# Thu, 13 May 2021 00:41:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 13 May 2021 00:41:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 13 May 2021 00:41:05 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 13 May 2021 00:41:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 13 May 2021 00:41:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c54d9402d498e45ed396b5b6fe836f55e4ccadbad745decda3e9f83d880bc677`  
		Last Modified: Wed, 12 May 2021 01:01:40 GMT  
		Size: 49.2 MB (49225351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91bbb3592d6685d1c683c8c20e60901274c636605800608685274c194d43d25`  
		Last Modified: Wed, 12 May 2021 01:48:24 GMT  
		Size: 7.7 MB (7695057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d8c28b9129321858810cff4cd78385949579ed18d991f98c77f912c7a754f8`  
		Last Modified: Wed, 12 May 2021 01:48:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c2afe1661b16b31414e984301464c54a688d670588da65e09acae49436f1c7`  
		Last Modified: Thu, 13 May 2021 00:41:27 GMT  
		Size: 17.3 MB (17269543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf8effe0189a9fabb276a8737e536476f360929816dd52b787ac4daba9033a9`  
		Last Modified: Thu, 13 May 2021 00:41:21 GMT  
		Size: 2.9 KB (2896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c35990993f5e776c9d3526c5d51df7c5ab3436c32d463630b1075286ade1b1`  
		Last Modified: Thu, 13 May 2021 00:41:58 GMT  
		Size: 23.3 MB (23318181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a46636f0388d9ab8d6ba1fb8731367cdebe248479c81bd0180d7708411d36e`  
		Last Modified: Thu, 13 May 2021 00:41:46 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
