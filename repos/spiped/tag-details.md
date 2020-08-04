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
$ docker pull spiped@sha256:c186489ce8d5b4665a3aba1ee7765dc0355a5712723f1734c8c5ad691b84cc89
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

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:1b3703b88c0276c49f6418cee6564711b22776ffac26ec226cd6ed3e5d597923
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e40d718c053f12a2f6145e68d9d8628a8316d4d443be41670b50186bb4d865`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:00:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 22:00:49 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 22:00:50 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 22:01:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 22:01:21 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 22:01:22 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 22:01:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 22:01:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 22:01:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e455e1b26a4f40221478d7ce62207280d0d13dedbfc7ca0aaf58c4340e0ddee8`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fccce412a71b5cfa4e30d597dd3a99cfe0db930c43a313bf55a4f714a1e3e46`  
		Last Modified: Wed, 22 Jul 2020 22:01:39 GMT  
		Size: 2.1 MB (2128096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf999adeab53fe5283762e7b188189794e3ab64b206b60b0cbaadbb2b4ebfb5`  
		Last Modified: Wed, 22 Jul 2020 22:01:40 GMT  
		Size: 7.0 MB (7037497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cb2457cdb40f945efdbe8b28f3b34265e1c058d0157ed4d9229949c448fede`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a140f8355f046a042ebbc60094d8df9aebef5deec4ed96b1f68d9cd26ff79bc0`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:db19d895fb6a9d435471972a00bad053d42c260a845d11ee7295d26eb0a9d569
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c974d20602696c79ad3326c6d1e9e96a70390a420aeca8fe2b35bd42d156d16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 03:13:17 GMT
ADD file:1a4c984d1bdb683e240e8bbdfeae45b146e1f8003444ce04a84096e58a437853 in / 
# Tue, 04 Aug 2020 03:13:27 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:48:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 06:48:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:48:26 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 06:48:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 06:48:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 06:49:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 06:49:37 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 06:49:38 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 06:49:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 06:49:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 06:50:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4eb4ac68461c572fdc826bae247c43484a232f91f165666714ce0f5f052b0bab`  
		Last Modified: Tue, 04 Aug 2020 03:34:09 GMT  
		Size: 24.8 MB (24836059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be79c9f269edfe97a3969652d481691516d6e3d3962970d286752ec267cdabb`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7c60c642cef1b748b289a9f5edc589ceee9ea8d3b4f975bd9f449c67467bbd`  
		Last Modified: Tue, 04 Aug 2020 06:50:21 GMT  
		Size: 1.8 MB (1839205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca2175b6694278f547776d37b858269feea55cc6ea6c75e86858c2cb492064e`  
		Last Modified: Tue, 04 Aug 2020 06:50:23 GMT  
		Size: 5.5 MB (5479896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0e27dc44576196364c3e47def03eb6b13be7429ecf695f9b1bf2ad58b990bb`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f32b6de5e9b0647fc040ab7ffc539c14b0982fbda33138e6343d938dc9b26b5`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bc1311bdb1275c4708af8e2cd81cb1dd11f150778a1a9e13ec6d53ee97510cd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df99957146f952e25c16b1313937c5316adf6e8007df66cc58ec7de40faddc89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:01:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:02:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:02:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:02:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:02:26 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:03:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:03:56 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:04:09 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:04:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:04:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:04:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22172af0169afa0272ff72035f6096febc5d3ede60ac04dc881d1f5800d26c5`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7f1fd14038efa078ebf94b7a162c116dccf414d7b1808cacccce99b0901b06`  
		Last Modified: Wed, 22 Jul 2020 20:05:19 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1cf7eb0ad13a880b9671f96239921ce5ef54c2f5d80739d3767cc6e9f4192d`  
		Last Modified: Wed, 22 Jul 2020 20:05:20 GMT  
		Size: 5.3 MB (5285371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a87f0dff307fe9f323cfd1b1b1cd03c3f80c7cf20ad189e632d3c404ec98b12`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffa36fa5c9d9b8b60adccf7841ed87be33586cfbc5df3f60268deccfc6e47c9`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:90ca459f2716fe31678308da1cd62d0af7b79d87b0401a7d3d0a776e1acc4ac0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd226f254c3be89ceb9c4bb6c20aefdc133df54afeb798bcdd4098fcb0a2892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:07:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:07:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:07:52 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:07:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:07:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:08:58 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:08:59 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:08:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:09:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:09:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090da1add6f1974e46f26d2d7f7f722c2b387919c849185bb10a219206f22062`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a8617f0abd2a6ab983a2f2837188637dfb2b47534998d9b7434d28953a4ffc`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 2.0 MB (2007866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f1e6d3329bb93eadc02dee0f5a04eff651b1486c3c23b92fa66712d006b6e`  
		Last Modified: Wed, 22 Jul 2020 20:09:20 GMT  
		Size: 5.9 MB (5905349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d31b1358e9f5e7cdb9a68fcac0ed93383f258525c9c26077aeb1861ffb6f52c`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a275c88ee92c00f538ac7771d7a052faf8a375fa59f2b9a2df2935bb34b44`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:b5f2f2310a9a18a1d32cdb874c7c5ae7b1b00daea074c03493694248af350c25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b03eea12202790aa4bbda365d8548cab39251e7e689592307463fb95ad3f3bff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:50:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 06:50:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 06:51:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 06:51:23 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 06:51:23 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 06:51:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 06:51:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 06:51:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300f881ca15feb57321700b3d988e8be855ed11fb7f0642226791b9cba968a19`  
		Last Modified: Tue, 04 Aug 2020 06:51:38 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaada7e04c42cdfa5da17209f4bb8b2247dd38fa88cb0e6c583367ff6ced6a54`  
		Last Modified: Tue, 04 Aug 2020 06:51:38 GMT  
		Size: 2.1 MB (2132346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff320cc8250c97cbe0c32e588f08e78b406095f5cc6eee92142a672358e8caf5`  
		Last Modified: Tue, 04 Aug 2020 06:51:41 GMT  
		Size: 11.6 MB (11633043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b0a67007b7b4fb0b3767c726474bb65742a3f94c52d6dfd06e5ab3767acacb`  
		Last Modified: Tue, 04 Aug 2020 06:51:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c9737acc508b5837f3673a5a0c1b5eb64d0b22ab6d0af857d2d1f5cd2782eb`  
		Last Modified: Tue, 04 Aug 2020 06:51:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

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

### `spiped:1` - linux; ppc64le

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

### `spiped:1` - linux; s390x

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

## `spiped:1.6`

```console
$ docker pull spiped@sha256:c186489ce8d5b4665a3aba1ee7765dc0355a5712723f1734c8c5ad691b84cc89
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

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:1b3703b88c0276c49f6418cee6564711b22776ffac26ec226cd6ed3e5d597923
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e40d718c053f12a2f6145e68d9d8628a8316d4d443be41670b50186bb4d865`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:00:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 22:00:49 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 22:00:50 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 22:01:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 22:01:21 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 22:01:22 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 22:01:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 22:01:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 22:01:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e455e1b26a4f40221478d7ce62207280d0d13dedbfc7ca0aaf58c4340e0ddee8`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fccce412a71b5cfa4e30d597dd3a99cfe0db930c43a313bf55a4f714a1e3e46`  
		Last Modified: Wed, 22 Jul 2020 22:01:39 GMT  
		Size: 2.1 MB (2128096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf999adeab53fe5283762e7b188189794e3ab64b206b60b0cbaadbb2b4ebfb5`  
		Last Modified: Wed, 22 Jul 2020 22:01:40 GMT  
		Size: 7.0 MB (7037497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cb2457cdb40f945efdbe8b28f3b34265e1c058d0157ed4d9229949c448fede`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a140f8355f046a042ebbc60094d8df9aebef5deec4ed96b1f68d9cd26ff79bc0`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:db19d895fb6a9d435471972a00bad053d42c260a845d11ee7295d26eb0a9d569
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c974d20602696c79ad3326c6d1e9e96a70390a420aeca8fe2b35bd42d156d16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 03:13:17 GMT
ADD file:1a4c984d1bdb683e240e8bbdfeae45b146e1f8003444ce04a84096e58a437853 in / 
# Tue, 04 Aug 2020 03:13:27 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:48:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 06:48:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:48:26 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 06:48:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 06:48:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 06:49:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 06:49:37 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 06:49:38 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 06:49:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 06:49:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 06:50:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4eb4ac68461c572fdc826bae247c43484a232f91f165666714ce0f5f052b0bab`  
		Last Modified: Tue, 04 Aug 2020 03:34:09 GMT  
		Size: 24.8 MB (24836059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be79c9f269edfe97a3969652d481691516d6e3d3962970d286752ec267cdabb`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7c60c642cef1b748b289a9f5edc589ceee9ea8d3b4f975bd9f449c67467bbd`  
		Last Modified: Tue, 04 Aug 2020 06:50:21 GMT  
		Size: 1.8 MB (1839205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca2175b6694278f547776d37b858269feea55cc6ea6c75e86858c2cb492064e`  
		Last Modified: Tue, 04 Aug 2020 06:50:23 GMT  
		Size: 5.5 MB (5479896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0e27dc44576196364c3e47def03eb6b13be7429ecf695f9b1bf2ad58b990bb`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f32b6de5e9b0647fc040ab7ffc539c14b0982fbda33138e6343d938dc9b26b5`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bc1311bdb1275c4708af8e2cd81cb1dd11f150778a1a9e13ec6d53ee97510cd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df99957146f952e25c16b1313937c5316adf6e8007df66cc58ec7de40faddc89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:01:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:02:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:02:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:02:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:02:26 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:03:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:03:56 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:04:09 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:04:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:04:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:04:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22172af0169afa0272ff72035f6096febc5d3ede60ac04dc881d1f5800d26c5`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7f1fd14038efa078ebf94b7a162c116dccf414d7b1808cacccce99b0901b06`  
		Last Modified: Wed, 22 Jul 2020 20:05:19 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1cf7eb0ad13a880b9671f96239921ce5ef54c2f5d80739d3767cc6e9f4192d`  
		Last Modified: Wed, 22 Jul 2020 20:05:20 GMT  
		Size: 5.3 MB (5285371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a87f0dff307fe9f323cfd1b1b1cd03c3f80c7cf20ad189e632d3c404ec98b12`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffa36fa5c9d9b8b60adccf7841ed87be33586cfbc5df3f60268deccfc6e47c9`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:90ca459f2716fe31678308da1cd62d0af7b79d87b0401a7d3d0a776e1acc4ac0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd226f254c3be89ceb9c4bb6c20aefdc133df54afeb798bcdd4098fcb0a2892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:07:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:07:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:07:52 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:07:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:07:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:08:58 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:08:59 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:08:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:09:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:09:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090da1add6f1974e46f26d2d7f7f722c2b387919c849185bb10a219206f22062`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a8617f0abd2a6ab983a2f2837188637dfb2b47534998d9b7434d28953a4ffc`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 2.0 MB (2007866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f1e6d3329bb93eadc02dee0f5a04eff651b1486c3c23b92fa66712d006b6e`  
		Last Modified: Wed, 22 Jul 2020 20:09:20 GMT  
		Size: 5.9 MB (5905349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d31b1358e9f5e7cdb9a68fcac0ed93383f258525c9c26077aeb1861ffb6f52c`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a275c88ee92c00f538ac7771d7a052faf8a375fa59f2b9a2df2935bb34b44`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:b5f2f2310a9a18a1d32cdb874c7c5ae7b1b00daea074c03493694248af350c25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b03eea12202790aa4bbda365d8548cab39251e7e689592307463fb95ad3f3bff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:50:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 06:50:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 06:51:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 06:51:23 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 06:51:23 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 06:51:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 06:51:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 06:51:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300f881ca15feb57321700b3d988e8be855ed11fb7f0642226791b9cba968a19`  
		Last Modified: Tue, 04 Aug 2020 06:51:38 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaada7e04c42cdfa5da17209f4bb8b2247dd38fa88cb0e6c583367ff6ced6a54`  
		Last Modified: Tue, 04 Aug 2020 06:51:38 GMT  
		Size: 2.1 MB (2132346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff320cc8250c97cbe0c32e588f08e78b406095f5cc6eee92142a672358e8caf5`  
		Last Modified: Tue, 04 Aug 2020 06:51:41 GMT  
		Size: 11.6 MB (11633043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b0a67007b7b4fb0b3767c726474bb65742a3f94c52d6dfd06e5ab3767acacb`  
		Last Modified: Tue, 04 Aug 2020 06:51:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c9737acc508b5837f3673a5a0c1b5eb64d0b22ab6d0af857d2d1f5cd2782eb`  
		Last Modified: Tue, 04 Aug 2020 06:51:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

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

### `spiped:1.6` - linux; ppc64le

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

### `spiped:1.6` - linux; s390x

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

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:c186489ce8d5b4665a3aba1ee7765dc0355a5712723f1734c8c5ad691b84cc89
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

### `spiped:1.6.1` - linux; amd64

```console
$ docker pull spiped@sha256:1b3703b88c0276c49f6418cee6564711b22776ffac26ec226cd6ed3e5d597923
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e40d718c053f12a2f6145e68d9d8628a8316d4d443be41670b50186bb4d865`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:00:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 22:00:49 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 22:00:50 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 22:01:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 22:01:21 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 22:01:22 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 22:01:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 22:01:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 22:01:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e455e1b26a4f40221478d7ce62207280d0d13dedbfc7ca0aaf58c4340e0ddee8`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fccce412a71b5cfa4e30d597dd3a99cfe0db930c43a313bf55a4f714a1e3e46`  
		Last Modified: Wed, 22 Jul 2020 22:01:39 GMT  
		Size: 2.1 MB (2128096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf999adeab53fe5283762e7b188189794e3ab64b206b60b0cbaadbb2b4ebfb5`  
		Last Modified: Wed, 22 Jul 2020 22:01:40 GMT  
		Size: 7.0 MB (7037497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cb2457cdb40f945efdbe8b28f3b34265e1c058d0157ed4d9229949c448fede`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a140f8355f046a042ebbc60094d8df9aebef5deec4ed96b1f68d9cd26ff79bc0`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:db19d895fb6a9d435471972a00bad053d42c260a845d11ee7295d26eb0a9d569
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c974d20602696c79ad3326c6d1e9e96a70390a420aeca8fe2b35bd42d156d16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 03:13:17 GMT
ADD file:1a4c984d1bdb683e240e8bbdfeae45b146e1f8003444ce04a84096e58a437853 in / 
# Tue, 04 Aug 2020 03:13:27 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:48:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 06:48:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:48:26 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 06:48:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 06:48:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 06:49:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 06:49:37 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 06:49:38 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 06:49:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 06:49:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 06:50:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4eb4ac68461c572fdc826bae247c43484a232f91f165666714ce0f5f052b0bab`  
		Last Modified: Tue, 04 Aug 2020 03:34:09 GMT  
		Size: 24.8 MB (24836059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be79c9f269edfe97a3969652d481691516d6e3d3962970d286752ec267cdabb`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7c60c642cef1b748b289a9f5edc589ceee9ea8d3b4f975bd9f449c67467bbd`  
		Last Modified: Tue, 04 Aug 2020 06:50:21 GMT  
		Size: 1.8 MB (1839205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca2175b6694278f547776d37b858269feea55cc6ea6c75e86858c2cb492064e`  
		Last Modified: Tue, 04 Aug 2020 06:50:23 GMT  
		Size: 5.5 MB (5479896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0e27dc44576196364c3e47def03eb6b13be7429ecf695f9b1bf2ad58b990bb`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f32b6de5e9b0647fc040ab7ffc539c14b0982fbda33138e6343d938dc9b26b5`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bc1311bdb1275c4708af8e2cd81cb1dd11f150778a1a9e13ec6d53ee97510cd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df99957146f952e25c16b1313937c5316adf6e8007df66cc58ec7de40faddc89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:01:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:02:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:02:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:02:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:02:26 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:03:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:03:56 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:04:09 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:04:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:04:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:04:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22172af0169afa0272ff72035f6096febc5d3ede60ac04dc881d1f5800d26c5`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7f1fd14038efa078ebf94b7a162c116dccf414d7b1808cacccce99b0901b06`  
		Last Modified: Wed, 22 Jul 2020 20:05:19 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1cf7eb0ad13a880b9671f96239921ce5ef54c2f5d80739d3767cc6e9f4192d`  
		Last Modified: Wed, 22 Jul 2020 20:05:20 GMT  
		Size: 5.3 MB (5285371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a87f0dff307fe9f323cfd1b1b1cd03c3f80c7cf20ad189e632d3c404ec98b12`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffa36fa5c9d9b8b60adccf7841ed87be33586cfbc5df3f60268deccfc6e47c9`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:90ca459f2716fe31678308da1cd62d0af7b79d87b0401a7d3d0a776e1acc4ac0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd226f254c3be89ceb9c4bb6c20aefdc133df54afeb798bcdd4098fcb0a2892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:07:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:07:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:07:52 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:07:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:07:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:08:58 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:08:59 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:08:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:09:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:09:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090da1add6f1974e46f26d2d7f7f722c2b387919c849185bb10a219206f22062`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a8617f0abd2a6ab983a2f2837188637dfb2b47534998d9b7434d28953a4ffc`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 2.0 MB (2007866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f1e6d3329bb93eadc02dee0f5a04eff651b1486c3c23b92fa66712d006b6e`  
		Last Modified: Wed, 22 Jul 2020 20:09:20 GMT  
		Size: 5.9 MB (5905349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d31b1358e9f5e7cdb9a68fcac0ed93383f258525c9c26077aeb1861ffb6f52c`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a275c88ee92c00f538ac7771d7a052faf8a375fa59f2b9a2df2935bb34b44`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:b5f2f2310a9a18a1d32cdb874c7c5ae7b1b00daea074c03493694248af350c25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b03eea12202790aa4bbda365d8548cab39251e7e689592307463fb95ad3f3bff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:50:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 06:50:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 06:51:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 06:51:23 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 06:51:23 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 06:51:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 06:51:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 06:51:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300f881ca15feb57321700b3d988e8be855ed11fb7f0642226791b9cba968a19`  
		Last Modified: Tue, 04 Aug 2020 06:51:38 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaada7e04c42cdfa5da17209f4bb8b2247dd38fa88cb0e6c583367ff6ced6a54`  
		Last Modified: Tue, 04 Aug 2020 06:51:38 GMT  
		Size: 2.1 MB (2132346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff320cc8250c97cbe0c32e588f08e78b406095f5cc6eee92142a672358e8caf5`  
		Last Modified: Tue, 04 Aug 2020 06:51:41 GMT  
		Size: 11.6 MB (11633043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b0a67007b7b4fb0b3767c726474bb65742a3f94c52d6dfd06e5ab3767acacb`  
		Last Modified: Tue, 04 Aug 2020 06:51:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c9737acc508b5837f3673a5a0c1b5eb64d0b22ab6d0af857d2d1f5cd2782eb`  
		Last Modified: Tue, 04 Aug 2020 06:51:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

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

### `spiped:1.6.1` - linux; ppc64le

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

### `spiped:1.6.1` - linux; s390x

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

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:c186489ce8d5b4665a3aba1ee7765dc0355a5712723f1734c8c5ad691b84cc89
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
$ docker pull spiped@sha256:1b3703b88c0276c49f6418cee6564711b22776ffac26ec226cd6ed3e5d597923
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e40d718c053f12a2f6145e68d9d8628a8316d4d443be41670b50186bb4d865`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:00:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 22:00:49 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 22:00:49 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 22:00:50 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 22:01:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 22:01:21 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 22:01:22 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 22:01:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 22:01:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 22:01:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e455e1b26a4f40221478d7ce62207280d0d13dedbfc7ca0aaf58c4340e0ddee8`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fccce412a71b5cfa4e30d597dd3a99cfe0db930c43a313bf55a4f714a1e3e46`  
		Last Modified: Wed, 22 Jul 2020 22:01:39 GMT  
		Size: 2.1 MB (2128096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf999adeab53fe5283762e7b188189794e3ab64b206b60b0cbaadbb2b4ebfb5`  
		Last Modified: Wed, 22 Jul 2020 22:01:40 GMT  
		Size: 7.0 MB (7037497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cb2457cdb40f945efdbe8b28f3b34265e1c058d0157ed4d9229949c448fede`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a140f8355f046a042ebbc60094d8df9aebef5deec4ed96b1f68d9cd26ff79bc0`  
		Last Modified: Wed, 22 Jul 2020 22:01:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:db19d895fb6a9d435471972a00bad053d42c260a845d11ee7295d26eb0a9d569
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c974d20602696c79ad3326c6d1e9e96a70390a420aeca8fe2b35bd42d156d16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 03:13:17 GMT
ADD file:1a4c984d1bdb683e240e8bbdfeae45b146e1f8003444ce04a84096e58a437853 in / 
# Tue, 04 Aug 2020 03:13:27 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:48:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 06:48:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:48:26 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 06:48:28 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 06:48:28 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 06:49:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 06:49:37 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 06:49:38 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 06:49:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 06:49:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 06:50:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4eb4ac68461c572fdc826bae247c43484a232f91f165666714ce0f5f052b0bab`  
		Last Modified: Tue, 04 Aug 2020 03:34:09 GMT  
		Size: 24.8 MB (24836059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be79c9f269edfe97a3969652d481691516d6e3d3962970d286752ec267cdabb`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7c60c642cef1b748b289a9f5edc589ceee9ea8d3b4f975bd9f449c67467bbd`  
		Last Modified: Tue, 04 Aug 2020 06:50:21 GMT  
		Size: 1.8 MB (1839205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca2175b6694278f547776d37b858269feea55cc6ea6c75e86858c2cb492064e`  
		Last Modified: Tue, 04 Aug 2020 06:50:23 GMT  
		Size: 5.5 MB (5479896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0e27dc44576196364c3e47def03eb6b13be7429ecf695f9b1bf2ad58b990bb`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f32b6de5e9b0647fc040ab7ffc539c14b0982fbda33138e6343d938dc9b26b5`  
		Last Modified: Tue, 04 Aug 2020 06:50:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:bc1311bdb1275c4708af8e2cd81cb1dd11f150778a1a9e13ec6d53ee97510cd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df99957146f952e25c16b1313937c5316adf6e8007df66cc58ec7de40faddc89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:01:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:02:05 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:02:12 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:02:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:02:26 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:03:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:03:56 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:04:09 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:04:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:04:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:04:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22172af0169afa0272ff72035f6096febc5d3ede60ac04dc881d1f5800d26c5`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7f1fd14038efa078ebf94b7a162c116dccf414d7b1808cacccce99b0901b06`  
		Last Modified: Wed, 22 Jul 2020 20:05:19 GMT  
		Size: 1.8 MB (1759438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1cf7eb0ad13a880b9671f96239921ce5ef54c2f5d80739d3767cc6e9f4192d`  
		Last Modified: Wed, 22 Jul 2020 20:05:20 GMT  
		Size: 5.3 MB (5285371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a87f0dff307fe9f323cfd1b1b1cd03c3f80c7cf20ad189e632d3c404ec98b12`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffa36fa5c9d9b8b60adccf7841ed87be33586cfbc5df3f60268deccfc6e47c9`  
		Last Modified: Wed, 22 Jul 2020 20:05:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:90ca459f2716fe31678308da1cd62d0af7b79d87b0401a7d3d0a776e1acc4ac0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd226f254c3be89ceb9c4bb6c20aefdc133df54afeb798bcdd4098fcb0a2892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:07:41 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Jul 2020 20:07:51 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:07:52 GMT
ENV SPIPED_VERSION=1.6.1
# Wed, 22 Jul 2020 20:07:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Wed, 22 Jul 2020 20:07:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 22 Jul 2020 20:08:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Jul 2020 20:08:58 GMT
VOLUME [/spiped]
# Wed, 22 Jul 2020 20:08:59 GMT
WORKDIR /spiped
# Wed, 22 Jul 2020 20:08:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Jul 2020 20:09:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 20:09:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090da1add6f1974e46f26d2d7f7f722c2b387919c849185bb10a219206f22062`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a8617f0abd2a6ab983a2f2837188637dfb2b47534998d9b7434d28953a4ffc`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 2.0 MB (2007866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f1e6d3329bb93eadc02dee0f5a04eff651b1486c3c23b92fa66712d006b6e`  
		Last Modified: Wed, 22 Jul 2020 20:09:20 GMT  
		Size: 5.9 MB (5905349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d31b1358e9f5e7cdb9a68fcac0ed93383f258525c9c26077aeb1861ffb6f52c`  
		Last Modified: Wed, 22 Jul 2020 20:09:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a275c88ee92c00f538ac7771d7a052faf8a375fa59f2b9a2df2935bb34b44`  
		Last Modified: Wed, 22 Jul 2020 20:09:19 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:b5f2f2310a9a18a1d32cdb874c7c5ae7b1b00daea074c03493694248af350c25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b03eea12202790aa4bbda365d8548cab39251e7e689592307463fb95ad3f3bff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:50:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 06:50:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 06:50:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 06:51:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 06:51:23 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 06:51:23 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 06:51:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 06:51:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 06:51:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300f881ca15feb57321700b3d988e8be855ed11fb7f0642226791b9cba968a19`  
		Last Modified: Tue, 04 Aug 2020 06:51:38 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaada7e04c42cdfa5da17209f4bb8b2247dd38fa88cb0e6c583367ff6ced6a54`  
		Last Modified: Tue, 04 Aug 2020 06:51:38 GMT  
		Size: 2.1 MB (2132346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff320cc8250c97cbe0c32e588f08e78b406095f5cc6eee92142a672358e8caf5`  
		Last Modified: Tue, 04 Aug 2020 06:51:41 GMT  
		Size: 11.6 MB (11633043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b0a67007b7b4fb0b3767c726474bb65742a3f94c52d6dfd06e5ab3767acacb`  
		Last Modified: Tue, 04 Aug 2020 06:51:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c9737acc508b5837f3673a5a0c1b5eb64d0b22ab6d0af857d2d1f5cd2782eb`  
		Last Modified: Tue, 04 Aug 2020 06:51:37 GMT  
		Size: 341.0 B  
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
