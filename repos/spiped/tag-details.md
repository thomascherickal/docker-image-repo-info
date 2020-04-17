<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6.1`](#spiped161)
-	[`spiped:1.6.1-alpine`](#spiped161-alpine)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:239a61dc04787e9ac73da6d90486cde8981dfa53222fbdb8218021f4ac0fa959
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:5992cb5c64c9374a42e1d3f9d90ba0ecf25e8e15ace2a1343aef9d8d71618e5d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36265820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cac3acb7248a1287a18933c29ca63fb7444285171b1b283950d636a3075dcada`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 22:31:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 22:31:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 22:31:50 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 22:31:50 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 22:31:51 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 22:32:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 22:32:36 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 22:32:36 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 22:32:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 22:32:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 22:32:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f65909e3f56df80c1218789672dc7a031626b491fe26347e79aefc9b19d462`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b77040a76a55aacb77de9d37f8424b516d3a83c193b2bec8dc40aea4524e9d`  
		Last Modified: Thu, 16 Apr 2020 22:32:59 GMT  
		Size: 2.1 MB (2128072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c8b526ba64e4f5a392d2b7b439a301c8eda97f4044d9ede8d73b6209363bbc`  
		Last Modified: Thu, 16 Apr 2020 22:33:01 GMT  
		Size: 7.0 MB (7037427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ed01c1e306eb2f9d66d551794e5b9a57abd93550d350ddfdfe91e9101c84d`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e9de8354fdc3d75f9d4c36d49d571637b8827a16280a8236892378d8412dda`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:7b3cbe0584b5bfce28c4e5b32e3067d47cc9f0fd111c9ee06c45d243f6b77e10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc38b8e5d013861323eea7bb10c1deaa83ad477005ab870c4b6e1ec46b2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:50:14 GMT
ADD file:761a556ec2a7d8c742c860e429c9b9ba3f7abfcd9383c6b3767499de6dcad4bc in / 
# Thu, 16 Apr 2020 00:50:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 08:11:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 08:12:28 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 08:12:29 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 08:12:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 08:12:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 08:13:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 08:13:45 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 08:13:47 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 08:13:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 08:13:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 08:13:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:600369660a591bc9594fcf333a847fe997901785f7032d3ad2822b2812c13243`  
		Last Modified: Thu, 16 Apr 2020 00:58:26 GMT  
		Size: 24.8 MB (24836437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d3efd96e0e3ae19bc1d98b7641152963a20946d22c27185f8bdbc39a323ffe`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a35d8a2c6636729c3109e6f8651a30e86db454e3d5fab2557a65eb0e7d970f`  
		Last Modified: Thu, 16 Apr 2020 08:14:03 GMT  
		Size: 1.8 MB (1839164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ef1836765ffc9b64f4f00062192c607111f1f9b8d8ae7dd17b38059ed38370`  
		Last Modified: Thu, 16 Apr 2020 08:14:04 GMT  
		Size: 5.5 MB (5479815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7ef6cf26d04f86d0149bed4f74d316fa5c6cd5298a92c2d32f55c9bdcfef0b`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9ca3401f9bc0c2209b13a4dfcbcd2d5cac5e6f8aa4f87a0bdc920326569d2e`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:83999f433e590988c2c2f68d879bac730747b4ca3de4b591ee3cc945b57566a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3799e9ef8bd587f79b60b19b6c6f68fd8dec6e26e921dbf683d7f67bad3d7449`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 18:14:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 18:14:43 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 18:14:44 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 18:14:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 18:14:45 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 18:15:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 18:15:28 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 18:15:29 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 18:15:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 18:15:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 18:15:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161e3b50373e52ebe2f239ba138fa317c227800d469908642fcaaa7738917205`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04ec01be0e1b6427232b9c18ffd4bb4fcce5edd9785cd3c5b770fc17fff3d6`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 1.8 MB (1759418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4fafe74230439ca4cf44a2d946f6a48d586952381ae57d03273f9f9b083759`  
		Last Modified: Thu, 16 Apr 2020 18:16:05 GMT  
		Size: 5.3 MB (5285305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3953c76d2ab2982c918cd4afa8405742993b721c0cf7b4f5de1090251f4b6f`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64e88d03257d714b230562d361ea0f089cce8556bbf6c443a8798edfcddc94d`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:75ffd27fc35a979876ca2245ac292822575f355b7a38e174678ef786702fafb8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ad8529c2720c626616890db5b75b7dcff52c80f5d89cdba782b541bf1764e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:52 GMT
ADD file:1aab17002a9095c31dd6928277a045cb26846ac58c3d2d63316332c99a5f90bd in / 
# Thu, 16 Apr 2020 02:41:57 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 20:13:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 20:13:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 20:13:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 20:13:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 20:13:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 20:14:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 20:14:42 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 20:14:43 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 20:14:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 20:14:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 20:14:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3d48095d71a365b5910cea98e5566c152a3f9aa11657560568259bf93ff2f4cb`  
		Last Modified: Thu, 16 Apr 2020 02:48:58 GMT  
		Size: 25.9 MB (25857715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd185084a2a8907950a1957520ab48f0e324f87472c1c4f00290c499e3af4c16`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72cb36bacab8361b509f73295e37fde282152056a403ec02113a10f5ffe7d85`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 2.0 MB (2007781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1704638bc3bd1a976d9c9a114196312166b1d952c4d97c344f7c2055bf7e7220`  
		Last Modified: Thu, 16 Apr 2020 20:15:18 GMT  
		Size: 5.9 MB (5905308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae49dac5dafb2bd487a5d23af3079ee6219e38678ff3e18b2653736befab067`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418a8cdbbb37964316e934e39bd2736fc3d7adae2a419f3214550eb33e28cac`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:9926733306f68b93f7403e712d3b174452088a30ec88351759d30d5839bfc58e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41521584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eec8d26a366a17ca23d236b412935e8c92f33dc3880d1deb82b45b5fe326b141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 01:39:55 GMT
ADD file:ab0bbfba6c4b56420ffffc6cdddcc4592fff018f0cd07578c7dc0a5faa49df2f in / 
# Thu, 16 Apr 2020 01:39:56 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:15:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 02:15:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 02:15:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 02:15:56 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 02:15:56 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 02:15:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 02:15:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:15:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75bc60a98e6523be3fadd9128c1a630cb5cbd2d2d813ee5e99dc146a3de22254`  
		Last Modified: Thu, 16 Apr 2020 01:46:20 GMT  
		Size: 27.8 MB (27753976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434723a2b224f8837fdc460dc5691152d12aef50da6942fee530583efeeffceb`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67147847d2314c76ba55152b85f65e0bda1f059986ec62f8e9aac2ec676b74e3`  
		Last Modified: Thu, 16 Apr 2020 02:16:13 GMT  
		Size: 2.1 MB (2132347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdb13b1b28ff00c192060d5705212c0a7926b2774b1bd103671208e4881b959`  
		Last Modified: Thu, 16 Apr 2020 02:16:16 GMT  
		Size: 11.6 MB (11633094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4dbb06458c59576e1e3db43237dd2731ea9aa6328a653f2fc99c8411a7949`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b71d15bb761995984f6d4c0242516ef565183f0ce7954ff39bda3f2351873e`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:1735539e3e7e65ef4d593b2f1e3c4d1c521d9f6257b9f933dfe8c908e47a82e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39494935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25ed7c69475d3ff2dff66671b3c85d66e3101aef828da38d6f348ae537664467`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 01:38:30 GMT
ADD file:9beea54416432abbd09d26b965c3c8e5bea8e233113f9bc308294c0008ee886f in / 
# Thu, 16 Apr 2020 01:38:39 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:32:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 06:33:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 06:33:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 06:33:11 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 06:33:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 06:36:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 06:36:18 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 06:36:25 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 06:36:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 06:36:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 06:36:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f268991f8af64097bbfefa3f01dd3fdb7f715051a3681f352504a3ecaa9d3596`  
		Last Modified: Thu, 16 Apr 2020 01:54:39 GMT  
		Size: 30.5 MB (30524651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11faf29322892c8e1a80bc63dd8d796125ee307f1e739960c976657247050849`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ccd1806ab2ac21ee209497c4c59d5575c5cfc5faaa1947e4cd86aa15528ceb`  
		Last Modified: Thu, 16 Apr 2020 06:37:13 GMT  
		Size: 2.2 MB (2224905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9229fa187f1524ad1611a629844a2268d6e05c41930bd0e1c7bb9f5a705ea0c`  
		Last Modified: Thu, 16 Apr 2020 06:37:13 GMT  
		Size: 6.7 MB (6743157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218baaa74ab7c90a3676e2b6df8502c735d933f9aed579caace6014489e22e7a`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a98a13b6647dbf2001ba52d55d8d20a502a25bb400ab75d79a9faf11e7cbc1`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:0597e20ac03ff66cfad7d104787ed5b96a9ac7697ee48060f324e00844ab9529
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33479404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38f98e83f85547ac7f6e4dda1d8bb5e464e22042c46615866633476a1105da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:19 GMT
ADD file:f328b5d6dce2eaf00360542c1e3280958b818268b9150b12ffd1fddf030daf2f in / 
# Thu, 16 Apr 2020 00:42:20 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 09:13:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 09:13:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 09:13:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 09:13:47 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 09:13:47 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 09:13:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 09:13:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 09:13:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:043f95f5412a986fb082b0193860bb9c0388c2fbcb5e8bf5bcbbeefb0e45c9c5`  
		Last Modified: Thu, 16 Apr 2020 00:46:19 GMT  
		Size: 25.7 MB (25712234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6aec151b4cc88c9dc5605c8f4e8bec9649a643c744148850a655376e5d20932`  
		Last Modified: Thu, 16 Apr 2020 09:14:11 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48029c5984714761c355bc50aa231eda2d011113b6fdab73d47c970d1f85f96`  
		Last Modified: Thu, 16 Apr 2020 09:14:11 GMT  
		Size: 1.8 MB (1821695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95a36959cf23bd7d1a58f5f9d1f28c72cdecf869e55df64e15021f89f5b3dde`  
		Last Modified: Thu, 16 Apr 2020 09:14:17 GMT  
		Size: 5.9 MB (5943266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048afd803e0dd2ab2e4606727a11b6edf89f5704a3c6a7d6f94fa6f362e00398`  
		Last Modified: Thu, 16 Apr 2020 09:14:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d243505dd1bf28f3938608bf19a96bea5c30535181778c60e26498da2ec8ba5`  
		Last Modified: Thu, 16 Apr 2020 09:14:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:239a61dc04787e9ac73da6d90486cde8981dfa53222fbdb8218021f4ac0fa959
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:5992cb5c64c9374a42e1d3f9d90ba0ecf25e8e15ace2a1343aef9d8d71618e5d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36265820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cac3acb7248a1287a18933c29ca63fb7444285171b1b283950d636a3075dcada`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 22:31:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 22:31:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 22:31:50 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 22:31:50 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 22:31:51 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 22:32:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 22:32:36 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 22:32:36 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 22:32:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 22:32:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 22:32:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f65909e3f56df80c1218789672dc7a031626b491fe26347e79aefc9b19d462`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b77040a76a55aacb77de9d37f8424b516d3a83c193b2bec8dc40aea4524e9d`  
		Last Modified: Thu, 16 Apr 2020 22:32:59 GMT  
		Size: 2.1 MB (2128072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c8b526ba64e4f5a392d2b7b439a301c8eda97f4044d9ede8d73b6209363bbc`  
		Last Modified: Thu, 16 Apr 2020 22:33:01 GMT  
		Size: 7.0 MB (7037427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ed01c1e306eb2f9d66d551794e5b9a57abd93550d350ddfdfe91e9101c84d`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e9de8354fdc3d75f9d4c36d49d571637b8827a16280a8236892378d8412dda`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:7b3cbe0584b5bfce28c4e5b32e3067d47cc9f0fd111c9ee06c45d243f6b77e10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc38b8e5d013861323eea7bb10c1deaa83ad477005ab870c4b6e1ec46b2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:50:14 GMT
ADD file:761a556ec2a7d8c742c860e429c9b9ba3f7abfcd9383c6b3767499de6dcad4bc in / 
# Thu, 16 Apr 2020 00:50:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 08:11:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 08:12:28 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 08:12:29 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 08:12:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 08:12:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 08:13:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 08:13:45 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 08:13:47 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 08:13:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 08:13:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 08:13:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:600369660a591bc9594fcf333a847fe997901785f7032d3ad2822b2812c13243`  
		Last Modified: Thu, 16 Apr 2020 00:58:26 GMT  
		Size: 24.8 MB (24836437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d3efd96e0e3ae19bc1d98b7641152963a20946d22c27185f8bdbc39a323ffe`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a35d8a2c6636729c3109e6f8651a30e86db454e3d5fab2557a65eb0e7d970f`  
		Last Modified: Thu, 16 Apr 2020 08:14:03 GMT  
		Size: 1.8 MB (1839164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ef1836765ffc9b64f4f00062192c607111f1f9b8d8ae7dd17b38059ed38370`  
		Last Modified: Thu, 16 Apr 2020 08:14:04 GMT  
		Size: 5.5 MB (5479815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7ef6cf26d04f86d0149bed4f74d316fa5c6cd5298a92c2d32f55c9bdcfef0b`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9ca3401f9bc0c2209b13a4dfcbcd2d5cac5e6f8aa4f87a0bdc920326569d2e`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:83999f433e590988c2c2f68d879bac730747b4ca3de4b591ee3cc945b57566a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3799e9ef8bd587f79b60b19b6c6f68fd8dec6e26e921dbf683d7f67bad3d7449`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 18:14:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 18:14:43 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 18:14:44 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 18:14:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 18:14:45 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 18:15:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 18:15:28 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 18:15:29 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 18:15:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 18:15:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 18:15:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161e3b50373e52ebe2f239ba138fa317c227800d469908642fcaaa7738917205`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04ec01be0e1b6427232b9c18ffd4bb4fcce5edd9785cd3c5b770fc17fff3d6`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 1.8 MB (1759418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4fafe74230439ca4cf44a2d946f6a48d586952381ae57d03273f9f9b083759`  
		Last Modified: Thu, 16 Apr 2020 18:16:05 GMT  
		Size: 5.3 MB (5285305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3953c76d2ab2982c918cd4afa8405742993b721c0cf7b4f5de1090251f4b6f`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64e88d03257d714b230562d361ea0f089cce8556bbf6c443a8798edfcddc94d`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:75ffd27fc35a979876ca2245ac292822575f355b7a38e174678ef786702fafb8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ad8529c2720c626616890db5b75b7dcff52c80f5d89cdba782b541bf1764e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:52 GMT
ADD file:1aab17002a9095c31dd6928277a045cb26846ac58c3d2d63316332c99a5f90bd in / 
# Thu, 16 Apr 2020 02:41:57 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 20:13:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 20:13:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 20:13:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 20:13:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 20:13:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 20:14:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 20:14:42 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 20:14:43 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 20:14:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 20:14:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 20:14:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3d48095d71a365b5910cea98e5566c152a3f9aa11657560568259bf93ff2f4cb`  
		Last Modified: Thu, 16 Apr 2020 02:48:58 GMT  
		Size: 25.9 MB (25857715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd185084a2a8907950a1957520ab48f0e324f87472c1c4f00290c499e3af4c16`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72cb36bacab8361b509f73295e37fde282152056a403ec02113a10f5ffe7d85`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 2.0 MB (2007781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1704638bc3bd1a976d9c9a114196312166b1d952c4d97c344f7c2055bf7e7220`  
		Last Modified: Thu, 16 Apr 2020 20:15:18 GMT  
		Size: 5.9 MB (5905308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae49dac5dafb2bd487a5d23af3079ee6219e38678ff3e18b2653736befab067`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418a8cdbbb37964316e934e39bd2736fc3d7adae2a419f3214550eb33e28cac`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:9926733306f68b93f7403e712d3b174452088a30ec88351759d30d5839bfc58e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41521584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eec8d26a366a17ca23d236b412935e8c92f33dc3880d1deb82b45b5fe326b141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 01:39:55 GMT
ADD file:ab0bbfba6c4b56420ffffc6cdddcc4592fff018f0cd07578c7dc0a5faa49df2f in / 
# Thu, 16 Apr 2020 01:39:56 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:15:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 02:15:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 02:15:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 02:15:56 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 02:15:56 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 02:15:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 02:15:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:15:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75bc60a98e6523be3fadd9128c1a630cb5cbd2d2d813ee5e99dc146a3de22254`  
		Last Modified: Thu, 16 Apr 2020 01:46:20 GMT  
		Size: 27.8 MB (27753976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434723a2b224f8837fdc460dc5691152d12aef50da6942fee530583efeeffceb`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67147847d2314c76ba55152b85f65e0bda1f059986ec62f8e9aac2ec676b74e3`  
		Last Modified: Thu, 16 Apr 2020 02:16:13 GMT  
		Size: 2.1 MB (2132347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdb13b1b28ff00c192060d5705212c0a7926b2774b1bd103671208e4881b959`  
		Last Modified: Thu, 16 Apr 2020 02:16:16 GMT  
		Size: 11.6 MB (11633094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4dbb06458c59576e1e3db43237dd2731ea9aa6328a653f2fc99c8411a7949`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b71d15bb761995984f6d4c0242516ef565183f0ce7954ff39bda3f2351873e`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:1735539e3e7e65ef4d593b2f1e3c4d1c521d9f6257b9f933dfe8c908e47a82e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39494935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25ed7c69475d3ff2dff66671b3c85d66e3101aef828da38d6f348ae537664467`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 01:38:30 GMT
ADD file:9beea54416432abbd09d26b965c3c8e5bea8e233113f9bc308294c0008ee886f in / 
# Thu, 16 Apr 2020 01:38:39 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:32:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 06:33:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 06:33:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 06:33:11 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 06:33:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 06:36:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 06:36:18 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 06:36:25 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 06:36:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 06:36:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 06:36:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f268991f8af64097bbfefa3f01dd3fdb7f715051a3681f352504a3ecaa9d3596`  
		Last Modified: Thu, 16 Apr 2020 01:54:39 GMT  
		Size: 30.5 MB (30524651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11faf29322892c8e1a80bc63dd8d796125ee307f1e739960c976657247050849`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ccd1806ab2ac21ee209497c4c59d5575c5cfc5faaa1947e4cd86aa15528ceb`  
		Last Modified: Thu, 16 Apr 2020 06:37:13 GMT  
		Size: 2.2 MB (2224905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9229fa187f1524ad1611a629844a2268d6e05c41930bd0e1c7bb9f5a705ea0c`  
		Last Modified: Thu, 16 Apr 2020 06:37:13 GMT  
		Size: 6.7 MB (6743157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218baaa74ab7c90a3676e2b6df8502c735d933f9aed579caace6014489e22e7a`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a98a13b6647dbf2001ba52d55d8d20a502a25bb400ab75d79a9faf11e7cbc1`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:0597e20ac03ff66cfad7d104787ed5b96a9ac7697ee48060f324e00844ab9529
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33479404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38f98e83f85547ac7f6e4dda1d8bb5e464e22042c46615866633476a1105da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:19 GMT
ADD file:f328b5d6dce2eaf00360542c1e3280958b818268b9150b12ffd1fddf030daf2f in / 
# Thu, 16 Apr 2020 00:42:20 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 09:13:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 09:13:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 09:13:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 09:13:47 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 09:13:47 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 09:13:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 09:13:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 09:13:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:043f95f5412a986fb082b0193860bb9c0388c2fbcb5e8bf5bcbbeefb0e45c9c5`  
		Last Modified: Thu, 16 Apr 2020 00:46:19 GMT  
		Size: 25.7 MB (25712234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6aec151b4cc88c9dc5605c8f4e8bec9649a643c744148850a655376e5d20932`  
		Last Modified: Thu, 16 Apr 2020 09:14:11 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48029c5984714761c355bc50aa231eda2d011113b6fdab73d47c970d1f85f96`  
		Last Modified: Thu, 16 Apr 2020 09:14:11 GMT  
		Size: 1.8 MB (1821695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95a36959cf23bd7d1a58f5f9d1f28c72cdecf869e55df64e15021f89f5b3dde`  
		Last Modified: Thu, 16 Apr 2020 09:14:17 GMT  
		Size: 5.9 MB (5943266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048afd803e0dd2ab2e4606727a11b6edf89f5704a3c6a7d6f94fa6f362e00398`  
		Last Modified: Thu, 16 Apr 2020 09:14:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d243505dd1bf28f3938608bf19a96bea5c30535181778c60e26498da2ec8ba5`  
		Last Modified: Thu, 16 Apr 2020 09:14:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:239a61dc04787e9ac73da6d90486cde8981dfa53222fbdb8218021f4ac0fa959
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.1` - linux; amd64

```console
$ docker pull spiped@sha256:5992cb5c64c9374a42e1d3f9d90ba0ecf25e8e15ace2a1343aef9d8d71618e5d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36265820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cac3acb7248a1287a18933c29ca63fb7444285171b1b283950d636a3075dcada`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 22:31:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 22:31:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 22:31:50 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 22:31:50 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 22:31:51 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 22:32:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 22:32:36 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 22:32:36 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 22:32:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 22:32:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 22:32:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f65909e3f56df80c1218789672dc7a031626b491fe26347e79aefc9b19d462`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b77040a76a55aacb77de9d37f8424b516d3a83c193b2bec8dc40aea4524e9d`  
		Last Modified: Thu, 16 Apr 2020 22:32:59 GMT  
		Size: 2.1 MB (2128072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c8b526ba64e4f5a392d2b7b439a301c8eda97f4044d9ede8d73b6209363bbc`  
		Last Modified: Thu, 16 Apr 2020 22:33:01 GMT  
		Size: 7.0 MB (7037427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ed01c1e306eb2f9d66d551794e5b9a57abd93550d350ddfdfe91e9101c84d`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e9de8354fdc3d75f9d4c36d49d571637b8827a16280a8236892378d8412dda`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:7b3cbe0584b5bfce28c4e5b32e3067d47cc9f0fd111c9ee06c45d243f6b77e10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc38b8e5d013861323eea7bb10c1deaa83ad477005ab870c4b6e1ec46b2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:50:14 GMT
ADD file:761a556ec2a7d8c742c860e429c9b9ba3f7abfcd9383c6b3767499de6dcad4bc in / 
# Thu, 16 Apr 2020 00:50:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 08:11:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 08:12:28 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 08:12:29 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 08:12:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 08:12:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 08:13:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 08:13:45 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 08:13:47 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 08:13:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 08:13:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 08:13:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:600369660a591bc9594fcf333a847fe997901785f7032d3ad2822b2812c13243`  
		Last Modified: Thu, 16 Apr 2020 00:58:26 GMT  
		Size: 24.8 MB (24836437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d3efd96e0e3ae19bc1d98b7641152963a20946d22c27185f8bdbc39a323ffe`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a35d8a2c6636729c3109e6f8651a30e86db454e3d5fab2557a65eb0e7d970f`  
		Last Modified: Thu, 16 Apr 2020 08:14:03 GMT  
		Size: 1.8 MB (1839164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ef1836765ffc9b64f4f00062192c607111f1f9b8d8ae7dd17b38059ed38370`  
		Last Modified: Thu, 16 Apr 2020 08:14:04 GMT  
		Size: 5.5 MB (5479815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7ef6cf26d04f86d0149bed4f74d316fa5c6cd5298a92c2d32f55c9bdcfef0b`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9ca3401f9bc0c2209b13a4dfcbcd2d5cac5e6f8aa4f87a0bdc920326569d2e`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:83999f433e590988c2c2f68d879bac730747b4ca3de4b591ee3cc945b57566a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3799e9ef8bd587f79b60b19b6c6f68fd8dec6e26e921dbf683d7f67bad3d7449`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 18:14:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 18:14:43 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 18:14:44 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 18:14:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 18:14:45 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 18:15:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 18:15:28 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 18:15:29 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 18:15:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 18:15:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 18:15:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161e3b50373e52ebe2f239ba138fa317c227800d469908642fcaaa7738917205`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04ec01be0e1b6427232b9c18ffd4bb4fcce5edd9785cd3c5b770fc17fff3d6`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 1.8 MB (1759418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4fafe74230439ca4cf44a2d946f6a48d586952381ae57d03273f9f9b083759`  
		Last Modified: Thu, 16 Apr 2020 18:16:05 GMT  
		Size: 5.3 MB (5285305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3953c76d2ab2982c918cd4afa8405742993b721c0cf7b4f5de1090251f4b6f`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64e88d03257d714b230562d361ea0f089cce8556bbf6c443a8798edfcddc94d`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:75ffd27fc35a979876ca2245ac292822575f355b7a38e174678ef786702fafb8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ad8529c2720c626616890db5b75b7dcff52c80f5d89cdba782b541bf1764e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:52 GMT
ADD file:1aab17002a9095c31dd6928277a045cb26846ac58c3d2d63316332c99a5f90bd in / 
# Thu, 16 Apr 2020 02:41:57 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 20:13:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 20:13:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 20:13:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 20:13:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 20:13:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 20:14:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 20:14:42 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 20:14:43 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 20:14:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 20:14:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 20:14:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3d48095d71a365b5910cea98e5566c152a3f9aa11657560568259bf93ff2f4cb`  
		Last Modified: Thu, 16 Apr 2020 02:48:58 GMT  
		Size: 25.9 MB (25857715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd185084a2a8907950a1957520ab48f0e324f87472c1c4f00290c499e3af4c16`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72cb36bacab8361b509f73295e37fde282152056a403ec02113a10f5ffe7d85`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 2.0 MB (2007781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1704638bc3bd1a976d9c9a114196312166b1d952c4d97c344f7c2055bf7e7220`  
		Last Modified: Thu, 16 Apr 2020 20:15:18 GMT  
		Size: 5.9 MB (5905308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae49dac5dafb2bd487a5d23af3079ee6219e38678ff3e18b2653736befab067`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418a8cdbbb37964316e934e39bd2736fc3d7adae2a419f3214550eb33e28cac`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:9926733306f68b93f7403e712d3b174452088a30ec88351759d30d5839bfc58e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41521584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eec8d26a366a17ca23d236b412935e8c92f33dc3880d1deb82b45b5fe326b141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 01:39:55 GMT
ADD file:ab0bbfba6c4b56420ffffc6cdddcc4592fff018f0cd07578c7dc0a5faa49df2f in / 
# Thu, 16 Apr 2020 01:39:56 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:15:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 02:15:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 02:15:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 02:15:56 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 02:15:56 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 02:15:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 02:15:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:15:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75bc60a98e6523be3fadd9128c1a630cb5cbd2d2d813ee5e99dc146a3de22254`  
		Last Modified: Thu, 16 Apr 2020 01:46:20 GMT  
		Size: 27.8 MB (27753976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434723a2b224f8837fdc460dc5691152d12aef50da6942fee530583efeeffceb`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67147847d2314c76ba55152b85f65e0bda1f059986ec62f8e9aac2ec676b74e3`  
		Last Modified: Thu, 16 Apr 2020 02:16:13 GMT  
		Size: 2.1 MB (2132347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdb13b1b28ff00c192060d5705212c0a7926b2774b1bd103671208e4881b959`  
		Last Modified: Thu, 16 Apr 2020 02:16:16 GMT  
		Size: 11.6 MB (11633094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4dbb06458c59576e1e3db43237dd2731ea9aa6328a653f2fc99c8411a7949`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b71d15bb761995984f6d4c0242516ef565183f0ce7954ff39bda3f2351873e`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:1735539e3e7e65ef4d593b2f1e3c4d1c521d9f6257b9f933dfe8c908e47a82e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39494935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25ed7c69475d3ff2dff66671b3c85d66e3101aef828da38d6f348ae537664467`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 01:38:30 GMT
ADD file:9beea54416432abbd09d26b965c3c8e5bea8e233113f9bc308294c0008ee886f in / 
# Thu, 16 Apr 2020 01:38:39 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:32:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 06:33:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 06:33:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 06:33:11 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 06:33:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 06:36:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 06:36:18 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 06:36:25 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 06:36:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 06:36:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 06:36:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f268991f8af64097bbfefa3f01dd3fdb7f715051a3681f352504a3ecaa9d3596`  
		Last Modified: Thu, 16 Apr 2020 01:54:39 GMT  
		Size: 30.5 MB (30524651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11faf29322892c8e1a80bc63dd8d796125ee307f1e739960c976657247050849`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ccd1806ab2ac21ee209497c4c59d5575c5cfc5faaa1947e4cd86aa15528ceb`  
		Last Modified: Thu, 16 Apr 2020 06:37:13 GMT  
		Size: 2.2 MB (2224905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9229fa187f1524ad1611a629844a2268d6e05c41930bd0e1c7bb9f5a705ea0c`  
		Last Modified: Thu, 16 Apr 2020 06:37:13 GMT  
		Size: 6.7 MB (6743157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218baaa74ab7c90a3676e2b6df8502c735d933f9aed579caace6014489e22e7a`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a98a13b6647dbf2001ba52d55d8d20a502a25bb400ab75d79a9faf11e7cbc1`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:0597e20ac03ff66cfad7d104787ed5b96a9ac7697ee48060f324e00844ab9529
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33479404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38f98e83f85547ac7f6e4dda1d8bb5e464e22042c46615866633476a1105da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:19 GMT
ADD file:f328b5d6dce2eaf00360542c1e3280958b818268b9150b12ffd1fddf030daf2f in / 
# Thu, 16 Apr 2020 00:42:20 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 09:13:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 09:13:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 09:13:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 09:13:47 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 09:13:47 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 09:13:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 09:13:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 09:13:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:043f95f5412a986fb082b0193860bb9c0388c2fbcb5e8bf5bcbbeefb0e45c9c5`  
		Last Modified: Thu, 16 Apr 2020 00:46:19 GMT  
		Size: 25.7 MB (25712234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6aec151b4cc88c9dc5605c8f4e8bec9649a643c744148850a655376e5d20932`  
		Last Modified: Thu, 16 Apr 2020 09:14:11 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48029c5984714761c355bc50aa231eda2d011113b6fdab73d47c970d1f85f96`  
		Last Modified: Thu, 16 Apr 2020 09:14:11 GMT  
		Size: 1.8 MB (1821695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95a36959cf23bd7d1a58f5f9d1f28c72cdecf869e55df64e15021f89f5b3dde`  
		Last Modified: Thu, 16 Apr 2020 09:14:17 GMT  
		Size: 5.9 MB (5943266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048afd803e0dd2ab2e4606727a11b6edf89f5704a3c6a7d6f94fa6f362e00398`  
		Last Modified: Thu, 16 Apr 2020 09:14:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d243505dd1bf28f3938608bf19a96bea5c30535181778c60e26498da2ec8ba5`  
		Last Modified: Thu, 16 Apr 2020 09:14:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:429322e56bd429da567aab90232ba7941a4edb8e64c2c09b9373402f91a44d4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:bce46785c0a6ec6e48a45f297dd5796fe2e5d9fafb6a3cf034c6971e7ff2780f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2883892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b78eb499d78cb9b4325629fbc90c2735a1cf1c1bd4af69bd8ef608587d02cb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 21:13:07 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:13:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 21:13:34 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:13:34 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:13:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:13:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:13:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc29e947b9ccbbe548f4f1f66f2a845c61ab555b046909b89e4fd420a3e93f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 88.9 KB (88915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb514126aa1d85c9fc37f7d50649132790a408d0ddd0cd279c2a832ade0b08df`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90b1f71237aa2be63e283a61cdc07fc8342b12601060003bfa959a95253b0f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:6f13ddc4cb1716a895e69405631a68d99c7addad9078453402ad5938856a0687
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0bd97d067a154cda46a3674de70626059520bfaf9d8f8b3fc4557df053d73ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:49:34 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:49:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:49:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:50:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:50:08 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:50:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:50:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:50:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:50:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7a9eb0c9ab5fc279a9e98ef9e98de63123b64ca04af635a1f73af9a6d15b24`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 75.0 KB (74952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9967718642289f730242b2a77c0515672aec66c1a838dd2a4f80d444ee79b8`  
		Last Modified: Mon, 06 Apr 2020 19:50:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f4a4b862c429a85eeacb3270f4cc64c2c61e9357769a9c151d183ff8ca31a9`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d6d6923d0c2d9d8e954815efdf9c9669fa23bd9548d55ead413e69dfe7d52d7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa542a4d5cbae70b3e71e20948df53d2d5b7c0002792bacd5bbf792a6f52f6e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:59:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:59:49 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d441b71208c64b2bc2218499780ec39d9cfd3edbdd8e2e4d7c45a80f6d84bc5f`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 68.1 KB (68096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd2cbe47130d1b62eefe8efad8296a2e4160621db07811a387f646ec3c0589`  
		Last Modified: Mon, 06 Apr 2020 20:00:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d62488071b8b3ca44afce89ea5c8de19fdf6db9cc18bceda022deb8bfc6f79`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:33dd11964e68275c0de9bdd90576f1bd3b07ed9b35be0d3cdd3ca1f750a618c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2807814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371dcc8679ed28f64596dd03ffcbc8756f215a13eabd2677793a1cd1f4ff6ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:53:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:53:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:53:38 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:53:38 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:53:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:53:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:53:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b182ea73fc29e32821dfc68455a6582b2b46be25a46a61c72df2fc9787013`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 82.0 KB (81989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a5ef743131210844f90d7217bb848a2baa687b4c7831815cebb46a94ea8b`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01cf4b79b4817343f95634a3b4cdd1066462a5435b81c0147d585090b50051e`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:2f99e8ca94d16bef32ae67a69bf093ea7df131d656e0d5bf94d217755375eef3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc64ad00fc662dc2350d81e426695cc56dc2ee3fb92c25e9573a5e41edb6207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:43:44 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:45 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c23f29e92934601486929bc683a1c1ce6b5d17de8710ffb64ae444a6edf74bd`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 98.4 KB (98396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11754050cbbe0e5f1e3f040f12eb326523d160784b4bf4053eb29c607abb6106`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802418066b370d7b8c1b666fbd6ba2090c2f354f5a84ee7b3771c1d5181fa148`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:51027e899bfe55d1432c89de3d9b71bac3fbcc342373f1111aa03217c0d11b67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1d379d08a7d62d83cb2d138d3d260429659fe214c06248975f439fe8837fea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 20:26:12 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:26:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:26:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 20:26:46 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:26:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:26:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:26:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68e315a19f730564cead7324b439d4c893d7bb4661c6aa88a863dff413222be`  
		Last Modified: Mon, 06 Apr 2020 20:27:35 GMT  
		Size: 97.5 KB (97516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1fcb0a480d90f3ae48043a675f479aab1cc1f315674ce71db46b2b5ddea7e2`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad7ed01644a076eb4f0e4ee3ff1981a0383df44638b5cb6a1e811ac29b7affa`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9d875e8421a60f09bc74f0103800a7e000690cd17d9eac43042cdbb8308cf8a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2662697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bbcb97371eba97b63ff9fbf44afe6eeaa0cdbc6bc9be9fe8494fcaa4e254d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:46:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:29 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66314c6e3c0080fcb0f7264c3aaa35fe5fd5d1bab9428aa378638125af56c3c`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 81.0 KB (81006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f3a2df50f521de78c8d5d6df53bf6bbc15080b09c18d64eb7cef65f3f516ba`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a08476e03d2df5c637df812d7ebb17ed6fc5dee82ea4da393a867a6c394db`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:429322e56bd429da567aab90232ba7941a4edb8e64c2c09b9373402f91a44d4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:bce46785c0a6ec6e48a45f297dd5796fe2e5d9fafb6a3cf034c6971e7ff2780f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2883892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b78eb499d78cb9b4325629fbc90c2735a1cf1c1bd4af69bd8ef608587d02cb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 21:13:07 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:13:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 21:13:34 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:13:34 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:13:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:13:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:13:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc29e947b9ccbbe548f4f1f66f2a845c61ab555b046909b89e4fd420a3e93f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 88.9 KB (88915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb514126aa1d85c9fc37f7d50649132790a408d0ddd0cd279c2a832ade0b08df`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90b1f71237aa2be63e283a61cdc07fc8342b12601060003bfa959a95253b0f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:6f13ddc4cb1716a895e69405631a68d99c7addad9078453402ad5938856a0687
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0bd97d067a154cda46a3674de70626059520bfaf9d8f8b3fc4557df053d73ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:49:34 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:49:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:49:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:50:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:50:08 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:50:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:50:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:50:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:50:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7a9eb0c9ab5fc279a9e98ef9e98de63123b64ca04af635a1f73af9a6d15b24`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 75.0 KB (74952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9967718642289f730242b2a77c0515672aec66c1a838dd2a4f80d444ee79b8`  
		Last Modified: Mon, 06 Apr 2020 19:50:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f4a4b862c429a85eeacb3270f4cc64c2c61e9357769a9c151d183ff8ca31a9`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d6d6923d0c2d9d8e954815efdf9c9669fa23bd9548d55ead413e69dfe7d52d7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa542a4d5cbae70b3e71e20948df53d2d5b7c0002792bacd5bbf792a6f52f6e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:59:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:59:49 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d441b71208c64b2bc2218499780ec39d9cfd3edbdd8e2e4d7c45a80f6d84bc5f`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 68.1 KB (68096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd2cbe47130d1b62eefe8efad8296a2e4160621db07811a387f646ec3c0589`  
		Last Modified: Mon, 06 Apr 2020 20:00:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d62488071b8b3ca44afce89ea5c8de19fdf6db9cc18bceda022deb8bfc6f79`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:33dd11964e68275c0de9bdd90576f1bd3b07ed9b35be0d3cdd3ca1f750a618c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2807814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371dcc8679ed28f64596dd03ffcbc8756f215a13eabd2677793a1cd1f4ff6ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:53:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:53:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:53:38 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:53:38 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:53:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:53:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:53:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b182ea73fc29e32821dfc68455a6582b2b46be25a46a61c72df2fc9787013`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 82.0 KB (81989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a5ef743131210844f90d7217bb848a2baa687b4c7831815cebb46a94ea8b`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01cf4b79b4817343f95634a3b4cdd1066462a5435b81c0147d585090b50051e`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:2f99e8ca94d16bef32ae67a69bf093ea7df131d656e0d5bf94d217755375eef3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc64ad00fc662dc2350d81e426695cc56dc2ee3fb92c25e9573a5e41edb6207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:43:44 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:45 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c23f29e92934601486929bc683a1c1ce6b5d17de8710ffb64ae444a6edf74bd`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 98.4 KB (98396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11754050cbbe0e5f1e3f040f12eb326523d160784b4bf4053eb29c607abb6106`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802418066b370d7b8c1b666fbd6ba2090c2f354f5a84ee7b3771c1d5181fa148`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:51027e899bfe55d1432c89de3d9b71bac3fbcc342373f1111aa03217c0d11b67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1d379d08a7d62d83cb2d138d3d260429659fe214c06248975f439fe8837fea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 20:26:12 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:26:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:26:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 20:26:46 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:26:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:26:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:26:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68e315a19f730564cead7324b439d4c893d7bb4661c6aa88a863dff413222be`  
		Last Modified: Mon, 06 Apr 2020 20:27:35 GMT  
		Size: 97.5 KB (97516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1fcb0a480d90f3ae48043a675f479aab1cc1f315674ce71db46b2b5ddea7e2`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad7ed01644a076eb4f0e4ee3ff1981a0383df44638b5cb6a1e811ac29b7affa`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9d875e8421a60f09bc74f0103800a7e000690cd17d9eac43042cdbb8308cf8a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2662697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bbcb97371eba97b63ff9fbf44afe6eeaa0cdbc6bc9be9fe8494fcaa4e254d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:46:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:29 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66314c6e3c0080fcb0f7264c3aaa35fe5fd5d1bab9428aa378638125af56c3c`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 81.0 KB (81006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f3a2df50f521de78c8d5d6df53bf6bbc15080b09c18d64eb7cef65f3f516ba`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a08476e03d2df5c637df812d7ebb17ed6fc5dee82ea4da393a867a6c394db`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:429322e56bd429da567aab90232ba7941a4edb8e64c2c09b9373402f91a44d4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:bce46785c0a6ec6e48a45f297dd5796fe2e5d9fafb6a3cf034c6971e7ff2780f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2883892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b78eb499d78cb9b4325629fbc90c2735a1cf1c1bd4af69bd8ef608587d02cb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 21:13:07 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:13:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 21:13:34 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:13:34 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:13:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:13:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:13:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc29e947b9ccbbe548f4f1f66f2a845c61ab555b046909b89e4fd420a3e93f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 88.9 KB (88915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb514126aa1d85c9fc37f7d50649132790a408d0ddd0cd279c2a832ade0b08df`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90b1f71237aa2be63e283a61cdc07fc8342b12601060003bfa959a95253b0f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:6f13ddc4cb1716a895e69405631a68d99c7addad9078453402ad5938856a0687
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0bd97d067a154cda46a3674de70626059520bfaf9d8f8b3fc4557df053d73ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:49:34 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:49:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:49:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:50:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:50:08 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:50:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:50:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:50:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:50:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7a9eb0c9ab5fc279a9e98ef9e98de63123b64ca04af635a1f73af9a6d15b24`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 75.0 KB (74952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9967718642289f730242b2a77c0515672aec66c1a838dd2a4f80d444ee79b8`  
		Last Modified: Mon, 06 Apr 2020 19:50:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f4a4b862c429a85eeacb3270f4cc64c2c61e9357769a9c151d183ff8ca31a9`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d6d6923d0c2d9d8e954815efdf9c9669fa23bd9548d55ead413e69dfe7d52d7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa542a4d5cbae70b3e71e20948df53d2d5b7c0002792bacd5bbf792a6f52f6e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:59:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:59:49 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d441b71208c64b2bc2218499780ec39d9cfd3edbdd8e2e4d7c45a80f6d84bc5f`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 68.1 KB (68096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd2cbe47130d1b62eefe8efad8296a2e4160621db07811a387f646ec3c0589`  
		Last Modified: Mon, 06 Apr 2020 20:00:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d62488071b8b3ca44afce89ea5c8de19fdf6db9cc18bceda022deb8bfc6f79`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:33dd11964e68275c0de9bdd90576f1bd3b07ed9b35be0d3cdd3ca1f750a618c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2807814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371dcc8679ed28f64596dd03ffcbc8756f215a13eabd2677793a1cd1f4ff6ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:53:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:53:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:53:38 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:53:38 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:53:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:53:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:53:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b182ea73fc29e32821dfc68455a6582b2b46be25a46a61c72df2fc9787013`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 82.0 KB (81989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a5ef743131210844f90d7217bb848a2baa687b4c7831815cebb46a94ea8b`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01cf4b79b4817343f95634a3b4cdd1066462a5435b81c0147d585090b50051e`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:2f99e8ca94d16bef32ae67a69bf093ea7df131d656e0d5bf94d217755375eef3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc64ad00fc662dc2350d81e426695cc56dc2ee3fb92c25e9573a5e41edb6207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:43:44 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:45 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c23f29e92934601486929bc683a1c1ce6b5d17de8710ffb64ae444a6edf74bd`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 98.4 KB (98396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11754050cbbe0e5f1e3f040f12eb326523d160784b4bf4053eb29c607abb6106`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802418066b370d7b8c1b666fbd6ba2090c2f354f5a84ee7b3771c1d5181fa148`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:51027e899bfe55d1432c89de3d9b71bac3fbcc342373f1111aa03217c0d11b67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1d379d08a7d62d83cb2d138d3d260429659fe214c06248975f439fe8837fea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 20:26:12 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:26:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:26:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 20:26:46 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:26:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:26:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:26:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68e315a19f730564cead7324b439d4c893d7bb4661c6aa88a863dff413222be`  
		Last Modified: Mon, 06 Apr 2020 20:27:35 GMT  
		Size: 97.5 KB (97516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1fcb0a480d90f3ae48043a675f479aab1cc1f315674ce71db46b2b5ddea7e2`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad7ed01644a076eb4f0e4ee3ff1981a0383df44638b5cb6a1e811ac29b7affa`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9d875e8421a60f09bc74f0103800a7e000690cd17d9eac43042cdbb8308cf8a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2662697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bbcb97371eba97b63ff9fbf44afe6eeaa0cdbc6bc9be9fe8494fcaa4e254d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:46:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:29 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66314c6e3c0080fcb0f7264c3aaa35fe5fd5d1bab9428aa378638125af56c3c`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 81.0 KB (81006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f3a2df50f521de78c8d5d6df53bf6bbc15080b09c18d64eb7cef65f3f516ba`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a08476e03d2df5c637df812d7ebb17ed6fc5dee82ea4da393a867a6c394db`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:429322e56bd429da567aab90232ba7941a4edb8e64c2c09b9373402f91a44d4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:bce46785c0a6ec6e48a45f297dd5796fe2e5d9fafb6a3cf034c6971e7ff2780f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2883892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b78eb499d78cb9b4325629fbc90c2735a1cf1c1bd4af69bd8ef608587d02cb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:05 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 06:03:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 21:13:07 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:13:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 21:13:34 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:13:34 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:13:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:13:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:13:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc06614bab390a9f65e534efa1155fe7dd1311893a11f6f4967981fafdaefd3`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c348138de7d3b0e5c5fb05f433065ad04c6aca51cc39ae4d40ce336644aee5`  
		Last Modified: Fri, 24 Jan 2020 06:03:27 GMT  
		Size: 6.3 KB (6316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc29e947b9ccbbe548f4f1f66f2a845c61ab555b046909b89e4fd420a3e93f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 88.9 KB (88915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb514126aa1d85c9fc37f7d50649132790a408d0ddd0cd279c2a832ade0b08df`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90b1f71237aa2be63e283a61cdc07fc8342b12601060003bfa959a95253b0f`  
		Last Modified: Mon, 06 Apr 2020 21:13:57 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:6f13ddc4cb1716a895e69405631a68d99c7addad9078453402ad5938856a0687
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2654448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0bd97d067a154cda46a3674de70626059520bfaf9d8f8b3fc4557df053d73ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 21:07:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 21:07:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:49:34 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:49:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:49:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:50:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:50:08 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:50:10 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:50:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:50:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:50:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041552ff85cdb0b3534cf0c9740911bb5396f66f689a9588d679db8d39ba30cf`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99168294acba08dff442387ce408077fa19318b9438dfd63acd12731999f449b`  
		Last Modified: Thu, 23 Jan 2020 21:07:56 GMT  
		Size: 6.3 KB (6330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7a9eb0c9ab5fc279a9e98ef9e98de63123b64ca04af635a1f73af9a6d15b24`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 75.0 KB (74952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9967718642289f730242b2a77c0515672aec66c1a838dd2a4f80d444ee79b8`  
		Last Modified: Mon, 06 Apr 2020 19:50:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f4a4b862c429a85eeacb3270f4cc64c2c61e9357769a9c151d183ff8ca31a9`  
		Last Modified: Mon, 06 Apr 2020 19:50:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d6d6923d0c2d9d8e954815efdf9c9669fa23bd9548d55ead413e69dfe7d52d7a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa542a4d5cbae70b3e71e20948df53d2d5b7c0002792bacd5bbf792a6f52f6e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:56:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:56:50 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:59:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:59:25 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:59:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:59:49 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:59:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44109046b3edfc2a6f5871a1151727205dc9340cb7755b528a8a66b7b6611d`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35c670710669e985d296decde16a878826688fa423b230f94688bf695cd8cb`  
		Last Modified: Thu, 23 Jan 2020 17:57:31 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d441b71208c64b2bc2218499780ec39d9cfd3edbdd8e2e4d7c45a80f6d84bc5f`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 68.1 KB (68096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd2cbe47130d1b62eefe8efad8296a2e4160621db07811a387f646ec3c0589`  
		Last Modified: Mon, 06 Apr 2020 20:00:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d62488071b8b3ca44afce89ea5c8de19fdf6db9cc18bceda022deb8bfc6f79`  
		Last Modified: Mon, 06 Apr 2020 20:00:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:33dd11964e68275c0de9bdd90576f1bd3b07ed9b35be0d3cdd3ca1f750a618c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2807814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371dcc8679ed28f64596dd03ffcbc8756f215a13eabd2677793a1cd1f4ff6ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:03:17 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 23:03:19 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:53:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:53:10 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:53:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:53:38 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:53:38 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:53:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:53:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:53:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3404575dfd4e3d90feaa85bb9536b6d2f7303c91de5579ba6a44b1fa8018cd2`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086976ffc73adca7915ccce8816879191aec90d27fd329100f2ba1d727d7c8`  
		Last Modified: Thu, 23 Jan 2020 23:04:02 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b182ea73fc29e32821dfc68455a6582b2b46be25a46a61c72df2fc9787013`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 82.0 KB (81989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a5ef743131210844f90d7217bb848a2baa687b4c7831815cebb46a94ea8b`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01cf4b79b4817343f95634a3b4cdd1066462a5435b81c0147d585090b50051e`  
		Last Modified: Mon, 06 Apr 2020 19:54:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:2f99e8ca94d16bef32ae67a69bf093ea7df131d656e0d5bf94d217755375eef3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc64ad00fc662dc2350d81e426695cc56dc2ee3fb92c25e9573a5e41edb6207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:05:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Jan 2020 04:05:27 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:43:27 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:43:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:43:44 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:43:45 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:43:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:43:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a71c93f25a9940525e378b97eb4dfc31ce3f08b803b56803769c64d044f96`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92ca427ba9a83e544b6e54adf1955abd91dfdfaf42eabe991ec55e777da99d3`  
		Last Modified: Fri, 24 Jan 2020 04:05:47 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c23f29e92934601486929bc683a1c1ce6b5d17de8710ffb64ae444a6edf74bd`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 98.4 KB (98396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11754050cbbe0e5f1e3f040f12eb326523d160784b4bf4053eb29c607abb6106`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802418066b370d7b8c1b666fbd6ba2090c2f354f5a84ee7b3771c1d5181fa148`  
		Last Modified: Mon, 06 Apr 2020 19:44:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:51027e899bfe55d1432c89de3d9b71bac3fbcc342373f1111aa03217c0d11b67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1d379d08a7d62d83cb2d138d3d260429659fe214c06248975f439fe8837fea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:57:54 GMT
ADD file:5e383dfaf3281b9cc17caf519d1aeba934fa92632c10afb8cc189f6ba12d9f64 in / 
# Thu, 23 Jan 2020 16:57:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 22:48:57 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 20:26:12 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 20:26:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 20:26:19 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 20:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 20:26:46 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 20:26:50 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 20:26:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 20:26:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:27:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ae00dedbff84a762d4b8b9176da2beee50017c43fe09a5ae92c2417d5634510`  
		Last Modified: Thu, 23 Jan 2020 16:58:43 GMT  
		Size: 2.8 MB (2808535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f2b65d7bb1394f4c89cbccccdd5d618958d26a5356864b87387a09e38b03b7`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bab7a31e28999301e8eb42d8c24257e06fc7bd2550872beaeb2b85248b501c`  
		Last Modified: Thu, 23 Jan 2020 22:49:56 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68e315a19f730564cead7324b439d4c893d7bb4661c6aa88a863dff413222be`  
		Last Modified: Mon, 06 Apr 2020 20:27:35 GMT  
		Size: 97.5 KB (97516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1fcb0a480d90f3ae48043a675f479aab1cc1f315674ce71db46b2b5ddea7e2`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad7ed01644a076eb4f0e4ee3ff1981a0383df44638b5cb6a1e811ac29b7affa`  
		Last Modified: Mon, 06 Apr 2020 20:27:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:9d875e8421a60f09bc74f0103800a7e000690cd17d9eac43042cdbb8308cf8a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2662697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bbcb97371eba97b63ff9fbf44afe6eeaa0cdbc6bc9be9fe8494fcaa4e254d7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:43 GMT
ADD file:922e12714922ae035a33d6ceb8d2683ad3e454deca21ad02b699db908443342b in / 
# Thu, 23 Jan 2020 16:52:44 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Jan 2020 17:10:00 GMT
RUN apk add --no-cache libssl1.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 19:46:16 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 19:46:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 06 Apr 2020 19:46:29 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 19:46:29 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 19:46:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 19:46:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 19:46:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0449d076b2977b7e7ce4c35b0fe5199d86cabaf453e869da73b2efb66d6282dd`  
		Last Modified: Thu, 23 Jan 2020 16:53:07 GMT  
		Size: 2.6 MB (2573620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e42d5d6b574cf439c940dba20b8a3482a2ec896724f0e07843d3bd74c485680`  
		Last Modified: Thu, 23 Jan 2020 17:10:16 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6e359bd1502566c84b381f6bd4c606e6233830984c92329607c27cf8c3dd7`  
		Last Modified: Thu, 23 Jan 2020 17:10:17 GMT  
		Size: 6.3 KB (6339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66314c6e3c0080fcb0f7264c3aaa35fe5fd5d1bab9428aa378638125af56c3c`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 81.0 KB (81006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f3a2df50f521de78c8d5d6df53bf6bbc15080b09c18d64eb7cef65f3f516ba`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a08476e03d2df5c637df812d7ebb17ed6fc5dee82ea4da393a867a6c394db`  
		Last Modified: Mon, 06 Apr 2020 19:46:51 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:239a61dc04787e9ac73da6d90486cde8981dfa53222fbdb8218021f4ac0fa959
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:5992cb5c64c9374a42e1d3f9d90ba0ecf25e8e15ace2a1343aef9d8d71618e5d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36265820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cac3acb7248a1287a18933c29ca63fb7444285171b1b283950d636a3075dcada`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 22:31:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 22:31:50 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 22:31:50 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 22:31:50 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 22:31:51 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 22:32:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 22:32:36 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 22:32:36 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 22:32:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 22:32:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 22:32:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f65909e3f56df80c1218789672dc7a031626b491fe26347e79aefc9b19d462`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b77040a76a55aacb77de9d37f8424b516d3a83c193b2bec8dc40aea4524e9d`  
		Last Modified: Thu, 16 Apr 2020 22:32:59 GMT  
		Size: 2.1 MB (2128072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c8b526ba64e4f5a392d2b7b439a301c8eda97f4044d9ede8d73b6209363bbc`  
		Last Modified: Thu, 16 Apr 2020 22:33:01 GMT  
		Size: 7.0 MB (7037427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6ed01c1e306eb2f9d66d551794e5b9a57abd93550d350ddfdfe91e9101c84d`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e9de8354fdc3d75f9d4c36d49d571637b8827a16280a8236892378d8412dda`  
		Last Modified: Thu, 16 Apr 2020 22:32:58 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:7b3cbe0584b5bfce28c4e5b32e3067d47cc9f0fd111c9ee06c45d243f6b77e10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbc38b8e5d013861323eea7bb10c1deaa83ad477005ab870c4b6e1ec46b2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:50:14 GMT
ADD file:761a556ec2a7d8c742c860e429c9b9ba3f7abfcd9383c6b3767499de6dcad4bc in / 
# Thu, 16 Apr 2020 00:50:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 08:11:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 08:12:28 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 08:12:29 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 08:12:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 08:12:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 08:13:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 08:13:45 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 08:13:47 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 08:13:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 08:13:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 08:13:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:600369660a591bc9594fcf333a847fe997901785f7032d3ad2822b2812c13243`  
		Last Modified: Thu, 16 Apr 2020 00:58:26 GMT  
		Size: 24.8 MB (24836437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d3efd96e0e3ae19bc1d98b7641152963a20946d22c27185f8bdbc39a323ffe`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a35d8a2c6636729c3109e6f8651a30e86db454e3d5fab2557a65eb0e7d970f`  
		Last Modified: Thu, 16 Apr 2020 08:14:03 GMT  
		Size: 1.8 MB (1839164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ef1836765ffc9b64f4f00062192c607111f1f9b8d8ae7dd17b38059ed38370`  
		Last Modified: Thu, 16 Apr 2020 08:14:04 GMT  
		Size: 5.5 MB (5479815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7ef6cf26d04f86d0149bed4f74d316fa5c6cd5298a92c2d32f55c9bdcfef0b`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9ca3401f9bc0c2209b13a4dfcbcd2d5cac5e6f8aa4f87a0bdc920326569d2e`  
		Last Modified: Thu, 16 Apr 2020 08:14:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:83999f433e590988c2c2f68d879bac730747b4ca3de4b591ee3cc945b57566a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3799e9ef8bd587f79b60b19b6c6f68fd8dec6e26e921dbf683d7f67bad3d7449`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 18:14:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 18:14:43 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 18:14:44 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 18:14:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 18:14:45 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 18:15:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 18:15:28 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 18:15:29 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 18:15:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 18:15:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 18:15:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161e3b50373e52ebe2f239ba138fa317c227800d469908642fcaaa7738917205`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04ec01be0e1b6427232b9c18ffd4bb4fcce5edd9785cd3c5b770fc17fff3d6`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 1.8 MB (1759418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4fafe74230439ca4cf44a2d946f6a48d586952381ae57d03273f9f9b083759`  
		Last Modified: Thu, 16 Apr 2020 18:16:05 GMT  
		Size: 5.3 MB (5285305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3953c76d2ab2982c918cd4afa8405742993b721c0cf7b4f5de1090251f4b6f`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64e88d03257d714b230562d361ea0f089cce8556bbf6c443a8798edfcddc94d`  
		Last Modified: Thu, 16 Apr 2020 18:16:03 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:75ffd27fc35a979876ca2245ac292822575f355b7a38e174678ef786702fafb8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ad8529c2720c626616890db5b75b7dcff52c80f5d89cdba782b541bf1764e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:52 GMT
ADD file:1aab17002a9095c31dd6928277a045cb26846ac58c3d2d63316332c99a5f90bd in / 
# Thu, 16 Apr 2020 02:41:57 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 20:13:45 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 20:13:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 20:13:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 20:13:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 20:13:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 20:14:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 20:14:42 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 20:14:43 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 20:14:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 20:14:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 20:14:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3d48095d71a365b5910cea98e5566c152a3f9aa11657560568259bf93ff2f4cb`  
		Last Modified: Thu, 16 Apr 2020 02:48:58 GMT  
		Size: 25.9 MB (25857715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd185084a2a8907950a1957520ab48f0e324f87472c1c4f00290c499e3af4c16`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72cb36bacab8361b509f73295e37fde282152056a403ec02113a10f5ffe7d85`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 2.0 MB (2007781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1704638bc3bd1a976d9c9a114196312166b1d952c4d97c344f7c2055bf7e7220`  
		Last Modified: Thu, 16 Apr 2020 20:15:18 GMT  
		Size: 5.9 MB (5905308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae49dac5dafb2bd487a5d23af3079ee6219e38678ff3e18b2653736befab067`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1418a8cdbbb37964316e934e39bd2736fc3d7adae2a419f3214550eb33e28cac`  
		Last Modified: Thu, 16 Apr 2020 20:15:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:9926733306f68b93f7403e712d3b174452088a30ec88351759d30d5839bfc58e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41521584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eec8d26a366a17ca23d236b412935e8c92f33dc3880d1deb82b45b5fe326b141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 01:39:55 GMT
ADD file:ab0bbfba6c4b56420ffffc6cdddcc4592fff018f0cd07578c7dc0a5faa49df2f in / 
# Thu, 16 Apr 2020 01:39:56 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:15:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 02:15:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 02:15:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 02:15:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 02:15:56 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 02:15:56 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 02:15:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 02:15:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 02:15:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75bc60a98e6523be3fadd9128c1a630cb5cbd2d2d813ee5e99dc146a3de22254`  
		Last Modified: Thu, 16 Apr 2020 01:46:20 GMT  
		Size: 27.8 MB (27753976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434723a2b224f8837fdc460dc5691152d12aef50da6942fee530583efeeffceb`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67147847d2314c76ba55152b85f65e0bda1f059986ec62f8e9aac2ec676b74e3`  
		Last Modified: Thu, 16 Apr 2020 02:16:13 GMT  
		Size: 2.1 MB (2132347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdb13b1b28ff00c192060d5705212c0a7926b2774b1bd103671208e4881b959`  
		Last Modified: Thu, 16 Apr 2020 02:16:16 GMT  
		Size: 11.6 MB (11633094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4dbb06458c59576e1e3db43237dd2731ea9aa6328a653f2fc99c8411a7949`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b71d15bb761995984f6d4c0242516ef565183f0ce7954ff39bda3f2351873e`  
		Last Modified: Thu, 16 Apr 2020 02:16:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:1735539e3e7e65ef4d593b2f1e3c4d1c521d9f6257b9f933dfe8c908e47a82e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39494935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25ed7c69475d3ff2dff66671b3c85d66e3101aef828da38d6f348ae537664467`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 01:38:30 GMT
ADD file:9beea54416432abbd09d26b965c3c8e5bea8e233113f9bc308294c0008ee886f in / 
# Thu, 16 Apr 2020 01:38:39 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:32:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 06:33:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 06:33:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 06:33:11 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 06:33:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 06:36:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 06:36:18 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 06:36:25 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 06:36:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 06:36:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 06:36:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f268991f8af64097bbfefa3f01dd3fdb7f715051a3681f352504a3ecaa9d3596`  
		Last Modified: Thu, 16 Apr 2020 01:54:39 GMT  
		Size: 30.5 MB (30524651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11faf29322892c8e1a80bc63dd8d796125ee307f1e739960c976657247050849`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ccd1806ab2ac21ee209497c4c59d5575c5cfc5faaa1947e4cd86aa15528ceb`  
		Last Modified: Thu, 16 Apr 2020 06:37:13 GMT  
		Size: 2.2 MB (2224905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9229fa187f1524ad1611a629844a2268d6e05c41930bd0e1c7bb9f5a705ea0c`  
		Last Modified: Thu, 16 Apr 2020 06:37:13 GMT  
		Size: 6.7 MB (6743157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218baaa74ab7c90a3676e2b6df8502c735d933f9aed579caace6014489e22e7a`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a98a13b6647dbf2001ba52d55d8d20a502a25bb400ab75d79a9faf11e7cbc1`  
		Last Modified: Thu, 16 Apr 2020 06:37:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:0597e20ac03ff66cfad7d104787ed5b96a9ac7697ee48060f324e00844ab9529
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33479404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38f98e83f85547ac7f6e4dda1d8bb5e464e22042c46615866633476a1105da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:19 GMT
ADD file:f328b5d6dce2eaf00360542c1e3280958b818268b9150b12ffd1fddf030daf2f in / 
# Thu, 16 Apr 2020 00:42:20 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 09:13:28 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 16 Apr 2020 09:13:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 16 Apr 2020 09:13:32 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 16 Apr 2020 09:13:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 16 Apr 2020 09:13:47 GMT
VOLUME [/spiped]
# Thu, 16 Apr 2020 09:13:47 GMT
WORKDIR /spiped
# Thu, 16 Apr 2020 09:13:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 16 Apr 2020 09:13:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 09:13:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:043f95f5412a986fb082b0193860bb9c0388c2fbcb5e8bf5bcbbeefb0e45c9c5`  
		Last Modified: Thu, 16 Apr 2020 00:46:19 GMT  
		Size: 25.7 MB (25712234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6aec151b4cc88c9dc5605c8f4e8bec9649a643c744148850a655376e5d20932`  
		Last Modified: Thu, 16 Apr 2020 09:14:11 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48029c5984714761c355bc50aa231eda2d011113b6fdab73d47c970d1f85f96`  
		Last Modified: Thu, 16 Apr 2020 09:14:11 GMT  
		Size: 1.8 MB (1821695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95a36959cf23bd7d1a58f5f9d1f28c72cdecf869e55df64e15021f89f5b3dde`  
		Last Modified: Thu, 16 Apr 2020 09:14:17 GMT  
		Size: 5.9 MB (5943266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048afd803e0dd2ab2e4606727a11b6edf89f5704a3c6a7d6f94fa6f362e00398`  
		Last Modified: Thu, 16 Apr 2020 09:14:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d243505dd1bf28f3938608bf19a96bea5c30535181778c60e26498da2ec8ba5`  
		Last Modified: Thu, 16 Apr 2020 09:14:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
