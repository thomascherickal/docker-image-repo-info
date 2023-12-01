<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1.6.2`](#spiped162)
-	[`spiped:1.6.2-alpine`](#spiped162-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:682342279f587fb9710d8ae48633a1f21c9b8b9db46441a369799e8a8034ae12
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
$ docker pull spiped@sha256:fc3b908a26fb9e7a920f3103dd6ab8dd8d4e2ddf9199d6fd3e427d27e1813509
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38217301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59df6dfe09d725bf32ab563c2a0855c886b9a1d5ec6602ae719f009e0f673d9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 19:56:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 19:56:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:56:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 19:57:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 19:57:20 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 19:57:20 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 19:57:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 19:57:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 19:57:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89098fb70aba03de1d0a340fa9730ebf791943e1ddd82b20c54381bad68d1821`  
		Last Modified: Tue, 21 Nov 2023 19:57:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d1d9c52903bd04e0b1aa2d6271b43398bc23d10dffadaef056b4978ea20038`  
		Last Modified: Tue, 21 Nov 2023 19:57:32 GMT  
		Size: 2.6 MB (2591886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450c30ae667851f890ead982bd7dcd85a72bce3e071687a16436543d5a17759f`  
		Last Modified: Tue, 21 Nov 2023 19:57:33 GMT  
		Size: 6.5 MB (6473909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2d81e4e280c8c0c5ea1466e8c68915ab09769685596cea9b0c40c5bae43813`  
		Last Modified: Tue, 21 Nov 2023 19:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3476d0aeb59e34ab31b0327be0940e18de5a1c7b369fd86feb394c3d28c35e`  
		Last Modified: Tue, 21 Nov 2023 19:57:32 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a22fc52e1353a81c0b5e864f000d5b7c6f511f31d25d33161d7fff1fa66a128f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34250716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:805e4bd68f268c5a14b0391f350041c251fc5129caa5978c1f2bd4a998995836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:48:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:48:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:48:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:48:30 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:48:31 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:48:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c4d22227960e496eb464146dc866dad412f31aa91c728607dde4278de637ee`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53633f32e999cc192394918d73de2f3ad375e658d9e7dd207468ea6b664eb6d4`  
		Last Modified: Tue, 21 Nov 2023 05:48:39 GMT  
		Size: 2.2 MB (2186814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82ff098495f0ea42040c5184eb059c29c59d5d6e660aa0b1fbc7fff91b2ad4b`  
		Last Modified: Tue, 21 Nov 2023 05:48:40 GMT  
		Size: 5.1 MB (5140150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f734161b12b1fc00f0c981ce9f8176dacc5ca02b74484b806d289850efaa8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f8f249901f701b78f48d77ef49a7fe721309da08eae74507aec894e5a49af8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d49e38f255892c26d1cde15165c35c32cf857b3446c025ecbd69a009b6d59a12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31677806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97542227ddc0fffbebd6a1fa7da3015089ed0e15aa7d37d4d6c22aa77e4748e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 11:53:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 11:53:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 11:53:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 11:54:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 11:54:13 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 11:54:13 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 11:54:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 11:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 11:54:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac591a8672b5dba3bfcbe0fe6c21f8387ab9a4f56d6ea32f9eebf5e37feca3`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0fa0448ca0214cd73bf754ce7fd1d9686bd3de6b1bf5840a2c8bd3587f1109`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 2.0 MB (2046224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efda8a5518d4c16d427ac57f16268ce4060b4a3d1760ff2cd9b1743185072436`  
		Last Modified: Tue, 21 Nov 2023 11:54:28 GMT  
		Size: 4.9 MB (4881057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37767eb2f6144694ce685d9751a24751196daeb9c3b4a24cda3aa648169b599c`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac67ec8ea82fe47e96246ff7b13f0fbfe7d1fd1f42e5e299ada512bc129fb30`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:57c39c08bbf544370ee603edc8311c0ae6ae5544b2e36b00f992a4c7d61979ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37098308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee328258fcaccf097e36c2041f5623138c3e45fba88ae8fb0a2346b4a7abff8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:36:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 20:36:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 20:36:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 20:36:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 20:36:46 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 20:36:46 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 20:36:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 20:36:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 20:36:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67d14d16729f6a29d5643e5739ce8f277db88c76e8576b74466bed71e9614a3`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667f3b336a76ba92a985040ecc81f1e4b96ab00b9bffb9691d4a0909fee7d70`  
		Last Modified: Tue, 21 Nov 2023 20:36:59 GMT  
		Size: 2.4 MB (2434842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365e0235c5f2467bccbbc07ea82e8e9f2af172d10ad8cb487a501738c975909`  
		Last Modified: Tue, 21 Nov 2023 20:37:00 GMT  
		Size: 5.5 MB (5482590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfecc897f46254770f57aee0cf4c99b9ddfd59416111300bcae84be0bb3661e`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8280277e4e1e138609865f279ff5fef4c40a0bb4f48d2230459299b00d656ad0`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:c2feb65880bc509150accfd419e6813f14627257be2627bbe31de9a5184a5e0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38697733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36feabcb5b8aebe526989cb605bfe36f6ba227f20c4202055c68d66994900b1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Wed, 22 Nov 2023 01:09:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Nov 2023 01:09:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:09:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 22 Nov 2023 01:09:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Nov 2023 01:09:56 GMT
VOLUME [/spiped]
# Wed, 22 Nov 2023 01:09:56 GMT
WORKDIR /spiped
# Wed, 22 Nov 2023 01:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Nov 2023 01:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Nov 2023 01:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d9077e40b47c5791b4ac20b24d8deff63a5dc8bf5207083f56177fda752514`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e71210812cdeec1bdcbcdc0d631c3eadb6ea9c8b9858c611a0182299588731`  
		Last Modified: Wed, 22 Nov 2023 01:10:13 GMT  
		Size: 2.6 MB (2588158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f18e97e0027d314fc775390b955ca68e6a4cc69d6077de1fc07ccefcd18758f`  
		Last Modified: Wed, 22 Nov 2023 01:10:14 GMT  
		Size: 5.9 MB (5943867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48894c0f6daf466b673d54c1f3536c05d1e8de633a2a517c55a0946adfc311ec`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c404496be4d3107996737e0d3b4b2b5766ee34e42c1a7e6961de6efcec4dde`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:0d61d0a1ea5ac2651b170d9096365703860743a0df774ddcdc327b0915c4544f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36783306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287250c56678b233b997a1c6059e730e147815a68e1df4f12eda08a5eed1ebe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:42:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 16:42:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 16:44:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 16:44:19 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 16:44:22 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 16:44:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 16:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ff2608f3497720032e30b79ae5d65cfa2c8dd359565c1c8dd638f5b3a6f0d`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab7308e1ec6dfefbe63dcd0ffdd71389fcdc64536e65a12a0d4e0b039458285`  
		Last Modified: Tue, 21 Nov 2023 16:44:46 GMT  
		Size: 1.8 MB (1834326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bede55fcddef2dca32fd1854933f48d44eb852b04607b5ca0ee5f0ceede864c`  
		Last Modified: Tue, 21 Nov 2023 16:44:49 GMT  
		Size: 5.8 MB (5805479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8ac4180d595ed6276f96e62a762ce81e1cbc8d5adb99021d674d703250377a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6377814988f39cd05c902f86328248c9751a1903ed8401e8827bf7540cc4a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:99a36d31339087c56743fcd7b09255be818296337c1ee9b0b9e5caa4d6d2a629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42336939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbf18f5d582e136651ca47bbf5c8553330ac36b69e4beb1e957d147dbc321fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:49:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 12:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:49:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 12:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:49:48 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 12:49:48 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 12:49:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 12:49:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e3e9a6e83461086d799b3c35e7086e930106125c74069a1510c25bdb6afb6d`  
		Last Modified: Tue, 21 Nov 2023 12:50:01 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956ee3303181032f855a7b2887c1bdca6910e0cb1ec3c92b65d6509c2f907abb`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 2.8 MB (2770520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ddbd7552dcc1e8096f1f690fb7a8f6d94f6b14b70ac7c130e5224ccc99ae5`  
		Last Modified: Tue, 21 Nov 2023 12:50:03 GMT  
		Size: 6.4 MB (6423216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acdb31d4ba61d5a1503eb5bf6cd716ec162f811fe2c79c2ff5c2e727033efc0`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da63bf7cb4ff2b34de84cd9caefa0d255c9965665b50f421172e3d96c2ee315a`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:e55796d4c561e3f8eec223e5e69fb5d024ac8574c4aace38477a60420ff5414c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35164381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ea59dc57dc93fac49f303c8c58d6d153d1c8a8ffab3500ff5649eb63c8b568`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:54:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:54:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:54:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:54:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:54:34 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:54:34 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:54:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:54:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a1488c1c72f51fc67f2f92a4266ad144068e6265f09a6854a0edda69d1e634`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850f941b1cd09719d174b6a90cb013528879a956734598472118c9ba95f4f146`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 2.3 MB (2262458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647d17c59a394362c94984e56f3babc4addd9e026c843bede6b3b295b4b9439c`  
		Last Modified: Tue, 21 Nov 2023 05:54:55 GMT  
		Size: 5.4 MB (5387438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5763b7fbe5d4e9c3ba3f58020db82f8a9bba3e6a9a702f785249dd13161a253b`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d519c5ded3c9d38ab8b28f40d83037fc367671ed767a048f773b935af62381f`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:88dccc72f75f2fc6cc962aaf58d6d7f85f43ef29d88e5eaba0e7d2dbebbc982d
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
$ docker pull spiped@sha256:bbcb559f4d5d2f95adfeef51c918f2c078dcf991b30279a34be08e7614eda451
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5058435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e068a31dc93f7fbe323b521ca3e2dce275263b1eb366f065ef43b018191ac2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:00:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 06:00:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 06:00:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 06:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 06:00:14 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 06:00:14 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 06:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 06:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 06:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc456d15d6c4f02d60102c7538cc196adfd3073fa382d3a6c9410c2acfa02238`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac40e9085148fd6ad0718c4bb551770cb399db60f6d9e0e6ae11e2af695afc`  
		Last Modified: Fri, 01 Dec 2023 06:00:26 GMT  
		Size: 1.4 MB (1433002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b55d95977f08a50d321f83fd17bb10e943234260c0d005d9596170d5ef3941b`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 221.3 KB (221271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fa71cb099a874587efb2d18cba67b14c33ca2472939d01c1695f39e969163c`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1429def50f578086adeafeb1154a9f6683ab8f11715a60a8a1b321413c7c7f38`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9df8a0a34577ec497d4f3f9c496c80e25780fb1f7f65b7b4dca4ebeac8ae1519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4991026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1406a1e174e65b701e8309b0f54ca9baedca4ad65edc6f10a353bb3d572a13f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:06:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:06:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:06:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:06:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:06:12 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:06:12 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:06:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:06:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d862c0d3de0fac486d6fadbba838d9e7f39d8a7dfc4bf9b581acadbda1fa5b`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3191ed9fa9a76370d05de08851632bb6705a7774f50f7665aa9d4e8116ccb0`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.2 MB (1236779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88370d736f5a7966cfdc651335576668afabbcc66a8194b21ff91e010f4c55b8`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 607.2 KB (607212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c59b5e58ec67619e90903390555d8eb0bdb23cc0abd3d1bf00650a37e7d9b7`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195a434068a95af750df05a3f069cad835530de205cfea200155c2bbb3d17bbc`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7e217a6b1042b741dc317dbc9f5aa1d0a6e846ffb75181e5b4f5a30ecfdf527f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4638967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17d535585fee20a92f1ac79b6c94a3b1217e954e28e5a8f8078c998df038557`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:32:35 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:32:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:32:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:32:45 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:32:45 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:32:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:32:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0685d1c97bb4ab51c253c5c084c6e78be0db7a3c5791be1c9d4602fce3953b79`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8980deddc51628db59e13ee670457530ea101bc22548d04eb2eb5ddb82abe598`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 1.2 MB (1163903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882273c520366a5009c0c5ffff4ce6d70e9a8172dbc529636efffede2a77696a`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 573.4 KB (573421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336e75adcb6641cba93182ecfadbbc458f58873a923a6a73ccb7c2660db3b32d`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34003432a0d18065614a57c50acd83bd03210ffdc601a0c5f14c8eca3cdd072`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b3e6d8b6dba4bb203308f2890a66da1d82b1118bfd06f4388d7bb74947459a42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5318202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2979e47c65cc5da347c11efd63887a9a5d3c9a725fdb77d77881c953a600d7af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:04:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:04:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:04:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:04:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:04:32 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:04:33 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:04:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:04:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83a0f29ff084b101d2bedb67bd954464c8ea2c833f6d9e463637ce1e3b85570`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cf75f2a3111f44f8592427f7aa844af1ebf62fa9f9866aa379e5f18d39808f`  
		Last Modified: Sat, 21 Oct 2023 03:04:45 GMT  
		Size: 1.4 MB (1362691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33a4554df0c7945678d4b7f22a6c2516b8138ea1b7e2c83c2a1f18701c9546`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 621.9 KB (621941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0902852a7093c6199857d5a4667571b9d5e3760d5aadc7e95add0b0057fc489c`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5d88ecfb88d6b48191b0de36de2710a9103aef771473701ea711287a3afe1a`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:4a64fa7debbe2222651433cc328105fe1aa8b355b63ae4bba61400f4040ea000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5226880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac627aa6486fd0f2e81ceb74df0a13d52ae058d3f0f360e08a6675b84c84e9c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:04:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 02:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 02:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 02:04:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 02:04:44 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 02:04:44 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 02:04:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 02:04:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33b43d22e223fc31335df903a86b4f1171d08db94ddae5efe5d08e9698f98c1`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04497d2dbca17493cffd45065a4e72ff59533fc06618373387f34e38f0bb1cc0`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 1.4 MB (1353884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e332fd0c16912f90a54e5b24c4dafc83d5784af7379b6be3d69a819fffe3241f`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 635.5 KB (635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc81899e8c005908b85605328231e95708866ba7922deec256bd6437ad48e73`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73737104e3f919559d15046753e769e225f3b531266273778a4ae009548336f9`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f69c272bb3ae2e9b8a177329b2b5e54dc8802654de744089994cb7228ede3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5329375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b87c1a119db9fdddaaeb16754aa4b07f637b42436a69111204d05c75c186608`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:13:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:13:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:13:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:13:41 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:13:42 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:13:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d410f45a90c70f879443ba3946c24240dbe040601a76f35dcb5a380fdc82b60`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a364f51b947cc7eba299e40137deb29c1254d4515d6ef730313422214dbeb7c7`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.4 MB (1361736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7659f4cc5c2bdbf6a67f465a448677fa9c15a6ab68580bec70ffbd57aba9a3f3`  
		Last Modified: Sat, 21 Oct 2023 01:13:59 GMT  
		Size: 619.4 KB (619386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783eb3619067a542b443f39b00f570a8ab027ee35bf4b494c7f658d9ebd6f73`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c72af5246df895d51bbbcaa58fba103965d608a0e9e4bf6b18b08f614317a5`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:98284a17fa0c80767981bd99393cd484fe002e68450233bfaea1b5a88b9b22d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5053046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb467c3a7dc5ff285adfe703953cf1ab92bf7b5d99ff8fd56c7a06b24c551713`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:08:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:08:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:08:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:08:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:08:22 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:08:22 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:08:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:08:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:08:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892540ac0e1d481800201bd26b19bff2b8fb7676da32f32627f7608c581964e`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c30da304e376763e7fb5589b18a8fe13f6efb87563b6578db8f5c52527aae34`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.2 MB (1221479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dff0df9199f69591bd6f28e91cee32ed9da4b645d33d9b7e3f0b618122f4cda`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 614.7 KB (614722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58582257555f94a55275ed46f9a805fef4b3b420a10ba1e5df6382a465b42b6d`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0658640d198e3dd6b2e5b71a78c003d7578a7ab2d3d51b3aa6620b727ebcc370`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:682342279f587fb9710d8ae48633a1f21c9b8b9db46441a369799e8a8034ae12
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
$ docker pull spiped@sha256:fc3b908a26fb9e7a920f3103dd6ab8dd8d4e2ddf9199d6fd3e427d27e1813509
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38217301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59df6dfe09d725bf32ab563c2a0855c886b9a1d5ec6602ae719f009e0f673d9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 19:56:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 19:56:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:56:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 19:57:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 19:57:20 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 19:57:20 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 19:57:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 19:57:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 19:57:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89098fb70aba03de1d0a340fa9730ebf791943e1ddd82b20c54381bad68d1821`  
		Last Modified: Tue, 21 Nov 2023 19:57:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d1d9c52903bd04e0b1aa2d6271b43398bc23d10dffadaef056b4978ea20038`  
		Last Modified: Tue, 21 Nov 2023 19:57:32 GMT  
		Size: 2.6 MB (2591886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450c30ae667851f890ead982bd7dcd85a72bce3e071687a16436543d5a17759f`  
		Last Modified: Tue, 21 Nov 2023 19:57:33 GMT  
		Size: 6.5 MB (6473909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2d81e4e280c8c0c5ea1466e8c68915ab09769685596cea9b0c40c5bae43813`  
		Last Modified: Tue, 21 Nov 2023 19:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3476d0aeb59e34ab31b0327be0940e18de5a1c7b369fd86feb394c3d28c35e`  
		Last Modified: Tue, 21 Nov 2023 19:57:32 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a22fc52e1353a81c0b5e864f000d5b7c6f511f31d25d33161d7fff1fa66a128f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34250716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:805e4bd68f268c5a14b0391f350041c251fc5129caa5978c1f2bd4a998995836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:48:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:48:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:48:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:48:30 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:48:31 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:48:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c4d22227960e496eb464146dc866dad412f31aa91c728607dde4278de637ee`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53633f32e999cc192394918d73de2f3ad375e658d9e7dd207468ea6b664eb6d4`  
		Last Modified: Tue, 21 Nov 2023 05:48:39 GMT  
		Size: 2.2 MB (2186814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82ff098495f0ea42040c5184eb059c29c59d5d6e660aa0b1fbc7fff91b2ad4b`  
		Last Modified: Tue, 21 Nov 2023 05:48:40 GMT  
		Size: 5.1 MB (5140150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f734161b12b1fc00f0c981ce9f8176dacc5ca02b74484b806d289850efaa8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f8f249901f701b78f48d77ef49a7fe721309da08eae74507aec894e5a49af8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d49e38f255892c26d1cde15165c35c32cf857b3446c025ecbd69a009b6d59a12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31677806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97542227ddc0fffbebd6a1fa7da3015089ed0e15aa7d37d4d6c22aa77e4748e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 11:53:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 11:53:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 11:53:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 11:54:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 11:54:13 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 11:54:13 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 11:54:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 11:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 11:54:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac591a8672b5dba3bfcbe0fe6c21f8387ab9a4f56d6ea32f9eebf5e37feca3`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0fa0448ca0214cd73bf754ce7fd1d9686bd3de6b1bf5840a2c8bd3587f1109`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 2.0 MB (2046224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efda8a5518d4c16d427ac57f16268ce4060b4a3d1760ff2cd9b1743185072436`  
		Last Modified: Tue, 21 Nov 2023 11:54:28 GMT  
		Size: 4.9 MB (4881057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37767eb2f6144694ce685d9751a24751196daeb9c3b4a24cda3aa648169b599c`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac67ec8ea82fe47e96246ff7b13f0fbfe7d1fd1f42e5e299ada512bc129fb30`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:57c39c08bbf544370ee603edc8311c0ae6ae5544b2e36b00f992a4c7d61979ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37098308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee328258fcaccf097e36c2041f5623138c3e45fba88ae8fb0a2346b4a7abff8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:36:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 20:36:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 20:36:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 20:36:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 20:36:46 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 20:36:46 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 20:36:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 20:36:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 20:36:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67d14d16729f6a29d5643e5739ce8f277db88c76e8576b74466bed71e9614a3`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667f3b336a76ba92a985040ecc81f1e4b96ab00b9bffb9691d4a0909fee7d70`  
		Last Modified: Tue, 21 Nov 2023 20:36:59 GMT  
		Size: 2.4 MB (2434842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365e0235c5f2467bccbbc07ea82e8e9f2af172d10ad8cb487a501738c975909`  
		Last Modified: Tue, 21 Nov 2023 20:37:00 GMT  
		Size: 5.5 MB (5482590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfecc897f46254770f57aee0cf4c99b9ddfd59416111300bcae84be0bb3661e`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8280277e4e1e138609865f279ff5fef4c40a0bb4f48d2230459299b00d656ad0`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:c2feb65880bc509150accfd419e6813f14627257be2627bbe31de9a5184a5e0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38697733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36feabcb5b8aebe526989cb605bfe36f6ba227f20c4202055c68d66994900b1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Wed, 22 Nov 2023 01:09:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Nov 2023 01:09:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:09:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 22 Nov 2023 01:09:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Nov 2023 01:09:56 GMT
VOLUME [/spiped]
# Wed, 22 Nov 2023 01:09:56 GMT
WORKDIR /spiped
# Wed, 22 Nov 2023 01:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Nov 2023 01:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Nov 2023 01:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d9077e40b47c5791b4ac20b24d8deff63a5dc8bf5207083f56177fda752514`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e71210812cdeec1bdcbcdc0d631c3eadb6ea9c8b9858c611a0182299588731`  
		Last Modified: Wed, 22 Nov 2023 01:10:13 GMT  
		Size: 2.6 MB (2588158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f18e97e0027d314fc775390b955ca68e6a4cc69d6077de1fc07ccefcd18758f`  
		Last Modified: Wed, 22 Nov 2023 01:10:14 GMT  
		Size: 5.9 MB (5943867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48894c0f6daf466b673d54c1f3536c05d1e8de633a2a517c55a0946adfc311ec`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c404496be4d3107996737e0d3b4b2b5766ee34e42c1a7e6961de6efcec4dde`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:0d61d0a1ea5ac2651b170d9096365703860743a0df774ddcdc327b0915c4544f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36783306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287250c56678b233b997a1c6059e730e147815a68e1df4f12eda08a5eed1ebe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:42:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 16:42:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 16:44:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 16:44:19 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 16:44:22 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 16:44:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 16:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ff2608f3497720032e30b79ae5d65cfa2c8dd359565c1c8dd638f5b3a6f0d`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab7308e1ec6dfefbe63dcd0ffdd71389fcdc64536e65a12a0d4e0b039458285`  
		Last Modified: Tue, 21 Nov 2023 16:44:46 GMT  
		Size: 1.8 MB (1834326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bede55fcddef2dca32fd1854933f48d44eb852b04607b5ca0ee5f0ceede864c`  
		Last Modified: Tue, 21 Nov 2023 16:44:49 GMT  
		Size: 5.8 MB (5805479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8ac4180d595ed6276f96e62a762ce81e1cbc8d5adb99021d674d703250377a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6377814988f39cd05c902f86328248c9751a1903ed8401e8827bf7540cc4a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:99a36d31339087c56743fcd7b09255be818296337c1ee9b0b9e5caa4d6d2a629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42336939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbf18f5d582e136651ca47bbf5c8553330ac36b69e4beb1e957d147dbc321fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:49:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 12:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:49:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 12:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:49:48 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 12:49:48 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 12:49:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 12:49:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e3e9a6e83461086d799b3c35e7086e930106125c74069a1510c25bdb6afb6d`  
		Last Modified: Tue, 21 Nov 2023 12:50:01 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956ee3303181032f855a7b2887c1bdca6910e0cb1ec3c92b65d6509c2f907abb`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 2.8 MB (2770520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ddbd7552dcc1e8096f1f690fb7a8f6d94f6b14b70ac7c130e5224ccc99ae5`  
		Last Modified: Tue, 21 Nov 2023 12:50:03 GMT  
		Size: 6.4 MB (6423216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acdb31d4ba61d5a1503eb5bf6cd716ec162f811fe2c79c2ff5c2e727033efc0`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da63bf7cb4ff2b34de84cd9caefa0d255c9965665b50f421172e3d96c2ee315a`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:e55796d4c561e3f8eec223e5e69fb5d024ac8574c4aace38477a60420ff5414c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35164381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ea59dc57dc93fac49f303c8c58d6d153d1c8a8ffab3500ff5649eb63c8b568`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:54:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:54:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:54:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:54:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:54:34 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:54:34 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:54:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:54:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a1488c1c72f51fc67f2f92a4266ad144068e6265f09a6854a0edda69d1e634`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850f941b1cd09719d174b6a90cb013528879a956734598472118c9ba95f4f146`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 2.3 MB (2262458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647d17c59a394362c94984e56f3babc4addd9e026c843bede6b3b295b4b9439c`  
		Last Modified: Tue, 21 Nov 2023 05:54:55 GMT  
		Size: 5.4 MB (5387438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5763b7fbe5d4e9c3ba3f58020db82f8a9bba3e6a9a702f785249dd13161a253b`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d519c5ded3c9d38ab8b28f40d83037fc367671ed767a048f773b935af62381f`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:88dccc72f75f2fc6cc962aaf58d6d7f85f43ef29d88e5eaba0e7d2dbebbc982d
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
$ docker pull spiped@sha256:bbcb559f4d5d2f95adfeef51c918f2c078dcf991b30279a34be08e7614eda451
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5058435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e068a31dc93f7fbe323b521ca3e2dce275263b1eb366f065ef43b018191ac2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:00:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 06:00:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 06:00:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 06:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 06:00:14 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 06:00:14 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 06:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 06:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 06:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc456d15d6c4f02d60102c7538cc196adfd3073fa382d3a6c9410c2acfa02238`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac40e9085148fd6ad0718c4bb551770cb399db60f6d9e0e6ae11e2af695afc`  
		Last Modified: Fri, 01 Dec 2023 06:00:26 GMT  
		Size: 1.4 MB (1433002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b55d95977f08a50d321f83fd17bb10e943234260c0d005d9596170d5ef3941b`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 221.3 KB (221271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fa71cb099a874587efb2d18cba67b14c33ca2472939d01c1695f39e969163c`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1429def50f578086adeafeb1154a9f6683ab8f11715a60a8a1b321413c7c7f38`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9df8a0a34577ec497d4f3f9c496c80e25780fb1f7f65b7b4dca4ebeac8ae1519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4991026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1406a1e174e65b701e8309b0f54ca9baedca4ad65edc6f10a353bb3d572a13f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:06:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:06:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:06:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:06:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:06:12 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:06:12 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:06:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:06:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d862c0d3de0fac486d6fadbba838d9e7f39d8a7dfc4bf9b581acadbda1fa5b`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3191ed9fa9a76370d05de08851632bb6705a7774f50f7665aa9d4e8116ccb0`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.2 MB (1236779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88370d736f5a7966cfdc651335576668afabbcc66a8194b21ff91e010f4c55b8`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 607.2 KB (607212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c59b5e58ec67619e90903390555d8eb0bdb23cc0abd3d1bf00650a37e7d9b7`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195a434068a95af750df05a3f069cad835530de205cfea200155c2bbb3d17bbc`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7e217a6b1042b741dc317dbc9f5aa1d0a6e846ffb75181e5b4f5a30ecfdf527f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4638967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17d535585fee20a92f1ac79b6c94a3b1217e954e28e5a8f8078c998df038557`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:32:35 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:32:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:32:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:32:45 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:32:45 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:32:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:32:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0685d1c97bb4ab51c253c5c084c6e78be0db7a3c5791be1c9d4602fce3953b79`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8980deddc51628db59e13ee670457530ea101bc22548d04eb2eb5ddb82abe598`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 1.2 MB (1163903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882273c520366a5009c0c5ffff4ce6d70e9a8172dbc529636efffede2a77696a`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 573.4 KB (573421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336e75adcb6641cba93182ecfadbbc458f58873a923a6a73ccb7c2660db3b32d`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34003432a0d18065614a57c50acd83bd03210ffdc601a0c5f14c8eca3cdd072`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b3e6d8b6dba4bb203308f2890a66da1d82b1118bfd06f4388d7bb74947459a42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5318202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2979e47c65cc5da347c11efd63887a9a5d3c9a725fdb77d77881c953a600d7af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:04:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:04:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:04:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:04:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:04:32 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:04:33 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:04:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:04:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83a0f29ff084b101d2bedb67bd954464c8ea2c833f6d9e463637ce1e3b85570`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cf75f2a3111f44f8592427f7aa844af1ebf62fa9f9866aa379e5f18d39808f`  
		Last Modified: Sat, 21 Oct 2023 03:04:45 GMT  
		Size: 1.4 MB (1362691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33a4554df0c7945678d4b7f22a6c2516b8138ea1b7e2c83c2a1f18701c9546`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 621.9 KB (621941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0902852a7093c6199857d5a4667571b9d5e3760d5aadc7e95add0b0057fc489c`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5d88ecfb88d6b48191b0de36de2710a9103aef771473701ea711287a3afe1a`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:4a64fa7debbe2222651433cc328105fe1aa8b355b63ae4bba61400f4040ea000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5226880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac627aa6486fd0f2e81ceb74df0a13d52ae058d3f0f360e08a6675b84c84e9c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:04:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 02:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 02:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 02:04:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 02:04:44 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 02:04:44 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 02:04:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 02:04:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33b43d22e223fc31335df903a86b4f1171d08db94ddae5efe5d08e9698f98c1`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04497d2dbca17493cffd45065a4e72ff59533fc06618373387f34e38f0bb1cc0`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 1.4 MB (1353884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e332fd0c16912f90a54e5b24c4dafc83d5784af7379b6be3d69a819fffe3241f`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 635.5 KB (635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc81899e8c005908b85605328231e95708866ba7922deec256bd6437ad48e73`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73737104e3f919559d15046753e769e225f3b531266273778a4ae009548336f9`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f69c272bb3ae2e9b8a177329b2b5e54dc8802654de744089994cb7228ede3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5329375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b87c1a119db9fdddaaeb16754aa4b07f637b42436a69111204d05c75c186608`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:13:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:13:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:13:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:13:41 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:13:42 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:13:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d410f45a90c70f879443ba3946c24240dbe040601a76f35dcb5a380fdc82b60`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a364f51b947cc7eba299e40137deb29c1254d4515d6ef730313422214dbeb7c7`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.4 MB (1361736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7659f4cc5c2bdbf6a67f465a448677fa9c15a6ab68580bec70ffbd57aba9a3f3`  
		Last Modified: Sat, 21 Oct 2023 01:13:59 GMT  
		Size: 619.4 KB (619386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783eb3619067a542b443f39b00f570a8ab027ee35bf4b494c7f658d9ebd6f73`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c72af5246df895d51bbbcaa58fba103965d608a0e9e4bf6b18b08f614317a5`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:98284a17fa0c80767981bd99393cd484fe002e68450233bfaea1b5a88b9b22d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5053046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb467c3a7dc5ff285adfe703953cf1ab92bf7b5d99ff8fd56c7a06b24c551713`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:08:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:08:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:08:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:08:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:08:22 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:08:22 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:08:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:08:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:08:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892540ac0e1d481800201bd26b19bff2b8fb7676da32f32627f7608c581964e`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c30da304e376763e7fb5589b18a8fe13f6efb87563b6578db8f5c52527aae34`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.2 MB (1221479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dff0df9199f69591bd6f28e91cee32ed9da4b645d33d9b7e3f0b618122f4cda`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 614.7 KB (614722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58582257555f94a55275ed46f9a805fef4b3b420a10ba1e5df6382a465b42b6d`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0658640d198e3dd6b2e5b71a78c003d7578a7ab2d3d51b3aa6620b727ebcc370`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:682342279f587fb9710d8ae48633a1f21c9b8b9db46441a369799e8a8034ae12
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

### `spiped:1.6.2` - linux; amd64

```console
$ docker pull spiped@sha256:fc3b908a26fb9e7a920f3103dd6ab8dd8d4e2ddf9199d6fd3e427d27e1813509
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38217301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59df6dfe09d725bf32ab563c2a0855c886b9a1d5ec6602ae719f009e0f673d9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 19:56:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 19:56:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:56:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 19:57:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 19:57:20 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 19:57:20 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 19:57:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 19:57:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 19:57:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89098fb70aba03de1d0a340fa9730ebf791943e1ddd82b20c54381bad68d1821`  
		Last Modified: Tue, 21 Nov 2023 19:57:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d1d9c52903bd04e0b1aa2d6271b43398bc23d10dffadaef056b4978ea20038`  
		Last Modified: Tue, 21 Nov 2023 19:57:32 GMT  
		Size: 2.6 MB (2591886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450c30ae667851f890ead982bd7dcd85a72bce3e071687a16436543d5a17759f`  
		Last Modified: Tue, 21 Nov 2023 19:57:33 GMT  
		Size: 6.5 MB (6473909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2d81e4e280c8c0c5ea1466e8c68915ab09769685596cea9b0c40c5bae43813`  
		Last Modified: Tue, 21 Nov 2023 19:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3476d0aeb59e34ab31b0327be0940e18de5a1c7b369fd86feb394c3d28c35e`  
		Last Modified: Tue, 21 Nov 2023 19:57:32 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a22fc52e1353a81c0b5e864f000d5b7c6f511f31d25d33161d7fff1fa66a128f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34250716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:805e4bd68f268c5a14b0391f350041c251fc5129caa5978c1f2bd4a998995836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:48:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:48:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:48:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:48:30 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:48:31 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:48:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c4d22227960e496eb464146dc866dad412f31aa91c728607dde4278de637ee`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53633f32e999cc192394918d73de2f3ad375e658d9e7dd207468ea6b664eb6d4`  
		Last Modified: Tue, 21 Nov 2023 05:48:39 GMT  
		Size: 2.2 MB (2186814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82ff098495f0ea42040c5184eb059c29c59d5d6e660aa0b1fbc7fff91b2ad4b`  
		Last Modified: Tue, 21 Nov 2023 05:48:40 GMT  
		Size: 5.1 MB (5140150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f734161b12b1fc00f0c981ce9f8176dacc5ca02b74484b806d289850efaa8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f8f249901f701b78f48d77ef49a7fe721309da08eae74507aec894e5a49af8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d49e38f255892c26d1cde15165c35c32cf857b3446c025ecbd69a009b6d59a12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31677806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97542227ddc0fffbebd6a1fa7da3015089ed0e15aa7d37d4d6c22aa77e4748e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 11:53:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 11:53:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 11:53:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 11:54:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 11:54:13 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 11:54:13 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 11:54:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 11:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 11:54:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac591a8672b5dba3bfcbe0fe6c21f8387ab9a4f56d6ea32f9eebf5e37feca3`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0fa0448ca0214cd73bf754ce7fd1d9686bd3de6b1bf5840a2c8bd3587f1109`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 2.0 MB (2046224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efda8a5518d4c16d427ac57f16268ce4060b4a3d1760ff2cd9b1743185072436`  
		Last Modified: Tue, 21 Nov 2023 11:54:28 GMT  
		Size: 4.9 MB (4881057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37767eb2f6144694ce685d9751a24751196daeb9c3b4a24cda3aa648169b599c`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac67ec8ea82fe47e96246ff7b13f0fbfe7d1fd1f42e5e299ada512bc129fb30`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:57c39c08bbf544370ee603edc8311c0ae6ae5544b2e36b00f992a4c7d61979ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37098308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee328258fcaccf097e36c2041f5623138c3e45fba88ae8fb0a2346b4a7abff8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:36:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 20:36:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 20:36:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 20:36:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 20:36:46 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 20:36:46 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 20:36:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 20:36:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 20:36:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67d14d16729f6a29d5643e5739ce8f277db88c76e8576b74466bed71e9614a3`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667f3b336a76ba92a985040ecc81f1e4b96ab00b9bffb9691d4a0909fee7d70`  
		Last Modified: Tue, 21 Nov 2023 20:36:59 GMT  
		Size: 2.4 MB (2434842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365e0235c5f2467bccbbc07ea82e8e9f2af172d10ad8cb487a501738c975909`  
		Last Modified: Tue, 21 Nov 2023 20:37:00 GMT  
		Size: 5.5 MB (5482590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfecc897f46254770f57aee0cf4c99b9ddfd59416111300bcae84be0bb3661e`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8280277e4e1e138609865f279ff5fef4c40a0bb4f48d2230459299b00d656ad0`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:c2feb65880bc509150accfd419e6813f14627257be2627bbe31de9a5184a5e0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38697733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36feabcb5b8aebe526989cb605bfe36f6ba227f20c4202055c68d66994900b1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Wed, 22 Nov 2023 01:09:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Nov 2023 01:09:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:09:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 22 Nov 2023 01:09:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Nov 2023 01:09:56 GMT
VOLUME [/spiped]
# Wed, 22 Nov 2023 01:09:56 GMT
WORKDIR /spiped
# Wed, 22 Nov 2023 01:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Nov 2023 01:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Nov 2023 01:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d9077e40b47c5791b4ac20b24d8deff63a5dc8bf5207083f56177fda752514`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e71210812cdeec1bdcbcdc0d631c3eadb6ea9c8b9858c611a0182299588731`  
		Last Modified: Wed, 22 Nov 2023 01:10:13 GMT  
		Size: 2.6 MB (2588158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f18e97e0027d314fc775390b955ca68e6a4cc69d6077de1fc07ccefcd18758f`  
		Last Modified: Wed, 22 Nov 2023 01:10:14 GMT  
		Size: 5.9 MB (5943867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48894c0f6daf466b673d54c1f3536c05d1e8de633a2a517c55a0946adfc311ec`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c404496be4d3107996737e0d3b4b2b5766ee34e42c1a7e6961de6efcec4dde`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:0d61d0a1ea5ac2651b170d9096365703860743a0df774ddcdc327b0915c4544f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36783306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287250c56678b233b997a1c6059e730e147815a68e1df4f12eda08a5eed1ebe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:42:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 16:42:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 16:44:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 16:44:19 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 16:44:22 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 16:44:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 16:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ff2608f3497720032e30b79ae5d65cfa2c8dd359565c1c8dd638f5b3a6f0d`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab7308e1ec6dfefbe63dcd0ffdd71389fcdc64536e65a12a0d4e0b039458285`  
		Last Modified: Tue, 21 Nov 2023 16:44:46 GMT  
		Size: 1.8 MB (1834326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bede55fcddef2dca32fd1854933f48d44eb852b04607b5ca0ee5f0ceede864c`  
		Last Modified: Tue, 21 Nov 2023 16:44:49 GMT  
		Size: 5.8 MB (5805479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8ac4180d595ed6276f96e62a762ce81e1cbc8d5adb99021d674d703250377a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6377814988f39cd05c902f86328248c9751a1903ed8401e8827bf7540cc4a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:99a36d31339087c56743fcd7b09255be818296337c1ee9b0b9e5caa4d6d2a629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42336939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbf18f5d582e136651ca47bbf5c8553330ac36b69e4beb1e957d147dbc321fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:49:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 12:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:49:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 12:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:49:48 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 12:49:48 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 12:49:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 12:49:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e3e9a6e83461086d799b3c35e7086e930106125c74069a1510c25bdb6afb6d`  
		Last Modified: Tue, 21 Nov 2023 12:50:01 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956ee3303181032f855a7b2887c1bdca6910e0cb1ec3c92b65d6509c2f907abb`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 2.8 MB (2770520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ddbd7552dcc1e8096f1f690fb7a8f6d94f6b14b70ac7c130e5224ccc99ae5`  
		Last Modified: Tue, 21 Nov 2023 12:50:03 GMT  
		Size: 6.4 MB (6423216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acdb31d4ba61d5a1503eb5bf6cd716ec162f811fe2c79c2ff5c2e727033efc0`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da63bf7cb4ff2b34de84cd9caefa0d255c9965665b50f421172e3d96c2ee315a`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:e55796d4c561e3f8eec223e5e69fb5d024ac8574c4aace38477a60420ff5414c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35164381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ea59dc57dc93fac49f303c8c58d6d153d1c8a8ffab3500ff5649eb63c8b568`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:54:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:54:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:54:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:54:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:54:34 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:54:34 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:54:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:54:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a1488c1c72f51fc67f2f92a4266ad144068e6265f09a6854a0edda69d1e634`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850f941b1cd09719d174b6a90cb013528879a956734598472118c9ba95f4f146`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 2.3 MB (2262458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647d17c59a394362c94984e56f3babc4addd9e026c843bede6b3b295b4b9439c`  
		Last Modified: Tue, 21 Nov 2023 05:54:55 GMT  
		Size: 5.4 MB (5387438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5763b7fbe5d4e9c3ba3f58020db82f8a9bba3e6a9a702f785249dd13161a253b`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d519c5ded3c9d38ab8b28f40d83037fc367671ed767a048f773b935af62381f`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:88dccc72f75f2fc6cc962aaf58d6d7f85f43ef29d88e5eaba0e7d2dbebbc982d
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

### `spiped:1.6.2-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:bbcb559f4d5d2f95adfeef51c918f2c078dcf991b30279a34be08e7614eda451
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5058435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e068a31dc93f7fbe323b521ca3e2dce275263b1eb366f065ef43b018191ac2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:00:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 06:00:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 06:00:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 06:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 06:00:14 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 06:00:14 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 06:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 06:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 06:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc456d15d6c4f02d60102c7538cc196adfd3073fa382d3a6c9410c2acfa02238`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac40e9085148fd6ad0718c4bb551770cb399db60f6d9e0e6ae11e2af695afc`  
		Last Modified: Fri, 01 Dec 2023 06:00:26 GMT  
		Size: 1.4 MB (1433002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b55d95977f08a50d321f83fd17bb10e943234260c0d005d9596170d5ef3941b`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 221.3 KB (221271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fa71cb099a874587efb2d18cba67b14c33ca2472939d01c1695f39e969163c`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1429def50f578086adeafeb1154a9f6683ab8f11715a60a8a1b321413c7c7f38`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9df8a0a34577ec497d4f3f9c496c80e25780fb1f7f65b7b4dca4ebeac8ae1519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4991026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1406a1e174e65b701e8309b0f54ca9baedca4ad65edc6f10a353bb3d572a13f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:06:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:06:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:06:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:06:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:06:12 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:06:12 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:06:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:06:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d862c0d3de0fac486d6fadbba838d9e7f39d8a7dfc4bf9b581acadbda1fa5b`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3191ed9fa9a76370d05de08851632bb6705a7774f50f7665aa9d4e8116ccb0`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.2 MB (1236779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88370d736f5a7966cfdc651335576668afabbcc66a8194b21ff91e010f4c55b8`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 607.2 KB (607212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c59b5e58ec67619e90903390555d8eb0bdb23cc0abd3d1bf00650a37e7d9b7`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195a434068a95af750df05a3f069cad835530de205cfea200155c2bbb3d17bbc`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7e217a6b1042b741dc317dbc9f5aa1d0a6e846ffb75181e5b4f5a30ecfdf527f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4638967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17d535585fee20a92f1ac79b6c94a3b1217e954e28e5a8f8078c998df038557`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:32:35 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:32:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:32:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:32:45 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:32:45 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:32:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:32:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0685d1c97bb4ab51c253c5c084c6e78be0db7a3c5791be1c9d4602fce3953b79`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8980deddc51628db59e13ee670457530ea101bc22548d04eb2eb5ddb82abe598`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 1.2 MB (1163903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882273c520366a5009c0c5ffff4ce6d70e9a8172dbc529636efffede2a77696a`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 573.4 KB (573421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336e75adcb6641cba93182ecfadbbc458f58873a923a6a73ccb7c2660db3b32d`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34003432a0d18065614a57c50acd83bd03210ffdc601a0c5f14c8eca3cdd072`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b3e6d8b6dba4bb203308f2890a66da1d82b1118bfd06f4388d7bb74947459a42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5318202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2979e47c65cc5da347c11efd63887a9a5d3c9a725fdb77d77881c953a600d7af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:04:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:04:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:04:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:04:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:04:32 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:04:33 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:04:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:04:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83a0f29ff084b101d2bedb67bd954464c8ea2c833f6d9e463637ce1e3b85570`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cf75f2a3111f44f8592427f7aa844af1ebf62fa9f9866aa379e5f18d39808f`  
		Last Modified: Sat, 21 Oct 2023 03:04:45 GMT  
		Size: 1.4 MB (1362691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33a4554df0c7945678d4b7f22a6c2516b8138ea1b7e2c83c2a1f18701c9546`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 621.9 KB (621941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0902852a7093c6199857d5a4667571b9d5e3760d5aadc7e95add0b0057fc489c`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5d88ecfb88d6b48191b0de36de2710a9103aef771473701ea711287a3afe1a`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:4a64fa7debbe2222651433cc328105fe1aa8b355b63ae4bba61400f4040ea000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5226880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac627aa6486fd0f2e81ceb74df0a13d52ae058d3f0f360e08a6675b84c84e9c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:04:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 02:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 02:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 02:04:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 02:04:44 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 02:04:44 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 02:04:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 02:04:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33b43d22e223fc31335df903a86b4f1171d08db94ddae5efe5d08e9698f98c1`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04497d2dbca17493cffd45065a4e72ff59533fc06618373387f34e38f0bb1cc0`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 1.4 MB (1353884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e332fd0c16912f90a54e5b24c4dafc83d5784af7379b6be3d69a819fffe3241f`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 635.5 KB (635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc81899e8c005908b85605328231e95708866ba7922deec256bd6437ad48e73`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73737104e3f919559d15046753e769e225f3b531266273778a4ae009548336f9`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f69c272bb3ae2e9b8a177329b2b5e54dc8802654de744089994cb7228ede3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5329375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b87c1a119db9fdddaaeb16754aa4b07f637b42436a69111204d05c75c186608`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:13:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:13:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:13:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:13:41 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:13:42 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:13:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d410f45a90c70f879443ba3946c24240dbe040601a76f35dcb5a380fdc82b60`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a364f51b947cc7eba299e40137deb29c1254d4515d6ef730313422214dbeb7c7`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.4 MB (1361736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7659f4cc5c2bdbf6a67f465a448677fa9c15a6ab68580bec70ffbd57aba9a3f3`  
		Last Modified: Sat, 21 Oct 2023 01:13:59 GMT  
		Size: 619.4 KB (619386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783eb3619067a542b443f39b00f570a8ab027ee35bf4b494c7f658d9ebd6f73`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c72af5246df895d51bbbcaa58fba103965d608a0e9e4bf6b18b08f614317a5`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:98284a17fa0c80767981bd99393cd484fe002e68450233bfaea1b5a88b9b22d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5053046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb467c3a7dc5ff285adfe703953cf1ab92bf7b5d99ff8fd56c7a06b24c551713`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:08:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:08:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:08:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:08:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:08:22 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:08:22 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:08:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:08:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:08:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892540ac0e1d481800201bd26b19bff2b8fb7676da32f32627f7608c581964e`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c30da304e376763e7fb5589b18a8fe13f6efb87563b6578db8f5c52527aae34`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.2 MB (1221479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dff0df9199f69591bd6f28e91cee32ed9da4b645d33d9b7e3f0b618122f4cda`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 614.7 KB (614722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58582257555f94a55275ed46f9a805fef4b3b420a10ba1e5df6382a465b42b6d`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0658640d198e3dd6b2e5b71a78c003d7578a7ab2d3d51b3aa6620b727ebcc370`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:88dccc72f75f2fc6cc962aaf58d6d7f85f43ef29d88e5eaba0e7d2dbebbc982d
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
$ docker pull spiped@sha256:bbcb559f4d5d2f95adfeef51c918f2c078dcf991b30279a34be08e7614eda451
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5058435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e068a31dc93f7fbe323b521ca3e2dce275263b1eb366f065ef43b018191ac2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:00:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 06:00:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 06:00:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 06:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 06:00:14 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 06:00:14 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 06:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 06:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 06:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc456d15d6c4f02d60102c7538cc196adfd3073fa382d3a6c9410c2acfa02238`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac40e9085148fd6ad0718c4bb551770cb399db60f6d9e0e6ae11e2af695afc`  
		Last Modified: Fri, 01 Dec 2023 06:00:26 GMT  
		Size: 1.4 MB (1433002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b55d95977f08a50d321f83fd17bb10e943234260c0d005d9596170d5ef3941b`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 221.3 KB (221271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fa71cb099a874587efb2d18cba67b14c33ca2472939d01c1695f39e969163c`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1429def50f578086adeafeb1154a9f6683ab8f11715a60a8a1b321413c7c7f38`  
		Last Modified: Fri, 01 Dec 2023 06:00:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9df8a0a34577ec497d4f3f9c496c80e25780fb1f7f65b7b4dca4ebeac8ae1519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4991026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1406a1e174e65b701e8309b0f54ca9baedca4ad65edc6f10a353bb3d572a13f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:06:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:06:04 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:06:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:06:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:06:12 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:06:12 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:06:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:06:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d862c0d3de0fac486d6fadbba838d9e7f39d8a7dfc4bf9b581acadbda1fa5b`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3191ed9fa9a76370d05de08851632bb6705a7774f50f7665aa9d4e8116ccb0`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 1.2 MB (1236779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88370d736f5a7966cfdc651335576668afabbcc66a8194b21ff91e010f4c55b8`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 607.2 KB (607212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c59b5e58ec67619e90903390555d8eb0bdb23cc0abd3d1bf00650a37e7d9b7`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195a434068a95af750df05a3f069cad835530de205cfea200155c2bbb3d17bbc`  
		Last Modified: Sat, 21 Oct 2023 01:06:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7e217a6b1042b741dc317dbc9f5aa1d0a6e846ffb75181e5b4f5a30ecfdf527f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4638967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17d535585fee20a92f1ac79b6c94a3b1217e954e28e5a8f8078c998df038557`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:32:35 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:32:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:32:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:32:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:32:45 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:32:45 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:32:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:32:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:32:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0685d1c97bb4ab51c253c5c084c6e78be0db7a3c5791be1c9d4602fce3953b79`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8980deddc51628db59e13ee670457530ea101bc22548d04eb2eb5ddb82abe598`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 1.2 MB (1163903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882273c520366a5009c0c5ffff4ce6d70e9a8172dbc529636efffede2a77696a`  
		Last Modified: Sat, 21 Oct 2023 01:32:59 GMT  
		Size: 573.4 KB (573421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336e75adcb6641cba93182ecfadbbc458f58873a923a6a73ccb7c2660db3b32d`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34003432a0d18065614a57c50acd83bd03210ffdc601a0c5f14c8eca3cdd072`  
		Last Modified: Sat, 21 Oct 2023 01:32:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b3e6d8b6dba4bb203308f2890a66da1d82b1118bfd06f4388d7bb74947459a42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5318202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2979e47c65cc5da347c11efd63887a9a5d3c9a725fdb77d77881c953a600d7af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:04:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 03:04:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 03:04:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 03:04:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 03:04:32 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 03:04:33 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 03:04:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 03:04:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83a0f29ff084b101d2bedb67bd954464c8ea2c833f6d9e463637ce1e3b85570`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cf75f2a3111f44f8592427f7aa844af1ebf62fa9f9866aa379e5f18d39808f`  
		Last Modified: Sat, 21 Oct 2023 03:04:45 GMT  
		Size: 1.4 MB (1362691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33a4554df0c7945678d4b7f22a6c2516b8138ea1b7e2c83c2a1f18701c9546`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 621.9 KB (621941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0902852a7093c6199857d5a4667571b9d5e3760d5aadc7e95add0b0057fc489c`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5d88ecfb88d6b48191b0de36de2710a9103aef771473701ea711287a3afe1a`  
		Last Modified: Sat, 21 Oct 2023 03:04:44 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:4a64fa7debbe2222651433cc328105fe1aa8b355b63ae4bba61400f4040ea000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5226880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac627aa6486fd0f2e81ceb74df0a13d52ae058d3f0f360e08a6675b84c84e9c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:04:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 02:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 02:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 02:04:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 02:04:44 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 02:04:44 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 02:04:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 02:04:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33b43d22e223fc31335df903a86b4f1171d08db94ddae5efe5d08e9698f98c1`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04497d2dbca17493cffd45065a4e72ff59533fc06618373387f34e38f0bb1cc0`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 1.4 MB (1353884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e332fd0c16912f90a54e5b24c4dafc83d5784af7379b6be3d69a819fffe3241f`  
		Last Modified: Sat, 21 Oct 2023 02:04:57 GMT  
		Size: 635.5 KB (635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc81899e8c005908b85605328231e95708866ba7922deec256bd6437ad48e73`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73737104e3f919559d15046753e769e225f3b531266273778a4ae009548336f9`  
		Last Modified: Sat, 21 Oct 2023 02:04:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f69c272bb3ae2e9b8a177329b2b5e54dc8802654de744089994cb7228ede3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5329375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b87c1a119db9fdddaaeb16754aa4b07f637b42436a69111204d05c75c186608`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:13:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:13:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:13:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:13:41 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:13:42 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:13:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d410f45a90c70f879443ba3946c24240dbe040601a76f35dcb5a380fdc82b60`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a364f51b947cc7eba299e40137deb29c1254d4515d6ef730313422214dbeb7c7`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 1.4 MB (1361736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7659f4cc5c2bdbf6a67f465a448677fa9c15a6ab68580bec70ffbd57aba9a3f3`  
		Last Modified: Sat, 21 Oct 2023 01:13:59 GMT  
		Size: 619.4 KB (619386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b783eb3619067a542b443f39b00f570a8ab027ee35bf4b494c7f658d9ebd6f73`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c72af5246df895d51bbbcaa58fba103965d608a0e9e4bf6b18b08f614317a5`  
		Last Modified: Sat, 21 Oct 2023 01:13:58 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:98284a17fa0c80767981bd99393cd484fe002e68450233bfaea1b5a88b9b22d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5053046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb467c3a7dc5ff285adfe703953cf1ab92bf7b5d99ff8fd56c7a06b24c551713`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:08:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 21 Oct 2023 01:08:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 21 Oct 2023 01:08:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 21 Oct 2023 01:08:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 21 Oct 2023 01:08:22 GMT
VOLUME [/spiped]
# Sat, 21 Oct 2023 01:08:22 GMT
WORKDIR /spiped
# Sat, 21 Oct 2023 01:08:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 21 Oct 2023 01:08:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Oct 2023 01:08:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892540ac0e1d481800201bd26b19bff2b8fb7676da32f32627f7608c581964e`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c30da304e376763e7fb5589b18a8fe13f6efb87563b6578db8f5c52527aae34`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 1.2 MB (1221479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dff0df9199f69591bd6f28e91cee32ed9da4b645d33d9b7e3f0b618122f4cda`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 614.7 KB (614722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58582257555f94a55275ed46f9a805fef4b3b420a10ba1e5df6382a465b42b6d`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0658640d198e3dd6b2e5b71a78c003d7578a7ab2d3d51b3aa6620b727ebcc370`  
		Last Modified: Sat, 21 Oct 2023 01:08:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:682342279f587fb9710d8ae48633a1f21c9b8b9db46441a369799e8a8034ae12
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
$ docker pull spiped@sha256:fc3b908a26fb9e7a920f3103dd6ab8dd8d4e2ddf9199d6fd3e427d27e1813509
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38217301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59df6dfe09d725bf32ab563c2a0855c886b9a1d5ec6602ae719f009e0f673d9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 19:56:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 19:56:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:56:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 19:57:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 19:57:20 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 19:57:20 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 19:57:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 19:57:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 19:57:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89098fb70aba03de1d0a340fa9730ebf791943e1ddd82b20c54381bad68d1821`  
		Last Modified: Tue, 21 Nov 2023 19:57:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d1d9c52903bd04e0b1aa2d6271b43398bc23d10dffadaef056b4978ea20038`  
		Last Modified: Tue, 21 Nov 2023 19:57:32 GMT  
		Size: 2.6 MB (2591886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450c30ae667851f890ead982bd7dcd85a72bce3e071687a16436543d5a17759f`  
		Last Modified: Tue, 21 Nov 2023 19:57:33 GMT  
		Size: 6.5 MB (6473909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2d81e4e280c8c0c5ea1466e8c68915ab09769685596cea9b0c40c5bae43813`  
		Last Modified: Tue, 21 Nov 2023 19:57:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3476d0aeb59e34ab31b0327be0940e18de5a1c7b369fd86feb394c3d28c35e`  
		Last Modified: Tue, 21 Nov 2023 19:57:32 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a22fc52e1353a81c0b5e864f000d5b7c6f511f31d25d33161d7fff1fa66a128f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34250716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:805e4bd68f268c5a14b0391f350041c251fc5129caa5978c1f2bd4a998995836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:48:05 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:48:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:48:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:48:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:48:30 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:48:31 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:48:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c4d22227960e496eb464146dc866dad412f31aa91c728607dde4278de637ee`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53633f32e999cc192394918d73de2f3ad375e658d9e7dd207468ea6b664eb6d4`  
		Last Modified: Tue, 21 Nov 2023 05:48:39 GMT  
		Size: 2.2 MB (2186814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82ff098495f0ea42040c5184eb059c29c59d5d6e660aa0b1fbc7fff91b2ad4b`  
		Last Modified: Tue, 21 Nov 2023 05:48:40 GMT  
		Size: 5.1 MB (5140150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f734161b12b1fc00f0c981ce9f8176dacc5ca02b74484b806d289850efaa8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f8f249901f701b78f48d77ef49a7fe721309da08eae74507aec894e5a49af8`  
		Last Modified: Tue, 21 Nov 2023 05:48:38 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d49e38f255892c26d1cde15165c35c32cf857b3446c025ecbd69a009b6d59a12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31677806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97542227ddc0fffbebd6a1fa7da3015089ed0e15aa7d37d4d6c22aa77e4748e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 11:53:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 11:53:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 11:53:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 11:54:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 11:54:13 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 11:54:13 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 11:54:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 11:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 11:54:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cac591a8672b5dba3bfcbe0fe6c21f8387ab9a4f56d6ea32f9eebf5e37feca3`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0fa0448ca0214cd73bf754ce7fd1d9686bd3de6b1bf5840a2c8bd3587f1109`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 2.0 MB (2046224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efda8a5518d4c16d427ac57f16268ce4060b4a3d1760ff2cd9b1743185072436`  
		Last Modified: Tue, 21 Nov 2023 11:54:28 GMT  
		Size: 4.9 MB (4881057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37767eb2f6144694ce685d9751a24751196daeb9c3b4a24cda3aa648169b599c`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac67ec8ea82fe47e96246ff7b13f0fbfe7d1fd1f42e5e299ada512bc129fb30`  
		Last Modified: Tue, 21 Nov 2023 11:54:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:57c39c08bbf544370ee603edc8311c0ae6ae5544b2e36b00f992a4c7d61979ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37098308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee328258fcaccf097e36c2041f5623138c3e45fba88ae8fb0a2346b4a7abff8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:36:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 20:36:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 20:36:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 20:36:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 20:36:46 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 20:36:46 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 20:36:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 20:36:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 20:36:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67d14d16729f6a29d5643e5739ce8f277db88c76e8576b74466bed71e9614a3`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667f3b336a76ba92a985040ecc81f1e4b96ab00b9bffb9691d4a0909fee7d70`  
		Last Modified: Tue, 21 Nov 2023 20:36:59 GMT  
		Size: 2.4 MB (2434842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365e0235c5f2467bccbbc07ea82e8e9f2af172d10ad8cb487a501738c975909`  
		Last Modified: Tue, 21 Nov 2023 20:37:00 GMT  
		Size: 5.5 MB (5482590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfecc897f46254770f57aee0cf4c99b9ddfd59416111300bcae84be0bb3661e`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8280277e4e1e138609865f279ff5fef4c40a0bb4f48d2230459299b00d656ad0`  
		Last Modified: Tue, 21 Nov 2023 20:36:58 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:c2feb65880bc509150accfd419e6813f14627257be2627bbe31de9a5184a5e0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38697733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36feabcb5b8aebe526989cb605bfe36f6ba227f20c4202055c68d66994900b1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Wed, 22 Nov 2023 01:09:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 22 Nov 2023 01:09:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:09:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 22 Nov 2023 01:09:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 22 Nov 2023 01:09:56 GMT
VOLUME [/spiped]
# Wed, 22 Nov 2023 01:09:56 GMT
WORKDIR /spiped
# Wed, 22 Nov 2023 01:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 22 Nov 2023 01:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Nov 2023 01:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d9077e40b47c5791b4ac20b24d8deff63a5dc8bf5207083f56177fda752514`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e71210812cdeec1bdcbcdc0d631c3eadb6ea9c8b9858c611a0182299588731`  
		Last Modified: Wed, 22 Nov 2023 01:10:13 GMT  
		Size: 2.6 MB (2588158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f18e97e0027d314fc775390b955ca68e6a4cc69d6077de1fc07ccefcd18758f`  
		Last Modified: Wed, 22 Nov 2023 01:10:14 GMT  
		Size: 5.9 MB (5943867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48894c0f6daf466b673d54c1f3536c05d1e8de633a2a517c55a0946adfc311ec`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c404496be4d3107996737e0d3b4b2b5766ee34e42c1a7e6961de6efcec4dde`  
		Last Modified: Wed, 22 Nov 2023 01:10:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:0d61d0a1ea5ac2651b170d9096365703860743a0df774ddcdc327b0915c4544f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36783306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287250c56678b233b997a1c6059e730e147815a68e1df4f12eda08a5eed1ebe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:42:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 16:42:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 16:44:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 16:44:19 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 16:44:22 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 16:44:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 16:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ff2608f3497720032e30b79ae5d65cfa2c8dd359565c1c8dd638f5b3a6f0d`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab7308e1ec6dfefbe63dcd0ffdd71389fcdc64536e65a12a0d4e0b039458285`  
		Last Modified: Tue, 21 Nov 2023 16:44:46 GMT  
		Size: 1.8 MB (1834326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bede55fcddef2dca32fd1854933f48d44eb852b04607b5ca0ee5f0ceede864c`  
		Last Modified: Tue, 21 Nov 2023 16:44:49 GMT  
		Size: 5.8 MB (5805479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8ac4180d595ed6276f96e62a762ce81e1cbc8d5adb99021d674d703250377a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6377814988f39cd05c902f86328248c9751a1903ed8401e8827bf7540cc4a`  
		Last Modified: Tue, 21 Nov 2023 16:44:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:99a36d31339087c56743fcd7b09255be818296337c1ee9b0b9e5caa4d6d2a629
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42336939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbf18f5d582e136651ca47bbf5c8553330ac36b69e4beb1e957d147dbc321fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:49:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 12:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:49:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 12:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:49:48 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 12:49:48 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 12:49:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 12:49:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e3e9a6e83461086d799b3c35e7086e930106125c74069a1510c25bdb6afb6d`  
		Last Modified: Tue, 21 Nov 2023 12:50:01 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956ee3303181032f855a7b2887c1bdca6910e0cb1ec3c92b65d6509c2f907abb`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 2.8 MB (2770520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ddbd7552dcc1e8096f1f690fb7a8f6d94f6b14b70ac7c130e5224ccc99ae5`  
		Last Modified: Tue, 21 Nov 2023 12:50:03 GMT  
		Size: 6.4 MB (6423216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acdb31d4ba61d5a1503eb5bf6cd716ec162f811fe2c79c2ff5c2e727033efc0`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da63bf7cb4ff2b34de84cd9caefa0d255c9965665b50f421172e3d96c2ee315a`  
		Last Modified: Tue, 21 Nov 2023 12:50:02 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:e55796d4c561e3f8eec223e5e69fb5d024ac8574c4aace38477a60420ff5414c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35164381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ea59dc57dc93fac49f303c8c58d6d153d1c8a8ffab3500ff5649eb63c8b568`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:54:15 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Nov 2023 05:54:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl3 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:54:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 21 Nov 2023 05:54:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:54:34 GMT
VOLUME [/spiped]
# Tue, 21 Nov 2023 05:54:34 GMT
WORKDIR /spiped
# Tue, 21 Nov 2023 05:54:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Nov 2023 05:54:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a1488c1c72f51fc67f2f92a4266ad144068e6265f09a6854a0edda69d1e634`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850f941b1cd09719d174b6a90cb013528879a956734598472118c9ba95f4f146`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 2.3 MB (2262458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647d17c59a394362c94984e56f3babc4addd9e026c843bede6b3b295b4b9439c`  
		Last Modified: Tue, 21 Nov 2023 05:54:55 GMT  
		Size: 5.4 MB (5387438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5763b7fbe5d4e9c3ba3f58020db82f8a9bba3e6a9a702f785249dd13161a253b`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d519c5ded3c9d38ab8b28f40d83037fc367671ed767a048f773b935af62381f`  
		Last Modified: Tue, 21 Nov 2023 05:54:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
