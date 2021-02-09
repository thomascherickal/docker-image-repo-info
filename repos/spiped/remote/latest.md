## `spiped:latest`

```console
$ docker pull spiped@sha256:983be21b5d12b2e717eff2a1b61b3da5a954605ef645d945fd402fde0d8a9766
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
$ docker pull spiped@sha256:813fe508ddf7ef14c654e08581a59df5889155822eb779846196b8e849333938
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36263367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67f39dd2d121caaec0db3bb313564c512f9f974333b8a772963e9a9790a21a3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:21:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 11:21:43 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:21:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 11:21:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 11:21:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 11:22:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 11:22:13 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 11:22:14 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 11:22:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 11:22:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 11:22:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de752b69da20dffa4f368194c801b91db7f8109eb73f00e28fcf2534595c2391`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29700ba41d506288d95fe910fe16a1412fdf652d9919afe82028b5ee5b3c04ca`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 2.1 MB (2128396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412d577285af429a0e5119c64eb42081167590075ec5fb38a4d4433890b406ba`  
		Last Modified: Tue, 09 Feb 2021 11:22:40 GMT  
		Size: 7.0 MB (7037659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc602331c59adaf25976f51dc954d66801d075f027483281c6b79bd2f12c468`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3991a274f6591f9860d4f7e3d73124d6024fd27dc097414d36cda87813ef0619`  
		Last Modified: Tue, 09 Feb 2021 11:22:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:7f6d7dcae2bcbc63a71c78634690325aa893f07b23ebdf89d495772e2b76e9c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32161112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7630b8d3c6a6778b6bf060e33944e07408a5d869c0790a7912fdb44c722221d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:50:10 GMT
ADD file:fbd00ef7871dc27d7ed5fa8c238cdc80652bd87b8033be7de9e54a799bbf10a4 in / 
# Tue, 09 Feb 2021 02:50:11 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:43:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 11:43:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:43:33 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 11:43:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 11:43:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 11:44:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 11:44:28 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 11:44:29 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 11:44:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 11:44:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 11:44:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8e683fcc73f4da7d69ce1d5f4e1d77510aa459490068f38db2d8663698b391a0`  
		Last Modified: Tue, 09 Feb 2021 02:59:07 GMT  
		Size: 24.8 MB (24839297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346f1f77623bfcedac114c95542f4a432dbfac2903c21d7af096733db6f08d7a`  
		Last Modified: Tue, 09 Feb 2021 11:44:58 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46e79f1e8ee1ac5539cad7eefe848b44ce737e874098030fc6156b53ef573a9`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 1.8 MB (1839405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c4f4a4d55f4bff867187ec0fc856d3831a4013bc7b2439663a05c05e0bceba`  
		Last Modified: Tue, 09 Feb 2021 11:45:01 GMT  
		Size: 5.5 MB (5480212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722e4239f41acf1439f868feb56543ec05a7990de0b7e19b785a656ed9cc8245`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3795fccfaef5453c447609dbd35488bfe50615dbc8aabc29d60f5c70747a28`  
		Last Modified: Tue, 09 Feb 2021 11:44:59 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3ac6871810ed67f5b21e7cd83802fdae6ecb8cc0adcf6f04aaeb1bb55469b360
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29763190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:618f6b2b1cf55feedae7e3db3ca36f7b0e57e0e8df3027fa07ea587c77c1fcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:56:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 16:56:53 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:56:54 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 16:56:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 16:56:57 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 16:57:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 16:57:52 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 16:57:54 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 16:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 16:57:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 16:58:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d8c6b0eb8c3c505236b6ba8f4abeac7cb42c568eaf1638d25605157eed1665`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48182b80525569a49c82ed71c8174f895558d9cb63f669e97286a51ffc26a6`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 1.8 MB (1759589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374c08338c9f1b9019e7e9285ef3d48d0f993f4714a4cbdb5d918dbf578488c3`  
		Last Modified: Tue, 12 Jan 2021 16:58:26 GMT  
		Size: 5.3 MB (5285488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3720b24b60513881270a650b3c1d4177311c5c61ba11e7333f0231487e96596`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97338a06275c6f888b2a3c5fe0b46e06182ab49c90fb9eba4c659df33d10c06e`  
		Last Modified: Tue, 12 Jan 2021 16:58:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31637f8d6ad0ee45f28895469c0e04c06f6fac3d7f150cc80fe078c4cad24ce9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33767135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b7372db271f79369881f951f67daf6bb9c182e12ed0fa8c7733f512edbd2231`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:18:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 18:18:41 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 18:18:42 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 18:18:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 18:18:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 18:19:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 18:19:36 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 18:19:37 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 18:19:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 18:19:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 18:19:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516c8ae6b6958174393d642fd4693aea0a041e432ce8d8758b052224d96cb2fa`  
		Last Modified: Tue, 09 Feb 2021 18:20:06 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaa1313bd324e5619976d9a300f6b8270de044856e53fd25b80f90d13cc5f01`  
		Last Modified: Tue, 09 Feb 2021 18:20:06 GMT  
		Size: 2.0 MB (2007840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c146b1359c1aa6edb520a730ce0d1ecef2b90a6f1c3d7bd7c6b92e4eb3ded6`  
		Last Modified: Tue, 09 Feb 2021 18:20:08 GMT  
		Size: 5.9 MB (5905639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942793b643fefa9c5d8c29e1d1afdf91e8fb3e2b219a2c25aea1c1f227d7ff9e`  
		Last Modified: Tue, 09 Feb 2021 18:20:06 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e0b8f80105f5c4eedc0c9bd6b91ad252978658eb4ea07bd7c5275bf60a2d12`  
		Last Modified: Tue, 09 Feb 2021 18:20:06 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:7c10d16a5cdc4eb038d7d3db80fff79e0c87596803df904adca7467720db9c2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41520623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a49946de815afcc582a42860d709dbcaa88738202bce1c869d9b53deb27e606`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:39:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 18:40:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 18:40:02 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 18:40:02 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 18:40:02 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 18:40:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 18:40:35 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 18:40:35 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 18:40:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 18:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 18:40:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbea90aac4746d1c996386053d6406bfa4610451eae6d17da249dee74c9b3a68`  
		Last Modified: Tue, 09 Feb 2021 18:40:55 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88ece221099a0a2111a5d7bf95569c3145edd7f6b05b5af10a7d0168f306530`  
		Last Modified: Tue, 09 Feb 2021 18:40:55 GMT  
		Size: 2.1 MB (2132497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfc4419687d796b347009d81739f5a4453ff609e1404aab76fa4fdbf98c18a2`  
		Last Modified: Tue, 09 Feb 2021 18:40:59 GMT  
		Size: 11.6 MB (11633232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54dba4e4aa0b7a97f0fc826eb1c9f7d260755b576173deb1101957612258f1b`  
		Last Modified: Tue, 09 Feb 2021 18:40:55 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8958cc7a50959aa2eef610a3178a26f8a5ba452d96d230552f26c400460e5289`  
		Last Modified: Tue, 09 Feb 2021 18:40:55 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:92252fa9e4780548e358d5b38d69316a06e12e220122b9610404582f92a89094
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33895800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03dadb4a8dbd4dd9d533ab18afe023801e08b08d448eb320d54abb567df20df4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 03:09:26 GMT
ADD file:0222a151f4e5033d9eae98ce2b703a63f52d049dd72ac40bdd0dc2dafe619f0a in / 
# Tue, 09 Feb 2021 03:09:27 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:51:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 17:52:01 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:52:01 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 17:52:02 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 17:52:02 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 17:53:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 17:53:09 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 17:53:10 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 17:53:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 17:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 17:53:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dfb81134097d874e01b495d1fba82e384056d0a3a45f01a69a2e86ae82af1e96`  
		Last Modified: Tue, 09 Feb 2021 03:15:55 GMT  
		Size: 25.8 MB (25764640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8e1cbf99b578f9b5da0b78824733a66db880b685f597795dd41a08ac6b4f2f`  
		Last Modified: Tue, 09 Feb 2021 17:53:36 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1aacac04ed58354f88d08f5ca6f467ecf1a60a5eef64bab754793eaa0ca8c4`  
		Last Modified: Tue, 09 Feb 2021 17:53:38 GMT  
		Size: 1.7 MB (1712353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a175c21b572d3e361f5b75f83a345f0b2ee8243ddca2e2d104ca4d66fb177036`  
		Last Modified: Tue, 09 Feb 2021 17:53:45 GMT  
		Size: 6.4 MB (6416637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894a85f2308dfdacce5e052bb76f888a07a78c9898d4af348dd3d704d39abb72`  
		Last Modified: Tue, 09 Feb 2021 17:53:36 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdde0a7f0aac61ee28e4cfd0c1a73b01d1252df7f66e484817c647e92c75a8ff`  
		Last Modified: Tue, 09 Feb 2021 17:53:36 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:84ac8fc004070cc9c2effe0bb5054983c3b9ddc67d98f29310d5ccb7b6e0317a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39490582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18323e6de87099c0fdb5d1f21f7d13b343c56015aa0c28f67210e1773adf20fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:15:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 04:17:12 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:17:15 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 04:17:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 04:17:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 04:25:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 04:25:48 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 04:25:57 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 04:25:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 04:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 04:26:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46b97146405ece3ed453ad4ebc496b4b66b0fff54fdc49d2f4d3175043dffaf`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74075dd02f1d1e43b4fc1df6e050d800b9cee069d728e418758c5de00c8aab8`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 2.2 MB (2225177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea580c66676d35f6b86a60aed47a5cc5d25cb3a5d40d018953269820a453e5c`  
		Last Modified: Tue, 09 Feb 2021 04:26:41 GMT  
		Size: 6.7 MB (6743685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e9b505e0637e70b6aeacc7c2b4871dae0dc64900ccc75b80a1cb38714f859`  
		Last Modified: Tue, 09 Feb 2021 04:26:39 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37ff63f62cb2d6c72f328cc4550e6e65dc3382a23b9d6dd4e61a8d6752d0ecc`  
		Last Modified: Tue, 09 Feb 2021 04:26:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:e1324194f0c52dc9f439b3ffcbe90f7063ed357377449c6e03ac3b1e99c9b922
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33477883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cd7089a6ca9e042116c7af0c6f1e0972068d5dab27a545d24e1442f6a42b11a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:10 GMT
ADD file:0edb2de05df54191a141bd125f59d7e14eef0cc4576927a247b8dd7d6f255d04 in / 
# Tue, 09 Feb 2021 02:42:12 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:33:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Feb 2021 06:33:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 06:33:42 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Feb 2021 06:33:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Feb 2021 06:33:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Feb 2021 06:33:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Feb 2021 06:33:59 GMT
VOLUME [/spiped]
# Tue, 09 Feb 2021 06:33:59 GMT
WORKDIR /spiped
# Tue, 09 Feb 2021 06:33:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:34:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Feb 2021 06:34:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:032413a44cf56b097e48b8221bf475ca1bec26e7a27f35fe61d699366a335b79`  
		Last Modified: Tue, 09 Feb 2021 02:45:31 GMT  
		Size: 25.7 MB (25710021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b494d8c5eab48f88712e47a52fa76da28e3b84d610e47c02ef6554cc1e57e98a`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee2f8e8efcd7e5d4ee3b434aed6008829ab2a40fc4e406d28c78b30a00a46d`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 1.8 MB (1821962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ff6c2fa7826622f66fc54c0ce06350d1802aaf2e378e77109208395d04b813`  
		Last Modified: Tue, 09 Feb 2021 06:34:20 GMT  
		Size: 5.9 MB (5943696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d941fa4c020c2b7bee864d1838e2a9a16d366a7f438cfb3ca5bf698a54491a7`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156da7b644b5b54170a00a318c3f2c9b93383aff76d10e828cbec301ad2aac2e`  
		Last Modified: Tue, 09 Feb 2021 06:34:18 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
