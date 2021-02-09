## `spiped:latest`

```console
$ docker pull spiped@sha256:fd515ccae2a03ed9e83c9f92ceb1437100ed687359fd08c1b3952a2ce225e5de
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
$ docker pull spiped@sha256:5bd55a1a73670e68370f209d9dd01c217eb5b6c67598f25bac68f60e27549889
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32173489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:811e01c7a839fa25b3fa40b7bffd77378fd7aba6ca8bf106e7f581006320d266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:42:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 10:43:03 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:43:04 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 10:43:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 10:43:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 10:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 10:44:01 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 10:44:02 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 10:44:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 10:44:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 10:44:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f88dec7258b86e4e8c96100efc159399e0850fae2548f42d46fef4c3ae47f6`  
		Last Modified: Tue, 12 Jan 2021 10:44:33 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92eb800b9e7b936c989b77428553ebd597012e1fd451c62077a5b319c5c5381c`  
		Last Modified: Tue, 12 Jan 2021 10:44:32 GMT  
		Size: 1.8 MB (1839430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192c478305b485d2d6512913428673bf7ccb9da73b48f2fbde43de07bde0b00d`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 5.5 MB (5479951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce1e5fcf0c5c7851002a65cbff0bc261cf64ef0cb1e856adf7f699ba5aa83b8`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a0ef96e7bb574336736be33888eadcff04b2105f2d98247d8083da825c65f`  
		Last Modified: Tue, 12 Jan 2021 10:44:31 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:969538e0bd3f0f122782eb6c61db00162aff06e57f195fb7ace7ae809105ac13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33780003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12318f64d90b9d0808ffaa7b23d758bc88b955d911c00951492f829cdd34c72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 15:42:12 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 15:42:20 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 15:42:21 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 15:42:21 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 15:42:22 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 15:43:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 15:43:10 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 15:43:10 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 15:43:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 15:43:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 15:43:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0eb9193d09b9481c9b7e8fb170147ce6e276d8856a469a550dec5cc90f7a03`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2415476e63e7d74ef4ca52faea84bfe67a05fe3a41a47e686bdd2cf3b02f85e`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 2.0 MB (2007856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f5953f7f6533ef92426e5d329b897f1907b7330ff21c1e496fbb13c1b26665`  
		Last Modified: Tue, 12 Jan 2021 15:43:54 GMT  
		Size: 5.9 MB (5905445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2b2ae8ded9d7b7e98010d34f8ee794a0a263558bf21efe4b7d11635912c0d9`  
		Last Modified: Tue, 12 Jan 2021 15:43:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadf145025c1ea60655010dbbec8968401844445366f2b5d747e43c7c5c9d4a`  
		Last Modified: Tue, 12 Jan 2021 15:43:46 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:c52d50d68d3bf72bbc961fae84e92d8cdaa061fc499248160b21f00f75c92e57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41535877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb514975d8dd949f947658497f4cd64bd2d5e5290b67e7536c61242ab41e2160`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:35:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 03:35:59 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:35:59 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 03:36:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 03:36:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 03:36:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 03:36:31 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 03:36:31 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 03:36:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 03:36:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 03:36:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae7ed45a540b81c1438ebda1856d950d9f22d471261017cee150ae44932e51`  
		Last Modified: Tue, 12 Jan 2021 03:36:55 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5731e457264a48ebae724947ba8a4074df0cf2c7bb83f2a09bb2719add7a6de5`  
		Last Modified: Tue, 12 Jan 2021 03:36:56 GMT  
		Size: 2.1 MB (2132528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c7122a22a25bc5e765da780d4cb941efbcf58e2ff86d8fa040f99a07ac1e2e`  
		Last Modified: Tue, 12 Jan 2021 03:37:00 GMT  
		Size: 11.6 MB (11633191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388a70059ec0f0ead585cc8fda996f88c967af935dc16e884f488f2419810615`  
		Last Modified: Tue, 12 Jan 2021 03:36:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7120861ce4e70688817e734037c5d8ac88a9d1dd0285babe73f1950c6ece48`  
		Last Modified: Tue, 12 Jan 2021 03:36:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:2c5c7421c8ddb9e24d202b0b0f77f7354cca4312bb92fd52b19e3e3d1deb1455
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33909503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:130497a6932d05f130672da9e0c0c050ccdeed9288a72445f94bb50297b51440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:21 GMT
ADD file:e75a4429a4b3b0f7a646f85af88d412a98006cdf44ea6744b90fea7419840831 in / 
# Tue, 12 Jan 2021 01:16:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:09:54 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jan 2021 16:10:06 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:10:06 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 12 Jan 2021 16:10:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 12 Jan 2021 16:10:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Jan 2021 16:11:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jan 2021 16:11:15 GMT
VOLUME [/spiped]
# Tue, 12 Jan 2021 16:11:16 GMT
WORKDIR /spiped
# Tue, 12 Jan 2021 16:11:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jan 2021 16:11:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 16:11:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c8d46df0b1a64c5ee6879aa09ea5818b36bcae5d39b941d7262bcff617be9873`  
		Last Modified: Tue, 12 Jan 2021 01:23:17 GMT  
		Size: 25.8 MB (25778695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa189ea5f1588e15d59aea364d7de5cf737660a7be5b43b7838447509c32fcf5`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8d546d9d0c67dd04e87cf92d1a953c59c48c19c4db573963fe4364487cc71f`  
		Last Modified: Tue, 12 Jan 2021 16:11:45 GMT  
		Size: 1.7 MB (1712346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340c9dd0d095f9bbe833a6c77c9e39053c0f4e19ce8c5d830747f9e30eac6525`  
		Last Modified: Tue, 12 Jan 2021 16:11:50 GMT  
		Size: 6.4 MB (6416289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bd43028d62609898d5fb217183fa9057c98781503e5330eadb3ad69932e4c`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad75ef390a2ace5a55e7f62becd07b6ca302b837691052bef8a2cd259b290d1`  
		Last Modified: Tue, 12 Jan 2021 16:11:44 GMT  
		Size: 342.0 B  
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
