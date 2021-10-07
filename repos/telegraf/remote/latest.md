## `telegraf:latest`

```console
$ docker pull telegraf@sha256:961a5f10ddc54c76e908ebbfcada6902b66d4f39d33434d13594f9691be9c488
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:ad36536b343bbedecb8aff4a51dab50d6179c24c57b7bc3ff78719c46328d8cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120433152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9e97bb72318d1d857ed566db069fd19139381083fc5f51daffd919db65d4c2b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 29 Sep 2021 06:44:40 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 06:44:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Oct 2021 00:20:57 GMT
ENV TELEGRAF_VERSION=1.20.1
# Thu, 07 Oct 2021 00:21:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 07 Oct 2021 00:21:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 07 Oct 2021 00:21:03 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 07 Oct 2021 00:21:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Oct 2021 00:21:03 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538325b9471ae16e29f3a2b95a2a75cd9eae9cfce82b09776af2ea917f7d8f1c`  
		Last Modified: Wed, 29 Sep 2021 06:45:42 GMT  
		Size: 17.4 MB (17415015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd9b0a906f2a2c346339837795984130161b39b2923b71aceff1e98611044b4`  
		Last Modified: Wed, 29 Sep 2021 06:45:38 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a6f5e27058a477baefd252752c3c7090e4c8081e8730edee16463627226ac4`  
		Last Modified: Thu, 07 Oct 2021 00:21:55 GMT  
		Size: 34.7 MB (34748045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afbf8704d55d2b35f9b61eee4a9e54d2abebd20a49eeb85a2377a1f6689d42a`  
		Last Modified: Thu, 07 Oct 2021 00:21:47 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:2802711a7fa966afcf1c80f414b5fc317d649d08eaab6e568105f5901ffed29b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110905760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7df69344b8d7f4a55ba18525f56dbab8bdbee9d07a02045ea733a0c49bd5fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:34 GMT
ADD file:da3730d9c05fab2433637063dc9d51b2505bb6023c391d606419bc9a0874c131 in / 
# Thu, 30 Sep 2021 18:03:35 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:35:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:35:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 15:33:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 15:33:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 02 Oct 2021 15:34:43 GMT
ENV TELEGRAF_VERSION=1.20.0
# Sat, 02 Oct 2021 15:34:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 02 Oct 2021 15:34:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 02 Oct 2021 15:34:56 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Sat, 02 Oct 2021 15:34:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Oct 2021 15:34:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2d333743b3b21fdfd6ba3f4a0624204b620b72c3d0eb2c3dd9e39d23f3a87e9c`  
		Last Modified: Thu, 30 Sep 2021 18:20:10 GMT  
		Size: 45.9 MB (45917880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d8928e133ca4adc2e7f254a958f120743ac165e45332c8f2713144cf1e1c5`  
		Last Modified: Fri, 01 Oct 2021 05:55:55 GMT  
		Size: 7.1 MB (7124916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a975074459ff1f9c6b99644b138401f840f49a4dc1ef138661e138db9cd00038`  
		Last Modified: Fri, 01 Oct 2021 05:55:56 GMT  
		Size: 9.3 MB (9343736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954ac84f090b20ef8e2460a554dc719264bde71f0b61b698782beb5db970fd68`  
		Last Modified: Sat, 02 Oct 2021 15:35:52 GMT  
		Size: 16.2 MB (16160686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8afc9277cc9e8025cd5a51124e72967a287e1c6a4c4cfe39721bb5e75557d9a`  
		Last Modified: Sat, 02 Oct 2021 15:35:40 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bceaf27831f3c9bf683a89dfc47566706ac5c74000186928545af3cdc01fcbaa`  
		Last Modified: Sat, 02 Oct 2021 15:37:12 GMT  
		Size: 32.4 MB (32355452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b134be47fc258634650c51d9978fc471ea7853041b0bb8f9e15060262eca84`  
		Last Modified: Sat, 02 Oct 2021 15:36:50 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a7f4eeede73ea1195141316cdca51bfe0ea420e3cf26e4703dba863a8344683c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115740984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:965a0c609a83adf75ca45b1d426e75f688a268a4ac166a1279fc35d6a064297f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:56 GMT
ADD file:51975e5f400da759b2cd8f7eba13ad61dd4edbbee0d0fac09b697bfa039d1515 in / 
# Tue, 28 Sep 2021 01:40:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 22:00:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 22:00:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 28 Sep 2021 22:01:10 GMT
ENV TELEGRAF_VERSION=1.20.0
# Tue, 28 Sep 2021 22:01:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 28 Sep 2021 22:01:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 28 Sep 2021 22:01:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 28 Sep 2021 22:01:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Sep 2021 22:01:19 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:70fe10514d0290bd1e8986c0fd63a67204813d37fc5863cf9bf8bf61b2031537`  
		Last Modified: Tue, 28 Sep 2021 01:48:53 GMT  
		Size: 49.2 MB (49222381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9679d540d5f2659fa72eaa9fa11dc318510dc1e7795eab1bc39295855a03d1d0`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 7.7 MB (7695855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052683e57413fa9352045785beb2e5728edac5063c3b899145698f812b5fb903`  
		Last Modified: Tue, 28 Sep 2021 02:26:00 GMT  
		Size: 10.0 MB (9984315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4d5fcea6ed1c367bb5afd8d9645f13354ce42d08c4132db556b432e0776770`  
		Last Modified: Tue, 28 Sep 2021 22:01:48 GMT  
		Size: 17.3 MB (17268487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d6e634d2e44e6a1dcde1c7d3b4b2f9627e9f0ae90e650eb73ba5b7d5e55b56`  
		Last Modified: Tue, 28 Sep 2021 22:01:45 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f911e54efba3515dfcfa1657510d2e32792d5b7f96d2fea6a54aab0345d609cf`  
		Last Modified: Tue, 28 Sep 2021 22:02:25 GMT  
		Size: 31.6 MB (31566857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394f7164a79e3be174829778ccd4baff6af9254b378fe40ac926bab3bbfb7bb7`  
		Last Modified: Tue, 28 Sep 2021 22:02:20 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
