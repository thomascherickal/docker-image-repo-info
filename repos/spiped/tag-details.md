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
$ docker pull spiped@sha256:73c463bbbd5f620dbb1aa0ab91b6f7973c8579ba6d720f3642f9b1550c8cca95
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
$ docker pull spiped@sha256:56621f2fd5b22773d7a82548848c99caa44d7526774fccbff6db3e6cf6e2ed7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc63c886e4bd1a4b9a2c5f65cb983191d831e4c5e90b709a27b7ad0468306b5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:13:47 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 11:13:49 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 11:13:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 11:13:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 11:13:57 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 11:13:57 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 11:13:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 11:13:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 11:13:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3d326b144045f9766875844acf4350469a75b0a68c61aab0f7ff911f87c40`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39220be7b9073c1b18c05a3956edc927bf596eaf0d654d7b0056fd406cb2a9d9`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 1.2 MB (1236778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2272caa48ca2695c3ee259c5049bda74ac674fc0349ffce0eb63c15cbcfb373b`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 205.9 KB (205868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c103f3bdb7f64e2684703c5f2a8310fa523b4b883c094984d24a0953897db969`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af16d05b1bfd95db714b4710e950d578ad3ded205b96654b373384e99c72a64`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e20e033984b23e87d819762aa3be4ac888c7573b1fe380a37edc231668cabab1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4266186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f75811072665665f41fe5fd77242815ccd7ba1ada919ff4d133df4c010228f82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:09:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:09:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:09:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:09:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:09:21 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:09:21 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:09:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:09:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d776ef4d306aa7de299bd8db61e455d766a093b7f593b4cb003b7c7436d79d6b`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80582de4f02357b676b2af9cdb5e56aa702680fd50254af56c20b451949c4efb`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 1.2 MB (1163890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4fd5daf33693bf1e78930cd893f86c3b358b42b11140bad181d50be0636580`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 199.5 KB (199547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a963f13cfdeafcdd2c65f6a266762a0e9f1679aeba08b0ebe2f515f4188753`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfc83b30d29a5ba12424db7d486ed08e84ab517be2c9518f1cde49bb01a6853`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b7bbfd15a130193c126e6305dde27ab1f812b1bde9bcdce939a472c991928997
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4913154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a827ded63ac80140d8297b83d5b15fbe600917d04d811f7a104d5a81a45446f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:28:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:28:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:28:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:28:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:28:50 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:28:50 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:28:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:28:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:28:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329a00b6b0251227c993c68fbac4ca61cbf6db9b390d4c9dfe2a005132c2c753`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29c1951c258ad0eb59a0d4d33d432578b0760a47bef312a1e5bf8cccf477f47`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 1.4 MB (1362693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733da67e58e7549c947540df4ff581a3d9297a816340ca183083f623809e34bc`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f459526992eea15e16c15645ca376ef0435b204fc518f1fc404a1a1e2ebec6fc`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a81f75355f25a9bd668c3d651a02f8124af05c3fa0dfb1e2265074389ca80`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:f975a9f3d41c92bff597add76b603827306ff8055d25df0b20f1186aa29b952c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4826091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c779ff3e48cf1e88a23dff62390543e9e2ab6c1b75a812f8d5dfa915323f58d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:03:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:03:26 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:03:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:03:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:03:39 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:03:39 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:03:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:03:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:03:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b1d22c178557ad5427b2e2e39899f1ac5e8a7d3cbdbccccd75d44ef6c2ac2a`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f618f916fa34a39758083d0aea4bb87b1a9ac184745b09c642b66a0771671`  
		Last Modified: Fri, 01 Dec 2023 09:03:53 GMT  
		Size: 1.4 MB (1353891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88db827583d93974059d468003fccdeccfdcd9a21fc15a9286c04d5162b60f00`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 231.6 KB (231631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75849bdf81842f9eff8ef36f098d4df3977533d63126bd042ce3dbf0feb91482`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b858156e16033fc7497c09956fac005c37a0f152b38074431dd9e5bf0d25ce`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:81cf97596c96bf2c8a7f16eec43b20e866143ae03a0cf8161f1f48263918269c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a86b6487c29a72435af58323fd6eb163641668280416e87e7ee28eb55ea2b72d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:20:53 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:20:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:20:58 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:21:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:21:15 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:21:19 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:21:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:21:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:21:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9351f6531fdc8fd4540a86dac5a66a5860f3985ed2e1e145f0eefecf312a4fc0`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041f2592c836041c592a462e184775818c484807025efe56ec1473d2b13465d0`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 1.4 MB (1361751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015f71b1afe6f19e25c6412567f2ad476a7153baa201b4d75943e2cf9a041475`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 220.0 KB (220038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b30773a6064abc0c64614a42aca7bb8a0357867cd6ff0810d45240ab0de638`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edff0700419d6610c5b04cf162c75c7bccadfc322ab5c27f670963d1e7b1165`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f8bed32d8fdba1fdb13b94080f008c65343ad2b3f05ae4cfffa6668cbe5eb52d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4649318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38c98b6934770e5e69df9564d2c52b9f16c900aa31148984cc7a432c75a5f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:48:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 08:48:25 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 08:48:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 08:48:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 08:48:31 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 08:48:31 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 08:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 08:48:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 08:48:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b69c2be0d2e048804506af3efc37e709bf98661c409d99087d1184f0304631`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae960024d613c1bc136f3ae0b33c9fa92f11bdf496d5a2a40fe6c46f1132e06f`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 1.2 MB (1221481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c1ec3a08579d63b87f03caf7152bed9ee8fda71ebaa41c5f0565b423dd6ec1`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 208.6 KB (208647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613853307ecba30c7c7f935ec69ed6aab0e74d6f261598b8e3504b156232c4ef`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c380a4795962e93d6ce5552fe1957ccbb666076846f911fe97fc8aa3b9513ec`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 337.0 B  
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
$ docker pull spiped@sha256:73c463bbbd5f620dbb1aa0ab91b6f7973c8579ba6d720f3642f9b1550c8cca95
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
$ docker pull spiped@sha256:56621f2fd5b22773d7a82548848c99caa44d7526774fccbff6db3e6cf6e2ed7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc63c886e4bd1a4b9a2c5f65cb983191d831e4c5e90b709a27b7ad0468306b5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:13:47 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 11:13:49 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 11:13:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 11:13:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 11:13:57 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 11:13:57 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 11:13:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 11:13:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 11:13:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3d326b144045f9766875844acf4350469a75b0a68c61aab0f7ff911f87c40`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39220be7b9073c1b18c05a3956edc927bf596eaf0d654d7b0056fd406cb2a9d9`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 1.2 MB (1236778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2272caa48ca2695c3ee259c5049bda74ac674fc0349ffce0eb63c15cbcfb373b`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 205.9 KB (205868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c103f3bdb7f64e2684703c5f2a8310fa523b4b883c094984d24a0953897db969`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af16d05b1bfd95db714b4710e950d578ad3ded205b96654b373384e99c72a64`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e20e033984b23e87d819762aa3be4ac888c7573b1fe380a37edc231668cabab1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4266186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f75811072665665f41fe5fd77242815ccd7ba1ada919ff4d133df4c010228f82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:09:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:09:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:09:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:09:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:09:21 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:09:21 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:09:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:09:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d776ef4d306aa7de299bd8db61e455d766a093b7f593b4cb003b7c7436d79d6b`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80582de4f02357b676b2af9cdb5e56aa702680fd50254af56c20b451949c4efb`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 1.2 MB (1163890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4fd5daf33693bf1e78930cd893f86c3b358b42b11140bad181d50be0636580`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 199.5 KB (199547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a963f13cfdeafcdd2c65f6a266762a0e9f1679aeba08b0ebe2f515f4188753`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfc83b30d29a5ba12424db7d486ed08e84ab517be2c9518f1cde49bb01a6853`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b7bbfd15a130193c126e6305dde27ab1f812b1bde9bcdce939a472c991928997
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4913154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a827ded63ac80140d8297b83d5b15fbe600917d04d811f7a104d5a81a45446f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:28:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:28:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:28:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:28:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:28:50 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:28:50 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:28:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:28:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:28:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329a00b6b0251227c993c68fbac4ca61cbf6db9b390d4c9dfe2a005132c2c753`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29c1951c258ad0eb59a0d4d33d432578b0760a47bef312a1e5bf8cccf477f47`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 1.4 MB (1362693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733da67e58e7549c947540df4ff581a3d9297a816340ca183083f623809e34bc`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f459526992eea15e16c15645ca376ef0435b204fc518f1fc404a1a1e2ebec6fc`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a81f75355f25a9bd668c3d651a02f8124af05c3fa0dfb1e2265074389ca80`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:f975a9f3d41c92bff597add76b603827306ff8055d25df0b20f1186aa29b952c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4826091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c779ff3e48cf1e88a23dff62390543e9e2ab6c1b75a812f8d5dfa915323f58d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:03:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:03:26 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:03:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:03:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:03:39 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:03:39 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:03:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:03:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:03:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b1d22c178557ad5427b2e2e39899f1ac5e8a7d3cbdbccccd75d44ef6c2ac2a`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f618f916fa34a39758083d0aea4bb87b1a9ac184745b09c642b66a0771671`  
		Last Modified: Fri, 01 Dec 2023 09:03:53 GMT  
		Size: 1.4 MB (1353891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88db827583d93974059d468003fccdeccfdcd9a21fc15a9286c04d5162b60f00`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 231.6 KB (231631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75849bdf81842f9eff8ef36f098d4df3977533d63126bd042ce3dbf0feb91482`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b858156e16033fc7497c09956fac005c37a0f152b38074431dd9e5bf0d25ce`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:81cf97596c96bf2c8a7f16eec43b20e866143ae03a0cf8161f1f48263918269c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a86b6487c29a72435af58323fd6eb163641668280416e87e7ee28eb55ea2b72d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:20:53 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:20:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:20:58 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:21:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:21:15 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:21:19 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:21:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:21:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:21:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9351f6531fdc8fd4540a86dac5a66a5860f3985ed2e1e145f0eefecf312a4fc0`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041f2592c836041c592a462e184775818c484807025efe56ec1473d2b13465d0`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 1.4 MB (1361751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015f71b1afe6f19e25c6412567f2ad476a7153baa201b4d75943e2cf9a041475`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 220.0 KB (220038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b30773a6064abc0c64614a42aca7bb8a0357867cd6ff0810d45240ab0de638`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edff0700419d6610c5b04cf162c75c7bccadfc322ab5c27f670963d1e7b1165`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f8bed32d8fdba1fdb13b94080f008c65343ad2b3f05ae4cfffa6668cbe5eb52d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4649318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38c98b6934770e5e69df9564d2c52b9f16c900aa31148984cc7a432c75a5f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:48:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 08:48:25 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 08:48:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 08:48:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 08:48:31 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 08:48:31 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 08:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 08:48:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 08:48:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b69c2be0d2e048804506af3efc37e709bf98661c409d99087d1184f0304631`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae960024d613c1bc136f3ae0b33c9fa92f11bdf496d5a2a40fe6c46f1132e06f`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 1.2 MB (1221481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c1ec3a08579d63b87f03caf7152bed9ee8fda71ebaa41c5f0565b423dd6ec1`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 208.6 KB (208647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613853307ecba30c7c7f935ec69ed6aab0e74d6f261598b8e3504b156232c4ef`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c380a4795962e93d6ce5552fe1957ccbb666076846f911fe97fc8aa3b9513ec`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 337.0 B  
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
$ docker pull spiped@sha256:73c463bbbd5f620dbb1aa0ab91b6f7973c8579ba6d720f3642f9b1550c8cca95
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
$ docker pull spiped@sha256:56621f2fd5b22773d7a82548848c99caa44d7526774fccbff6db3e6cf6e2ed7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc63c886e4bd1a4b9a2c5f65cb983191d831e4c5e90b709a27b7ad0468306b5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:13:47 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 11:13:49 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 11:13:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 11:13:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 11:13:57 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 11:13:57 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 11:13:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 11:13:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 11:13:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3d326b144045f9766875844acf4350469a75b0a68c61aab0f7ff911f87c40`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39220be7b9073c1b18c05a3956edc927bf596eaf0d654d7b0056fd406cb2a9d9`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 1.2 MB (1236778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2272caa48ca2695c3ee259c5049bda74ac674fc0349ffce0eb63c15cbcfb373b`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 205.9 KB (205868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c103f3bdb7f64e2684703c5f2a8310fa523b4b883c094984d24a0953897db969`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af16d05b1bfd95db714b4710e950d578ad3ded205b96654b373384e99c72a64`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e20e033984b23e87d819762aa3be4ac888c7573b1fe380a37edc231668cabab1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4266186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f75811072665665f41fe5fd77242815ccd7ba1ada919ff4d133df4c010228f82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:09:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:09:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:09:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:09:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:09:21 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:09:21 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:09:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:09:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d776ef4d306aa7de299bd8db61e455d766a093b7f593b4cb003b7c7436d79d6b`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80582de4f02357b676b2af9cdb5e56aa702680fd50254af56c20b451949c4efb`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 1.2 MB (1163890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4fd5daf33693bf1e78930cd893f86c3b358b42b11140bad181d50be0636580`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 199.5 KB (199547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a963f13cfdeafcdd2c65f6a266762a0e9f1679aeba08b0ebe2f515f4188753`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfc83b30d29a5ba12424db7d486ed08e84ab517be2c9518f1cde49bb01a6853`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b7bbfd15a130193c126e6305dde27ab1f812b1bde9bcdce939a472c991928997
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4913154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a827ded63ac80140d8297b83d5b15fbe600917d04d811f7a104d5a81a45446f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:28:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:28:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:28:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:28:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:28:50 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:28:50 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:28:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:28:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:28:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329a00b6b0251227c993c68fbac4ca61cbf6db9b390d4c9dfe2a005132c2c753`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29c1951c258ad0eb59a0d4d33d432578b0760a47bef312a1e5bf8cccf477f47`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 1.4 MB (1362693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733da67e58e7549c947540df4ff581a3d9297a816340ca183083f623809e34bc`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f459526992eea15e16c15645ca376ef0435b204fc518f1fc404a1a1e2ebec6fc`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a81f75355f25a9bd668c3d651a02f8124af05c3fa0dfb1e2265074389ca80`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:f975a9f3d41c92bff597add76b603827306ff8055d25df0b20f1186aa29b952c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4826091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c779ff3e48cf1e88a23dff62390543e9e2ab6c1b75a812f8d5dfa915323f58d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:03:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:03:26 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:03:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:03:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:03:39 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:03:39 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:03:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:03:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:03:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b1d22c178557ad5427b2e2e39899f1ac5e8a7d3cbdbccccd75d44ef6c2ac2a`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f618f916fa34a39758083d0aea4bb87b1a9ac184745b09c642b66a0771671`  
		Last Modified: Fri, 01 Dec 2023 09:03:53 GMT  
		Size: 1.4 MB (1353891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88db827583d93974059d468003fccdeccfdcd9a21fc15a9286c04d5162b60f00`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 231.6 KB (231631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75849bdf81842f9eff8ef36f098d4df3977533d63126bd042ce3dbf0feb91482`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b858156e16033fc7497c09956fac005c37a0f152b38074431dd9e5bf0d25ce`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:81cf97596c96bf2c8a7f16eec43b20e866143ae03a0cf8161f1f48263918269c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a86b6487c29a72435af58323fd6eb163641668280416e87e7ee28eb55ea2b72d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:20:53 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:20:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:20:58 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:21:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:21:15 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:21:19 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:21:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:21:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:21:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9351f6531fdc8fd4540a86dac5a66a5860f3985ed2e1e145f0eefecf312a4fc0`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041f2592c836041c592a462e184775818c484807025efe56ec1473d2b13465d0`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 1.4 MB (1361751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015f71b1afe6f19e25c6412567f2ad476a7153baa201b4d75943e2cf9a041475`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 220.0 KB (220038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b30773a6064abc0c64614a42aca7bb8a0357867cd6ff0810d45240ab0de638`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edff0700419d6610c5b04cf162c75c7bccadfc322ab5c27f670963d1e7b1165`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f8bed32d8fdba1fdb13b94080f008c65343ad2b3f05ae4cfffa6668cbe5eb52d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4649318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38c98b6934770e5e69df9564d2c52b9f16c900aa31148984cc7a432c75a5f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:48:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 08:48:25 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 08:48:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 08:48:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 08:48:31 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 08:48:31 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 08:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 08:48:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 08:48:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b69c2be0d2e048804506af3efc37e709bf98661c409d99087d1184f0304631`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae960024d613c1bc136f3ae0b33c9fa92f11bdf496d5a2a40fe6c46f1132e06f`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 1.2 MB (1221481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c1ec3a08579d63b87f03caf7152bed9ee8fda71ebaa41c5f0565b423dd6ec1`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 208.6 KB (208647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613853307ecba30c7c7f935ec69ed6aab0e74d6f261598b8e3504b156232c4ef`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c380a4795962e93d6ce5552fe1957ccbb666076846f911fe97fc8aa3b9513ec`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:73c463bbbd5f620dbb1aa0ab91b6f7973c8579ba6d720f3642f9b1550c8cca95
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
$ docker pull spiped@sha256:56621f2fd5b22773d7a82548848c99caa44d7526774fccbff6db3e6cf6e2ed7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc63c886e4bd1a4b9a2c5f65cb983191d831e4c5e90b709a27b7ad0468306b5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:13:47 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 11:13:49 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 11:13:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 11:13:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 11:13:57 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 11:13:57 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 11:13:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 11:13:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 11:13:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3d326b144045f9766875844acf4350469a75b0a68c61aab0f7ff911f87c40`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39220be7b9073c1b18c05a3956edc927bf596eaf0d654d7b0056fd406cb2a9d9`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 1.2 MB (1236778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2272caa48ca2695c3ee259c5049bda74ac674fc0349ffce0eb63c15cbcfb373b`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 205.9 KB (205868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c103f3bdb7f64e2684703c5f2a8310fa523b4b883c094984d24a0953897db969`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af16d05b1bfd95db714b4710e950d578ad3ded205b96654b373384e99c72a64`  
		Last Modified: Fri, 01 Dec 2023 11:14:06 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e20e033984b23e87d819762aa3be4ac888c7573b1fe380a37edc231668cabab1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4266186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f75811072665665f41fe5fd77242815ccd7ba1ada919ff4d133df4c010228f82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:09:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:09:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:09:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:09:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:09:21 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:09:21 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:09:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:09:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d776ef4d306aa7de299bd8db61e455d766a093b7f593b4cb003b7c7436d79d6b`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80582de4f02357b676b2af9cdb5e56aa702680fd50254af56c20b451949c4efb`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 1.2 MB (1163890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4fd5daf33693bf1e78930cd893f86c3b358b42b11140bad181d50be0636580`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 199.5 KB (199547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a963f13cfdeafcdd2c65f6a266762a0e9f1679aeba08b0ebe2f515f4188753`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfc83b30d29a5ba12424db7d486ed08e84ab517be2c9518f1cde49bb01a6853`  
		Last Modified: Fri, 01 Dec 2023 09:09:31 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b7bbfd15a130193c126e6305dde27ab1f812b1bde9bcdce939a472c991928997
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4913154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a827ded63ac80140d8297b83d5b15fbe600917d04d811f7a104d5a81a45446f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:28:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:28:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:28:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:28:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:28:50 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:28:50 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:28:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:28:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:28:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329a00b6b0251227c993c68fbac4ca61cbf6db9b390d4c9dfe2a005132c2c753`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29c1951c258ad0eb59a0d4d33d432578b0760a47bef312a1e5bf8cccf477f47`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 1.4 MB (1362693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733da67e58e7549c947540df4ff581a3d9297a816340ca183083f623809e34bc`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f459526992eea15e16c15645ca376ef0435b204fc518f1fc404a1a1e2ebec6fc`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a81f75355f25a9bd668c3d651a02f8124af05c3fa0dfb1e2265074389ca80`  
		Last Modified: Fri, 01 Dec 2023 09:29:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:f975a9f3d41c92bff597add76b603827306ff8055d25df0b20f1186aa29b952c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4826091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c779ff3e48cf1e88a23dff62390543e9e2ab6c1b75a812f8d5dfa915323f58d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:03:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:03:26 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:03:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:03:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:03:39 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:03:39 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:03:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:03:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:03:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b1d22c178557ad5427b2e2e39899f1ac5e8a7d3cbdbccccd75d44ef6c2ac2a`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f618f916fa34a39758083d0aea4bb87b1a9ac184745b09c642b66a0771671`  
		Last Modified: Fri, 01 Dec 2023 09:03:53 GMT  
		Size: 1.4 MB (1353891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88db827583d93974059d468003fccdeccfdcd9a21fc15a9286c04d5162b60f00`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 231.6 KB (231631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75849bdf81842f9eff8ef36f098d4df3977533d63126bd042ce3dbf0feb91482`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b858156e16033fc7497c09956fac005c37a0f152b38074431dd9e5bf0d25ce`  
		Last Modified: Fri, 01 Dec 2023 09:03:52 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:81cf97596c96bf2c8a7f16eec43b20e866143ae03a0cf8161f1f48263918269c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a86b6487c29a72435af58323fd6eb163641668280416e87e7ee28eb55ea2b72d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:20:53 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 09:20:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 09:20:58 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 09:21:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 09:21:15 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 09:21:19 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 09:21:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 09:21:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 09:21:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9351f6531fdc8fd4540a86dac5a66a5860f3985ed2e1e145f0eefecf312a4fc0`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041f2592c836041c592a462e184775818c484807025efe56ec1473d2b13465d0`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 1.4 MB (1361751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015f71b1afe6f19e25c6412567f2ad476a7153baa201b4d75943e2cf9a041475`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 220.0 KB (220038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b30773a6064abc0c64614a42aca7bb8a0357867cd6ff0810d45240ab0de638`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edff0700419d6610c5b04cf162c75c7bccadfc322ab5c27f670963d1e7b1165`  
		Last Modified: Fri, 01 Dec 2023 09:21:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f8bed32d8fdba1fdb13b94080f008c65343ad2b3f05ae4cfffa6668cbe5eb52d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4649318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38c98b6934770e5e69df9564d2c52b9f16c900aa31148984cc7a432c75a5f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:48:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 01 Dec 2023 08:48:25 GMT
RUN apk add --no-cache libssl1.1
# Fri, 01 Dec 2023 08:48:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 01 Dec 2023 08:48:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Fri, 01 Dec 2023 08:48:31 GMT
VOLUME [/spiped]
# Fri, 01 Dec 2023 08:48:31 GMT
WORKDIR /spiped
# Fri, 01 Dec 2023 08:48:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 01 Dec 2023 08:48:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 08:48:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b69c2be0d2e048804506af3efc37e709bf98661c409d99087d1184f0304631`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae960024d613c1bc136f3ae0b33c9fa92f11bdf496d5a2a40fe6c46f1132e06f`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 1.2 MB (1221481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c1ec3a08579d63b87f03caf7152bed9ee8fda71ebaa41c5f0565b423dd6ec1`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 208.6 KB (208647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613853307ecba30c7c7f935ec69ed6aab0e74d6f261598b8e3504b156232c4ef`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c380a4795962e93d6ce5552fe1957ccbb666076846f911fe97fc8aa3b9513ec`  
		Last Modified: Fri, 01 Dec 2023 08:48:47 GMT  
		Size: 337.0 B  
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
