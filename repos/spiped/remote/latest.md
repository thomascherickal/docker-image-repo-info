## `spiped:latest`

```console
$ docker pull spiped@sha256:5d84ef9ec0f9743c8099eb3678e0952f763c223f2789c488251c9a6073d86cdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
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
$ docker pull spiped@sha256:64c9ff6d4e90807fd06162f08c850797563f8a574f8d88c0e2177bba5343f9f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38181865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5caff7b7b3c368e50a4fe67474a9e454e570e0b9caf6a8fe447aea979e74ea3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:14:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 03:14:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:14:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 03:14:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 03:14:32 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 03:14:32 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 03:14:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:14:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:14:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b92b5954cfa789f1b5a0f545fd5a9a7e46a792aefca79339341f124d855f4dc`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6444d4e339eab2f9fb3ed43a84bcf11ef6cd483c5053f3176367a1b14fff3c61`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 2.6 MB (2586434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa1621f45212a870ec5dd0e4ef6e3378976c464c684c75ea52f65b4c9bb4ce8`  
		Last Modified: Tue, 04 Jul 2023 03:14:50 GMT  
		Size: 6.5 MB (6469003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea71d68d11725a63267fb85323478f0f1b5fbda3319b518987790561b52c868e`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9f406c97cfa32a6fd2ae3bc84894bc16b4c74eee2cb342a8174a9a388f783`  
		Last Modified: Tue, 04 Jul 2023 03:14:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:5bcd09c77588a67caae49433d4c86c6f91c69bae205ad672619afc5d749b5aba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34305753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:756c18f247bb62bc63d31e0a50b9c68a64cd1a3347826060fc7e1eb4ed5b5785`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:18:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 28 Jul 2023 06:18:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:18:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 28 Jul 2023 06:18:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 06:18:32 GMT
VOLUME [/spiped]
# Fri, 28 Jul 2023 06:18:32 GMT
WORKDIR /spiped
# Fri, 28 Jul 2023 06:18:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 28 Jul 2023 06:18:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 06:18:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca7867b868ea0c086b3cc19dffa7c4079dcd6909627f2495585866ef6686512`  
		Last Modified: Fri, 28 Jul 2023 06:18:47 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26eab6f4031dd2cbeb97b96eef0ca6ddeba7937c5a9fcb18252ba28e5f4c781b`  
		Last Modified: Fri, 28 Jul 2023 06:18:47 GMT  
		Size: 2.2 MB (2184071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a21b08acfc2c6384677556aa01a3474ac7b9a055627d511785767566f9b7199`  
		Last Modified: Fri, 28 Jul 2023 06:18:48 GMT  
		Size: 5.1 MB (5136574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfc10c0d99355974881d1e65b5a900d628c5d5beac6aeaa79ed789dd684a4e9`  
		Last Modified: Fri, 28 Jul 2023 06:18:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0b0514ba063b176ab332ff323fe4db1c5853e0bef483a0f7c0a0201fb4a6b2`  
		Last Modified: Fri, 28 Jul 2023 06:18:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:fa8d158ea62aae373b010ecee32e5ecea6fb4b437a2eb49aca790fae1736d647
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31723078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11b1b970d4425fc1f51cea7f5490f388e981e5d34fb3d9ce808c13f03413e26b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 15:38:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 15:38:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 15:38:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 15:38:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 15:39:00 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 15:39:00 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 15:39:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 15:39:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:39:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3403c8419ded94d78b4756589f9377598959311520c9817d426929dd63659d`  
		Last Modified: Tue, 04 Jul 2023 15:39:18 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e44f54d21c1788863d34d076c0eb22f62f3a2ae411d37e866f85c47e68b9e38`  
		Last Modified: Tue, 04 Jul 2023 15:39:19 GMT  
		Size: 2.0 MB (2043275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fb7cd0361eb4be25908a03aad1082a7bf6098ee6b8d10b3d2a5903eb5ed391`  
		Last Modified: Tue, 04 Jul 2023 15:39:20 GMT  
		Size: 4.9 MB (4876936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9151574768b755fac6c25ce6badff07f10c8c3faef3210d692cba091ef8bc2a9`  
		Last Modified: Tue, 04 Jul 2023 15:39:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d35983368786e50998af1a99a87e7b6667403aeecdcb0b06bf199bb5ac02d7d`  
		Last Modified: Tue, 04 Jul 2023 15:39:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:d88ac9d16fa209562e1a5179a8f008564588f851a68aee3ec5a597bb542d7df2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37067376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa29c1d765fbe597c57928bb35b8f9aa041e162896456d044076dae18b92d5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:19:38 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 28 Jul 2023 01:19:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:19:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 28 Jul 2023 01:20:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 01:20:03 GMT
VOLUME [/spiped]
# Fri, 28 Jul 2023 01:20:03 GMT
WORKDIR /spiped
# Fri, 28 Jul 2023 01:20:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:20:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:20:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f060019e05b5b6d10ebdcdfff5a1a17f7ea00e0c44edfa1a5d072061224979a8`  
		Last Modified: Fri, 28 Jul 2023 01:20:15 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c02a5e6dc6cb81fd967dcdd4813036b6e464930632ce048376eead8ee42a31d`  
		Last Modified: Fri, 28 Jul 2023 01:20:16 GMT  
		Size: 2.4 MB (2429832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c0fde9cbba82047d390c8e027e769c909fd6ab0fda3c2275ed45f504faeb79`  
		Last Modified: Fri, 28 Jul 2023 01:20:16 GMT  
		Size: 5.5 MB (5478716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a1efc6ee647d9b6aabdca7ed186fadc36667099750b3e749529f10bd02dd7c`  
		Last Modified: Fri, 28 Jul 2023 01:20:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6344e88b061ad36bcf2280ada625717ab2f97a1a36c5221c4987a23ca75fdec8`  
		Last Modified: Fri, 28 Jul 2023 01:20:15 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:29541e31c04fba759b1721e2c06b26bc4e7a494f3c4018c7d4b8c2d9e96b84eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38665735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:303ebec07d82a379e4aba61f9171623a882bc738ab3efcf669c972f36601fb20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:36 GMT
ADD file:441addef37edd5da10ca045fe9cc7863b0785f468d83c3884456efd567e97536 in / 
# Tue, 04 Jul 2023 01:38:36 GMT
CMD ["bash"]
# Wed, 05 Jul 2023 00:07:58 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Jul 2023 00:08:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 00:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Jul 2023 00:08:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Jul 2023 00:08:33 GMT
VOLUME [/spiped]
# Wed, 05 Jul 2023 00:08:33 GMT
WORKDIR /spiped
# Wed, 05 Jul 2023 00:08:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Jul 2023 00:08:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 00:08:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7d4b098d102e200415126181e2b6aae752738430f2ed6a601f84baf29e2f7d01`  
		Last Modified: Tue, 04 Jul 2023 01:43:28 GMT  
		Size: 30.1 MB (30140746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f71ebd54c1834f39015b12fcceaf889f346cc69a2391eee0d220d7eb532f8d`  
		Last Modified: Wed, 05 Jul 2023 00:08:47 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2047450d3047e2ff45ad251d3812e96e90d2477be7a26c624a672248ce57f1`  
		Last Modified: Wed, 05 Jul 2023 00:08:48 GMT  
		Size: 2.6 MB (2583532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bb884e2021728a069d79f3d8a2a33e652056df426db6265c4f64866ba70821`  
		Last Modified: Wed, 05 Jul 2023 00:08:49 GMT  
		Size: 5.9 MB (5939859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0702f841b65cba8c924a5eacabbf1acf24d959709c8cc023675bb4c72704d1`  
		Last Modified: Wed, 05 Jul 2023 00:08:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a2d10352b8f16d0f4545f217c3f0ef7e83807b6fde00eb8b83f57f8c422c14`  
		Last Modified: Wed, 05 Jul 2023 00:08:47 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:7828d1ba4ad693f840919aad0cb1e0e41abf15d45e4e18003cace27821904f6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36751895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f8be90d1d0cd2a6310b0bb4f84e20519e4cef602052b662880c8b18e9ffdfc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:09:28 GMT
ADD file:cf4b72a35644a7b9f5f1ca39a54e484822f408f6821f0800f1167ae48ad6e38e in / 
# Tue, 04 Jul 2023 01:09:32 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 19:26:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 19:27:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 19:27:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 19:28:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 19:28:59 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 19:29:02 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 19:29:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 19:29:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 19:29:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:502a81d5004983c2a770a910286271410d8e2b20d0cb61ef7397e664e1e72654`  
		Last Modified: Tue, 04 Jul 2023 01:19:57 GMT  
		Size: 29.1 MB (29118201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd72a1da8eadcc7f546db387b7d5db2cb3f5c275470134400731b157019549`  
		Last Modified: Tue, 04 Jul 2023 19:29:23 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94883ccc7bee39640c9c5e1367539c5c1f804f0b93b617f05df643875af480ed`  
		Last Modified: Tue, 04 Jul 2023 19:29:24 GMT  
		Size: 1.8 MB (1831639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91bd9d103397dcbe82f481782e4dd0f11d6d09507e1dc10260613fd2cad06e7`  
		Last Modified: Tue, 04 Jul 2023 19:29:28 GMT  
		Size: 5.8 MB (5800537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2070ac4c1d28067212b8eb40f2ad23b8418704e0fa5964286420c72d250f061f`  
		Last Modified: Tue, 04 Jul 2023 19:29:23 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7ab12d58ce7a0d93d2b5e99bef7c2303828489033eb8a77edc5912eb28b4ba`  
		Last Modified: Tue, 04 Jul 2023 19:29:23 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:2c54e716fcb927b30b4b3fe0032309ad8a591ae4e92fe98e3e2fba918031eebd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42302938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30f9f282a1636b8418b157a3ed06be634bab551e70e8a2ad37effa916e7d63d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Wed, 05 Jul 2023 00:09:03 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 05 Jul 2023 00:09:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 00:09:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 05 Jul 2023 00:10:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 05 Jul 2023 00:10:33 GMT
VOLUME [/spiped]
# Wed, 05 Jul 2023 00:10:35 GMT
WORKDIR /spiped
# Wed, 05 Jul 2023 00:10:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 05 Jul 2023 00:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Jul 2023 00:10:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a39a388af948200a4e561b00de04538d9947cf1e29d1872f2cf6f3c3dd935`  
		Last Modified: Wed, 05 Jul 2023 00:11:13 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25d83e982668054b305ba44163a931df81da3708a1ceded42aa9429f12b866a`  
		Last Modified: Wed, 05 Jul 2023 00:11:14 GMT  
		Size: 2.8 MB (2764933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0a3735828ac07a66a264b164f7cac05d968a2078561335afd2a6cf3d2de359`  
		Last Modified: Wed, 05 Jul 2023 00:11:15 GMT  
		Size: 6.4 MB (6419685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6620cd47540c782f6598e62183a73223916c5e476217743b621ec6c1f3634311`  
		Last Modified: Wed, 05 Jul 2023 00:11:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e184deae76b559502798232742fdfa90fb90794931cc4918540d9286fc5014c`  
		Last Modified: Wed, 05 Jul 2023 00:11:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:6695b8886374089b52406741f61cb350dc5a1f9d41f60f0b52c85d9fbc812637
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35129722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad5988cde06c6a38a111b372df2c8b99d2b6541541eb4fb44dd3354686008d07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Jul 2023 01:32:13 GMT
ADD file:7c6e123333ed463aaf550f8adb75415706fc8573337b76140d393910a5166731 in / 
# Tue, 04 Jul 2023 01:32:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:05:25 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Jul 2023 16:05:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:05:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 04 Jul 2023 16:05:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 16:05:46 GMT
VOLUME [/spiped]
# Tue, 04 Jul 2023 16:05:46 GMT
WORKDIR /spiped
# Tue, 04 Jul 2023 16:05:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:05:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:05:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0df7967bae0170739ec7f61c7bf3adbc2799d4ca7704b10725a46942717891fc`  
		Last Modified: Tue, 04 Jul 2023 01:37:07 GMT  
		Size: 27.5 MB (27487968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b52b17b7b0c9386b8962feb3f4686b7ac5564ac599e42c00b3d23551c049a5`  
		Last Modified: Tue, 04 Jul 2023 16:06:07 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfae8833e2a258532f6ab478dc6a4e8625734abcba21fa7ffa88e67013fdc823`  
		Last Modified: Tue, 04 Jul 2023 16:06:07 GMT  
		Size: 2.3 MB (2257951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1165a3528f2fadbdc2474b790173c325b55ae3d78836046042914c06d98fa2`  
		Last Modified: Tue, 04 Jul 2023 16:06:08 GMT  
		Size: 5.4 MB (5382206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531b8a926b8c6ed65398923a8e916420943b6c7f8f978ccf3a25ddbb13843332`  
		Last Modified: Tue, 04 Jul 2023 16:06:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c281bc5a1b7998673c1b8cfeb00e5f0bb2a167a1d3d2d04f817fb809c6dd23ad`  
		Last Modified: Tue, 04 Jul 2023 16:06:07 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
