<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1.6.1`](#spiped161)
-	[`spiped:1.6.1-alpine`](#spiped161-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:37e3f53dd3891f6249a391008eaad0cd841f419981020db94f7728f90513d12f
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

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:1494dd15abab70ff861f11b7aadcfb1913d7ad7e0c95fd9fa866fd8a997faae6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37332544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fe7196e9627619f9949f053a86afbc40496ceea34000b3b4ebaf24419e51df4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 22:24:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 22:24:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 22:24:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 22:25:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 22:25:00 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 22:25:01 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 22:25:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 22:25:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:25:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c16f44407339913efe8feb7893634dfbd49fdb363f86acc003a5264fd624a`  
		Last Modified: Tue, 28 Sep 2021 22:25:22 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c6c38eeca4ff05d1e9ec76ba7d4487d0301289ccb5e1887cc097cb52812f0`  
		Last Modified: Tue, 28 Sep 2021 22:25:21 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d3ddbaa314fafbcacbfc77277508c88563cf86d10c7ef081d1c2192c94fe62`  
		Last Modified: Tue, 28 Sep 2021 22:25:23 GMT  
		Size: 6.0 MB (5960379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70bf92a5d2ba79534d0d2f8bddde011587181eddf3b8f0d4a195d014da730fb`  
		Last Modified: Tue, 28 Sep 2021 22:25:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef36802cb5494594cbe25bf22ec477072dfe41486e99081666044bdd6d25fd3`  
		Last Modified: Tue, 28 Sep 2021 22:25:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:8436dc3d0b9307c6728fddf500bbfc53e22883abd81495bef1dbd786b56533a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33939113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6464f913e7d0a0d02b9c987ff12c419ca24b2f6a2b1c36ca7a5ec61982e60e32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:38 GMT
ADD file:da0067258fc1c6a50273e6b3b2673e88fad974a5a1fe4d5eecfeca2df1ff54b3 in / 
# Tue, 28 Sep 2021 01:50:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 19:39:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 19:39:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 19:39:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 19:40:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 19:40:18 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 19:40:18 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 19:40:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 19:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 19:40:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86f2b8be18fc44e8eb430e2c472979a79cda6eb6fa3add10cc8c5d8764eb90ac`  
		Last Modified: Tue, 28 Sep 2021 02:06:35 GMT  
		Size: 28.9 MB (28910670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3d70c7ae48d1f12dbe64e009353b0f4ae5906751228150eea7d8fa1071740f`  
		Last Modified: Tue, 28 Sep 2021 19:40:57 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e560d9a265326647c6bf0ec61bd636c1fc32bb12a184dd1754edbf4b4ac050`  
		Last Modified: Tue, 28 Sep 2021 19:40:57 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25dd92193301a114db15601dbcf4a5954c8d0de076495781fd6c9adaca0080f`  
		Last Modified: Tue, 28 Sep 2021 19:41:01 GMT  
		Size: 5.0 MB (5025194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f46212d749999bf7419078fc626db777dc61f530dc11ea65f671f6b0dfbbe9f`  
		Last Modified: Tue, 28 Sep 2021 19:40:56 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fb1ae610eeb08a59770348cf7cf160343c05595fbf209e65f24f2b989ec1ea`  
		Last Modified: Tue, 28 Sep 2021 19:40:56 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:958d2e76bb92a4709c36123b6553d179419227b06b733ec19cf1a4899da20853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31309843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0880cb9c6c234ff2fe6a3c163710a28845c22e1207ecd0b31cd8887cb77d26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:43:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 03:43:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:43:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 03:44:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 03:44:37 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 03:44:38 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 03:44:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:44:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 03:44:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ecc7e48d063e5bf0a086847e03c73699a183e8a9129e1b8ee3cab1482dde2d`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584009012f86b47c7e4e6d1fd99c2d00976e77d0c5c66f0179ed3c7ea7c54725`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae397080ab7f297afe0c2760bc744f5c6ab5ff8f88b8e0830bc8ae8d97b565f`  
		Last Modified: Tue, 12 Oct 2021 03:45:44 GMT  
		Size: 4.7 MB (4745527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c697bb38b9e3862762d00df70d8a431fd891e25b33a03308c9e1cf59a02c712`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c305948d80dae9d7e0b495eba60d890696dba8079d33af0619bb473c03c079`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b84b5dfa3a45a4a3247d03ea8e53134778a370366d4967ca1648de394559ff0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35323470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fbc4195f2bf091db9b87db926b163df95846c96bc02823cf4035017216ea876`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:43 GMT
ADD file:6472ab63529e688735f77634402740e08fdbd5bfa788c150915027993df7e8ec in / 
# Tue, 28 Sep 2021 01:40:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:51:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 15:51:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:51:46 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 15:52:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 15:52:08 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 15:52:08 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 15:52:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:52:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 15:52:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2f8871a8654eb1158cb626f8dc69992dba7e4bd8796fae6aa7cf967f951f5fe9`  
		Last Modified: Tue, 28 Sep 2021 01:48:25 GMT  
		Size: 30.1 MB (30055408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0bac6bf3efd88e9704f2f7b6a2c409b1df5ed4d12bf39715b3a2e61907fb1`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4facf47a49fb1694033154000aac13d2c30aafbf19e2c674bb4b27df60af7e2a`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8071a27573edf8bf22065560ce728d2de0654433685de5e18c1d26c7e8d1b66`  
		Last Modified: Tue, 28 Sep 2021 15:52:42 GMT  
		Size: 5.3 MB (5264803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeea85f6d4b4c5f24b4c9a75aface87afc9ef6b3c57fc95bc4c614dd809768`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309d496f924a836fede76deb85d262cb73b2ad70167020cab673d985568e24a9`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:af2b655879555e25f940b5bc902cb8ab828971b47b2238d6321f8df278c9137a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40267457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b96d038ad9160f431be6656aade8a3d2894947eadca6167bf2e19a3053fb6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:08 GMT
ADD file:8466bd8df052ea7fa26e49575ac95fd4934ddafdad54a9736ac2bd8e7fc6e735 in / 
# Tue, 28 Sep 2021 01:40:08 GMT
CMD ["bash"]
# Wed, 29 Sep 2021 01:05:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 29 Sep 2021 01:05:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 01:05:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 29 Sep 2021 01:06:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 29 Sep 2021 01:06:24 GMT
VOLUME [/spiped]
# Wed, 29 Sep 2021 01:06:24 GMT
WORKDIR /spiped
# Wed, 29 Sep 2021 01:06:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 29 Sep 2021 01:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 01:06:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e79fce1f6442094a82dc5f6b4d1aa352e04aae39bba821c9021f6da08b1cacaf`  
		Last Modified: Tue, 28 Sep 2021 01:49:07 GMT  
		Size: 32.4 MB (32380160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ea16e10fc5a5a0c4d62cf75b45ed7ad926cec71dc07cd1e46bfcec64a34e09`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7e9cd8372b882a460f62793c1c0d821b3a2d51e3777788be1dfef41055e4d3`  
		Last Modified: Wed, 29 Sep 2021 01:07:17 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200cd2275f388ecc2501c7ab0be9e5795e5aca50325dd9fcf253f1069890417a`  
		Last Modified: Wed, 29 Sep 2021 01:07:20 GMT  
		Size: 7.9 MB (7884038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a169c2e014ded4f64624fb6773ef8fb0c5f3e524fbe12a7f545b861f2bcf54ec`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c16912aa5431d3f809850fa2f91c9d56ea38463628134f5b3b55935f54f5dc`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:028091d21c83e82c61f42923008ed53b9b6e9b130901b2b130429ae0ff355b70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e3374098957b2318d62eead2991c25245a9a698f601f8546440c6c6e83fa9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 02:10:40 GMT
ADD file:43593ef3d79c9b74a92e318d44aacb578f6f8d835dd72665e057bbfe73df1a93 in / 
# Tue, 28 Sep 2021 02:10:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 02:48:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 02:50:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 02:50:03 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 02:50:03 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 02:50:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:50:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f46ea49e27fccc580c8910db39ba7f51ae208a8d24d46a33140afa92ea3d955`  
		Last Modified: Tue, 28 Sep 2021 02:20:45 GMT  
		Size: 29.6 MB (29627871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa45c48be690dce117b2c0dce958f833f4ce085161cd4c6c5b633016534a89ea`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcf26a9aa3a964a21c42b56fd150ed69b7acd005c6629fb4623f95398a88425`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa171fdf362c6c554abf987cede2b8b25abb86afcde7578fea5c091f2cc1197d`  
		Last Modified: Tue, 28 Sep 2021 02:50:31 GMT  
		Size: 5.7 MB (5706116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e04cfec760a4c1a4925c2e96350ddc653e81d2bf92b7ffb7b9239f64aaae387`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b355a5bc54137c27f6b9f4b8e9e3caef346c4d0c43bf9d7496bfa69f266085e`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:b854abceecf263ecd3af9062c9bddf00c657ddc847f0a7beffa3d324806c6bfc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41277029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9de0b22b9d88c7e7b941d2522f2954d1ff0b9cdfde5162978baa1f74ddd6d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Oct 2021 17:55:01 GMT
ADD file:f4b696a766a0d9a808c171a1d5db4f0877b0a784649d63bf461dfcf54b532239 in / 
# Mon, 04 Oct 2021 17:55:06 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 04:33:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 06 Oct 2021 04:33:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 04:33:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 06 Oct 2021 04:35:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 06 Oct 2021 04:35:21 GMT
VOLUME [/spiped]
# Wed, 06 Oct 2021 04:35:23 GMT
WORKDIR /spiped
# Wed, 06 Oct 2021 04:35:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 06 Oct 2021 04:35:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Oct 2021 04:35:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c3b7af0ed242d09d9fee2dfc48d4553d58ad90c5fb862ab58fb89e2d04c5b922`  
		Last Modified: Mon, 04 Oct 2021 18:07:32 GMT  
		Size: 35.3 MB (35272408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61743fc20904f8539cf80302250d866a1c6417663826735c20362034cef7501a`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da94c352893f839938e7606a77c9b6a0c747558c66e01483dd5ef4a69a07383`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534d0224ab6f6639dbd9d41948087e426816f7e37e5940c041d0b712088c87b3`  
		Last Modified: Wed, 06 Oct 2021 04:36:08 GMT  
		Size: 6.0 MB (6001359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eb63df061584de7f6a9d4c754a21f5a3426f46c6704a41d99439d92f398a56`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8bfc7f69743b3fb3ffefa3ccfdcbc84807fe7c346480cc8313ee1af72d33c`  
		Last Modified: Wed, 06 Oct 2021 04:36:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:a81d059af60f158dfb49e3e03962db08aa2b6e40cbd80347d509d2026369a479
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db5d72188d3d25ba7347f1a8ea21b01cf4a27445b632afe2b83bdd2f0f06c798`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:57 GMT
ADD file:2daa8824c30440336bc6ea1448af03234d491ad7c0d0cac917cae5eb54c315fc in / 
# Tue, 28 Sep 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:55:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 09:55:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:55:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 09:55:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 09:55:36 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 09:55:36 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 09:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 09:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 09:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e8e2938f4df931c46d7575f0b7bad5bc357277fc3e132b720e704ac7a4d1c9ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:01 GMT  
		Size: 29.7 MB (29650795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f460f8990cce2d9f2e25c13b42c5513a2129ef1a318b1097f6ff1186a5fbef71`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e214e0743e5982442db728a32fd9951aa1a7e6d14317d4cec1824fa8eeca957a`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4f812c2b3b5fbebd9e26191ed62c7eac5f1012927dfb8571c9f99a57d3db8`  
		Last Modified: Tue, 28 Sep 2021 09:56:09 GMT  
		Size: 5.2 MB (5183853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972d8d742129ea070e9be63d7a5e8bc2840090dfe9ed23aa907c2508a1e9c3c9`  
		Last Modified: Tue, 28 Sep 2021 09:56:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216f4500775537761e72820f3bb08e33e37ebf36fb33e73f0dca40bb88e2bf48`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:89f362dd004a510b0e2dfdfdf849444c25d6fb0c60e3b7df331ece34ce763a31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:44015ddc42ceef8878c9b2bad7a6bcbf2b5d2ca42ab52cca20f9f66b2c15ffd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65d8337530e6b8e116202287d477945c4375886702df4698f8740106658a777`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:56:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:56:13 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:56:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:56:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:56:31 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:56:31 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:56:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:56:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:56:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72fe484884c949a7fba8b7d917cbe40b9fa50036f4c10e4b82e3075576fe3fc`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06083e8d35a44724cf84de43d971fb5b141e8ce6468a5c267c43c96f79869f23`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037fda176acae1eef93fa1dde784253576faf4d880c75c8d7df76fdf212dda`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 212.5 KB (212547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb3cd7f024c8cfa70e1c8e8f282e44395bbaa20cd69851af0552d8041deaea2`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fccea2af66d4ffdbdd93edf485c1e6e17f14ac10329842af6fea7741bd3504`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:7e548b9910cf9bcbce660ff537e09660dbd9d84cbc06621e45fb2282f2f52270
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2838978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8539d235dbd2d180f98df622ec1586ed595c7026c53f57b67876cbe0b641be9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:39:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:39:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:39:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:39:57 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:39:58 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:39:58 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:39:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:39:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:40:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ec865614b924d3ebd8faaf1468ff031de3ccb2f178656d907e4a89f8673776`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07908dc20812a0124cb96563b08ff2d4ebd32f0ca0cef02511faa0c127496e96`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 7.3 KB (7290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2ce7f8303145adfe2a17235c758d30fa18338c417eb73738b591c1dd3d1315`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 202.5 KB (202499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07f8ab6ed47190923d1d152d960c5fd80b7d9f27f84a289e8236a1e4f22843c`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17d0a64e682741c70413fc90f0d8a4dac61425dcc5c98ce054909120977e587`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:24d05f05df7127b2aa61654a9d29c77a0c2a00f8ba29dbfc127a672700d5f652
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2635217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c197156cacbfdbdb870ce3391ad1bdf7d6c922d18648489e7549033356f432b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 03:04:23 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 03:04:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 03:04:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 03:04:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 03:04:59 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 03:05:00 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 03:05:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 03:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 03:05:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c187e6961a8f3ae8bf645e1fbec375c4f7c3d8146ab5ee5a09f57cd5615f33cb`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56c389f9017243d26a8fd61b3cc3385e2b4dcf930d608cc682a5ff3b437137`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0da469457d5465481ffd06dc86cd457daaf02e8b501cbee7b9cb52b675525`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 195.8 KB (195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea4333c9f229866ca36ab2d7e036e1d23031e78c62c3ad0bcbbeacaaf8f8e65`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4907440a689992d3e1fbcc2fcef650c5ef7b7abe5b8b3aa9c97d6d697d5050fd`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:026d11edbbedc8b8a63207a745859b0ada912c11cbd6bf77d2eb162cfb1a6577
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7dbad85a08f79ca7ef7c449feb1dfbd6973498a21db9a0721af19e181fc39f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 01:45:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 01:45:36 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 01:45:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 01:45:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 01:45:53 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 01:45:53 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 01:45:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 01:45:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130a79b60aae9998377169e6355792370bb064e6148684353d6ed4826039492f`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43519aa40fdf82f3b05cab9731634890c7e8dc8b9731ce4c7c3fbbc35def0274`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 7.3 KB (7299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a1b5762b7444935215ce9e31bc9a68cac110a8b0bf2f9ca433a2d78620fe35`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 204.6 KB (204622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f156837dee9efeb5125ef7fc8d079ccf996015838cfe028bfb81695eb1230b99`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f221da4d2654d1b1432ad3c77afeed7392661b44c6a50fc1fd5e2cede5dfcb`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:da842be683e4aa6e7f0e6581d7d9bd1604d2d140a1b452e47a1ca595261af814
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3055327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7b5670b88fbd238447f1f65531173381d0aff05ec6d63ef2df4dfb7b8c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:35:24 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:35:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:35:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:35:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:35:45 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:35:45 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:35:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:35:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:35:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95070702ac27305ca355fc2880dec01d9e18d3c8a4a22842a599db59ea5467e0`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35be501885b2efd06479a1d05af31f0d06d6b0a5c4dfb3f760af81657d7919ea`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 7.3 KB (7287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f5e404d9d5a395b15445e0403dfa9a598ab9ecd02814798d33098ac6a8ba9c`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 223.4 KB (223445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b8287cb974321164bff4ca80e9a231471fecf0bbab1bbf130172709ae47ae`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c88353a13d0403b037e398aa01ea54701b91f2adf180d6ed9df1b155b62c89`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:3c83af52715b14ccfd27cc89b7b988ae73b9d05500efd053b99b027c0328f14d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f59b6df7881927f19f4b2dcab5974d93c4284e7e9ba9c21098a82d888389b26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:36:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 27 Aug 2021 21:36:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 27 Aug 2021 21:37:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 27 Aug 2021 21:37:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 27 Aug 2021 21:37:41 GMT
VOLUME [/spiped]
# Fri, 27 Aug 2021 21:37:48 GMT
WORKDIR /spiped
# Fri, 27 Aug 2021 21:37:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:38:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f143c775bd94ef9de49da05aab2353301bc02ceb74a237332f8d9b23e193234b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9067169d42bea9851adf89b67776e5a280513855fb73120a8d2c5f0051a1097b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 7.3 KB (7292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe10232ba40d32a7b84a0fe16aa0a2b418d2bdf093335c9fbaf56b08e751c54e`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 221.2 KB (221238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c7d84f077aa3ad717767ac56d4b1ea509bc7a9c81e57e3f4e210fe09205ee9`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c90dd2a4fa5a2acd662ddc7f2ec01550257e4bbaae18ab7a94fdd288523cf8`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:3852ee4130c6bfe6eb29489ab1f82c2aceed2d65ba3a11477360199bd6ba4bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2817762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d772c7d45678813ce17e2e65d11aa3e23e0517de39acbfe03eaaadf3558b6f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 04:23:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 04:23:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 04:23:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 04:24:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 04:24:08 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 04:24:08 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 04:24:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 04:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 04:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a66831aa123cebdb722d7d1efb39f1ffb26129fdf9b8937935375852a206`  
		Last Modified: Sat, 28 Aug 2021 04:24:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b103bd0361f6fb48151c8780e205c3fde97140b66762b27effcf2c3b73c05c`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 7.3 KB (7283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce02139d2773db6b3c7033d9dbc6fdb427c918a69c29b8bb01669296d18c9fe`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 205.3 KB (205277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c3cb214e79007442b4d21bc48516c0ef35753d8db03a0cc129fa63d01bedde`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29859d07f0b507288c642deae1bae6cbe9d019152647a0c4e76bd86474fda106`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:37e3f53dd3891f6249a391008eaad0cd841f419981020db94f7728f90513d12f
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

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:1494dd15abab70ff861f11b7aadcfb1913d7ad7e0c95fd9fa866fd8a997faae6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37332544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fe7196e9627619f9949f053a86afbc40496ceea34000b3b4ebaf24419e51df4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 22:24:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 22:24:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 22:24:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 22:25:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 22:25:00 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 22:25:01 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 22:25:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 22:25:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:25:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c16f44407339913efe8feb7893634dfbd49fdb363f86acc003a5264fd624a`  
		Last Modified: Tue, 28 Sep 2021 22:25:22 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c6c38eeca4ff05d1e9ec76ba7d4487d0301289ccb5e1887cc097cb52812f0`  
		Last Modified: Tue, 28 Sep 2021 22:25:21 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d3ddbaa314fafbcacbfc77277508c88563cf86d10c7ef081d1c2192c94fe62`  
		Last Modified: Tue, 28 Sep 2021 22:25:23 GMT  
		Size: 6.0 MB (5960379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70bf92a5d2ba79534d0d2f8bddde011587181eddf3b8f0d4a195d014da730fb`  
		Last Modified: Tue, 28 Sep 2021 22:25:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef36802cb5494594cbe25bf22ec477072dfe41486e99081666044bdd6d25fd3`  
		Last Modified: Tue, 28 Sep 2021 22:25:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:8436dc3d0b9307c6728fddf500bbfc53e22883abd81495bef1dbd786b56533a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33939113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6464f913e7d0a0d02b9c987ff12c419ca24b2f6a2b1c36ca7a5ec61982e60e32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:38 GMT
ADD file:da0067258fc1c6a50273e6b3b2673e88fad974a5a1fe4d5eecfeca2df1ff54b3 in / 
# Tue, 28 Sep 2021 01:50:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 19:39:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 19:39:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 19:39:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 19:40:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 19:40:18 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 19:40:18 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 19:40:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 19:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 19:40:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86f2b8be18fc44e8eb430e2c472979a79cda6eb6fa3add10cc8c5d8764eb90ac`  
		Last Modified: Tue, 28 Sep 2021 02:06:35 GMT  
		Size: 28.9 MB (28910670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3d70c7ae48d1f12dbe64e009353b0f4ae5906751228150eea7d8fa1071740f`  
		Last Modified: Tue, 28 Sep 2021 19:40:57 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e560d9a265326647c6bf0ec61bd636c1fc32bb12a184dd1754edbf4b4ac050`  
		Last Modified: Tue, 28 Sep 2021 19:40:57 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25dd92193301a114db15601dbcf4a5954c8d0de076495781fd6c9adaca0080f`  
		Last Modified: Tue, 28 Sep 2021 19:41:01 GMT  
		Size: 5.0 MB (5025194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f46212d749999bf7419078fc626db777dc61f530dc11ea65f671f6b0dfbbe9f`  
		Last Modified: Tue, 28 Sep 2021 19:40:56 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fb1ae610eeb08a59770348cf7cf160343c05595fbf209e65f24f2b989ec1ea`  
		Last Modified: Tue, 28 Sep 2021 19:40:56 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:958d2e76bb92a4709c36123b6553d179419227b06b733ec19cf1a4899da20853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31309843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0880cb9c6c234ff2fe6a3c163710a28845c22e1207ecd0b31cd8887cb77d26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:43:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 03:43:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:43:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 03:44:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 03:44:37 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 03:44:38 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 03:44:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:44:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 03:44:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ecc7e48d063e5bf0a086847e03c73699a183e8a9129e1b8ee3cab1482dde2d`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584009012f86b47c7e4e6d1fd99c2d00976e77d0c5c66f0179ed3c7ea7c54725`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae397080ab7f297afe0c2760bc744f5c6ab5ff8f88b8e0830bc8ae8d97b565f`  
		Last Modified: Tue, 12 Oct 2021 03:45:44 GMT  
		Size: 4.7 MB (4745527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c697bb38b9e3862762d00df70d8a431fd891e25b33a03308c9e1cf59a02c712`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c305948d80dae9d7e0b495eba60d890696dba8079d33af0619bb473c03c079`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b84b5dfa3a45a4a3247d03ea8e53134778a370366d4967ca1648de394559ff0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35323470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fbc4195f2bf091db9b87db926b163df95846c96bc02823cf4035017216ea876`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:43 GMT
ADD file:6472ab63529e688735f77634402740e08fdbd5bfa788c150915027993df7e8ec in / 
# Tue, 28 Sep 2021 01:40:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:51:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 15:51:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:51:46 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 15:52:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 15:52:08 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 15:52:08 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 15:52:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:52:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 15:52:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2f8871a8654eb1158cb626f8dc69992dba7e4bd8796fae6aa7cf967f951f5fe9`  
		Last Modified: Tue, 28 Sep 2021 01:48:25 GMT  
		Size: 30.1 MB (30055408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0bac6bf3efd88e9704f2f7b6a2c409b1df5ed4d12bf39715b3a2e61907fb1`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4facf47a49fb1694033154000aac13d2c30aafbf19e2c674bb4b27df60af7e2a`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8071a27573edf8bf22065560ce728d2de0654433685de5e18c1d26c7e8d1b66`  
		Last Modified: Tue, 28 Sep 2021 15:52:42 GMT  
		Size: 5.3 MB (5264803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeea85f6d4b4c5f24b4c9a75aface87afc9ef6b3c57fc95bc4c614dd809768`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309d496f924a836fede76deb85d262cb73b2ad70167020cab673d985568e24a9`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:af2b655879555e25f940b5bc902cb8ab828971b47b2238d6321f8df278c9137a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40267457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b96d038ad9160f431be6656aade8a3d2894947eadca6167bf2e19a3053fb6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:08 GMT
ADD file:8466bd8df052ea7fa26e49575ac95fd4934ddafdad54a9736ac2bd8e7fc6e735 in / 
# Tue, 28 Sep 2021 01:40:08 GMT
CMD ["bash"]
# Wed, 29 Sep 2021 01:05:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 29 Sep 2021 01:05:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 01:05:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 29 Sep 2021 01:06:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 29 Sep 2021 01:06:24 GMT
VOLUME [/spiped]
# Wed, 29 Sep 2021 01:06:24 GMT
WORKDIR /spiped
# Wed, 29 Sep 2021 01:06:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 29 Sep 2021 01:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 01:06:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e79fce1f6442094a82dc5f6b4d1aa352e04aae39bba821c9021f6da08b1cacaf`  
		Last Modified: Tue, 28 Sep 2021 01:49:07 GMT  
		Size: 32.4 MB (32380160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ea16e10fc5a5a0c4d62cf75b45ed7ad926cec71dc07cd1e46bfcec64a34e09`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7e9cd8372b882a460f62793c1c0d821b3a2d51e3777788be1dfef41055e4d3`  
		Last Modified: Wed, 29 Sep 2021 01:07:17 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200cd2275f388ecc2501c7ab0be9e5795e5aca50325dd9fcf253f1069890417a`  
		Last Modified: Wed, 29 Sep 2021 01:07:20 GMT  
		Size: 7.9 MB (7884038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a169c2e014ded4f64624fb6773ef8fb0c5f3e524fbe12a7f545b861f2bcf54ec`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c16912aa5431d3f809850fa2f91c9d56ea38463628134f5b3b55935f54f5dc`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:028091d21c83e82c61f42923008ed53b9b6e9b130901b2b130429ae0ff355b70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e3374098957b2318d62eead2991c25245a9a698f601f8546440c6c6e83fa9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 02:10:40 GMT
ADD file:43593ef3d79c9b74a92e318d44aacb578f6f8d835dd72665e057bbfe73df1a93 in / 
# Tue, 28 Sep 2021 02:10:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 02:48:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 02:50:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 02:50:03 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 02:50:03 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 02:50:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:50:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f46ea49e27fccc580c8910db39ba7f51ae208a8d24d46a33140afa92ea3d955`  
		Last Modified: Tue, 28 Sep 2021 02:20:45 GMT  
		Size: 29.6 MB (29627871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa45c48be690dce117b2c0dce958f833f4ce085161cd4c6c5b633016534a89ea`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcf26a9aa3a964a21c42b56fd150ed69b7acd005c6629fb4623f95398a88425`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa171fdf362c6c554abf987cede2b8b25abb86afcde7578fea5c091f2cc1197d`  
		Last Modified: Tue, 28 Sep 2021 02:50:31 GMT  
		Size: 5.7 MB (5706116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e04cfec760a4c1a4925c2e96350ddc653e81d2bf92b7ffb7b9239f64aaae387`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b355a5bc54137c27f6b9f4b8e9e3caef346c4d0c43bf9d7496bfa69f266085e`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:b854abceecf263ecd3af9062c9bddf00c657ddc847f0a7beffa3d324806c6bfc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41277029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9de0b22b9d88c7e7b941d2522f2954d1ff0b9cdfde5162978baa1f74ddd6d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Oct 2021 17:55:01 GMT
ADD file:f4b696a766a0d9a808c171a1d5db4f0877b0a784649d63bf461dfcf54b532239 in / 
# Mon, 04 Oct 2021 17:55:06 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 04:33:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 06 Oct 2021 04:33:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 04:33:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 06 Oct 2021 04:35:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 06 Oct 2021 04:35:21 GMT
VOLUME [/spiped]
# Wed, 06 Oct 2021 04:35:23 GMT
WORKDIR /spiped
# Wed, 06 Oct 2021 04:35:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 06 Oct 2021 04:35:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Oct 2021 04:35:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c3b7af0ed242d09d9fee2dfc48d4553d58ad90c5fb862ab58fb89e2d04c5b922`  
		Last Modified: Mon, 04 Oct 2021 18:07:32 GMT  
		Size: 35.3 MB (35272408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61743fc20904f8539cf80302250d866a1c6417663826735c20362034cef7501a`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da94c352893f839938e7606a77c9b6a0c747558c66e01483dd5ef4a69a07383`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534d0224ab6f6639dbd9d41948087e426816f7e37e5940c041d0b712088c87b3`  
		Last Modified: Wed, 06 Oct 2021 04:36:08 GMT  
		Size: 6.0 MB (6001359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eb63df061584de7f6a9d4c754a21f5a3426f46c6704a41d99439d92f398a56`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8bfc7f69743b3fb3ffefa3ccfdcbc84807fe7c346480cc8313ee1af72d33c`  
		Last Modified: Wed, 06 Oct 2021 04:36:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:a81d059af60f158dfb49e3e03962db08aa2b6e40cbd80347d509d2026369a479
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db5d72188d3d25ba7347f1a8ea21b01cf4a27445b632afe2b83bdd2f0f06c798`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:57 GMT
ADD file:2daa8824c30440336bc6ea1448af03234d491ad7c0d0cac917cae5eb54c315fc in / 
# Tue, 28 Sep 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:55:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 09:55:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:55:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 09:55:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 09:55:36 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 09:55:36 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 09:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 09:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 09:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e8e2938f4df931c46d7575f0b7bad5bc357277fc3e132b720e704ac7a4d1c9ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:01 GMT  
		Size: 29.7 MB (29650795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f460f8990cce2d9f2e25c13b42c5513a2129ef1a318b1097f6ff1186a5fbef71`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e214e0743e5982442db728a32fd9951aa1a7e6d14317d4cec1824fa8eeca957a`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4f812c2b3b5fbebd9e26191ed62c7eac5f1012927dfb8571c9f99a57d3db8`  
		Last Modified: Tue, 28 Sep 2021 09:56:09 GMT  
		Size: 5.2 MB (5183853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972d8d742129ea070e9be63d7a5e8bc2840090dfe9ed23aa907c2508a1e9c3c9`  
		Last Modified: Tue, 28 Sep 2021 09:56:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216f4500775537761e72820f3bb08e33e37ebf36fb33e73f0dca40bb88e2bf48`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:89f362dd004a510b0e2dfdfdf849444c25d6fb0c60e3b7df331ece34ce763a31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:44015ddc42ceef8878c9b2bad7a6bcbf2b5d2ca42ab52cca20f9f66b2c15ffd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65d8337530e6b8e116202287d477945c4375886702df4698f8740106658a777`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:56:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:56:13 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:56:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:56:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:56:31 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:56:31 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:56:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:56:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:56:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72fe484884c949a7fba8b7d917cbe40b9fa50036f4c10e4b82e3075576fe3fc`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06083e8d35a44724cf84de43d971fb5b141e8ce6468a5c267c43c96f79869f23`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037fda176acae1eef93fa1dde784253576faf4d880c75c8d7df76fdf212dda`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 212.5 KB (212547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb3cd7f024c8cfa70e1c8e8f282e44395bbaa20cd69851af0552d8041deaea2`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fccea2af66d4ffdbdd93edf485c1e6e17f14ac10329842af6fea7741bd3504`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:7e548b9910cf9bcbce660ff537e09660dbd9d84cbc06621e45fb2282f2f52270
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2838978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8539d235dbd2d180f98df622ec1586ed595c7026c53f57b67876cbe0b641be9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:39:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:39:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:39:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:39:57 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:39:58 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:39:58 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:39:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:39:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:40:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ec865614b924d3ebd8faaf1468ff031de3ccb2f178656d907e4a89f8673776`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07908dc20812a0124cb96563b08ff2d4ebd32f0ca0cef02511faa0c127496e96`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 7.3 KB (7290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2ce7f8303145adfe2a17235c758d30fa18338c417eb73738b591c1dd3d1315`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 202.5 KB (202499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07f8ab6ed47190923d1d152d960c5fd80b7d9f27f84a289e8236a1e4f22843c`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17d0a64e682741c70413fc90f0d8a4dac61425dcc5c98ce054909120977e587`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:24d05f05df7127b2aa61654a9d29c77a0c2a00f8ba29dbfc127a672700d5f652
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2635217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c197156cacbfdbdb870ce3391ad1bdf7d6c922d18648489e7549033356f432b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 03:04:23 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 03:04:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 03:04:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 03:04:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 03:04:59 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 03:05:00 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 03:05:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 03:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 03:05:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c187e6961a8f3ae8bf645e1fbec375c4f7c3d8146ab5ee5a09f57cd5615f33cb`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56c389f9017243d26a8fd61b3cc3385e2b4dcf930d608cc682a5ff3b437137`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0da469457d5465481ffd06dc86cd457daaf02e8b501cbee7b9cb52b675525`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 195.8 KB (195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea4333c9f229866ca36ab2d7e036e1d23031e78c62c3ad0bcbbeacaaf8f8e65`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4907440a689992d3e1fbcc2fcef650c5ef7b7abe5b8b3aa9c97d6d697d5050fd`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:026d11edbbedc8b8a63207a745859b0ada912c11cbd6bf77d2eb162cfb1a6577
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7dbad85a08f79ca7ef7c449feb1dfbd6973498a21db9a0721af19e181fc39f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 01:45:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 01:45:36 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 01:45:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 01:45:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 01:45:53 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 01:45:53 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 01:45:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 01:45:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130a79b60aae9998377169e6355792370bb064e6148684353d6ed4826039492f`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43519aa40fdf82f3b05cab9731634890c7e8dc8b9731ce4c7c3fbbc35def0274`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 7.3 KB (7299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a1b5762b7444935215ce9e31bc9a68cac110a8b0bf2f9ca433a2d78620fe35`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 204.6 KB (204622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f156837dee9efeb5125ef7fc8d079ccf996015838cfe028bfb81695eb1230b99`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f221da4d2654d1b1432ad3c77afeed7392661b44c6a50fc1fd5e2cede5dfcb`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:da842be683e4aa6e7f0e6581d7d9bd1604d2d140a1b452e47a1ca595261af814
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3055327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7b5670b88fbd238447f1f65531173381d0aff05ec6d63ef2df4dfb7b8c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:35:24 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:35:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:35:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:35:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:35:45 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:35:45 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:35:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:35:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:35:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95070702ac27305ca355fc2880dec01d9e18d3c8a4a22842a599db59ea5467e0`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35be501885b2efd06479a1d05af31f0d06d6b0a5c4dfb3f760af81657d7919ea`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 7.3 KB (7287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f5e404d9d5a395b15445e0403dfa9a598ab9ecd02814798d33098ac6a8ba9c`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 223.4 KB (223445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b8287cb974321164bff4ca80e9a231471fecf0bbab1bbf130172709ae47ae`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c88353a13d0403b037e398aa01ea54701b91f2adf180d6ed9df1b155b62c89`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:3c83af52715b14ccfd27cc89b7b988ae73b9d05500efd053b99b027c0328f14d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f59b6df7881927f19f4b2dcab5974d93c4284e7e9ba9c21098a82d888389b26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:36:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 27 Aug 2021 21:36:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 27 Aug 2021 21:37:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 27 Aug 2021 21:37:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 27 Aug 2021 21:37:41 GMT
VOLUME [/spiped]
# Fri, 27 Aug 2021 21:37:48 GMT
WORKDIR /spiped
# Fri, 27 Aug 2021 21:37:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:38:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f143c775bd94ef9de49da05aab2353301bc02ceb74a237332f8d9b23e193234b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9067169d42bea9851adf89b67776e5a280513855fb73120a8d2c5f0051a1097b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 7.3 KB (7292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe10232ba40d32a7b84a0fe16aa0a2b418d2bdf093335c9fbaf56b08e751c54e`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 221.2 KB (221238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c7d84f077aa3ad717767ac56d4b1ea509bc7a9c81e57e3f4e210fe09205ee9`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c90dd2a4fa5a2acd662ddc7f2ec01550257e4bbaae18ab7a94fdd288523cf8`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:3852ee4130c6bfe6eb29489ab1f82c2aceed2d65ba3a11477360199bd6ba4bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2817762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d772c7d45678813ce17e2e65d11aa3e23e0517de39acbfe03eaaadf3558b6f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 04:23:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 04:23:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 04:23:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 04:24:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 04:24:08 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 04:24:08 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 04:24:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 04:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 04:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a66831aa123cebdb722d7d1efb39f1ffb26129fdf9b8937935375852a206`  
		Last Modified: Sat, 28 Aug 2021 04:24:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b103bd0361f6fb48151c8780e205c3fde97140b66762b27effcf2c3b73c05c`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 7.3 KB (7283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce02139d2773db6b3c7033d9dbc6fdb427c918a69c29b8bb01669296d18c9fe`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 205.3 KB (205277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c3cb214e79007442b4d21bc48516c0ef35753d8db03a0cc129fa63d01bedde`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29859d07f0b507288c642deae1bae6cbe9d019152647a0c4e76bd86474fda106`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:37e3f53dd3891f6249a391008eaad0cd841f419981020db94f7728f90513d12f
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

### `spiped:1.6.1` - linux; amd64

```console
$ docker pull spiped@sha256:1494dd15abab70ff861f11b7aadcfb1913d7ad7e0c95fd9fa866fd8a997faae6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37332544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fe7196e9627619f9949f053a86afbc40496ceea34000b3b4ebaf24419e51df4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 22:24:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 22:24:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 22:24:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 22:25:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 22:25:00 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 22:25:01 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 22:25:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 22:25:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:25:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c16f44407339913efe8feb7893634dfbd49fdb363f86acc003a5264fd624a`  
		Last Modified: Tue, 28 Sep 2021 22:25:22 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c6c38eeca4ff05d1e9ec76ba7d4487d0301289ccb5e1887cc097cb52812f0`  
		Last Modified: Tue, 28 Sep 2021 22:25:21 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d3ddbaa314fafbcacbfc77277508c88563cf86d10c7ef081d1c2192c94fe62`  
		Last Modified: Tue, 28 Sep 2021 22:25:23 GMT  
		Size: 6.0 MB (5960379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70bf92a5d2ba79534d0d2f8bddde011587181eddf3b8f0d4a195d014da730fb`  
		Last Modified: Tue, 28 Sep 2021 22:25:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef36802cb5494594cbe25bf22ec477072dfe41486e99081666044bdd6d25fd3`  
		Last Modified: Tue, 28 Sep 2021 22:25:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:8436dc3d0b9307c6728fddf500bbfc53e22883abd81495bef1dbd786b56533a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33939113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6464f913e7d0a0d02b9c987ff12c419ca24b2f6a2b1c36ca7a5ec61982e60e32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:38 GMT
ADD file:da0067258fc1c6a50273e6b3b2673e88fad974a5a1fe4d5eecfeca2df1ff54b3 in / 
# Tue, 28 Sep 2021 01:50:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 19:39:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 19:39:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 19:39:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 19:40:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 19:40:18 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 19:40:18 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 19:40:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 19:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 19:40:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86f2b8be18fc44e8eb430e2c472979a79cda6eb6fa3add10cc8c5d8764eb90ac`  
		Last Modified: Tue, 28 Sep 2021 02:06:35 GMT  
		Size: 28.9 MB (28910670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3d70c7ae48d1f12dbe64e009353b0f4ae5906751228150eea7d8fa1071740f`  
		Last Modified: Tue, 28 Sep 2021 19:40:57 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e560d9a265326647c6bf0ec61bd636c1fc32bb12a184dd1754edbf4b4ac050`  
		Last Modified: Tue, 28 Sep 2021 19:40:57 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25dd92193301a114db15601dbcf4a5954c8d0de076495781fd6c9adaca0080f`  
		Last Modified: Tue, 28 Sep 2021 19:41:01 GMT  
		Size: 5.0 MB (5025194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f46212d749999bf7419078fc626db777dc61f530dc11ea65f671f6b0dfbbe9f`  
		Last Modified: Tue, 28 Sep 2021 19:40:56 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fb1ae610eeb08a59770348cf7cf160343c05595fbf209e65f24f2b989ec1ea`  
		Last Modified: Tue, 28 Sep 2021 19:40:56 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:958d2e76bb92a4709c36123b6553d179419227b06b733ec19cf1a4899da20853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31309843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0880cb9c6c234ff2fe6a3c163710a28845c22e1207ecd0b31cd8887cb77d26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:43:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 03:43:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:43:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 03:44:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 03:44:37 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 03:44:38 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 03:44:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:44:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 03:44:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ecc7e48d063e5bf0a086847e03c73699a183e8a9129e1b8ee3cab1482dde2d`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584009012f86b47c7e4e6d1fd99c2d00976e77d0c5c66f0179ed3c7ea7c54725`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae397080ab7f297afe0c2760bc744f5c6ab5ff8f88b8e0830bc8ae8d97b565f`  
		Last Modified: Tue, 12 Oct 2021 03:45:44 GMT  
		Size: 4.7 MB (4745527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c697bb38b9e3862762d00df70d8a431fd891e25b33a03308c9e1cf59a02c712`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c305948d80dae9d7e0b495eba60d890696dba8079d33af0619bb473c03c079`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b84b5dfa3a45a4a3247d03ea8e53134778a370366d4967ca1648de394559ff0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35323470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fbc4195f2bf091db9b87db926b163df95846c96bc02823cf4035017216ea876`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:43 GMT
ADD file:6472ab63529e688735f77634402740e08fdbd5bfa788c150915027993df7e8ec in / 
# Tue, 28 Sep 2021 01:40:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:51:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 15:51:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:51:46 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 15:52:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 15:52:08 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 15:52:08 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 15:52:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:52:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 15:52:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2f8871a8654eb1158cb626f8dc69992dba7e4bd8796fae6aa7cf967f951f5fe9`  
		Last Modified: Tue, 28 Sep 2021 01:48:25 GMT  
		Size: 30.1 MB (30055408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0bac6bf3efd88e9704f2f7b6a2c409b1df5ed4d12bf39715b3a2e61907fb1`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4facf47a49fb1694033154000aac13d2c30aafbf19e2c674bb4b27df60af7e2a`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8071a27573edf8bf22065560ce728d2de0654433685de5e18c1d26c7e8d1b66`  
		Last Modified: Tue, 28 Sep 2021 15:52:42 GMT  
		Size: 5.3 MB (5264803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeea85f6d4b4c5f24b4c9a75aface87afc9ef6b3c57fc95bc4c614dd809768`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309d496f924a836fede76deb85d262cb73b2ad70167020cab673d985568e24a9`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:af2b655879555e25f940b5bc902cb8ab828971b47b2238d6321f8df278c9137a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40267457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b96d038ad9160f431be6656aade8a3d2894947eadca6167bf2e19a3053fb6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:08 GMT
ADD file:8466bd8df052ea7fa26e49575ac95fd4934ddafdad54a9736ac2bd8e7fc6e735 in / 
# Tue, 28 Sep 2021 01:40:08 GMT
CMD ["bash"]
# Wed, 29 Sep 2021 01:05:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 29 Sep 2021 01:05:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 01:05:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 29 Sep 2021 01:06:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 29 Sep 2021 01:06:24 GMT
VOLUME [/spiped]
# Wed, 29 Sep 2021 01:06:24 GMT
WORKDIR /spiped
# Wed, 29 Sep 2021 01:06:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 29 Sep 2021 01:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 01:06:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e79fce1f6442094a82dc5f6b4d1aa352e04aae39bba821c9021f6da08b1cacaf`  
		Last Modified: Tue, 28 Sep 2021 01:49:07 GMT  
		Size: 32.4 MB (32380160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ea16e10fc5a5a0c4d62cf75b45ed7ad926cec71dc07cd1e46bfcec64a34e09`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7e9cd8372b882a460f62793c1c0d821b3a2d51e3777788be1dfef41055e4d3`  
		Last Modified: Wed, 29 Sep 2021 01:07:17 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200cd2275f388ecc2501c7ab0be9e5795e5aca50325dd9fcf253f1069890417a`  
		Last Modified: Wed, 29 Sep 2021 01:07:20 GMT  
		Size: 7.9 MB (7884038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a169c2e014ded4f64624fb6773ef8fb0c5f3e524fbe12a7f545b861f2bcf54ec`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c16912aa5431d3f809850fa2f91c9d56ea38463628134f5b3b55935f54f5dc`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:028091d21c83e82c61f42923008ed53b9b6e9b130901b2b130429ae0ff355b70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e3374098957b2318d62eead2991c25245a9a698f601f8546440c6c6e83fa9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 02:10:40 GMT
ADD file:43593ef3d79c9b74a92e318d44aacb578f6f8d835dd72665e057bbfe73df1a93 in / 
# Tue, 28 Sep 2021 02:10:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 02:48:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 02:50:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 02:50:03 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 02:50:03 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 02:50:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:50:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f46ea49e27fccc580c8910db39ba7f51ae208a8d24d46a33140afa92ea3d955`  
		Last Modified: Tue, 28 Sep 2021 02:20:45 GMT  
		Size: 29.6 MB (29627871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa45c48be690dce117b2c0dce958f833f4ce085161cd4c6c5b633016534a89ea`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcf26a9aa3a964a21c42b56fd150ed69b7acd005c6629fb4623f95398a88425`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa171fdf362c6c554abf987cede2b8b25abb86afcde7578fea5c091f2cc1197d`  
		Last Modified: Tue, 28 Sep 2021 02:50:31 GMT  
		Size: 5.7 MB (5706116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e04cfec760a4c1a4925c2e96350ddc653e81d2bf92b7ffb7b9239f64aaae387`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b355a5bc54137c27f6b9f4b8e9e3caef346c4d0c43bf9d7496bfa69f266085e`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:b854abceecf263ecd3af9062c9bddf00c657ddc847f0a7beffa3d324806c6bfc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41277029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9de0b22b9d88c7e7b941d2522f2954d1ff0b9cdfde5162978baa1f74ddd6d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Oct 2021 17:55:01 GMT
ADD file:f4b696a766a0d9a808c171a1d5db4f0877b0a784649d63bf461dfcf54b532239 in / 
# Mon, 04 Oct 2021 17:55:06 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 04:33:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 06 Oct 2021 04:33:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 04:33:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 06 Oct 2021 04:35:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 06 Oct 2021 04:35:21 GMT
VOLUME [/spiped]
# Wed, 06 Oct 2021 04:35:23 GMT
WORKDIR /spiped
# Wed, 06 Oct 2021 04:35:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 06 Oct 2021 04:35:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Oct 2021 04:35:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c3b7af0ed242d09d9fee2dfc48d4553d58ad90c5fb862ab58fb89e2d04c5b922`  
		Last Modified: Mon, 04 Oct 2021 18:07:32 GMT  
		Size: 35.3 MB (35272408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61743fc20904f8539cf80302250d866a1c6417663826735c20362034cef7501a`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da94c352893f839938e7606a77c9b6a0c747558c66e01483dd5ef4a69a07383`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534d0224ab6f6639dbd9d41948087e426816f7e37e5940c041d0b712088c87b3`  
		Last Modified: Wed, 06 Oct 2021 04:36:08 GMT  
		Size: 6.0 MB (6001359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eb63df061584de7f6a9d4c754a21f5a3426f46c6704a41d99439d92f398a56`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8bfc7f69743b3fb3ffefa3ccfdcbc84807fe7c346480cc8313ee1af72d33c`  
		Last Modified: Wed, 06 Oct 2021 04:36:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:a81d059af60f158dfb49e3e03962db08aa2b6e40cbd80347d509d2026369a479
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db5d72188d3d25ba7347f1a8ea21b01cf4a27445b632afe2b83bdd2f0f06c798`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:57 GMT
ADD file:2daa8824c30440336bc6ea1448af03234d491ad7c0d0cac917cae5eb54c315fc in / 
# Tue, 28 Sep 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:55:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 09:55:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:55:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 09:55:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 09:55:36 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 09:55:36 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 09:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 09:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 09:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e8e2938f4df931c46d7575f0b7bad5bc357277fc3e132b720e704ac7a4d1c9ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:01 GMT  
		Size: 29.7 MB (29650795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f460f8990cce2d9f2e25c13b42c5513a2129ef1a318b1097f6ff1186a5fbef71`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e214e0743e5982442db728a32fd9951aa1a7e6d14317d4cec1824fa8eeca957a`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4f812c2b3b5fbebd9e26191ed62c7eac5f1012927dfb8571c9f99a57d3db8`  
		Last Modified: Tue, 28 Sep 2021 09:56:09 GMT  
		Size: 5.2 MB (5183853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972d8d742129ea070e9be63d7a5e8bc2840090dfe9ed23aa907c2508a1e9c3c9`  
		Last Modified: Tue, 28 Sep 2021 09:56:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216f4500775537761e72820f3bb08e33e37ebf36fb33e73f0dca40bb88e2bf48`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:89f362dd004a510b0e2dfdfdf849444c25d6fb0c60e3b7df331ece34ce763a31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:44015ddc42ceef8878c9b2bad7a6bcbf2b5d2ca42ab52cca20f9f66b2c15ffd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65d8337530e6b8e116202287d477945c4375886702df4698f8740106658a777`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:56:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:56:13 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:56:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:56:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:56:31 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:56:31 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:56:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:56:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:56:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72fe484884c949a7fba8b7d917cbe40b9fa50036f4c10e4b82e3075576fe3fc`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06083e8d35a44724cf84de43d971fb5b141e8ce6468a5c267c43c96f79869f23`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037fda176acae1eef93fa1dde784253576faf4d880c75c8d7df76fdf212dda`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 212.5 KB (212547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb3cd7f024c8cfa70e1c8e8f282e44395bbaa20cd69851af0552d8041deaea2`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fccea2af66d4ffdbdd93edf485c1e6e17f14ac10329842af6fea7741bd3504`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:7e548b9910cf9bcbce660ff537e09660dbd9d84cbc06621e45fb2282f2f52270
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2838978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8539d235dbd2d180f98df622ec1586ed595c7026c53f57b67876cbe0b641be9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:39:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:39:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:39:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:39:57 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:39:58 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:39:58 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:39:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:39:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:40:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ec865614b924d3ebd8faaf1468ff031de3ccb2f178656d907e4a89f8673776`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07908dc20812a0124cb96563b08ff2d4ebd32f0ca0cef02511faa0c127496e96`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 7.3 KB (7290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2ce7f8303145adfe2a17235c758d30fa18338c417eb73738b591c1dd3d1315`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 202.5 KB (202499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07f8ab6ed47190923d1d152d960c5fd80b7d9f27f84a289e8236a1e4f22843c`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17d0a64e682741c70413fc90f0d8a4dac61425dcc5c98ce054909120977e587`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:24d05f05df7127b2aa61654a9d29c77a0c2a00f8ba29dbfc127a672700d5f652
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2635217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c197156cacbfdbdb870ce3391ad1bdf7d6c922d18648489e7549033356f432b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 03:04:23 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 03:04:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 03:04:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 03:04:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 03:04:59 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 03:05:00 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 03:05:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 03:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 03:05:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c187e6961a8f3ae8bf645e1fbec375c4f7c3d8146ab5ee5a09f57cd5615f33cb`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56c389f9017243d26a8fd61b3cc3385e2b4dcf930d608cc682a5ff3b437137`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0da469457d5465481ffd06dc86cd457daaf02e8b501cbee7b9cb52b675525`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 195.8 KB (195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea4333c9f229866ca36ab2d7e036e1d23031e78c62c3ad0bcbbeacaaf8f8e65`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4907440a689992d3e1fbcc2fcef650c5ef7b7abe5b8b3aa9c97d6d697d5050fd`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:026d11edbbedc8b8a63207a745859b0ada912c11cbd6bf77d2eb162cfb1a6577
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7dbad85a08f79ca7ef7c449feb1dfbd6973498a21db9a0721af19e181fc39f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 01:45:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 01:45:36 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 01:45:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 01:45:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 01:45:53 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 01:45:53 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 01:45:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 01:45:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130a79b60aae9998377169e6355792370bb064e6148684353d6ed4826039492f`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43519aa40fdf82f3b05cab9731634890c7e8dc8b9731ce4c7c3fbbc35def0274`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 7.3 KB (7299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a1b5762b7444935215ce9e31bc9a68cac110a8b0bf2f9ca433a2d78620fe35`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 204.6 KB (204622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f156837dee9efeb5125ef7fc8d079ccf996015838cfe028bfb81695eb1230b99`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f221da4d2654d1b1432ad3c77afeed7392661b44c6a50fc1fd5e2cede5dfcb`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:da842be683e4aa6e7f0e6581d7d9bd1604d2d140a1b452e47a1ca595261af814
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3055327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7b5670b88fbd238447f1f65531173381d0aff05ec6d63ef2df4dfb7b8c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:35:24 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:35:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:35:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:35:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:35:45 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:35:45 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:35:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:35:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:35:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95070702ac27305ca355fc2880dec01d9e18d3c8a4a22842a599db59ea5467e0`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35be501885b2efd06479a1d05af31f0d06d6b0a5c4dfb3f760af81657d7919ea`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 7.3 KB (7287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f5e404d9d5a395b15445e0403dfa9a598ab9ecd02814798d33098ac6a8ba9c`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 223.4 KB (223445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b8287cb974321164bff4ca80e9a231471fecf0bbab1bbf130172709ae47ae`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c88353a13d0403b037e398aa01ea54701b91f2adf180d6ed9df1b155b62c89`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:3c83af52715b14ccfd27cc89b7b988ae73b9d05500efd053b99b027c0328f14d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f59b6df7881927f19f4b2dcab5974d93c4284e7e9ba9c21098a82d888389b26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:36:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 27 Aug 2021 21:36:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 27 Aug 2021 21:37:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 27 Aug 2021 21:37:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 27 Aug 2021 21:37:41 GMT
VOLUME [/spiped]
# Fri, 27 Aug 2021 21:37:48 GMT
WORKDIR /spiped
# Fri, 27 Aug 2021 21:37:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:38:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f143c775bd94ef9de49da05aab2353301bc02ceb74a237332f8d9b23e193234b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9067169d42bea9851adf89b67776e5a280513855fb73120a8d2c5f0051a1097b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 7.3 KB (7292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe10232ba40d32a7b84a0fe16aa0a2b418d2bdf093335c9fbaf56b08e751c54e`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 221.2 KB (221238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c7d84f077aa3ad717767ac56d4b1ea509bc7a9c81e57e3f4e210fe09205ee9`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c90dd2a4fa5a2acd662ddc7f2ec01550257e4bbaae18ab7a94fdd288523cf8`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:3852ee4130c6bfe6eb29489ab1f82c2aceed2d65ba3a11477360199bd6ba4bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2817762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d772c7d45678813ce17e2e65d11aa3e23e0517de39acbfe03eaaadf3558b6f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 04:23:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 04:23:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 04:23:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 04:24:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 04:24:08 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 04:24:08 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 04:24:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 04:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 04:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a66831aa123cebdb722d7d1efb39f1ffb26129fdf9b8937935375852a206`  
		Last Modified: Sat, 28 Aug 2021 04:24:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b103bd0361f6fb48151c8780e205c3fde97140b66762b27effcf2c3b73c05c`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 7.3 KB (7283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce02139d2773db6b3c7033d9dbc6fdb427c918a69c29b8bb01669296d18c9fe`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 205.3 KB (205277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c3cb214e79007442b4d21bc48516c0ef35753d8db03a0cc129fa63d01bedde`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29859d07f0b507288c642deae1bae6cbe9d019152647a0c4e76bd86474fda106`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:89f362dd004a510b0e2dfdfdf849444c25d6fb0c60e3b7df331ece34ce763a31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:44015ddc42ceef8878c9b2bad7a6bcbf2b5d2ca42ab52cca20f9f66b2c15ffd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65d8337530e6b8e116202287d477945c4375886702df4698f8740106658a777`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:56:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:56:13 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:56:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:56:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:56:31 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:56:31 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:56:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:56:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:56:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72fe484884c949a7fba8b7d917cbe40b9fa50036f4c10e4b82e3075576fe3fc`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06083e8d35a44724cf84de43d971fb5b141e8ce6468a5c267c43c96f79869f23`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037fda176acae1eef93fa1dde784253576faf4d880c75c8d7df76fdf212dda`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 212.5 KB (212547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb3cd7f024c8cfa70e1c8e8f282e44395bbaa20cd69851af0552d8041deaea2`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fccea2af66d4ffdbdd93edf485c1e6e17f14ac10329842af6fea7741bd3504`  
		Last Modified: Sat, 28 Aug 2021 00:56:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:7e548b9910cf9bcbce660ff537e09660dbd9d84cbc06621e45fb2282f2f52270
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2838978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8539d235dbd2d180f98df622ec1586ed595c7026c53f57b67876cbe0b641be9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:39:21 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:39:23 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:39:23 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:39:57 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:39:58 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:39:58 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:39:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:39:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:40:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ec865614b924d3ebd8faaf1468ff031de3ccb2f178656d907e4a89f8673776`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07908dc20812a0124cb96563b08ff2d4ebd32f0ca0cef02511faa0c127496e96`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 7.3 KB (7290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2ce7f8303145adfe2a17235c758d30fa18338c417eb73738b591c1dd3d1315`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 202.5 KB (202499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07f8ab6ed47190923d1d152d960c5fd80b7d9f27f84a289e8236a1e4f22843c`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17d0a64e682741c70413fc90f0d8a4dac61425dcc5c98ce054909120977e587`  
		Last Modified: Sat, 28 Aug 2021 00:40:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:24d05f05df7127b2aa61654a9d29c77a0c2a00f8ba29dbfc127a672700d5f652
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2635217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c197156cacbfdbdb870ce3391ad1bdf7d6c922d18648489e7549033356f432b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 03:04:23 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 03:04:26 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 03:04:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 03:04:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 03:04:59 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 03:05:00 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 03:05:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 03:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 03:05:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c187e6961a8f3ae8bf645e1fbec375c4f7c3d8146ab5ee5a09f57cd5615f33cb`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56c389f9017243d26a8fd61b3cc3385e2b4dcf930d608cc682a5ff3b437137`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 7.3 KB (7298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b0da469457d5465481ffd06dc86cd457daaf02e8b501cbee7b9cb52b675525`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 195.8 KB (195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea4333c9f229866ca36ab2d7e036e1d23031e78c62c3ad0bcbbeacaaf8f8e65`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4907440a689992d3e1fbcc2fcef650c5ef7b7abe5b8b3aa9c97d6d697d5050fd`  
		Last Modified: Sat, 28 Aug 2021 03:05:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:026d11edbbedc8b8a63207a745859b0ada912c11cbd6bf77d2eb162cfb1a6577
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7dbad85a08f79ca7ef7c449feb1dfbd6973498a21db9a0721af19e181fc39f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 01:45:35 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 01:45:36 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 01:45:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 01:45:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 01:45:53 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 01:45:53 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 01:45:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 01:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 01:45:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130a79b60aae9998377169e6355792370bb064e6148684353d6ed4826039492f`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43519aa40fdf82f3b05cab9731634890c7e8dc8b9731ce4c7c3fbbc35def0274`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 7.3 KB (7299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a1b5762b7444935215ce9e31bc9a68cac110a8b0bf2f9ca433a2d78620fe35`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 204.6 KB (204622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f156837dee9efeb5125ef7fc8d079ccf996015838cfe028bfb81695eb1230b99`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f221da4d2654d1b1432ad3c77afeed7392661b44c6a50fc1fd5e2cede5dfcb`  
		Last Modified: Sat, 28 Aug 2021 01:46:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:da842be683e4aa6e7f0e6581d7d9bd1604d2d140a1b452e47a1ca595261af814
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3055327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a7b5670b88fbd238447f1f65531173381d0aff05ec6d63ef2df4dfb7b8c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:35:24 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 00:35:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 00:35:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 00:35:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 00:35:45 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 00:35:45 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 00:35:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 00:35:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 00:35:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95070702ac27305ca355fc2880dec01d9e18d3c8a4a22842a599db59ea5467e0`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35be501885b2efd06479a1d05af31f0d06d6b0a5c4dfb3f760af81657d7919ea`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 7.3 KB (7287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f5e404d9d5a395b15445e0403dfa9a598ab9ecd02814798d33098ac6a8ba9c`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 223.4 KB (223445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233b8287cb974321164bff4ca80e9a231471fecf0bbab1bbf130172709ae47ae`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c88353a13d0403b037e398aa01ea54701b91f2adf180d6ed9df1b155b62c89`  
		Last Modified: Sat, 28 Aug 2021 00:36:17 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:3c83af52715b14ccfd27cc89b7b988ae73b9d05500efd053b99b027c0328f14d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f59b6df7881927f19f4b2dcab5974d93c4284e7e9ba9c21098a82d888389b26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:36:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 27 Aug 2021 21:36:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 27 Aug 2021 21:37:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 27 Aug 2021 21:37:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 27 Aug 2021 21:37:41 GMT
VOLUME [/spiped]
# Fri, 27 Aug 2021 21:37:48 GMT
WORKDIR /spiped
# Fri, 27 Aug 2021 21:37:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:38:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f143c775bd94ef9de49da05aab2353301bc02ceb74a237332f8d9b23e193234b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9067169d42bea9851adf89b67776e5a280513855fb73120a8d2c5f0051a1097b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 7.3 KB (7292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe10232ba40d32a7b84a0fe16aa0a2b418d2bdf093335c9fbaf56b08e751c54e`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 221.2 KB (221238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c7d84f077aa3ad717767ac56d4b1ea509bc7a9c81e57e3f4e210fe09205ee9`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c90dd2a4fa5a2acd662ddc7f2ec01550257e4bbaae18ab7a94fdd288523cf8`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:3852ee4130c6bfe6eb29489ab1f82c2aceed2d65ba3a11477360199bd6ba4bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2817762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d772c7d45678813ce17e2e65d11aa3e23e0517de39acbfe03eaaadf3558b6f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 04:23:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 28 Aug 2021 04:23:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 28 Aug 2021 04:23:50 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 28 Aug 2021 04:24:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 28 Aug 2021 04:24:08 GMT
VOLUME [/spiped]
# Sat, 28 Aug 2021 04:24:08 GMT
WORKDIR /spiped
# Sat, 28 Aug 2021 04:24:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 Aug 2021 04:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Aug 2021 04:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447a66831aa123cebdb722d7d1efb39f1ffb26129fdf9b8937935375852a206`  
		Last Modified: Sat, 28 Aug 2021 04:24:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b103bd0361f6fb48151c8780e205c3fde97140b66762b27effcf2c3b73c05c`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 7.3 KB (7283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce02139d2773db6b3c7033d9dbc6fdb427c918a69c29b8bb01669296d18c9fe`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 205.3 KB (205277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c3cb214e79007442b4d21bc48516c0ef35753d8db03a0cc129fa63d01bedde`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29859d07f0b507288c642deae1bae6cbe9d019152647a0c4e76bd86474fda106`  
		Last Modified: Sat, 28 Aug 2021 04:24:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:37e3f53dd3891f6249a391008eaad0cd841f419981020db94f7728f90513d12f
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
$ docker pull spiped@sha256:1494dd15abab70ff861f11b7aadcfb1913d7ad7e0c95fd9fa866fd8a997faae6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37332544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fe7196e9627619f9949f053a86afbc40496ceea34000b3b4ebaf24419e51df4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 22:24:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 22:24:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 22:24:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 22:25:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 22:25:00 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 22:25:01 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 22:25:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 22:25:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:25:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c16f44407339913efe8feb7893634dfbd49fdb363f86acc003a5264fd624a`  
		Last Modified: Tue, 28 Sep 2021 22:25:22 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c6c38eeca4ff05d1e9ec76ba7d4487d0301289ccb5e1887cc097cb52812f0`  
		Last Modified: Tue, 28 Sep 2021 22:25:21 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d3ddbaa314fafbcacbfc77277508c88563cf86d10c7ef081d1c2192c94fe62`  
		Last Modified: Tue, 28 Sep 2021 22:25:23 GMT  
		Size: 6.0 MB (5960379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70bf92a5d2ba79534d0d2f8bddde011587181eddf3b8f0d4a195d014da730fb`  
		Last Modified: Tue, 28 Sep 2021 22:25:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef36802cb5494594cbe25bf22ec477072dfe41486e99081666044bdd6d25fd3`  
		Last Modified: Tue, 28 Sep 2021 22:25:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:8436dc3d0b9307c6728fddf500bbfc53e22883abd81495bef1dbd786b56533a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33939113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6464f913e7d0a0d02b9c987ff12c419ca24b2f6a2b1c36ca7a5ec61982e60e32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:38 GMT
ADD file:da0067258fc1c6a50273e6b3b2673e88fad974a5a1fe4d5eecfeca2df1ff54b3 in / 
# Tue, 28 Sep 2021 01:50:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 19:39:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 19:39:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 19:39:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 19:40:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 19:40:18 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 19:40:18 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 19:40:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 19:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 19:40:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86f2b8be18fc44e8eb430e2c472979a79cda6eb6fa3add10cc8c5d8764eb90ac`  
		Last Modified: Tue, 28 Sep 2021 02:06:35 GMT  
		Size: 28.9 MB (28910670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3d70c7ae48d1f12dbe64e009353b0f4ae5906751228150eea7d8fa1071740f`  
		Last Modified: Tue, 28 Sep 2021 19:40:57 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e560d9a265326647c6bf0ec61bd636c1fc32bb12a184dd1754edbf4b4ac050`  
		Last Modified: Tue, 28 Sep 2021 19:40:57 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25dd92193301a114db15601dbcf4a5954c8d0de076495781fd6c9adaca0080f`  
		Last Modified: Tue, 28 Sep 2021 19:41:01 GMT  
		Size: 5.0 MB (5025194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f46212d749999bf7419078fc626db777dc61f530dc11ea65f671f6b0dfbbe9f`  
		Last Modified: Tue, 28 Sep 2021 19:40:56 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fb1ae610eeb08a59770348cf7cf160343c05595fbf209e65f24f2b989ec1ea`  
		Last Modified: Tue, 28 Sep 2021 19:40:56 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:958d2e76bb92a4709c36123b6553d179419227b06b733ec19cf1a4899da20853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31309843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0880cb9c6c234ff2fe6a3c163710a28845c22e1207ecd0b31cd8887cb77d26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:43:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 03:43:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:43:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 03:44:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 03:44:37 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 03:44:38 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 03:44:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:44:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 03:44:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ecc7e48d063e5bf0a086847e03c73699a183e8a9129e1b8ee3cab1482dde2d`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584009012f86b47c7e4e6d1fd99c2d00976e77d0c5c66f0179ed3c7ea7c54725`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae397080ab7f297afe0c2760bc744f5c6ab5ff8f88b8e0830bc8ae8d97b565f`  
		Last Modified: Tue, 12 Oct 2021 03:45:44 GMT  
		Size: 4.7 MB (4745527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c697bb38b9e3862762d00df70d8a431fd891e25b33a03308c9e1cf59a02c712`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c305948d80dae9d7e0b495eba60d890696dba8079d33af0619bb473c03c079`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b84b5dfa3a45a4a3247d03ea8e53134778a370366d4967ca1648de394559ff0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35323470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fbc4195f2bf091db9b87db926b163df95846c96bc02823cf4035017216ea876`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:43 GMT
ADD file:6472ab63529e688735f77634402740e08fdbd5bfa788c150915027993df7e8ec in / 
# Tue, 28 Sep 2021 01:40:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:51:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 15:51:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:51:46 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 15:52:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 15:52:08 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 15:52:08 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 15:52:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 15:52:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 15:52:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2f8871a8654eb1158cb626f8dc69992dba7e4bd8796fae6aa7cf967f951f5fe9`  
		Last Modified: Tue, 28 Sep 2021 01:48:25 GMT  
		Size: 30.1 MB (30055408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0bac6bf3efd88e9704f2f7b6a2c409b1df5ed4d12bf39715b3a2e61907fb1`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4facf47a49fb1694033154000aac13d2c30aafbf19e2c674bb4b27df60af7e2a`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8071a27573edf8bf22065560ce728d2de0654433685de5e18c1d26c7e8d1b66`  
		Last Modified: Tue, 28 Sep 2021 15:52:42 GMT  
		Size: 5.3 MB (5264803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeea85f6d4b4c5f24b4c9a75aface87afc9ef6b3c57fc95bc4c614dd809768`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309d496f924a836fede76deb85d262cb73b2ad70167020cab673d985568e24a9`  
		Last Modified: Tue, 28 Sep 2021 15:52:41 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:af2b655879555e25f940b5bc902cb8ab828971b47b2238d6321f8df278c9137a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40267457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b96d038ad9160f431be6656aade8a3d2894947eadca6167bf2e19a3053fb6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:08 GMT
ADD file:8466bd8df052ea7fa26e49575ac95fd4934ddafdad54a9736ac2bd8e7fc6e735 in / 
# Tue, 28 Sep 2021 01:40:08 GMT
CMD ["bash"]
# Wed, 29 Sep 2021 01:05:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 29 Sep 2021 01:05:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 01:05:25 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 29 Sep 2021 01:06:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 29 Sep 2021 01:06:24 GMT
VOLUME [/spiped]
# Wed, 29 Sep 2021 01:06:24 GMT
WORKDIR /spiped
# Wed, 29 Sep 2021 01:06:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 29 Sep 2021 01:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 01:06:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e79fce1f6442094a82dc5f6b4d1aa352e04aae39bba821c9021f6da08b1cacaf`  
		Last Modified: Tue, 28 Sep 2021 01:49:07 GMT  
		Size: 32.4 MB (32380160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ea16e10fc5a5a0c4d62cf75b45ed7ad926cec71dc07cd1e46bfcec64a34e09`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7e9cd8372b882a460f62793c1c0d821b3a2d51e3777788be1dfef41055e4d3`  
		Last Modified: Wed, 29 Sep 2021 01:07:17 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200cd2275f388ecc2501c7ab0be9e5795e5aca50325dd9fcf253f1069890417a`  
		Last Modified: Wed, 29 Sep 2021 01:07:20 GMT  
		Size: 7.9 MB (7884038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a169c2e014ded4f64624fb6773ef8fb0c5f3e524fbe12a7f545b861f2bcf54ec`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c16912aa5431d3f809850fa2f91c9d56ea38463628134f5b3b55935f54f5dc`  
		Last Modified: Wed, 29 Sep 2021 01:07:16 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:028091d21c83e82c61f42923008ed53b9b6e9b130901b2b130429ae0ff355b70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e3374098957b2318d62eead2991c25245a9a698f601f8546440c6c6e83fa9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 02:10:40 GMT
ADD file:43593ef3d79c9b74a92e318d44aacb578f6f8d835dd72665e057bbfe73df1a93 in / 
# Tue, 28 Sep 2021 02:10:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:48:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 02:48:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:48:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 02:50:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 02:50:03 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 02:50:03 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 02:50:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 02:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 02:50:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f46ea49e27fccc580c8910db39ba7f51ae208a8d24d46a33140afa92ea3d955`  
		Last Modified: Tue, 28 Sep 2021 02:20:45 GMT  
		Size: 29.6 MB (29627871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa45c48be690dce117b2c0dce958f833f4ce085161cd4c6c5b633016534a89ea`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcf26a9aa3a964a21c42b56fd150ed69b7acd005c6629fb4623f95398a88425`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa171fdf362c6c554abf987cede2b8b25abb86afcde7578fea5c091f2cc1197d`  
		Last Modified: Tue, 28 Sep 2021 02:50:31 GMT  
		Size: 5.7 MB (5706116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e04cfec760a4c1a4925c2e96350ddc653e81d2bf92b7ffb7b9239f64aaae387`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b355a5bc54137c27f6b9f4b8e9e3caef346c4d0c43bf9d7496bfa69f266085e`  
		Last Modified: Tue, 28 Sep 2021 02:50:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:b854abceecf263ecd3af9062c9bddf00c657ddc847f0a7beffa3d324806c6bfc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41277029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9de0b22b9d88c7e7b941d2522f2954d1ff0b9cdfde5162978baa1f74ddd6d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Oct 2021 17:55:01 GMT
ADD file:f4b696a766a0d9a808c171a1d5db4f0877b0a784649d63bf461dfcf54b532239 in / 
# Mon, 04 Oct 2021 17:55:06 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 04:33:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 06 Oct 2021 04:33:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 04:33:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 06 Oct 2021 04:35:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 06 Oct 2021 04:35:21 GMT
VOLUME [/spiped]
# Wed, 06 Oct 2021 04:35:23 GMT
WORKDIR /spiped
# Wed, 06 Oct 2021 04:35:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 06 Oct 2021 04:35:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Oct 2021 04:35:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c3b7af0ed242d09d9fee2dfc48d4553d58ad90c5fb862ab58fb89e2d04c5b922`  
		Last Modified: Mon, 04 Oct 2021 18:07:32 GMT  
		Size: 35.3 MB (35272408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61743fc20904f8539cf80302250d866a1c6417663826735c20362034cef7501a`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da94c352893f839938e7606a77c9b6a0c747558c66e01483dd5ef4a69a07383`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534d0224ab6f6639dbd9d41948087e426816f7e37e5940c041d0b712088c87b3`  
		Last Modified: Wed, 06 Oct 2021 04:36:08 GMT  
		Size: 6.0 MB (6001359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eb63df061584de7f6a9d4c754a21f5a3426f46c6704a41d99439d92f398a56`  
		Last Modified: Wed, 06 Oct 2021 04:36:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8bfc7f69743b3fb3ffefa3ccfdcbc84807fe7c346480cc8313ee1af72d33c`  
		Last Modified: Wed, 06 Oct 2021 04:36:07 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:a81d059af60f158dfb49e3e03962db08aa2b6e40cbd80347d509d2026369a479
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db5d72188d3d25ba7347f1a8ea21b01cf4a27445b632afe2b83bdd2f0f06c798`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:57 GMT
ADD file:2daa8824c30440336bc6ea1448af03234d491ad7c0d0cac917cae5eb54c315fc in / 
# Tue, 28 Sep 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:55:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 28 Sep 2021 09:55:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:55:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 28 Sep 2021 09:55:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 28 Sep 2021 09:55:36 GMT
VOLUME [/spiped]
# Tue, 28 Sep 2021 09:55:36 GMT
WORKDIR /spiped
# Tue, 28 Sep 2021 09:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 28 Sep 2021 09:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 09:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e8e2938f4df931c46d7575f0b7bad5bc357277fc3e132b720e704ac7a4d1c9ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:01 GMT  
		Size: 29.7 MB (29650795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f460f8990cce2d9f2e25c13b42c5513a2129ef1a318b1097f6ff1186a5fbef71`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e214e0743e5982442db728a32fd9951aa1a7e6d14317d4cec1824fa8eeca957a`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4f812c2b3b5fbebd9e26191ed62c7eac5f1012927dfb8571c9f99a57d3db8`  
		Last Modified: Tue, 28 Sep 2021 09:56:09 GMT  
		Size: 5.2 MB (5183853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972d8d742129ea070e9be63d7a5e8bc2840090dfe9ed23aa907c2508a1e9c3c9`  
		Last Modified: Tue, 28 Sep 2021 09:56:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216f4500775537761e72820f3bb08e33e37ebf36fb33e73f0dca40bb88e2bf48`  
		Last Modified: Tue, 28 Sep 2021 09:56:08 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
