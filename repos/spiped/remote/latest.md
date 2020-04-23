## `spiped:latest`

```console
$ docker pull spiped@sha256:7190f774165bdc6fb0a911e86ed04b9cbbf5bebe3d60fb056f8d0dd0ea55f33a
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
$ docker pull spiped@sha256:87e594e6c297ab32b63899e657c1a54a8d1100d3b615aba3110b9c83af034bf4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3762d7fbd521ea9dd741d0c9728f84de283ec800689749f6154163ac375146ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:37:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 06:37:11 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 06:37:12 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 06:37:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 06:37:15 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 06:38:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 06:38:07 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 06:38:07 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 06:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 06:38:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c245760c54fc8d94586399ec9055355e4c3366a9bbb2fa8adfc6f906feb4be2e`  
		Last Modified: Thu, 23 Apr 2020 06:38:30 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e881f703761ee378af97245f067193b18a2e259c6960350af6bd58c50c17c9`  
		Last Modified: Thu, 23 Apr 2020 06:38:31 GMT  
		Size: 1.8 MB (1759439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff85ebb091bd4c189eb2fbb13813d47c9bb4a87981d5e5e7f024ba3a70413717`  
		Last Modified: Thu, 23 Apr 2020 06:38:33 GMT  
		Size: 5.3 MB (5285357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe372689bc3dcd9f9fcc3170419cbe8cdf8289b8ab46d6658e6f9afdb311b92`  
		Last Modified: Thu, 23 Apr 2020 06:38:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a07c2d12354b78115b49045a435919c09508a793f325a501637f134f608c3`  
		Last Modified: Thu, 23 Apr 2020 06:38:30 GMT  
		Size: 343.0 B  
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
$ docker pull spiped@sha256:b214baf0880f0e0bf92f0a90a36e57ce4e397b1cef91bd453c5ec1469be1009a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41521550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52544dbfee957c83d14c3ae836ec363c5cf19e2e670148c5c521237ecf624b72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:28:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 01:28:26 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:28:26 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 01:28:27 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 01:28:27 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 01:28:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 01:28:59 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 01:28:59 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 01:29:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 01:29:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 01:29:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351e27645b6f5e870fc78e7e83842a6acfae4f22264753cebffb3736d6c6b4e0`  
		Last Modified: Thu, 23 Apr 2020 01:29:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4caf13bd3757ace65a266e4db85f035bb32b641e7ada6686776f45ddfc92a7`  
		Last Modified: Thu, 23 Apr 2020 01:29:13 GMT  
		Size: 2.1 MB (2132300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a150a89f22944c7d67885dffb670eaff2528ad89c09300893b00bbb5f0f5d20`  
		Last Modified: Thu, 23 Apr 2020 01:29:16 GMT  
		Size: 11.6 MB (11633110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa045c9198af6fc070fae84ddaedfc5e048a77ecd5bee4cefe5e9e00090cd69a`  
		Last Modified: Thu, 23 Apr 2020 01:29:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4208cdaaa4a2654147de2ba2070864eafc67a4fce29e7c405408d20dbc0d9bf`  
		Last Modified: Thu, 23 Apr 2020 01:29:12 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:f91e47bbc5d31233784f17f5565a334606257d7e9a8693464e19e161ccf0ad55
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33892434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f619d07812967c4818dcd6cd9c058089617c714dd36691b599dddf20c7e80ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:03:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 06:03:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 06:03:51 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 06:03:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 06:03:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 06:05:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 06:05:01 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 06:05:01 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 06:05:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 06:05:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51904ae673f6205aeb18b4941b0b86dd612faf95ba48129549fb43f070abf2e6`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8a20e087a159fd2aeb1c2b68b7a8006cd0a9d69141c635cbe7100d4cb72547`  
		Last Modified: Thu, 23 Apr 2020 06:05:23 GMT  
		Size: 1.7 MB (1711985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbc1f20c1494ea8864c22058f6f84349cf689cdc791257665d01c137a543425`  
		Last Modified: Thu, 23 Apr 2020 06:05:29 GMT  
		Size: 6.4 MB (6416148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab5a2be89807e61f976284ab0b61756a179cb137a417fcd3284114bb22b515c`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084fea47f48a62a2012edff72d4d4c401e085a93313a868c4b8861d4b98e77fa`  
		Last Modified: Thu, 23 Apr 2020 06:05:22 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:02d48985307981eb8e7c97230ccaf92d0f5f40721ba3f7b1d8a68f7da46b3df5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33479371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26c393693b28332310170db4cf2d624c6d64ecb78cd4c34c205cad782200af22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 07:02:40 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Apr 2020 07:02:43 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 07:02:43 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 07:02:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 07:02:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 07:03:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Apr 2020 07:03:06 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 07:03:06 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 07:03:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:03:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 07:03:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ef404091af1564b11c8c1ac6b7eb84f2275bf60fd7dfb4c44eae598f04b971`  
		Last Modified: Thu, 23 Apr 2020 07:03:20 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a9f34b0c0e7fdb8035427c568008ce87f8d88998aa4d47d259ee3e077e8eb4`  
		Last Modified: Thu, 23 Apr 2020 07:03:26 GMT  
		Size: 1.8 MB (1821736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eafed14eaef28a5ccc87299b1a916f59f687d975423913c529867e347cddd6f`  
		Last Modified: Thu, 23 Apr 2020 07:03:22 GMT  
		Size: 5.9 MB (5943320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b26e5542e7d4323623b7f5d3e61b8ba8b24c86bf423a0ea5a706282cf7e975`  
		Last Modified: Thu, 23 Apr 2020 07:03:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f51c7886443a26f3b079bbbc826a33a0859fd26610414c4013fda6fd2f2578e`  
		Last Modified: Thu, 23 Apr 2020 07:03:36 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
