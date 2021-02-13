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
$ docker pull spiped@sha256:ba3e862e3aa6cd7acfdf6b4f6925e3f9a2a412f3c99150814e934c820aa53805
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
$ docker pull spiped@sha256:de2d45b0f59312e4abff77a82b78eaac004c3224734eedbc7334680c7ec5443f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36262768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897fcb40d5e49b8a35aa9e61c14eff1f62c615775ab19bff009fbbeafff2b106`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:21:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 00:09:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 00:09:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:09:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 00:09:59 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:10:00 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:10:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:10:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:10:02 GMT
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
	-	`sha256:04d13c52f8d2f79744057e6229950b1dfc5bd6291a85638e41c94d0bf6ae4e29`  
		Last Modified: Sat, 13 Feb 2021 00:11:29 GMT  
		Size: 2.1 MB (2128155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce83854aeaf080766f7945048114fa3e9b3416b345ca8aff96978c9c7f54953`  
		Last Modified: Sat, 13 Feb 2021 00:11:31 GMT  
		Size: 7.0 MB (7037301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb829d6ea4836c4cb76df6e6b6006024c209af26a1c18390c00a81ae68243bb`  
		Last Modified: Sat, 13 Feb 2021 00:11:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98a7fedb7f92d778864b0fcf2422f4ef009b2ab40c930b69020c825e6dec72c`  
		Last Modified: Sat, 13 Feb 2021 00:11:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:5fdf9146d8023cd6e901dbceff493b9883020acd456eb8bfbd5c480fcd681210
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32160479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781b7c6ba805844ffb5302f90107b4f5d7cc5f1fd80060ce54ea64fbad5616c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:50:10 GMT
ADD file:fbd00ef7871dc27d7ed5fa8c238cdc80652bd87b8033be7de9e54a799bbf10a4 in / 
# Tue, 09 Feb 2021 02:50:11 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:43:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 22:52:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 22:52:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:53:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 22:53:05 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:53:06 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:53:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:53:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:53:09 GMT
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
	-	`sha256:4b20e94947775259ce6bf04cfa19152b029d3365a89d4ccc0843ae79aa8bd4f2`  
		Last Modified: Fri, 12 Feb 2021 22:53:24 GMT  
		Size: 1.8 MB (1839109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5daf79a4e2ff35a482480dc5ed9294bc9b4a8973856555b77b39e3db207b7e`  
		Last Modified: Fri, 12 Feb 2021 22:53:26 GMT  
		Size: 5.5 MB (5479875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384e633e1a26bfac8686c377988482dd352c68b9f02ba80edcda2501879211a1`  
		Last Modified: Fri, 12 Feb 2021 22:53:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3d0ff8a742e94655d7e9b5e7444b78818640156c0ca4672cfa957a605307f`  
		Last Modified: Fri, 12 Feb 2021 22:53:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3f1874e1134dbfca6d910ae69ff8d37e2a72d12404d8a9fd0fe0bd0c91e6db78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29750488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c287c25628c3da85c966ccc96d6e3e6e7a542d2487caaa805d5fa8a0525ea5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:57 GMT
ADD file:e675d50366bde57173a75f9a29367d765e7da2b7254c5254b64e777cf6870502 in / 
# Tue, 09 Feb 2021 03:01:00 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 19:35:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 22:38:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 22:38:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:39:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 22:39:30 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:39:30 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:39:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:db574d82360c3b60abadbef4f3daf8dee01f24741fc6ab3692aa543558d8b624`  
		Last Modified: Tue, 09 Feb 2021 03:09:46 GMT  
		Size: 22.7 MB (22703384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afe0266f6b6542f91658ca8ec8b87ac3e40c9e40d88f3ebfb311da27ffaa976`  
		Last Modified: Tue, 09 Feb 2021 19:37:10 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a439028cc7f7cbb2502897e215fe8142424bac7b8461519a3721306ca16262`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 1.8 MB (1759313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175e160ff82eee0dc76239d6e920ad6fce1b07298b3bd90e8120c021b7af0dd`  
		Last Modified: Fri, 12 Feb 2021 22:40:40 GMT  
		Size: 5.3 MB (5285596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c31222b7eba85c87a5dbbee1012985dae7f842a0c60e03cc2641b409aa474`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88900a0b87f635433ee9e3c471b1a10b21ea199374733be54fb2595691999e2`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:aeb7d15ee44fc1b03bfd46be858735700424119244cb66f38e14e9630c63e7ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33766524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61e1f2dc0e564ffcc34b5a7d98c4213648ab3f8a22f84e0db2b43178567f3a12`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:18:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 01:48:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 01:48:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 01:48:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 01:48:57 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 01:48:58 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 01:48:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 01:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 01:49:01 GMT
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
	-	`sha256:03005b703ccb19a3569b35a5b9bf1bfef156941eaf489b91ff81efde2e7ea584`  
		Last Modified: Sat, 13 Feb 2021 01:50:07 GMT  
		Size: 2.0 MB (2007571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c581bbabc2c122ca024c49c3aa7d735e4cfba75a1560c8c873223c66d0c57e6a`  
		Last Modified: Sat, 13 Feb 2021 01:50:08 GMT  
		Size: 5.9 MB (5905293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c709ad2716ce7723cf89c0c553985816902e98c25f46520d8faa51d120c7508f`  
		Last Modified: Sat, 13 Feb 2021 01:50:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe585f4a68228bec2b5b6765c7a8a860d41e59a842e3b43871e7120172ab40c7`  
		Last Modified: Sat, 13 Feb 2021 01:50:06 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:4f80cd66b8eb83d68da1b3cd894fe37462760fe5278f6973301e26f1af90bc91
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41520139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e96e1652c7ef7e3d880320ae65765f36dfe4d599e1ca9ac8c0154dcf0e54633a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:39:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 00:58:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 00:58:43 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:59:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 00:59:17 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:59:17 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:59:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:59:18 GMT
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
	-	`sha256:a4b87a23d1edb8994421e0ef8e6ae3e7a6364755d7e174130d7b4076dfa2119e`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 2.1 MB (2132258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7cffa8181e625c430a03c89cc64ae89e03825bd80c01986ce5486ad61b4c12`  
		Last Modified: Sat, 13 Feb 2021 01:00:11 GMT  
		Size: 11.6 MB (11632985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15dfc8a7a89424ce7b74424465fcef8b14d61f39590f94169b3a7afd30130b0`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3837cf2d6a87c1b6e64337cafb4ddb0959d201146a766002cc849caa670bae`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:25a5e4c9bfecee13942120bcc34a2cdb13e00addd065a17df1302153ead12de4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33895238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:818a59f972b27eb92864d12c7304285f5966446e58096f31ad3b67a0bc8d07d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 03:09:26 GMT
ADD file:0222a151f4e5033d9eae98ce2b703a63f52d049dd72ac40bdd0dc2dafe619f0a in / 
# Tue, 09 Feb 2021 03:09:27 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:51:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 23:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 23:11:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 23:12:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 23:12:11 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 23:12:12 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 23:12:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 23:12:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 23:12:13 GMT
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
	-	`sha256:5463eef3d8ce71368876b45ca24071008cc083ea16ea90ad16da78aee1b06eb0`  
		Last Modified: Fri, 12 Feb 2021 23:12:26 GMT  
		Size: 1.7 MB (1712078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c83f952ec2caa0e8a9319f93360620700120836fe9678c29036c7cf9868e9`  
		Last Modified: Fri, 12 Feb 2021 23:12:31 GMT  
		Size: 6.4 MB (6416347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b88510861e3f585271a563d2bee51e8dc1659e7abc654317636fd8a6e35956`  
		Last Modified: Fri, 12 Feb 2021 23:12:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8a904b2624ec463e93f83225ac51eebd738a0473f323cf0121dcf664488951`  
		Last Modified: Fri, 12 Feb 2021 23:12:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:864f9629da12aace742df3cd8167639ca43ff06a00763b99c31dcba10699a00e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39490261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749c18efc7646905a7417cb2107c88294bb750ed6bc8039f46b4311923b6e779`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:15:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 02:30:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 02:30:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 02:33:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 02:34:02 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 02:34:09 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 02:34:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 02:34:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 02:34:18 GMT
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
	-	`sha256:47130d66484e5dc6224d68f7eaf7129048723a038246f1ba3288bc669594ce4d`  
		Last Modified: Sat, 13 Feb 2021 02:36:06 GMT  
		Size: 2.2 MB (2224915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7be408970c00a6f67d09788fe2ae7d9bee14d0ddedf38e826cbedc4e12d6e`  
		Last Modified: Sat, 13 Feb 2021 02:36:07 GMT  
		Size: 6.7 MB (6743622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed58efc2e2df4e58c29b6b3946f036cdf35e85ba6b21cf906c7fe425b1efc82a`  
		Last Modified: Sat, 13 Feb 2021 02:36:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5da930633055937f1ba62f43cf83b555b527d1cd8255d66ac9d6281f3afa41d`  
		Last Modified: Sat, 13 Feb 2021 02:36:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

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

## `spiped:1.6`

```console
$ docker pull spiped@sha256:4e0757d83a01c2abc624d004ea3feb13bbd81c33ff0294e91744575688e0e92c
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
$ docker pull spiped@sha256:de2d45b0f59312e4abff77a82b78eaac004c3224734eedbc7334680c7ec5443f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36262768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897fcb40d5e49b8a35aa9e61c14eff1f62c615775ab19bff009fbbeafff2b106`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:21:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 00:09:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 00:09:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:09:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 00:09:59 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:10:00 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:10:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:10:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:10:02 GMT
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
	-	`sha256:04d13c52f8d2f79744057e6229950b1dfc5bd6291a85638e41c94d0bf6ae4e29`  
		Last Modified: Sat, 13 Feb 2021 00:11:29 GMT  
		Size: 2.1 MB (2128155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce83854aeaf080766f7945048114fa3e9b3416b345ca8aff96978c9c7f54953`  
		Last Modified: Sat, 13 Feb 2021 00:11:31 GMT  
		Size: 7.0 MB (7037301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb829d6ea4836c4cb76df6e6b6006024c209af26a1c18390c00a81ae68243bb`  
		Last Modified: Sat, 13 Feb 2021 00:11:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98a7fedb7f92d778864b0fcf2422f4ef009b2ab40c930b69020c825e6dec72c`  
		Last Modified: Sat, 13 Feb 2021 00:11:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:5fdf9146d8023cd6e901dbceff493b9883020acd456eb8bfbd5c480fcd681210
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32160479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781b7c6ba805844ffb5302f90107b4f5d7cc5f1fd80060ce54ea64fbad5616c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:50:10 GMT
ADD file:fbd00ef7871dc27d7ed5fa8c238cdc80652bd87b8033be7de9e54a799bbf10a4 in / 
# Tue, 09 Feb 2021 02:50:11 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:43:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 22:52:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 22:52:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:53:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 22:53:05 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:53:06 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:53:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:53:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:53:09 GMT
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
	-	`sha256:4b20e94947775259ce6bf04cfa19152b029d3365a89d4ccc0843ae79aa8bd4f2`  
		Last Modified: Fri, 12 Feb 2021 22:53:24 GMT  
		Size: 1.8 MB (1839109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5daf79a4e2ff35a482480dc5ed9294bc9b4a8973856555b77b39e3db207b7e`  
		Last Modified: Fri, 12 Feb 2021 22:53:26 GMT  
		Size: 5.5 MB (5479875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384e633e1a26bfac8686c377988482dd352c68b9f02ba80edcda2501879211a1`  
		Last Modified: Fri, 12 Feb 2021 22:53:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3d0ff8a742e94655d7e9b5e7444b78818640156c0ca4672cfa957a605307f`  
		Last Modified: Fri, 12 Feb 2021 22:53:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3f1874e1134dbfca6d910ae69ff8d37e2a72d12404d8a9fd0fe0bd0c91e6db78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29750488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c287c25628c3da85c966ccc96d6e3e6e7a542d2487caaa805d5fa8a0525ea5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:57 GMT
ADD file:e675d50366bde57173a75f9a29367d765e7da2b7254c5254b64e777cf6870502 in / 
# Tue, 09 Feb 2021 03:01:00 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 19:35:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 22:38:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 22:38:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:39:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 22:39:30 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:39:30 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:39:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:db574d82360c3b60abadbef4f3daf8dee01f24741fc6ab3692aa543558d8b624`  
		Last Modified: Tue, 09 Feb 2021 03:09:46 GMT  
		Size: 22.7 MB (22703384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afe0266f6b6542f91658ca8ec8b87ac3e40c9e40d88f3ebfb311da27ffaa976`  
		Last Modified: Tue, 09 Feb 2021 19:37:10 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a439028cc7f7cbb2502897e215fe8142424bac7b8461519a3721306ca16262`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 1.8 MB (1759313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175e160ff82eee0dc76239d6e920ad6fce1b07298b3bd90e8120c021b7af0dd`  
		Last Modified: Fri, 12 Feb 2021 22:40:40 GMT  
		Size: 5.3 MB (5285596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c31222b7eba85c87a5dbbee1012985dae7f842a0c60e03cc2641b409aa474`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88900a0b87f635433ee9e3c471b1a10b21ea199374733be54fb2595691999e2`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:aeb7d15ee44fc1b03bfd46be858735700424119244cb66f38e14e9630c63e7ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33766524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61e1f2dc0e564ffcc34b5a7d98c4213648ab3f8a22f84e0db2b43178567f3a12`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:18:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 01:48:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 01:48:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 01:48:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 01:48:57 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 01:48:58 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 01:48:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 01:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 01:49:01 GMT
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
	-	`sha256:03005b703ccb19a3569b35a5b9bf1bfef156941eaf489b91ff81efde2e7ea584`  
		Last Modified: Sat, 13 Feb 2021 01:50:07 GMT  
		Size: 2.0 MB (2007571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c581bbabc2c122ca024c49c3aa7d735e4cfba75a1560c8c873223c66d0c57e6a`  
		Last Modified: Sat, 13 Feb 2021 01:50:08 GMT  
		Size: 5.9 MB (5905293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c709ad2716ce7723cf89c0c553985816902e98c25f46520d8faa51d120c7508f`  
		Last Modified: Sat, 13 Feb 2021 01:50:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe585f4a68228bec2b5b6765c7a8a860d41e59a842e3b43871e7120172ab40c7`  
		Last Modified: Sat, 13 Feb 2021 01:50:06 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:4f80cd66b8eb83d68da1b3cd894fe37462760fe5278f6973301e26f1af90bc91
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41520139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e96e1652c7ef7e3d880320ae65765f36dfe4d599e1ca9ac8c0154dcf0e54633a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:39:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 00:58:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 00:58:43 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:59:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 00:59:17 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:59:17 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:59:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:59:18 GMT
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
	-	`sha256:a4b87a23d1edb8994421e0ef8e6ae3e7a6364755d7e174130d7b4076dfa2119e`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 2.1 MB (2132258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7cffa8181e625c430a03c89cc64ae89e03825bd80c01986ce5486ad61b4c12`  
		Last Modified: Sat, 13 Feb 2021 01:00:11 GMT  
		Size: 11.6 MB (11632985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15dfc8a7a89424ce7b74424465fcef8b14d61f39590f94169b3a7afd30130b0`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3837cf2d6a87c1b6e64337cafb4ddb0959d201146a766002cc849caa670bae`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:25a5e4c9bfecee13942120bcc34a2cdb13e00addd065a17df1302153ead12de4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33895238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:818a59f972b27eb92864d12c7304285f5966446e58096f31ad3b67a0bc8d07d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 03:09:26 GMT
ADD file:0222a151f4e5033d9eae98ce2b703a63f52d049dd72ac40bdd0dc2dafe619f0a in / 
# Tue, 09 Feb 2021 03:09:27 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:51:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 23:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 23:11:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 23:12:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 23:12:11 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 23:12:12 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 23:12:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 23:12:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 23:12:13 GMT
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
	-	`sha256:5463eef3d8ce71368876b45ca24071008cc083ea16ea90ad16da78aee1b06eb0`  
		Last Modified: Fri, 12 Feb 2021 23:12:26 GMT  
		Size: 1.7 MB (1712078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c83f952ec2caa0e8a9319f93360620700120836fe9678c29036c7cf9868e9`  
		Last Modified: Fri, 12 Feb 2021 23:12:31 GMT  
		Size: 6.4 MB (6416347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b88510861e3f585271a563d2bee51e8dc1659e7abc654317636fd8a6e35956`  
		Last Modified: Fri, 12 Feb 2021 23:12:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8a904b2624ec463e93f83225ac51eebd738a0473f323cf0121dcf664488951`  
		Last Modified: Fri, 12 Feb 2021 23:12:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:864f9629da12aace742df3cd8167639ca43ff06a00763b99c31dcba10699a00e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39490261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749c18efc7646905a7417cb2107c88294bb750ed6bc8039f46b4311923b6e779`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:15:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 02:30:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 02:30:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 02:33:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 02:34:02 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 02:34:09 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 02:34:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 02:34:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 02:34:18 GMT
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
	-	`sha256:47130d66484e5dc6224d68f7eaf7129048723a038246f1ba3288bc669594ce4d`  
		Last Modified: Sat, 13 Feb 2021 02:36:06 GMT  
		Size: 2.2 MB (2224915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7be408970c00a6f67d09788fe2ae7d9bee14d0ddedf38e826cbedc4e12d6e`  
		Last Modified: Sat, 13 Feb 2021 02:36:07 GMT  
		Size: 6.7 MB (6743622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed58efc2e2df4e58c29b6b3946f036cdf35e85ba6b21cf906c7fe425b1efc82a`  
		Last Modified: Sat, 13 Feb 2021 02:36:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5da930633055937f1ba62f43cf83b555b527d1cd8255d66ac9d6281f3afa41d`  
		Last Modified: Sat, 13 Feb 2021 02:36:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:f1fc57dae92710b70032be2526f79e54964e55f92c1743f69ec7cf0a676d8116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33477416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dda528269da27ad9d1592ca7bc595ecbacc814c873d1441327b98560f8a43b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:10 GMT
ADD file:0edb2de05df54191a141bd125f59d7e14eef0cc4576927a247b8dd7d6f255d04 in / 
# Tue, 09 Feb 2021 02:42:12 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:33:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 03:10:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 03:10:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 03:11:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 03:11:22 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 03:11:22 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 03:11:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 03:11:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 03:11:23 GMT
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
	-	`sha256:916e90eba0ded4a99e0c1e86e0657b977665bf19661f2c18005fc6d6745d7fd4`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 1.8 MB (1821717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9478c638398830f42321041df73fb7c8005dd7c336c933045b5f043fe1e8786`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 5.9 MB (5943471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fb1c3cf1445657cf0a44894ccf3da2d62b39264d89fcbecc0e2db075fcfdcf`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f2ae3abab433a32b5e6ba282e6544117d7a01f4fd183d4a7582a4c5a64479f`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:4e0757d83a01c2abc624d004ea3feb13bbd81c33ff0294e91744575688e0e92c
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
$ docker pull spiped@sha256:de2d45b0f59312e4abff77a82b78eaac004c3224734eedbc7334680c7ec5443f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36262768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897fcb40d5e49b8a35aa9e61c14eff1f62c615775ab19bff009fbbeafff2b106`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:21:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 00:09:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 00:09:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:09:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 00:09:59 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:10:00 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:10:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:10:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:10:02 GMT
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
	-	`sha256:04d13c52f8d2f79744057e6229950b1dfc5bd6291a85638e41c94d0bf6ae4e29`  
		Last Modified: Sat, 13 Feb 2021 00:11:29 GMT  
		Size: 2.1 MB (2128155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce83854aeaf080766f7945048114fa3e9b3416b345ca8aff96978c9c7f54953`  
		Last Modified: Sat, 13 Feb 2021 00:11:31 GMT  
		Size: 7.0 MB (7037301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb829d6ea4836c4cb76df6e6b6006024c209af26a1c18390c00a81ae68243bb`  
		Last Modified: Sat, 13 Feb 2021 00:11:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98a7fedb7f92d778864b0fcf2422f4ef009b2ab40c930b69020c825e6dec72c`  
		Last Modified: Sat, 13 Feb 2021 00:11:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:5fdf9146d8023cd6e901dbceff493b9883020acd456eb8bfbd5c480fcd681210
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32160479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781b7c6ba805844ffb5302f90107b4f5d7cc5f1fd80060ce54ea64fbad5616c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:50:10 GMT
ADD file:fbd00ef7871dc27d7ed5fa8c238cdc80652bd87b8033be7de9e54a799bbf10a4 in / 
# Tue, 09 Feb 2021 02:50:11 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:43:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 22:52:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 22:52:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:53:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 22:53:05 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:53:06 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:53:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:53:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:53:09 GMT
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
	-	`sha256:4b20e94947775259ce6bf04cfa19152b029d3365a89d4ccc0843ae79aa8bd4f2`  
		Last Modified: Fri, 12 Feb 2021 22:53:24 GMT  
		Size: 1.8 MB (1839109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5daf79a4e2ff35a482480dc5ed9294bc9b4a8973856555b77b39e3db207b7e`  
		Last Modified: Fri, 12 Feb 2021 22:53:26 GMT  
		Size: 5.5 MB (5479875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384e633e1a26bfac8686c377988482dd352c68b9f02ba80edcda2501879211a1`  
		Last Modified: Fri, 12 Feb 2021 22:53:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3d0ff8a742e94655d7e9b5e7444b78818640156c0ca4672cfa957a605307f`  
		Last Modified: Fri, 12 Feb 2021 22:53:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3f1874e1134dbfca6d910ae69ff8d37e2a72d12404d8a9fd0fe0bd0c91e6db78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29750488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c287c25628c3da85c966ccc96d6e3e6e7a542d2487caaa805d5fa8a0525ea5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:57 GMT
ADD file:e675d50366bde57173a75f9a29367d765e7da2b7254c5254b64e777cf6870502 in / 
# Tue, 09 Feb 2021 03:01:00 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 19:35:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 22:38:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 22:38:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:39:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 22:39:30 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:39:30 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:39:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:db574d82360c3b60abadbef4f3daf8dee01f24741fc6ab3692aa543558d8b624`  
		Last Modified: Tue, 09 Feb 2021 03:09:46 GMT  
		Size: 22.7 MB (22703384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afe0266f6b6542f91658ca8ec8b87ac3e40c9e40d88f3ebfb311da27ffaa976`  
		Last Modified: Tue, 09 Feb 2021 19:37:10 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a439028cc7f7cbb2502897e215fe8142424bac7b8461519a3721306ca16262`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 1.8 MB (1759313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175e160ff82eee0dc76239d6e920ad6fce1b07298b3bd90e8120c021b7af0dd`  
		Last Modified: Fri, 12 Feb 2021 22:40:40 GMT  
		Size: 5.3 MB (5285596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c31222b7eba85c87a5dbbee1012985dae7f842a0c60e03cc2641b409aa474`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88900a0b87f635433ee9e3c471b1a10b21ea199374733be54fb2595691999e2`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:aeb7d15ee44fc1b03bfd46be858735700424119244cb66f38e14e9630c63e7ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33766524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61e1f2dc0e564ffcc34b5a7d98c4213648ab3f8a22f84e0db2b43178567f3a12`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:18:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 01:48:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 01:48:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 01:48:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 01:48:57 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 01:48:58 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 01:48:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 01:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 01:49:01 GMT
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
	-	`sha256:03005b703ccb19a3569b35a5b9bf1bfef156941eaf489b91ff81efde2e7ea584`  
		Last Modified: Sat, 13 Feb 2021 01:50:07 GMT  
		Size: 2.0 MB (2007571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c581bbabc2c122ca024c49c3aa7d735e4cfba75a1560c8c873223c66d0c57e6a`  
		Last Modified: Sat, 13 Feb 2021 01:50:08 GMT  
		Size: 5.9 MB (5905293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c709ad2716ce7723cf89c0c553985816902e98c25f46520d8faa51d120c7508f`  
		Last Modified: Sat, 13 Feb 2021 01:50:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe585f4a68228bec2b5b6765c7a8a860d41e59a842e3b43871e7120172ab40c7`  
		Last Modified: Sat, 13 Feb 2021 01:50:06 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:4f80cd66b8eb83d68da1b3cd894fe37462760fe5278f6973301e26f1af90bc91
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41520139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e96e1652c7ef7e3d880320ae65765f36dfe4d599e1ca9ac8c0154dcf0e54633a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:39:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 00:58:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 00:58:43 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:59:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 00:59:17 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:59:17 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:59:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:59:18 GMT
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
	-	`sha256:a4b87a23d1edb8994421e0ef8e6ae3e7a6364755d7e174130d7b4076dfa2119e`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 2.1 MB (2132258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7cffa8181e625c430a03c89cc64ae89e03825bd80c01986ce5486ad61b4c12`  
		Last Modified: Sat, 13 Feb 2021 01:00:11 GMT  
		Size: 11.6 MB (11632985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15dfc8a7a89424ce7b74424465fcef8b14d61f39590f94169b3a7afd30130b0`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3837cf2d6a87c1b6e64337cafb4ddb0959d201146a766002cc849caa670bae`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:25a5e4c9bfecee13942120bcc34a2cdb13e00addd065a17df1302153ead12de4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33895238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:818a59f972b27eb92864d12c7304285f5966446e58096f31ad3b67a0bc8d07d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 03:09:26 GMT
ADD file:0222a151f4e5033d9eae98ce2b703a63f52d049dd72ac40bdd0dc2dafe619f0a in / 
# Tue, 09 Feb 2021 03:09:27 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:51:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 23:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 23:11:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 23:12:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 23:12:11 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 23:12:12 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 23:12:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 23:12:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 23:12:13 GMT
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
	-	`sha256:5463eef3d8ce71368876b45ca24071008cc083ea16ea90ad16da78aee1b06eb0`  
		Last Modified: Fri, 12 Feb 2021 23:12:26 GMT  
		Size: 1.7 MB (1712078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c83f952ec2caa0e8a9319f93360620700120836fe9678c29036c7cf9868e9`  
		Last Modified: Fri, 12 Feb 2021 23:12:31 GMT  
		Size: 6.4 MB (6416347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b88510861e3f585271a563d2bee51e8dc1659e7abc654317636fd8a6e35956`  
		Last Modified: Fri, 12 Feb 2021 23:12:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8a904b2624ec463e93f83225ac51eebd738a0473f323cf0121dcf664488951`  
		Last Modified: Fri, 12 Feb 2021 23:12:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:864f9629da12aace742df3cd8167639ca43ff06a00763b99c31dcba10699a00e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39490261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749c18efc7646905a7417cb2107c88294bb750ed6bc8039f46b4311923b6e779`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:15:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 02:30:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 02:30:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 02:33:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 02:34:02 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 02:34:09 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 02:34:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 02:34:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 02:34:18 GMT
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
	-	`sha256:47130d66484e5dc6224d68f7eaf7129048723a038246f1ba3288bc669594ce4d`  
		Last Modified: Sat, 13 Feb 2021 02:36:06 GMT  
		Size: 2.2 MB (2224915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7be408970c00a6f67d09788fe2ae7d9bee14d0ddedf38e826cbedc4e12d6e`  
		Last Modified: Sat, 13 Feb 2021 02:36:07 GMT  
		Size: 6.7 MB (6743622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed58efc2e2df4e58c29b6b3946f036cdf35e85ba6b21cf906c7fe425b1efc82a`  
		Last Modified: Sat, 13 Feb 2021 02:36:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5da930633055937f1ba62f43cf83b555b527d1cd8255d66ac9d6281f3afa41d`  
		Last Modified: Sat, 13 Feb 2021 02:36:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:f1fc57dae92710b70032be2526f79e54964e55f92c1743f69ec7cf0a676d8116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33477416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dda528269da27ad9d1592ca7bc595ecbacc814c873d1441327b98560f8a43b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:10 GMT
ADD file:0edb2de05df54191a141bd125f59d7e14eef0cc4576927a247b8dd7d6f255d04 in / 
# Tue, 09 Feb 2021 02:42:12 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:33:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 03:10:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 03:10:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 03:11:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 03:11:22 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 03:11:22 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 03:11:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 03:11:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 03:11:23 GMT
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
	-	`sha256:916e90eba0ded4a99e0c1e86e0657b977665bf19661f2c18005fc6d6745d7fd4`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 1.8 MB (1821717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9478c638398830f42321041df73fb7c8005dd7c336c933045b5f043fe1e8786`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 5.9 MB (5943471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fb1c3cf1445657cf0a44894ccf3da2d62b39264d89fcbecc0e2db075fcfdcf`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f2ae3abab433a32b5e6ba282e6544117d7a01f4fd183d4a7582a4c5a64479f`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:d151d981ca0ebab580c3ff2c4360baa2e99aca02d7c13f9a4e9fcd89425eb2f0
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
$ docker pull spiped@sha256:835d7b06f38b14f3497dfa8ef3a3387976759c1d4da641bee7b66ab2614327e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883c5cce06c38a0f7a19e769ba33df23b5104eae4f2f2529c4b6c7d2540dd71a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 00:10:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 00:10:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 00:10:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:11:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 00:11:03 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:11:03 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:11:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:11:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:11:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ada2cbdd62e07ee40d2f05c48cbb06a172e5cde247cb27defa9146e342ee24`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0809851ee6dd7d72995918c73439754a4ff183f0aa0f142407150e9c75130e`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 7.0 KB (7049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814bb6e0e86dd762b94f3a86fe4ea3dcac961064cb970ae9852a2389eab5bc72`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 212.3 KB (212296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a22052f5d37047c574696d71e90ee4fc969f40189329fc130b69fd39cd39ab`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db107fe5f9add27475633bd978bdbc7404ae29a7f594d3a2e5aaff7ac44b63db`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c27babd1d2aafca8bda58fedee7d3038c7b20fbf7b5e1eb870270268eed209c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2832841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d677780adfebbeebb133e4df636a0d26d64e0813b9fd46fedf2f1d9db0a3783d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:49:59 GMT
ADD file:c197324e4979e2a7b257ad683d20dd9cbdae525a076bd68fe6aa0e0b126875df in / 
# Thu, 28 Jan 2021 23:49:59 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 23:07:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Feb 2021 23:07:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Feb 2021 23:07:57 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 23:08:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Feb 2021 23:08:24 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 23:08:25 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 23:08:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 23:08:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 23:08:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a66f440da051140fefcb0a520bdeb69d763b1eb4fd1b2ed46b4c0a168e335108`  
		Last Modified: Thu, 28 Jan 2021 23:50:33 GMT  
		Size: 2.6 MB (2621759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef16c09cad69b4f5ffbad02c5d05e54a8776d0f589b5070292f555188352fc2`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd09edfda78fafd09511434ad81f68f3aaa910006a0cf43dbd8c9aeea23e2fa`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b616073d9c59a7d6763e8532e2e8bd4c592396a4250e30e030e29ef220db07`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 202.3 KB (202293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcdea289e6dfa0b452fe3805b1859196021df0753f5954e2728ee1947cf9828`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa80572babecc8c62f006bbc854c927644a0939f8982217861c889a29c084e7`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ae4d066b309a39b651ddcafcf7e0b5544d6698a4cfc4a7eb1c4e493356befb0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2627898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79097e2ce8ba1eaa302fbfdff3d7cd160ef52f71c4e89a7e4d3c097be5fa9c82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:58:03 GMT
ADD file:98a89b90a8b442eed5301790dd2bd3a27391c5e4426126eed9d1cf44e70f8857 in / 
# Thu, 28 Jan 2021 23:58:04 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 22:39:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Feb 2021 22:39:48 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Feb 2021 22:39:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:40:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Feb 2021 22:40:17 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:40:17 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:40:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:40:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:40:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b1db703a337d301b1d50292acfbabd5fb3796511b962410c554420b85cd78dc`  
		Last Modified: Thu, 28 Jan 2021 23:58:38 GMT  
		Size: 2.4 MB (2423559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516139fc4bc5d3abbe484f41d65d96291d928c8313850bcfac5c409d91294e8e`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55705b9c11a25d31d806dae7cc70ba9979dbe2d872e5a1fa9675221a82cea552`  
		Last Modified: Fri, 12 Feb 2021 22:40:50 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19434ef650615c9f560946ec913d75335ea2c4da848dbe31002ba504051fe66`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 195.5 KB (195547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab2b83ef52894e4d6228617de9f67c33d742d2f237ee7fdfc38aeec8bf87f9a`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11720b6738d8b9681acab3a3423ae35fd9b3144467c23cb413deadffcfda6fd6`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:217ad97919e9aff3523891ff4cc50a783dd09a49976ae1f43a2cf615bd3167f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d125f8b9e25718ed14e33e37580e480d52edcf753f1cf917b1c4dd0ea4b9f358`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 01:49:09 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 01:49:12 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 01:49:12 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 01:49:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 01:49:42 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 01:49:43 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 01:49:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 01:49:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 01:49:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b73d7b095df7558c4913a1b56bc566a203d1705bceaf849063716da396aa3d`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a11963159741a5e3e3effd779670b8e3d7d46c46802b674c8c948528833d118`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 7.1 KB (7061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984eda174ae2399fbfdebdc2ed85bb966ca11956df853e13be5060029f19f345`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 204.4 KB (204443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d588ba06f796ba5588dbba0b0cacec4a16b2a60183e3cdffacf7f0d27bf18`  
		Last Modified: Sat, 13 Feb 2021 01:50:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e9caaa63d130b7c7a0ea6bcc1b2f984eae242f1ebea0d8bc7b5e487aea9a88`  
		Last Modified: Sat, 13 Feb 2021 01:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:4960ec29bb9ef335500e75f0083cd0266fe301739478d22c7eac9fd71a2a0ab3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3049596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4479a0b49914c6027a4470086fafeec21241b4ec58e6a9b2c913d6bca2d22ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:38:31 GMT
ADD file:c0e9ea135d66ad6504c77915a7a48b3bead60892d155d3258b746cb4945981c0 in / 
# Thu, 28 Jan 2021 23:38:31 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 00:59:25 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 00:59:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 00:59:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:59:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 00:59:50 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:59:50 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:59:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:59:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3fea00a81341ce917db671eb3ad24ef5750cb6928b7f760e3ce4dab619eeb1fa`  
		Last Modified: Thu, 28 Jan 2021 23:39:02 GMT  
		Size: 2.8 MB (2817627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7723c1203294add77f79b9f3aafc10eda8572905ac503c7f5a0b2d49e488ed`  
		Last Modified: Sat, 13 Feb 2021 01:00:17 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce806478241c0f699afc38824da58e636c67df1e42986b00e0984769077c20`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bd8240d52bc7724188c29d5ef4610ea463be9b970b707886910547d6edbf85`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 223.3 KB (223257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209f92f3e8326cecdb9a9e84435c267898cd9258f7a6ab104632b2653a905c9`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40d0142f6f8ec7c14fc1fbc2ea71a8ccf3e8f67ba870450c9b5601ea7a710ca`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:33c381176119d7660214d2991cb4a2ccfa254db448220f4df615870f3a84fc66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50abb8300ea994b3e481699c0929ed73d9007f8f85432f87cc74afeda4045cf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:55:50 GMT
ADD file:b14fd5f3f7fcd16e2b4ec6932d3e9c07c7400c577cee5fdcb88b0795a70a7bfb in / 
# Thu, 28 Jan 2021 23:55:52 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 02:34:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 02:34:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 02:34:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 02:35:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 02:35:24 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 02:35:28 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 02:35:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 02:35:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 02:35:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b94a1d8d591af02f1b419642bee91066ecbb9c65099d6903deed310fd1c2ff`  
		Last Modified: Thu, 28 Jan 2021 23:56:32 GMT  
		Size: 2.8 MB (2812517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e118e9785a8eefb11035770ba3f016fd6735fff79024dddf90bd04b98150410`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c02326e8246063ab1916219ed81aa1f954ca993bc3590ef06d7b6748d815977`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc9abddce71df5b7d8a16936252ae190e82033deb046797cf5341fff77f026e`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 221.0 KB (220996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d1ec7b1f9be796457a3f27e5d1d7644cac7c122fd210e179931e04dbc0e7ad`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce293f6c247be36cea3048f53a9ad45fe1640112b6b234e232b79e69a9f1efae`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:7b710fbed5a510700538e3437d8b3a418f829953d9b8fec0334ba9799219909c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2815889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fb1ee7014b5ab54030e234cfda6659e5d0d99d1c2033497d7f89f88cf5c2ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:41:35 GMT
ADD file:d97e6c37df0fb8306b072d9c0a32f68f5aff583ba849303926644deacfa25eb9 in / 
# Thu, 28 Jan 2021 23:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 03:11:30 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 03:11:31 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 03:11:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 03:11:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 03:11:42 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 03:11:42 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 03:11:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 03:11:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 03:11:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:43901f1af0ef9db6b0bf30ac6f6dacd78bf1ecfeb47ad0a93aa2370fa8e62407`  
		Last Modified: Thu, 28 Jan 2021 23:42:09 GMT  
		Size: 2.6 MB (2602059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345d8435943aca39411423265dc836788d9ec232e833f7cbc90ab835db3625c1`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b2484becfe02ade48d7c733db97b58e1ce5dfdafe33927ad4a722949f1d565`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 7.1 KB (7061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85179c983a9cffadd2d46f7ecf69991dc589c1dfb0379e6b34d372fb81f127e`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3949274cf2ec2bb3ad5931b5b9a119173d5ace06d37332a4d2c7a7d5f2199f91`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290cac537fab95725326ea6e10e2a1333216daaa916d670eac7fbf7005373593`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:d151d981ca0ebab580c3ff2c4360baa2e99aca02d7c13f9a4e9fcd89425eb2f0
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
$ docker pull spiped@sha256:835d7b06f38b14f3497dfa8ef3a3387976759c1d4da641bee7b66ab2614327e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883c5cce06c38a0f7a19e769ba33df23b5104eae4f2f2529c4b6c7d2540dd71a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 00:10:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 00:10:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 00:10:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:11:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 00:11:03 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:11:03 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:11:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:11:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:11:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ada2cbdd62e07ee40d2f05c48cbb06a172e5cde247cb27defa9146e342ee24`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0809851ee6dd7d72995918c73439754a4ff183f0aa0f142407150e9c75130e`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 7.0 KB (7049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814bb6e0e86dd762b94f3a86fe4ea3dcac961064cb970ae9852a2389eab5bc72`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 212.3 KB (212296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a22052f5d37047c574696d71e90ee4fc969f40189329fc130b69fd39cd39ab`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db107fe5f9add27475633bd978bdbc7404ae29a7f594d3a2e5aaff7ac44b63db`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c27babd1d2aafca8bda58fedee7d3038c7b20fbf7b5e1eb870270268eed209c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2832841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d677780adfebbeebb133e4df636a0d26d64e0813b9fd46fedf2f1d9db0a3783d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:49:59 GMT
ADD file:c197324e4979e2a7b257ad683d20dd9cbdae525a076bd68fe6aa0e0b126875df in / 
# Thu, 28 Jan 2021 23:49:59 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 23:07:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Feb 2021 23:07:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Feb 2021 23:07:57 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 23:08:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Feb 2021 23:08:24 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 23:08:25 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 23:08:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 23:08:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 23:08:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a66f440da051140fefcb0a520bdeb69d763b1eb4fd1b2ed46b4c0a168e335108`  
		Last Modified: Thu, 28 Jan 2021 23:50:33 GMT  
		Size: 2.6 MB (2621759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef16c09cad69b4f5ffbad02c5d05e54a8776d0f589b5070292f555188352fc2`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd09edfda78fafd09511434ad81f68f3aaa910006a0cf43dbd8c9aeea23e2fa`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b616073d9c59a7d6763e8532e2e8bd4c592396a4250e30e030e29ef220db07`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 202.3 KB (202293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcdea289e6dfa0b452fe3805b1859196021df0753f5954e2728ee1947cf9828`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa80572babecc8c62f006bbc854c927644a0939f8982217861c889a29c084e7`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ae4d066b309a39b651ddcafcf7e0b5544d6698a4cfc4a7eb1c4e493356befb0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2627898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79097e2ce8ba1eaa302fbfdff3d7cd160ef52f71c4e89a7e4d3c097be5fa9c82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:58:03 GMT
ADD file:98a89b90a8b442eed5301790dd2bd3a27391c5e4426126eed9d1cf44e70f8857 in / 
# Thu, 28 Jan 2021 23:58:04 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 22:39:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Feb 2021 22:39:48 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Feb 2021 22:39:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:40:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Feb 2021 22:40:17 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:40:17 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:40:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:40:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:40:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b1db703a337d301b1d50292acfbabd5fb3796511b962410c554420b85cd78dc`  
		Last Modified: Thu, 28 Jan 2021 23:58:38 GMT  
		Size: 2.4 MB (2423559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516139fc4bc5d3abbe484f41d65d96291d928c8313850bcfac5c409d91294e8e`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55705b9c11a25d31d806dae7cc70ba9979dbe2d872e5a1fa9675221a82cea552`  
		Last Modified: Fri, 12 Feb 2021 22:40:50 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19434ef650615c9f560946ec913d75335ea2c4da848dbe31002ba504051fe66`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 195.5 KB (195547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab2b83ef52894e4d6228617de9f67c33d742d2f237ee7fdfc38aeec8bf87f9a`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11720b6738d8b9681acab3a3423ae35fd9b3144467c23cb413deadffcfda6fd6`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:217ad97919e9aff3523891ff4cc50a783dd09a49976ae1f43a2cf615bd3167f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d125f8b9e25718ed14e33e37580e480d52edcf753f1cf917b1c4dd0ea4b9f358`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 01:49:09 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 01:49:12 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 01:49:12 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 01:49:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 01:49:42 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 01:49:43 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 01:49:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 01:49:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 01:49:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b73d7b095df7558c4913a1b56bc566a203d1705bceaf849063716da396aa3d`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a11963159741a5e3e3effd779670b8e3d7d46c46802b674c8c948528833d118`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 7.1 KB (7061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984eda174ae2399fbfdebdc2ed85bb966ca11956df853e13be5060029f19f345`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 204.4 KB (204443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d588ba06f796ba5588dbba0b0cacec4a16b2a60183e3cdffacf7f0d27bf18`  
		Last Modified: Sat, 13 Feb 2021 01:50:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e9caaa63d130b7c7a0ea6bcc1b2f984eae242f1ebea0d8bc7b5e487aea9a88`  
		Last Modified: Sat, 13 Feb 2021 01:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:4960ec29bb9ef335500e75f0083cd0266fe301739478d22c7eac9fd71a2a0ab3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3049596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4479a0b49914c6027a4470086fafeec21241b4ec58e6a9b2c913d6bca2d22ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:38:31 GMT
ADD file:c0e9ea135d66ad6504c77915a7a48b3bead60892d155d3258b746cb4945981c0 in / 
# Thu, 28 Jan 2021 23:38:31 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 00:59:25 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 00:59:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 00:59:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:59:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 00:59:50 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:59:50 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:59:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:59:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3fea00a81341ce917db671eb3ad24ef5750cb6928b7f760e3ce4dab619eeb1fa`  
		Last Modified: Thu, 28 Jan 2021 23:39:02 GMT  
		Size: 2.8 MB (2817627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7723c1203294add77f79b9f3aafc10eda8572905ac503c7f5a0b2d49e488ed`  
		Last Modified: Sat, 13 Feb 2021 01:00:17 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce806478241c0f699afc38824da58e636c67df1e42986b00e0984769077c20`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bd8240d52bc7724188c29d5ef4610ea463be9b970b707886910547d6edbf85`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 223.3 KB (223257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209f92f3e8326cecdb9a9e84435c267898cd9258f7a6ab104632b2653a905c9`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40d0142f6f8ec7c14fc1fbc2ea71a8ccf3e8f67ba870450c9b5601ea7a710ca`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:33c381176119d7660214d2991cb4a2ccfa254db448220f4df615870f3a84fc66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50abb8300ea994b3e481699c0929ed73d9007f8f85432f87cc74afeda4045cf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:55:50 GMT
ADD file:b14fd5f3f7fcd16e2b4ec6932d3e9c07c7400c577cee5fdcb88b0795a70a7bfb in / 
# Thu, 28 Jan 2021 23:55:52 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 02:34:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 02:34:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 02:34:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 02:35:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 02:35:24 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 02:35:28 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 02:35:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 02:35:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 02:35:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b94a1d8d591af02f1b419642bee91066ecbb9c65099d6903deed310fd1c2ff`  
		Last Modified: Thu, 28 Jan 2021 23:56:32 GMT  
		Size: 2.8 MB (2812517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e118e9785a8eefb11035770ba3f016fd6735fff79024dddf90bd04b98150410`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c02326e8246063ab1916219ed81aa1f954ca993bc3590ef06d7b6748d815977`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc9abddce71df5b7d8a16936252ae190e82033deb046797cf5341fff77f026e`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 221.0 KB (220996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d1ec7b1f9be796457a3f27e5d1d7644cac7c122fd210e179931e04dbc0e7ad`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce293f6c247be36cea3048f53a9ad45fe1640112b6b234e232b79e69a9f1efae`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:7b710fbed5a510700538e3437d8b3a418f829953d9b8fec0334ba9799219909c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2815889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fb1ee7014b5ab54030e234cfda6659e5d0d99d1c2033497d7f89f88cf5c2ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:41:35 GMT
ADD file:d97e6c37df0fb8306b072d9c0a32f68f5aff583ba849303926644deacfa25eb9 in / 
# Thu, 28 Jan 2021 23:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 03:11:30 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 03:11:31 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 03:11:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 03:11:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 03:11:42 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 03:11:42 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 03:11:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 03:11:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 03:11:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:43901f1af0ef9db6b0bf30ac6f6dacd78bf1ecfeb47ad0a93aa2370fa8e62407`  
		Last Modified: Thu, 28 Jan 2021 23:42:09 GMT  
		Size: 2.6 MB (2602059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345d8435943aca39411423265dc836788d9ec232e833f7cbc90ab835db3625c1`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b2484becfe02ade48d7c733db97b58e1ce5dfdafe33927ad4a722949f1d565`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 7.1 KB (7061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85179c983a9cffadd2d46f7ecf69991dc589c1dfb0379e6b34d372fb81f127e`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3949274cf2ec2bb3ad5931b5b9a119173d5ace06d37332a4d2c7a7d5f2199f91`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290cac537fab95725326ea6e10e2a1333216daaa916d670eac7fbf7005373593`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:d151d981ca0ebab580c3ff2c4360baa2e99aca02d7c13f9a4e9fcd89425eb2f0
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
$ docker pull spiped@sha256:835d7b06f38b14f3497dfa8ef3a3387976759c1d4da641bee7b66ab2614327e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883c5cce06c38a0f7a19e769ba33df23b5104eae4f2f2529c4b6c7d2540dd71a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 00:10:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 00:10:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 00:10:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:11:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 00:11:03 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:11:03 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:11:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:11:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:11:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ada2cbdd62e07ee40d2f05c48cbb06a172e5cde247cb27defa9146e342ee24`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0809851ee6dd7d72995918c73439754a4ff183f0aa0f142407150e9c75130e`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 7.0 KB (7049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814bb6e0e86dd762b94f3a86fe4ea3dcac961064cb970ae9852a2389eab5bc72`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 212.3 KB (212296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a22052f5d37047c574696d71e90ee4fc969f40189329fc130b69fd39cd39ab`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db107fe5f9add27475633bd978bdbc7404ae29a7f594d3a2e5aaff7ac44b63db`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c27babd1d2aafca8bda58fedee7d3038c7b20fbf7b5e1eb870270268eed209c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2832841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d677780adfebbeebb133e4df636a0d26d64e0813b9fd46fedf2f1d9db0a3783d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:49:59 GMT
ADD file:c197324e4979e2a7b257ad683d20dd9cbdae525a076bd68fe6aa0e0b126875df in / 
# Thu, 28 Jan 2021 23:49:59 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 23:07:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Feb 2021 23:07:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Feb 2021 23:07:57 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 23:08:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Feb 2021 23:08:24 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 23:08:25 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 23:08:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 23:08:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 23:08:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a66f440da051140fefcb0a520bdeb69d763b1eb4fd1b2ed46b4c0a168e335108`  
		Last Modified: Thu, 28 Jan 2021 23:50:33 GMT  
		Size: 2.6 MB (2621759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef16c09cad69b4f5ffbad02c5d05e54a8776d0f589b5070292f555188352fc2`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd09edfda78fafd09511434ad81f68f3aaa910006a0cf43dbd8c9aeea23e2fa`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b616073d9c59a7d6763e8532e2e8bd4c592396a4250e30e030e29ef220db07`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 202.3 KB (202293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcdea289e6dfa0b452fe3805b1859196021df0753f5954e2728ee1947cf9828`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa80572babecc8c62f006bbc854c927644a0939f8982217861c889a29c084e7`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ae4d066b309a39b651ddcafcf7e0b5544d6698a4cfc4a7eb1c4e493356befb0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2627898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79097e2ce8ba1eaa302fbfdff3d7cd160ef52f71c4e89a7e4d3c097be5fa9c82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:58:03 GMT
ADD file:98a89b90a8b442eed5301790dd2bd3a27391c5e4426126eed9d1cf44e70f8857 in / 
# Thu, 28 Jan 2021 23:58:04 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 22:39:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Feb 2021 22:39:48 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Feb 2021 22:39:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:40:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Feb 2021 22:40:17 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:40:17 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:40:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:40:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:40:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b1db703a337d301b1d50292acfbabd5fb3796511b962410c554420b85cd78dc`  
		Last Modified: Thu, 28 Jan 2021 23:58:38 GMT  
		Size: 2.4 MB (2423559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516139fc4bc5d3abbe484f41d65d96291d928c8313850bcfac5c409d91294e8e`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55705b9c11a25d31d806dae7cc70ba9979dbe2d872e5a1fa9675221a82cea552`  
		Last Modified: Fri, 12 Feb 2021 22:40:50 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19434ef650615c9f560946ec913d75335ea2c4da848dbe31002ba504051fe66`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 195.5 KB (195547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab2b83ef52894e4d6228617de9f67c33d742d2f237ee7fdfc38aeec8bf87f9a`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11720b6738d8b9681acab3a3423ae35fd9b3144467c23cb413deadffcfda6fd6`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:217ad97919e9aff3523891ff4cc50a783dd09a49976ae1f43a2cf615bd3167f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d125f8b9e25718ed14e33e37580e480d52edcf753f1cf917b1c4dd0ea4b9f358`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 01:49:09 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 01:49:12 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 01:49:12 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 01:49:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 01:49:42 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 01:49:43 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 01:49:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 01:49:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 01:49:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b73d7b095df7558c4913a1b56bc566a203d1705bceaf849063716da396aa3d`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a11963159741a5e3e3effd779670b8e3d7d46c46802b674c8c948528833d118`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 7.1 KB (7061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984eda174ae2399fbfdebdc2ed85bb966ca11956df853e13be5060029f19f345`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 204.4 KB (204443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d588ba06f796ba5588dbba0b0cacec4a16b2a60183e3cdffacf7f0d27bf18`  
		Last Modified: Sat, 13 Feb 2021 01:50:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e9caaa63d130b7c7a0ea6bcc1b2f984eae242f1ebea0d8bc7b5e487aea9a88`  
		Last Modified: Sat, 13 Feb 2021 01:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:4960ec29bb9ef335500e75f0083cd0266fe301739478d22c7eac9fd71a2a0ab3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3049596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4479a0b49914c6027a4470086fafeec21241b4ec58e6a9b2c913d6bca2d22ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:38:31 GMT
ADD file:c0e9ea135d66ad6504c77915a7a48b3bead60892d155d3258b746cb4945981c0 in / 
# Thu, 28 Jan 2021 23:38:31 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 00:59:25 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 00:59:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 00:59:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:59:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 00:59:50 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:59:50 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:59:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:59:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3fea00a81341ce917db671eb3ad24ef5750cb6928b7f760e3ce4dab619eeb1fa`  
		Last Modified: Thu, 28 Jan 2021 23:39:02 GMT  
		Size: 2.8 MB (2817627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7723c1203294add77f79b9f3aafc10eda8572905ac503c7f5a0b2d49e488ed`  
		Last Modified: Sat, 13 Feb 2021 01:00:17 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce806478241c0f699afc38824da58e636c67df1e42986b00e0984769077c20`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bd8240d52bc7724188c29d5ef4610ea463be9b970b707886910547d6edbf85`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 223.3 KB (223257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209f92f3e8326cecdb9a9e84435c267898cd9258f7a6ab104632b2653a905c9`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40d0142f6f8ec7c14fc1fbc2ea71a8ccf3e8f67ba870450c9b5601ea7a710ca`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:33c381176119d7660214d2991cb4a2ccfa254db448220f4df615870f3a84fc66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50abb8300ea994b3e481699c0929ed73d9007f8f85432f87cc74afeda4045cf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:55:50 GMT
ADD file:b14fd5f3f7fcd16e2b4ec6932d3e9c07c7400c577cee5fdcb88b0795a70a7bfb in / 
# Thu, 28 Jan 2021 23:55:52 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 02:34:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 02:34:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 02:34:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 02:35:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 02:35:24 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 02:35:28 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 02:35:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 02:35:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 02:35:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b94a1d8d591af02f1b419642bee91066ecbb9c65099d6903deed310fd1c2ff`  
		Last Modified: Thu, 28 Jan 2021 23:56:32 GMT  
		Size: 2.8 MB (2812517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e118e9785a8eefb11035770ba3f016fd6735fff79024dddf90bd04b98150410`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c02326e8246063ab1916219ed81aa1f954ca993bc3590ef06d7b6748d815977`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc9abddce71df5b7d8a16936252ae190e82033deb046797cf5341fff77f026e`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 221.0 KB (220996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d1ec7b1f9be796457a3f27e5d1d7644cac7c122fd210e179931e04dbc0e7ad`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce293f6c247be36cea3048f53a9ad45fe1640112b6b234e232b79e69a9f1efae`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:7b710fbed5a510700538e3437d8b3a418f829953d9b8fec0334ba9799219909c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2815889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fb1ee7014b5ab54030e234cfda6659e5d0d99d1c2033497d7f89f88cf5c2ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:41:35 GMT
ADD file:d97e6c37df0fb8306b072d9c0a32f68f5aff583ba849303926644deacfa25eb9 in / 
# Thu, 28 Jan 2021 23:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 03:11:30 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 03:11:31 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 03:11:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 03:11:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 03:11:42 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 03:11:42 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 03:11:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 03:11:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 03:11:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:43901f1af0ef9db6b0bf30ac6f6dacd78bf1ecfeb47ad0a93aa2370fa8e62407`  
		Last Modified: Thu, 28 Jan 2021 23:42:09 GMT  
		Size: 2.6 MB (2602059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345d8435943aca39411423265dc836788d9ec232e833f7cbc90ab835db3625c1`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b2484becfe02ade48d7c733db97b58e1ce5dfdafe33927ad4a722949f1d565`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 7.1 KB (7061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85179c983a9cffadd2d46f7ecf69991dc589c1dfb0379e6b34d372fb81f127e`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3949274cf2ec2bb3ad5931b5b9a119173d5ace06d37332a4d2c7a7d5f2199f91`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290cac537fab95725326ea6e10e2a1333216daaa916d670eac7fbf7005373593`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:d151d981ca0ebab580c3ff2c4360baa2e99aca02d7c13f9a4e9fcd89425eb2f0
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
$ docker pull spiped@sha256:835d7b06f38b14f3497dfa8ef3a3387976759c1d4da641bee7b66ab2614327e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883c5cce06c38a0f7a19e769ba33df23b5104eae4f2f2529c4b6c7d2540dd71a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 00:10:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 00:10:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 00:10:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:11:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 00:11:03 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:11:03 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:11:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:11:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:11:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ada2cbdd62e07ee40d2f05c48cbb06a172e5cde247cb27defa9146e342ee24`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0809851ee6dd7d72995918c73439754a4ff183f0aa0f142407150e9c75130e`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 7.0 KB (7049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814bb6e0e86dd762b94f3a86fe4ea3dcac961064cb970ae9852a2389eab5bc72`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 212.3 KB (212296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a22052f5d37047c574696d71e90ee4fc969f40189329fc130b69fd39cd39ab`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db107fe5f9add27475633bd978bdbc7404ae29a7f594d3a2e5aaff7ac44b63db`  
		Last Modified: Sat, 13 Feb 2021 00:11:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c27babd1d2aafca8bda58fedee7d3038c7b20fbf7b5e1eb870270268eed209c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2832841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d677780adfebbeebb133e4df636a0d26d64e0813b9fd46fedf2f1d9db0a3783d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:49:59 GMT
ADD file:c197324e4979e2a7b257ad683d20dd9cbdae525a076bd68fe6aa0e0b126875df in / 
# Thu, 28 Jan 2021 23:49:59 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 23:07:54 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Feb 2021 23:07:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Feb 2021 23:07:57 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 23:08:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Feb 2021 23:08:24 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 23:08:25 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 23:08:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 23:08:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 23:08:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a66f440da051140fefcb0a520bdeb69d763b1eb4fd1b2ed46b4c0a168e335108`  
		Last Modified: Thu, 28 Jan 2021 23:50:33 GMT  
		Size: 2.6 MB (2621759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef16c09cad69b4f5ffbad02c5d05e54a8776d0f589b5070292f555188352fc2`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd09edfda78fafd09511434ad81f68f3aaa910006a0cf43dbd8c9aeea23e2fa`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b616073d9c59a7d6763e8532e2e8bd4c592396a4250e30e030e29ef220db07`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 202.3 KB (202293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcdea289e6dfa0b452fe3805b1859196021df0753f5954e2728ee1947cf9828`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa80572babecc8c62f006bbc854c927644a0939f8982217861c889a29c084e7`  
		Last Modified: Fri, 12 Feb 2021 23:08:40 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ae4d066b309a39b651ddcafcf7e0b5544d6698a4cfc4a7eb1c4e493356befb0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2627898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79097e2ce8ba1eaa302fbfdff3d7cd160ef52f71c4e89a7e4d3c097be5fa9c82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:58:03 GMT
ADD file:98a89b90a8b442eed5301790dd2bd3a27391c5e4426126eed9d1cf44e70f8857 in / 
# Thu, 28 Jan 2021 23:58:04 GMT
CMD ["/bin/sh"]
# Fri, 12 Feb 2021 22:39:46 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Feb 2021 22:39:48 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Feb 2021 22:39:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:40:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Feb 2021 22:40:17 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:40:17 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:40:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:40:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:40:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b1db703a337d301b1d50292acfbabd5fb3796511b962410c554420b85cd78dc`  
		Last Modified: Thu, 28 Jan 2021 23:58:38 GMT  
		Size: 2.4 MB (2423559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516139fc4bc5d3abbe484f41d65d96291d928c8313850bcfac5c409d91294e8e`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55705b9c11a25d31d806dae7cc70ba9979dbe2d872e5a1fa9675221a82cea552`  
		Last Modified: Fri, 12 Feb 2021 22:40:50 GMT  
		Size: 7.1 KB (7062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19434ef650615c9f560946ec913d75335ea2c4da848dbe31002ba504051fe66`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 195.5 KB (195547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab2b83ef52894e4d6228617de9f67c33d742d2f237ee7fdfc38aeec8bf87f9a`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11720b6738d8b9681acab3a3423ae35fd9b3144467c23cb413deadffcfda6fd6`  
		Last Modified: Fri, 12 Feb 2021 22:40:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:217ad97919e9aff3523891ff4cc50a783dd09a49976ae1f43a2cf615bd3167f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d125f8b9e25718ed14e33e37580e480d52edcf753f1cf917b1c4dd0ea4b9f358`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 01:49:09 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 01:49:12 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 01:49:12 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 01:49:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 01:49:42 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 01:49:43 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 01:49:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 01:49:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 01:49:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b73d7b095df7558c4913a1b56bc566a203d1705bceaf849063716da396aa3d`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a11963159741a5e3e3effd779670b8e3d7d46c46802b674c8c948528833d118`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 7.1 KB (7061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984eda174ae2399fbfdebdc2ed85bb966ca11956df853e13be5060029f19f345`  
		Last Modified: Sat, 13 Feb 2021 01:50:16 GMT  
		Size: 204.4 KB (204443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d588ba06f796ba5588dbba0b0cacec4a16b2a60183e3cdffacf7f0d27bf18`  
		Last Modified: Sat, 13 Feb 2021 01:50:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e9caaa63d130b7c7a0ea6bcc1b2f984eae242f1ebea0d8bc7b5e487aea9a88`  
		Last Modified: Sat, 13 Feb 2021 01:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:4960ec29bb9ef335500e75f0083cd0266fe301739478d22c7eac9fd71a2a0ab3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3049596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4479a0b49914c6027a4470086fafeec21241b4ec58e6a9b2c913d6bca2d22ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:38:31 GMT
ADD file:c0e9ea135d66ad6504c77915a7a48b3bead60892d155d3258b746cb4945981c0 in / 
# Thu, 28 Jan 2021 23:38:31 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 00:59:25 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 00:59:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 00:59:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:59:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 00:59:50 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:59:50 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:59:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:59:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:59:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3fea00a81341ce917db671eb3ad24ef5750cb6928b7f760e3ce4dab619eeb1fa`  
		Last Modified: Thu, 28 Jan 2021 23:39:02 GMT  
		Size: 2.8 MB (2817627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7723c1203294add77f79b9f3aafc10eda8572905ac503c7f5a0b2d49e488ed`  
		Last Modified: Sat, 13 Feb 2021 01:00:17 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce806478241c0f699afc38824da58e636c67df1e42986b00e0984769077c20`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bd8240d52bc7724188c29d5ef4610ea463be9b970b707886910547d6edbf85`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 223.3 KB (223257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209f92f3e8326cecdb9a9e84435c267898cd9258f7a6ab104632b2653a905c9`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40d0142f6f8ec7c14fc1fbc2ea71a8ccf3e8f67ba870450c9b5601ea7a710ca`  
		Last Modified: Sat, 13 Feb 2021 01:00:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:33c381176119d7660214d2991cb4a2ccfa254db448220f4df615870f3a84fc66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50abb8300ea994b3e481699c0929ed73d9007f8f85432f87cc74afeda4045cf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:55:50 GMT
ADD file:b14fd5f3f7fcd16e2b4ec6932d3e9c07c7400c577cee5fdcb88b0795a70a7bfb in / 
# Thu, 28 Jan 2021 23:55:52 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 02:34:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 02:34:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 02:34:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 02:35:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 02:35:24 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 02:35:28 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 02:35:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 02:35:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 02:35:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b94a1d8d591af02f1b419642bee91066ecbb9c65099d6903deed310fd1c2ff`  
		Last Modified: Thu, 28 Jan 2021 23:56:32 GMT  
		Size: 2.8 MB (2812517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e118e9785a8eefb11035770ba3f016fd6735fff79024dddf90bd04b98150410`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c02326e8246063ab1916219ed81aa1f954ca993bc3590ef06d7b6748d815977`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc9abddce71df5b7d8a16936252ae190e82033deb046797cf5341fff77f026e`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 221.0 KB (220996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d1ec7b1f9be796457a3f27e5d1d7644cac7c122fd210e179931e04dbc0e7ad`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce293f6c247be36cea3048f53a9ad45fe1640112b6b234e232b79e69a9f1efae`  
		Last Modified: Sat, 13 Feb 2021 02:36:23 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:7b710fbed5a510700538e3437d8b3a418f829953d9b8fec0334ba9799219909c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2815889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fb1ee7014b5ab54030e234cfda6659e5d0d99d1c2033497d7f89f88cf5c2ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Jan 2021 23:41:35 GMT
ADD file:d97e6c37df0fb8306b072d9c0a32f68f5aff583ba849303926644deacfa25eb9 in / 
# Thu, 28 Jan 2021 23:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Feb 2021 03:11:30 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Feb 2021 03:11:31 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Feb 2021 03:11:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 03:11:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Feb 2021 03:11:42 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 03:11:42 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 03:11:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 03:11:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 03:11:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:43901f1af0ef9db6b0bf30ac6f6dacd78bf1ecfeb47ad0a93aa2370fa8e62407`  
		Last Modified: Thu, 28 Jan 2021 23:42:09 GMT  
		Size: 2.6 MB (2602059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345d8435943aca39411423265dc836788d9ec232e833f7cbc90ab835db3625c1`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b2484becfe02ade48d7c733db97b58e1ce5dfdafe33927ad4a722949f1d565`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 7.1 KB (7061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85179c983a9cffadd2d46f7ecf69991dc589c1dfb0379e6b34d372fb81f127e`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3949274cf2ec2bb3ad5931b5b9a119173d5ace06d37332a4d2c7a7d5f2199f91`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290cac537fab95725326ea6e10e2a1333216daaa916d670eac7fbf7005373593`  
		Last Modified: Sat, 13 Feb 2021 03:14:43 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:4e0757d83a01c2abc624d004ea3feb13bbd81c33ff0294e91744575688e0e92c
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
$ docker pull spiped@sha256:de2d45b0f59312e4abff77a82b78eaac004c3224734eedbc7334680c7ec5443f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36262768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897fcb40d5e49b8a35aa9e61c14eff1f62c615775ab19bff009fbbeafff2b106`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:21:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 00:09:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 00:09:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:09:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 00:09:59 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:10:00 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:10:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:10:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:10:02 GMT
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
	-	`sha256:04d13c52f8d2f79744057e6229950b1dfc5bd6291a85638e41c94d0bf6ae4e29`  
		Last Modified: Sat, 13 Feb 2021 00:11:29 GMT  
		Size: 2.1 MB (2128155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce83854aeaf080766f7945048114fa3e9b3416b345ca8aff96978c9c7f54953`  
		Last Modified: Sat, 13 Feb 2021 00:11:31 GMT  
		Size: 7.0 MB (7037301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb829d6ea4836c4cb76df6e6b6006024c209af26a1c18390c00a81ae68243bb`  
		Last Modified: Sat, 13 Feb 2021 00:11:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98a7fedb7f92d778864b0fcf2422f4ef009b2ab40c930b69020c825e6dec72c`  
		Last Modified: Sat, 13 Feb 2021 00:11:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:5fdf9146d8023cd6e901dbceff493b9883020acd456eb8bfbd5c480fcd681210
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32160479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781b7c6ba805844ffb5302f90107b4f5d7cc5f1fd80060ce54ea64fbad5616c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:50:10 GMT
ADD file:fbd00ef7871dc27d7ed5fa8c238cdc80652bd87b8033be7de9e54a799bbf10a4 in / 
# Tue, 09 Feb 2021 02:50:11 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:43:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 22:52:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 22:52:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:53:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 22:53:05 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:53:06 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:53:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:53:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:53:09 GMT
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
	-	`sha256:4b20e94947775259ce6bf04cfa19152b029d3365a89d4ccc0843ae79aa8bd4f2`  
		Last Modified: Fri, 12 Feb 2021 22:53:24 GMT  
		Size: 1.8 MB (1839109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5daf79a4e2ff35a482480dc5ed9294bc9b4a8973856555b77b39e3db207b7e`  
		Last Modified: Fri, 12 Feb 2021 22:53:26 GMT  
		Size: 5.5 MB (5479875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384e633e1a26bfac8686c377988482dd352c68b9f02ba80edcda2501879211a1`  
		Last Modified: Fri, 12 Feb 2021 22:53:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e3d0ff8a742e94655d7e9b5e7444b78818640156c0ca4672cfa957a605307f`  
		Last Modified: Fri, 12 Feb 2021 22:53:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3f1874e1134dbfca6d910ae69ff8d37e2a72d12404d8a9fd0fe0bd0c91e6db78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29750488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c287c25628c3da85c966ccc96d6e3e6e7a542d2487caaa805d5fa8a0525ea5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:57 GMT
ADD file:e675d50366bde57173a75f9a29367d765e7da2b7254c5254b64e777cf6870502 in / 
# Tue, 09 Feb 2021 03:01:00 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 19:35:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 22:38:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 22:38:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 22:39:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 22:39:30 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 22:39:30 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 22:39:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 22:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 22:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:db574d82360c3b60abadbef4f3daf8dee01f24741fc6ab3692aa543558d8b624`  
		Last Modified: Tue, 09 Feb 2021 03:09:46 GMT  
		Size: 22.7 MB (22703384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afe0266f6b6542f91658ca8ec8b87ac3e40c9e40d88f3ebfb311da27ffaa976`  
		Last Modified: Tue, 09 Feb 2021 19:37:10 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a439028cc7f7cbb2502897e215fe8142424bac7b8461519a3721306ca16262`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 1.8 MB (1759313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175e160ff82eee0dc76239d6e920ad6fce1b07298b3bd90e8120c021b7af0dd`  
		Last Modified: Fri, 12 Feb 2021 22:40:40 GMT  
		Size: 5.3 MB (5285596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4c31222b7eba85c87a5dbbee1012985dae7f842a0c60e03cc2641b409aa474`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88900a0b87f635433ee9e3c471b1a10b21ea199374733be54fb2595691999e2`  
		Last Modified: Fri, 12 Feb 2021 22:40:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:aeb7d15ee44fc1b03bfd46be858735700424119244cb66f38e14e9630c63e7ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33766524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61e1f2dc0e564ffcc34b5a7d98c4213648ab3f8a22f84e0db2b43178567f3a12`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:18:32 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 01:48:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 01:48:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 01:48:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 01:48:57 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 01:48:58 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 01:48:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 01:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 01:49:01 GMT
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
	-	`sha256:03005b703ccb19a3569b35a5b9bf1bfef156941eaf489b91ff81efde2e7ea584`  
		Last Modified: Sat, 13 Feb 2021 01:50:07 GMT  
		Size: 2.0 MB (2007571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c581bbabc2c122ca024c49c3aa7d735e4cfba75a1560c8c873223c66d0c57e6a`  
		Last Modified: Sat, 13 Feb 2021 01:50:08 GMT  
		Size: 5.9 MB (5905293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c709ad2716ce7723cf89c0c553985816902e98c25f46520d8faa51d120c7508f`  
		Last Modified: Sat, 13 Feb 2021 01:50:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe585f4a68228bec2b5b6765c7a8a860d41e59a842e3b43871e7120172ab40c7`  
		Last Modified: Sat, 13 Feb 2021 01:50:06 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:4f80cd66b8eb83d68da1b3cd894fe37462760fe5278f6973301e26f1af90bc91
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41520139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e96e1652c7ef7e3d880320ae65765f36dfe4d599e1ca9ac8c0154dcf0e54633a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:39:55 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 00:58:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 00:58:43 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 00:59:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 00:59:17 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 00:59:17 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 00:59:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 00:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 00:59:18 GMT
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
	-	`sha256:a4b87a23d1edb8994421e0ef8e6ae3e7a6364755d7e174130d7b4076dfa2119e`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 2.1 MB (2132258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7cffa8181e625c430a03c89cc64ae89e03825bd80c01986ce5486ad61b4c12`  
		Last Modified: Sat, 13 Feb 2021 01:00:11 GMT  
		Size: 11.6 MB (11632985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15dfc8a7a89424ce7b74424465fcef8b14d61f39590f94169b3a7afd30130b0`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3837cf2d6a87c1b6e64337cafb4ddb0959d201146a766002cc849caa670bae`  
		Last Modified: Sat, 13 Feb 2021 01:00:08 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:25a5e4c9bfecee13942120bcc34a2cdb13e00addd065a17df1302153ead12de4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33895238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:818a59f972b27eb92864d12c7304285f5966446e58096f31ad3b67a0bc8d07d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 03:09:26 GMT
ADD file:0222a151f4e5033d9eae98ce2b703a63f52d049dd72ac40bdd0dc2dafe619f0a in / 
# Tue, 09 Feb 2021 03:09:27 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:51:48 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Feb 2021 23:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Feb 2021 23:11:03 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Feb 2021 23:12:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Feb 2021 23:12:11 GMT
VOLUME [/spiped]
# Fri, 12 Feb 2021 23:12:12 GMT
WORKDIR /spiped
# Fri, 12 Feb 2021 23:12:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Feb 2021 23:12:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Feb 2021 23:12:13 GMT
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
	-	`sha256:5463eef3d8ce71368876b45ca24071008cc083ea16ea90ad16da78aee1b06eb0`  
		Last Modified: Fri, 12 Feb 2021 23:12:26 GMT  
		Size: 1.7 MB (1712078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c83f952ec2caa0e8a9319f93360620700120836fe9678c29036c7cf9868e9`  
		Last Modified: Fri, 12 Feb 2021 23:12:31 GMT  
		Size: 6.4 MB (6416347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b88510861e3f585271a563d2bee51e8dc1659e7abc654317636fd8a6e35956`  
		Last Modified: Fri, 12 Feb 2021 23:12:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8a904b2624ec463e93f83225ac51eebd738a0473f323cf0121dcf664488951`  
		Last Modified: Fri, 12 Feb 2021 23:12:25 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:864f9629da12aace742df3cd8167639ca43ff06a00763b99c31dcba10699a00e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39490261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749c18efc7646905a7417cb2107c88294bb750ed6bc8039f46b4311923b6e779`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:15:19 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 02:30:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 02:30:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 02:33:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 02:34:02 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 02:34:09 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 02:34:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 02:34:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 02:34:18 GMT
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
	-	`sha256:47130d66484e5dc6224d68f7eaf7129048723a038246f1ba3288bc669594ce4d`  
		Last Modified: Sat, 13 Feb 2021 02:36:06 GMT  
		Size: 2.2 MB (2224915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7be408970c00a6f67d09788fe2ae7d9bee14d0ddedf38e826cbedc4e12d6e`  
		Last Modified: Sat, 13 Feb 2021 02:36:07 GMT  
		Size: 6.7 MB (6743622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed58efc2e2df4e58c29b6b3946f036cdf35e85ba6b21cf906c7fe425b1efc82a`  
		Last Modified: Sat, 13 Feb 2021 02:36:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5da930633055937f1ba62f43cf83b555b527d1cd8255d66ac9d6281f3afa41d`  
		Last Modified: Sat, 13 Feb 2021 02:36:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:f1fc57dae92710b70032be2526f79e54964e55f92c1743f69ec7cf0a676d8116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33477416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dda528269da27ad9d1592ca7bc595ecbacc814c873d1441327b98560f8a43b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:10 GMT
ADD file:0edb2de05df54191a141bd125f59d7e14eef0cc4576927a247b8dd7d6f255d04 in / 
# Tue, 09 Feb 2021 02:42:12 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 06:33:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 13 Feb 2021 03:10:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 13 Feb 2021 03:10:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Feb 2021 03:11:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 13 Feb 2021 03:11:22 GMT
VOLUME [/spiped]
# Sat, 13 Feb 2021 03:11:22 GMT
WORKDIR /spiped
# Sat, 13 Feb 2021 03:11:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Feb 2021 03:11:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Feb 2021 03:11:23 GMT
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
	-	`sha256:916e90eba0ded4a99e0c1e86e0657b977665bf19661f2c18005fc6d6745d7fd4`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 1.8 MB (1821717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9478c638398830f42321041df73fb7c8005dd7c336c933045b5f043fe1e8786`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 5.9 MB (5943471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fb1c3cf1445657cf0a44894ccf3da2d62b39264d89fcbecc0e2db075fcfdcf`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f2ae3abab433a32b5e6ba282e6544117d7a01f4fd183d4a7582a4c5a64479f`  
		Last Modified: Sat, 13 Feb 2021 03:12:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
