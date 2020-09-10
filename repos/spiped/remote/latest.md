## `spiped:latest`

```console
$ docker pull spiped@sha256:33f4c03a177bb50e11c5d83a5afd12a13c4e8d136ff1b7653fee4398767cb6b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:70439d6dbe88f21aa856aaab7a7298438cc12ba3be7549ebd4420f806d307037
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36259837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5380b2b56cd6ec9efbd9d681f7e5bc0f685ddcae2e0e1ac3d3d091805925047d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 07:45:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Aug 2020 07:45:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 05 Aug 2020 07:45:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 05 Aug 2020 07:45:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Aug 2020 07:45:42 GMT
VOLUME [/spiped]
# Wed, 05 Aug 2020 07:45:42 GMT
WORKDIR /spiped
# Wed, 05 Aug 2020 07:45:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Aug 2020 07:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Aug 2020 07:45:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb460858f95f33833e9855747ba0a53d32cf243e9954e4b4a93fcaf7a1050c`  
		Last Modified: Wed, 05 Aug 2020 07:45:59 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386f27b678cc082575d2ebea9a65f8283c777429d9b1bb236ca3616f656cd500`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 2.1 MB (2128098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e579e4436d85d2674a21e0f2ba66a749c8a8f532d966769790061dddd49e52b`  
		Last Modified: Wed, 05 Aug 2020 07:46:00 GMT  
		Size: 7.0 MB (7037434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a652d9418b3d88fef1c5affe9eb20fdf3d4ec7bd9a9820e69be93a1ab7e53f`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7067335ae1b8e78625cb1fe80b7848b2978cd642958bbda66f28298b3da12`  
		Last Modified: Wed, 05 Aug 2020 07:45:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:0ffa7209cfe814b6558ab1e948cc440a965eb77f3af74f0e20e97e346d3b521f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d6fefca0c0605222f639cdc3d28477e5036c67425fb388f16b2d1d0f3bb3df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:53:49 GMT
ADD file:34835d84d87e3ee1178aa150793d75a4d4a7a28c013ca3495dbcca2b570270bf in / 
# Wed, 09 Sep 2020 23:53:53 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:24:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:24:31 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:24:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:24:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:24:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:25:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:25:32 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:25:34 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:25:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0a51b5143468e1b44dafa16fea3541e28e369071f6837337ee95e37f0ad81d99`  
		Last Modified: Thu, 10 Sep 2020 00:02:48 GMT  
		Size: 24.8 MB (24835974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16e60014503eeb6a9de0642540ffe398b65110a92e105ea725fe64050f133c7`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0bd36d1f55b67f92e906287f170c5ff225fa133082c4ac65bf0b026c8c1c61`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 1.8 MB (1839179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ddea53fb3a57a5e46a257e877538608b0b699eabf62195c6787df35c041c0`  
		Last Modified: Thu, 10 Sep 2020 00:26:00 GMT  
		Size: 5.5 MB (5479920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcc0f7c2e8d86cd9038ca26d518798de530b02f9d6a2625dea4fa37168eaf3f`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416e4e1edd36cc0942d8b1f16299321dcea276b757a77e44a69544b5f2716446`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3aacb61c327b386ee34f6b93b1fa0fd5374f619e4e2892eeb89bf106fedd68f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29746982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64f0c17703a1231aa28de1d610bbe7c71e9c4359c858c6b17e874c5c0046df2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:05:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 23:05:39 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:05:40 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 23:05:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 23:05:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 23:06:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 23:06:42 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 23:06:46 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 23:06:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:06:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069f16da332ada6f1ad07545e36cc298d95cc8aa48b90b032fa05c40ade00eb1`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10508b92cc5c67114d8c737d41e90f8fb787bfcf5b323b188f73fdb862db6a00`  
		Last Modified: Tue, 04 Aug 2020 23:07:17 GMT  
		Size: 1.8 MB (1759470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fd1ca266440f3d238e6839e5219c41bab5dd0d88b8ddbdaa24f8e00cfcb5a0`  
		Last Modified: Tue, 04 Aug 2020 23:07:19 GMT  
		Size: 5.3 MB (5285516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea228d83d648f1c8eae77bf202795643d64ff1ae73be870802716fc868c03c80`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33943a537cfaba6127939b8cd88291a552d5f04b4d35e8a0b5c88662f3b14cf3`  
		Last Modified: Tue, 04 Aug 2020 23:07:16 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b5559218e09ea14be189bc4849e65862923f193c32a411414000ab9ef9d78958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33764754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc4164d7a19420c2ade4b8da35eb1ee139c6222f7e1294f5fc19e5fcb9c210b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 15:37:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 15:37:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 15:37:13 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 15:37:13 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 15:37:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 15:38:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 15:38:04 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 15:38:05 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 15:38:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 15:38:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 15:38:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc32d378107720f326e540f83d46bf60a4bce7af8244906ed9526271eee31c3`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079ffe8630aa7835a3caef3a636edbb7a12d5ecddb5a60bfe8818de2559b2006`  
		Last Modified: Tue, 04 Aug 2020 15:38:39 GMT  
		Size: 2.0 MB (2007894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cd7433660d1423b7657db5c6d63e3a85c7d5f6f29c722623c496c5894962b2`  
		Last Modified: Tue, 04 Aug 2020 15:38:44 GMT  
		Size: 5.9 MB (5905348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d359b34f38b7c91489868441f4924bf12eb7ce4f499d08e9f6f27df6e1c315c8`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a9286120d5d507f14efb6bee85440a27254031d85a1aecd582401d1dd9adab`  
		Last Modified: Tue, 04 Aug 2020 15:38:38 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:7705a0fc3f3476409ebb0bc24d6d37d7fba3e5592d82ee6d2839e364a950456e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989705c9829172d17a6ede941662c041e3cf4cac305a6d4b388b20e91453b1b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:16:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:16:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:17:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:17:11 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:17:11 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:17:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:17:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:17:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860dd30325c96ffc8b96efe07adbb91c1bf07d1fbe88c2cde7cecd89da76d72`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4331fe8000d00915ae0827ce99d7946202943c5616440cd4fe768d9d7ed71a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 2.1 MB (2132352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c89212a59a8a3b09219d62baf7cfc20311e828bbf52b010ae9db5bc78c5b83`  
		Last Modified: Thu, 10 Sep 2020 00:17:29 GMT  
		Size: 11.6 MB (11633000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54072dfa562a77a02b96e37ade7b47dfdf8a9a27d4eee6db49dc154a2c89cf0a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe5b51ab58e39aa04cbe7d1f927049252d4d7b476925effe2c5e213e905108`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:016da36b9f7998b09d92b6cc8852d341e82ef59a357e95663cf2a912e99bf1c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195c77f25ce68e53cef2621cd2de83604d84f91dc5bdcebf623cfc31ce8aa130`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:18:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 11:18:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 11:19:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 11:19:31 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 11:19:32 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 11:19:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:19:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d54e34357c9f5fa48267296e6c6c1f76e35953b78ff71274dbf93d620fe713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808939bfa0b439c22bc52e424703f683009d54bc7b0e929bb95642a17e4cf346`  
		Last Modified: Tue, 04 Aug 2020 11:19:57 GMT  
		Size: 1.7 MB (1712064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1430e0259ffd64f678312f8e44b2331f9b36c5dfc010756f03d0b4b1d5278b`  
		Last Modified: Tue, 04 Aug 2020 11:20:02 GMT  
		Size: 6.4 MB (6416279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160144f3a0adf67512994233d3b27e3cf11991c2929b9ceb5fcbccce56af823`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a1586309f94ae81d1d5501572c464e6cf0b95721f6d0e54fad359886abb713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:1a26f6d748b9c6cd0cd3c33bd6326198eac44ee6695d90e32fa92c33d0efab15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffa18892130ac57caaa0c35c5e223f1f80929f3bca5753dfbbebd98c9d1a1ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:44:13 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 12:44:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 12:44:36 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 12:44:39 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 12:44:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 12:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 12:48:05 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 12:48:08 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 12:48:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 12:48:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 12:48:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ec976cf945c4c5a0725ce160b23b8fc7453ab53f7645cb507f81cc8f97ba1f`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b3868607138d28e33ab153c8f68521f00f2c00ee48d5542c62fef3ee508bcf`  
		Last Modified: Tue, 04 Aug 2020 12:48:52 GMT  
		Size: 2.2 MB (2224970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc4d03de8274dc06c34b37b24e819fe01a0d313e538a7a809f519e3a63d9418`  
		Last Modified: Tue, 04 Aug 2020 12:48:53 GMT  
		Size: 6.7 MB (6743232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff8e76a3ee77f253306f6c4c94eaf5df2e55c449d2a812c3bb843851031bc47`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58b79d7f675a5211c5c171567c5ff5762c0755bef406ed884efd50c9df4a3d1`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:fe495248fc843e3e7fe3fbf02c5130dda9ec60f29196a51bc7c38fa2abcc30a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33475012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054347711f47480fc68748dac617918f9dc83ab14e5327052f3fe1c455269ebf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:16 GMT
ADD file:2ffa27c57800f9370adbaecca870158ec38c3d25a58b8803e2447c5e9320c5bb in / 
# Tue, 04 Aug 2020 01:17:17 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 05:44:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 05:44:22 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 05:44:23 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 05:44:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 05:44:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 05:44:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 05:44:38 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 05:44:38 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 05:44:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 05:44:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 05:44:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c46adfa2de4a7b7eb1fe2f0cb928f9e15a4cc94b7b975f13392f397cbfb0f2c`  
		Last Modified: Tue, 04 Aug 2020 01:20:03 GMT  
		Size: 25.7 MB (25707641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc2e22e7c26e978fbd750c399bf784f421ba883e46fc25a6d12c3c4c0c0eb21`  
		Last Modified: Tue, 04 Aug 2020 05:44:55 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2241d2889b265c9d6e2f1c4be303610616a66cf281efebc2944920c551ce858`  
		Last Modified: Tue, 04 Aug 2020 05:44:56 GMT  
		Size: 1.8 MB (1821790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f50f475976e62937ae717f78f6260f8e11a240663268882612f0cd8db8b8173`  
		Last Modified: Tue, 04 Aug 2020 05:44:56 GMT  
		Size: 5.9 MB (5943371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9cca401af87e962176bad09359790d56a4b4293fab1289839ccc0d1e83800f`  
		Last Modified: Tue, 04 Aug 2020 05:44:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ed4a188f1957a2dae6be7d565da4d5a6accb58e9cecb8bf3d99b2616874a0b`  
		Last Modified: Tue, 04 Aug 2020 05:44:55 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
