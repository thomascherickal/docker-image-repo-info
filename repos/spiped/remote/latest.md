## `spiped:latest`

```console
$ docker pull spiped@sha256:b7cd1583573360b3a88cfaa2d9e7e0bb34f4460ae8935891073f30a6ae141765
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
$ docker pull spiped@sha256:be1e1273f203254dbe788f80482ad7eb3dda4a61446fa4d8fe046d8d6b342ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36259502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de3a9d7ad126b00ea958b4f0240d31d91c8a8582af4ddac8570e1935de03c70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 17:53:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 31 Mar 2020 17:54:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 06 Apr 2020 21:12:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 06 Apr 2020 21:12:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 06 Apr 2020 21:12:54 GMT
VOLUME [/spiped]
# Mon, 06 Apr 2020 21:12:55 GMT
WORKDIR /spiped
# Mon, 06 Apr 2020 21:12:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 06 Apr 2020 21:12:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Apr 2020 21:12:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af711a0248b008edeb7fc3ec89d9b65d0e6bc9a7812f17e7c0e1981713091b0`  
		Last Modified: Tue, 31 Mar 2020 17:54:57 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf07c97371206072919de7231d4a5b645fc9214d9477f21dff3c4bcf2d836ca`  
		Last Modified: Tue, 31 Mar 2020 17:54:57 GMT  
		Size: 2.1 MB (2128010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf676d0d98d691716d2c2ac3f58d9300f97af52c37052d44f1991d468c20da`  
		Last Modified: Mon, 06 Apr 2020 21:13:51 GMT  
		Size: 7.0 MB (7037456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772658cc02099a47df92d23a2dc7b78ff48f02f3c5eae197d45e5595ca79dae3`  
		Last Modified: Mon, 06 Apr 2020 21:13:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9fba6c68631c186e227ec9fc3a8bec328a5ea49571cbd3718c6872dfa9474`  
		Last Modified: Mon, 06 Apr 2020 21:13:48 GMT  
		Size: 342.0 B  
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
