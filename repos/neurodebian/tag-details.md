<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neurodebian`

-	[`neurodebian:bionic`](#neurodebianbionic)
-	[`neurodebian:bionic-non-free`](#neurodebianbionic-non-free)
-	[`neurodebian:bookworm`](#neurodebianbookworm)
-	[`neurodebian:bookworm-non-free`](#neurodebianbookworm-non-free)
-	[`neurodebian:bullseye`](#neurodebianbullseye)
-	[`neurodebian:bullseye-non-free`](#neurodebianbullseye-non-free)
-	[`neurodebian:buster`](#neurodebianbuster)
-	[`neurodebian:buster-non-free`](#neurodebianbuster-non-free)
-	[`neurodebian:focal`](#neurodebianfocal)
-	[`neurodebian:focal-non-free`](#neurodebianfocal-non-free)
-	[`neurodebian:jammy`](#neurodebianjammy)
-	[`neurodebian:jammy-non-free`](#neurodebianjammy-non-free)
-	[`neurodebian:latest`](#neurodebianlatest)
-	[`neurodebian:nd`](#neurodebiannd)
-	[`neurodebian:nd-non-free`](#neurodebiannd-non-free)
-	[`neurodebian:nd100`](#neurodebiannd100)
-	[`neurodebian:nd100-non-free`](#neurodebiannd100-non-free)
-	[`neurodebian:nd110`](#neurodebiannd110)
-	[`neurodebian:nd110-non-free`](#neurodebiannd110-non-free)
-	[`neurodebian:nd120`](#neurodebiannd120)
-	[`neurodebian:nd120-non-free`](#neurodebiannd120-non-free)
-	[`neurodebian:nd18.04`](#neurodebiannd1804)
-	[`neurodebian:nd18.04-non-free`](#neurodebiannd1804-non-free)
-	[`neurodebian:nd20.04`](#neurodebiannd2004)
-	[`neurodebian:nd20.04-non-free`](#neurodebiannd2004-non-free)
-	[`neurodebian:nd22.04`](#neurodebiannd2204)
-	[`neurodebian:nd22.04-non-free`](#neurodebiannd2204-non-free)
-	[`neurodebian:non-free`](#neurodebiannon-free)
-	[`neurodebian:sid`](#neurodebiansid)
-	[`neurodebian:sid-non-free`](#neurodebiansid-non-free)

## `neurodebian:bionic`

```console
$ docker pull neurodebian@sha256:e8d04969d017bf258e6f3e3823d029ffa862d189269e840eebf1773ca343ef85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:bionic` - linux; amd64

```console
$ docker pull neurodebian@sha256:a46f35fb0fb8e1d62203cb73a8b9a35304958af2d0da86536680428b3826d6e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31778913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797d9b9af21ae983270561edc6bf2f86d96409f0fa4554d7f312bf28bc98af90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:02:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:02:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 16 May 2023 01:02:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 16 May 2023 01:02:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2372d6e43648bec4df62a3d55e7f95e72243565b07c6d5920d3406d6eefbd5a8`  
		Last Modified: Tue, 16 May 2023 01:03:22 GMT  
		Size: 4.8 MB (4821195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620a82a5993926d5580487c99ad1a0938a9b68875b3c29746a0f4374f50e4ed6`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fb021293ae8fb1060eeeb057accbc60b7390f8cf2b9edfa122e80294f3de7c`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c786576ffd5a24ecad657d482b765f09fa254580fc4d6a4ab147d457f6a89`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 240.3 KB (240297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bionic` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:4d086ea47c67c213bb766b47a3728a21e11f606d760c3a61aa25575f109121cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28387601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1017979b144e550cac6c7ab43aa5f25dc69263722eddfdc4511926239bd89adf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:25:37 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:25:38 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 16 May 2023 01:25:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 16 May 2023 01:25:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592501afdaec24bcc465ef26abc1b7d532782a85c6cbe7893a7fd774b7ddb8c1`  
		Last Modified: Tue, 16 May 2023 01:26:19 GMT  
		Size: 4.4 MB (4403694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e0312aba612c00a457099681cef3a29c3e73ce54ce0e4aac34fdd08b0adfeb`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 1.7 KB (1665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fdfd9ebabe147a93ab87064e56e524fc5ae9821794b68014d92124bd1ce284`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d273709265897dc91aaf15ee076766e0c6660e13254c4aade22b856ed3e5bca`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 241.1 KB (241071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bionic-non-free`

```console
$ docker pull neurodebian@sha256:2740f34f475ff2fd1961eb7b2b58ae91961ef74a6f2d18ff32de78afe60def75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:bionic-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:dd86543f59520f317599a56451050f712c0a117c420e4e6e30cbcc1fb8db8b84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31779170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940ae3002ffa7baadfa10c87d888bb9be5fe56c1d95565f40821ed9ff2b94bea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:02:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:02:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 16 May 2023 01:02:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 16 May 2023 01:02:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:02:42 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2372d6e43648bec4df62a3d55e7f95e72243565b07c6d5920d3406d6eefbd5a8`  
		Last Modified: Tue, 16 May 2023 01:03:22 GMT  
		Size: 4.8 MB (4821195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620a82a5993926d5580487c99ad1a0938a9b68875b3c29746a0f4374f50e4ed6`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fb021293ae8fb1060eeeb057accbc60b7390f8cf2b9edfa122e80294f3de7c`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c786576ffd5a24ecad657d482b765f09fa254580fc4d6a4ab147d457f6a89`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 240.3 KB (240297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd3984fa38330d1b3b2590d00da5c0e2052ec84b96bd48683df7d0fd5bc299b`  
		Last Modified: Tue, 16 May 2023 01:03:29 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bionic-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:51567a48e4ee4ab6244cac21df91a34de9ac8631e64cb62003c3692aaa09b61d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28387860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c879b3d4ab74022bc603e9e94dff0eec069290bf4d4a3de32a44954b0d82dd38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:25:37 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:25:38 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 16 May 2023 01:25:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 16 May 2023 01:25:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:25:47 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592501afdaec24bcc465ef26abc1b7d532782a85c6cbe7893a7fd774b7ddb8c1`  
		Last Modified: Tue, 16 May 2023 01:26:19 GMT  
		Size: 4.4 MB (4403694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e0312aba612c00a457099681cef3a29c3e73ce54ce0e4aac34fdd08b0adfeb`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 1.7 KB (1665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fdfd9ebabe147a93ab87064e56e524fc5ae9821794b68014d92124bd1ce284`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d273709265897dc91aaf15ee076766e0c6660e13254c4aade22b856ed3e5bca`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 241.1 KB (241071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2a8256b93deb2dd3244eaf3d152d923018cd4332060d4a4ec7842e728aae9b`  
		Last Modified: Tue, 16 May 2023 01:26:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm`

```console
$ docker pull neurodebian@sha256:6d11433337327f59e8310b362ced377bb97fadc30760c4d7150030e4a2430381
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm` - linux; amd64

```console
$ docker pull neurodebian@sha256:4bbebb1af3fa42edeb7daa76429594832677c061fbaa59f2176c8cbe40d8b607
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61305663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592dcc4b1cc3783782cfea69d58dcf8a1738781d2842c3849fd90d40df1b899a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:33 GMT
ADD file:168af20819ee8d7bc6ca3fd35873fe0b65f567f6fc4763ae2fed655e04826ef6 in / 
# Tue, 02 May 2023 23:46:33 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:879480f6969a02afb639ba9b35bc2df992fec064538a2e8af5e14cf6b6fbeac3`  
		Last Modified: Tue, 02 May 2023 23:49:26 GMT  
		Size: 49.3 MB (49299247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd09f14e055c828315e856789d20b8946366f27edf267f3902b57215e239d7ef`  
		Last Modified: Wed, 03 May 2023 21:27:34 GMT  
		Size: 11.7 MB (11719796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173622f5d1ba65e0d94854aa9998708f35b2a78b4a0c65ce6ec9cb2d772d4c39`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3666043593436d5565d087183a46b53a6ae13cb63c743b728fd872c3c48aa0e8`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f690a06a4d5ee8090896ae8454bdb93732d1e61586082cd7b596aad4aaf087`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 284.6 KB (284613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:648d84e2d1b843835b3fa399b85eeaf865c48c3be470f229543f63a4c1f56a04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61320411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a9c9e342134ca145b25d98ab14e66f984bda18bcc60e0a0f0141083df122e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:42:54 GMT
ADD file:91184714f613e1768e87fad722350f471376a88cb595664e8e23864ce5d79071 in / 
# Tue, 23 May 2023 00:42:55 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:30:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:30:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:30:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3485dc61c38c6db2e8092e9f4326fe6c51e867a1841f55346f74ec25847d7401`  
		Last Modified: Tue, 23 May 2023 00:45:14 GMT  
		Size: 49.3 MB (49347785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27205be5ff69de2ea80daf475b7d6782f5bd2c4eff02242061f43eaf6012d24`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 11.7 MB (11685619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a91d72189acf1f099b7b4f36d85c03907fb5bacd266f36caa6b04ef2e3fd7fb`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae3bb66bd12fcefd327ecdad94e32054fc3501ea2c5f23a797f919ad31b9bc9`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e899ae9f9f58a47c33891e8ef8311f802cbff074ff152ecd2f6fa34be22900d1`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 285.0 KB (284995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; 386

```console
$ docker pull neurodebian@sha256:a8950e781f0d7e413cb43a35939504243936f723a3362cbfb4579ada1646af1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62752170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0397aab4130cfdd8b1bc6e0c4a66596c8d00e10ba6805e93f72fbdd0f7ea47b7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:17 GMT
ADD file:cd02b45138959c7ec7d466eff66efaa68d03b2e72f294b468f08c576643ac084 in / 
# Wed, 03 May 2023 00:00:18 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:17:02 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:04 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:17:04 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:17:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:028db28caf3d2a0b3bc8b8281c9f370a6ca8a97954f596e2b27e20ebf7f3b578`  
		Last Modified: Wed, 03 May 2023 00:04:07 GMT  
		Size: 50.3 MB (50321827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa3f2ae1595f6575bfc69faed0d539bf88a71f81033a72dd7cd6a6b16533a26`  
		Last Modified: Wed, 03 May 2023 23:18:26 GMT  
		Size: 12.1 MB (12143607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030d5cafe5a4885634636dec550fa431c5d4332902b7fa1e592504eb10cb4698`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc4a181c2202a0f49007cfb365321e0dc3352e79f05f6028e41b534da7b6018`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b687257037f8146aecaffcb99f883d553e938ba2d1635186ff1fde12e64952d8`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 284.7 KB (284726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm-non-free`

```console
$ docker pull neurodebian@sha256:9297ea57c8e4c3f13f28668610b9ae587a610d42b430898b1819d0b02a50f882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:d52d4af080b7f4a4e2587186062e52d88603493ad425402cf20c95c0b116a2ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3e6a45d91905bfd06f5fbdcba0eab1a5024f5f049356cec05dd240eaaf04d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:33 GMT
ADD file:168af20819ee8d7bc6ca3fd35873fe0b65f567f6fc4763ae2fed655e04826ef6 in / 
# Tue, 02 May 2023 23:46:33 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:56 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:879480f6969a02afb639ba9b35bc2df992fec064538a2e8af5e14cf6b6fbeac3`  
		Last Modified: Tue, 02 May 2023 23:49:26 GMT  
		Size: 49.3 MB (49299247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd09f14e055c828315e856789d20b8946366f27edf267f3902b57215e239d7ef`  
		Last Modified: Wed, 03 May 2023 21:27:34 GMT  
		Size: 11.7 MB (11719796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173622f5d1ba65e0d94854aa9998708f35b2a78b4a0c65ce6ec9cb2d772d4c39`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3666043593436d5565d087183a46b53a6ae13cb63c743b728fd872c3c48aa0e8`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f690a06a4d5ee8090896ae8454bdb93732d1e61586082cd7b596aad4aaf087`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 284.6 KB (284613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5ffbe0a5537ef8771e9443b26e7da93ca8f8f2a26af66c24911e7d5259053a`  
		Last Modified: Wed, 03 May 2023 21:27:41 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:b69bfc4ed29a6d42fb7f32af35e35b1635ad6ed11266fabae4dead54f1adffc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61320839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:778d928a3fee1ce61884892a6b7f775f1089f3724facee289f262e14452a8abf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:42:54 GMT
ADD file:91184714f613e1768e87fad722350f471376a88cb595664e8e23864ce5d79071 in / 
# Tue, 23 May 2023 00:42:55 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:30:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:30:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:30:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:3485dc61c38c6db2e8092e9f4326fe6c51e867a1841f55346f74ec25847d7401`  
		Last Modified: Tue, 23 May 2023 00:45:14 GMT  
		Size: 49.3 MB (49347785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27205be5ff69de2ea80daf475b7d6782f5bd2c4eff02242061f43eaf6012d24`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 11.7 MB (11685619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a91d72189acf1f099b7b4f36d85c03907fb5bacd266f36caa6b04ef2e3fd7fb`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae3bb66bd12fcefd327ecdad94e32054fc3501ea2c5f23a797f919ad31b9bc9`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e899ae9f9f58a47c33891e8ef8311f802cbff074ff152ecd2f6fa34be22900d1`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 285.0 KB (284995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f11898d17a3e3cea8f36f6751eb691a7fc506a165af741c28422a9e0b52a8e5`  
		Last Modified: Tue, 23 May 2023 02:31:46 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:16cc40944ba50beee287eba7c32319d476c46ee7c1d316ce96367ac84fb64a5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62752596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df71d0bb8af9de01eb06854a17e811ed4938dcce437ab398a47e2992b8a637d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:17 GMT
ADD file:cd02b45138959c7ec7d466eff66efaa68d03b2e72f294b468f08c576643ac084 in / 
# Wed, 03 May 2023 00:00:18 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:17:02 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:04 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:17:04 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:17:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:14 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:028db28caf3d2a0b3bc8b8281c9f370a6ca8a97954f596e2b27e20ebf7f3b578`  
		Last Modified: Wed, 03 May 2023 00:04:07 GMT  
		Size: 50.3 MB (50321827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa3f2ae1595f6575bfc69faed0d539bf88a71f81033a72dd7cd6a6b16533a26`  
		Last Modified: Wed, 03 May 2023 23:18:26 GMT  
		Size: 12.1 MB (12143607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030d5cafe5a4885634636dec550fa431c5d4332902b7fa1e592504eb10cb4698`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc4a181c2202a0f49007cfb365321e0dc3352e79f05f6028e41b534da7b6018`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b687257037f8146aecaffcb99f883d553e938ba2d1635186ff1fde12e64952d8`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 284.7 KB (284726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df75504459b747f4070dddcbeda95a33709c7b6352069c3f655621932713a20`  
		Last Modified: Wed, 03 May 2023 23:18:34 GMT  
		Size: 426.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:d50522f5919d76c352799a16f6ee33cea1110ea1e7b1ba6f61ba4d444e4673c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:a8b160ad81cc7caee38ea9b4ecee4f76acc1063d87bccc3d4676f16b0c1cd3aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b5e10477f27ce6cbba3962cae22f891689c7f08dd7644ff9e66f4996f98de28`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:31 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b9629c74f273da9190027c7e4cc11bf7b9c6a5bc037f53f26812b96307cee1`  
		Last Modified: Wed, 03 May 2023 21:27:14 GMT  
		Size: 11.3 MB (11310941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e479d911c8ceb5e5f2c92b8d68425475e3255bf6caf9fb40846df32dd54750`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b2393d1b1e6ae558b4e42a05a8fbd0a1cb5a6deadd71a2bdaff11b3fb8691d`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103058a946030129417ba0563768d175caae3f6b41f4787c1b86b420cdb7e639`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:8e9a1ffc99ee63822e0d6d473744ca2ad41ef31639f50b2db48affd80c7cee32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65319625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a17259e4c5d36ea6062363803be00e2629bf3ed07156e49ed82adb0c75b262`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:29:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:29:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187c756d024d4e7c2776681889618e1a5149fc672ed0aac61d785f286e69cb45`  
		Last Modified: Tue, 23 May 2023 02:31:19 GMT  
		Size: 11.3 MB (11313121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0227cf7a0eaf0af3c3c1164de31c4c5555f9f5b511769db242fdc93b238f9876`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78eb1f7c1bac7ebaea871680d53583c59acee5339b44ced2f4aa3cb3e1aa6cb`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7532dbe02d3f898678b483d0df372497ea9472a859b411edd0993544bab9cd6c`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 311.9 KB (311882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; 386

```console
$ docker pull neurodebian@sha256:50ee6db1dc9787f13d68e670b76ee5bb188abdb37df2eeb108a02993ca515ddc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68050919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae6bd51d8bd61bb7ffc759874939575238eac0ebc86f65e55035ade609fde7c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:45 GMT
ADD file:59d53253d7691be0330c735eb4b57791a8fc5894572d3deaeb7138cce45132ad in / 
# Wed, 03 May 2023 00:00:46 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:16:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:16:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:16:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ac0eb37fce5e6fca952bf804df5de5ebb63724d4d44bf23abc5d5736ee32afd`  
		Last Modified: Wed, 03 May 2023 00:04:44 GMT  
		Size: 56.0 MB (56029150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c794418bd1e96a39bea1aef2c4f245b825ec4e16a1d2fa3222521c51cbe7cd8`  
		Last Modified: Wed, 03 May 2023 23:18:05 GMT  
		Size: 11.7 MB (11707936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e0e0e73c24570aa784364602cf64cd9331769082f140bfa988aad91ce79b9`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6e2c410c8e6b068d6692e30b9d8d56a1e0bf11cf420a3f030fe862b4a566f`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbe2da83496475fac6b9656e8be553e28e545fab227c1cc1c666a89f3141f1b`  
		Last Modified: Wed, 03 May 2023 23:18:04 GMT  
		Size: 311.8 KB (311820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye-non-free`

```console
$ docker pull neurodebian@sha256:0f540c18829c6396c0c23e747525582fa1e7cbbed1540d58be6c9b359e58f23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:0e03b2debd7a1d5f28aa746ae3e4ce140ed6790d63f39f6a5b71521e88769c50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3331ef22a29d7e47c420e4814e93b37e21973c5540cbb66fd17f4fc9a81b223`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:31 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:38 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b9629c74f273da9190027c7e4cc11bf7b9c6a5bc037f53f26812b96307cee1`  
		Last Modified: Wed, 03 May 2023 21:27:14 GMT  
		Size: 11.3 MB (11310941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e479d911c8ceb5e5f2c92b8d68425475e3255bf6caf9fb40846df32dd54750`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b2393d1b1e6ae558b4e42a05a8fbd0a1cb5a6deadd71a2bdaff11b3fb8691d`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103058a946030129417ba0563768d175caae3f6b41f4787c1b86b420cdb7e639`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a786115a54951b49a2de00541f08f3fb81963b0a9827b745be73197ea4ddb51f`  
		Last Modified: Wed, 03 May 2023 21:27:23 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:efc47b01c41eca49e029b269638c650adfd2a8f0e73807c748f9c7bc1f36cbce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65319984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4ebde6630ed604716cbd5f83c480bc3a7e5e2d8cce1d68c1355581fcfcf157`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:29:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:29:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:57 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187c756d024d4e7c2776681889618e1a5149fc672ed0aac61d785f286e69cb45`  
		Last Modified: Tue, 23 May 2023 02:31:19 GMT  
		Size: 11.3 MB (11313121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0227cf7a0eaf0af3c3c1164de31c4c5555f9f5b511769db242fdc93b238f9876`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78eb1f7c1bac7ebaea871680d53583c59acee5339b44ced2f4aa3cb3e1aa6cb`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7532dbe02d3f898678b483d0df372497ea9472a859b411edd0993544bab9cd6c`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 311.9 KB (311882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfc256c442e8e637b8a0cece189d2a76422322f8ee48f5be12c1dce583cbdd2`  
		Last Modified: Tue, 23 May 2023 02:31:28 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:fe3bde78aeb9790898d619b54ac53eb63822edbd4b7823a0984d80631bb65fed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68051278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7adfc07d9da7329f3d6d9ae824556b77b534f5b7c95c239975fbedff4eb071e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:45 GMT
ADD file:59d53253d7691be0330c735eb4b57791a8fc5894572d3deaeb7138cce45132ad in / 
# Wed, 03 May 2023 00:00:46 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:16:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:16:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:16:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:52 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:6ac0eb37fce5e6fca952bf804df5de5ebb63724d4d44bf23abc5d5736ee32afd`  
		Last Modified: Wed, 03 May 2023 00:04:44 GMT  
		Size: 56.0 MB (56029150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c794418bd1e96a39bea1aef2c4f245b825ec4e16a1d2fa3222521c51cbe7cd8`  
		Last Modified: Wed, 03 May 2023 23:18:05 GMT  
		Size: 11.7 MB (11707936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e0e0e73c24570aa784364602cf64cd9331769082f140bfa988aad91ce79b9`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6e2c410c8e6b068d6692e30b9d8d56a1e0bf11cf420a3f030fe862b4a566f`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbe2da83496475fac6b9656e8be553e28e545fab227c1cc1c666a89f3141f1b`  
		Last Modified: Wed, 03 May 2023 23:18:04 GMT  
		Size: 311.8 KB (311820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c5defbdb36be91b752ff0f2512091c04e98799ae0c1c8c8ace8eede4671471`  
		Last Modified: Wed, 03 May 2023 23:18:15 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:44b51fdc7b4248178d4ccb740761403b0b68bdd5561eb0b2c70e8d482ff1fb64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:14859d5c917b06ea663d297456f90292ba40d282f0250c3cfa738f73292630d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61259514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:477c74a581e9ea7f67ce9724de9fc8cf463e08391beb08a301ae72c534f3d88f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:07 GMT
ADD file:d176a72312205fc75b2950df98f4ed25abadd4b053b9d85bea67466a5b30220f in / 
# Tue, 02 May 2023 23:47:08 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:13 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a94073ab46f8d565f5938cc345d32f7adda10a2585e39555079da9d4ee595974`  
		Last Modified: Tue, 02 May 2023 23:50:40 GMT  
		Size: 50.4 MB (50448697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f87762e02dad34eb08994cd86e167edfd44474c49108468eb082ae17364bec7`  
		Last Modified: Wed, 03 May 2023 21:26:56 GMT  
		Size: 10.5 MB (10504492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbda83cc39ef32e5179634236082fd77e94c2021179b379bc60fc6f077b3a80`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada04c68f4b4be2aa312f558542d687e6f998884d6831a2bdee4a124b3a2cf66`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd97b4a7da61a8033aa1a379b164d4f7e19016db0f734d6f6d35ed16e42cfd4`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 304.3 KB (304318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:749db235498965a5f1361bf7f23ce1d0629d6b51d66fdbd75a817837b8169248
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60055122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0492c0aef76c50f117312fd94b88bd6ba0dc7be2214987b1ffa406bf623e5cd1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:21 GMT
ADD file:a5100e7ed3c2665c1b4dfbb32eb2b47b85783f2a6800e0ae9004db0ce021dfa5 in / 
# Tue, 23 May 2023 00:43:22 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:29:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:29:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ea482247e9a0d1ae4ed218fb0828063b9cce53822e64fd4621f587ab85a7e6d`  
		Last Modified: Tue, 23 May 2023 00:46:24 GMT  
		Size: 49.2 MB (49238292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3669f12602d08f0dbf725c5e531299324f34d80aa1333c05e17213b09f9b4f82`  
		Last Modified: Tue, 23 May 2023 02:31:02 GMT  
		Size: 10.5 MB (10510471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35875484f4c75482356db7b88ff96956756ca2ddf9fcf0db615fa7fac9e6795`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dad3d877033dd23fd3219c87d8586351dbe14d7ab3c9fe9c25296df7bbb2901`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1424958f76e02c936033580d62bee2972bde5e1f1a8b6d5c0a8781046a3b37`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 304.4 KB (304350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; 386

```console
$ docker pull neurodebian@sha256:c0fbae788aeae82e38c9733aa4f5732ccef69a616953a913c69e2ece707a4ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62380642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90225822130b7f5284a53b778c0c2b770de586e2d8561342b384b36569cb8823`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:10 GMT
ADD file:d427d53c0d42e21426b53d60a17dd7014d2504084ae758c35f088cee043ff9ed in / 
# Wed, 03 May 2023 00:01:11 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:16:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:16:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:16:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc3c764404274f8a6e2edf459bc863892205283aa5069a204e16cce54455cb83`  
		Last Modified: Wed, 03 May 2023 00:05:33 GMT  
		Size: 51.2 MB (51206158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43844ba53e304f4440b1717d17b7f4739ebd73aaea1b850a3697ccb354ca152b`  
		Last Modified: Wed, 03 May 2023 23:17:48 GMT  
		Size: 10.9 MB (10868216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2599c7f3672a192bf65ce0684c0be96a9a476901c4f5a1f5fdad43d3f14250`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e99eacf5db7dc7bf3ebc61365890bf33ee0892276ba2c0681514f7e6e457792`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ca39efb9f207d4de5ab6495531fa5fbc3cfe9d73d19ccc4ca83e73a7d29e6f`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 304.3 KB (304255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:f4a5c204470a35db95ee5fae5aa1924d7b8dfb31aeb46d3abba33c6af31f7965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:3c0e2236cddaca2f0f0fae30da44146a0bafc3de4555d70dbf48bdc11ffd6263
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61259872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d79f353601fa8661f09c7864b043a90ffe8c169b228b249899f3666aa4a9c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:07 GMT
ADD file:d176a72312205fc75b2950df98f4ed25abadd4b053b9d85bea67466a5b30220f in / 
# Tue, 02 May 2023 23:47:08 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:13 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a94073ab46f8d565f5938cc345d32f7adda10a2585e39555079da9d4ee595974`  
		Last Modified: Tue, 02 May 2023 23:50:40 GMT  
		Size: 50.4 MB (50448697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f87762e02dad34eb08994cd86e167edfd44474c49108468eb082ae17364bec7`  
		Last Modified: Wed, 03 May 2023 21:26:56 GMT  
		Size: 10.5 MB (10504492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbda83cc39ef32e5179634236082fd77e94c2021179b379bc60fc6f077b3a80`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada04c68f4b4be2aa312f558542d687e6f998884d6831a2bdee4a124b3a2cf66`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd97b4a7da61a8033aa1a379b164d4f7e19016db0f734d6f6d35ed16e42cfd4`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 304.3 KB (304318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b9a9a523f32160714296229f8f14f21b13da05df951a196f2f47cfa5c19b45`  
		Last Modified: Wed, 03 May 2023 21:27:04 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:d1d384571538549ef9e73096923d7672000b32b10260d4d105c910338942bcbc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60055480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:826fc2babca4e62a146037fa97738c0993582f625ae3657fc35c11f46f10fd4d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:21 GMT
ADD file:a5100e7ed3c2665c1b4dfbb32eb2b47b85783f2a6800e0ae9004db0ce021dfa5 in / 
# Tue, 23 May 2023 00:43:22 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:29:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:29:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:40 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:5ea482247e9a0d1ae4ed218fb0828063b9cce53822e64fd4621f587ab85a7e6d`  
		Last Modified: Tue, 23 May 2023 00:46:24 GMT  
		Size: 49.2 MB (49238292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3669f12602d08f0dbf725c5e531299324f34d80aa1333c05e17213b09f9b4f82`  
		Last Modified: Tue, 23 May 2023 02:31:02 GMT  
		Size: 10.5 MB (10510471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35875484f4c75482356db7b88ff96956756ca2ddf9fcf0db615fa7fac9e6795`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dad3d877033dd23fd3219c87d8586351dbe14d7ab3c9fe9c25296df7bbb2901`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1424958f76e02c936033580d62bee2972bde5e1f1a8b6d5c0a8781046a3b37`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 304.4 KB (304350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5600a1971a0e2142139cffffa014177321f94569310c622a4f530cc99eee5a72`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:b565467f94285936ab3a8d8d852cccba66345b8f508d33946bc4e40011ee2e8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62380998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c27bc0c72ef518da8e561f830d119f105da8970c80685b386314fc6d01a045`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:10 GMT
ADD file:d427d53c0d42e21426b53d60a17dd7014d2504084ae758c35f088cee043ff9ed in / 
# Wed, 03 May 2023 00:01:11 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:16:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:16:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:16:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:35 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:cc3c764404274f8a6e2edf459bc863892205283aa5069a204e16cce54455cb83`  
		Last Modified: Wed, 03 May 2023 00:05:33 GMT  
		Size: 51.2 MB (51206158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43844ba53e304f4440b1717d17b7f4739ebd73aaea1b850a3697ccb354ca152b`  
		Last Modified: Wed, 03 May 2023 23:17:48 GMT  
		Size: 10.9 MB (10868216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2599c7f3672a192bf65ce0684c0be96a9a476901c4f5a1f5fdad43d3f14250`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e99eacf5db7dc7bf3ebc61365890bf33ee0892276ba2c0681514f7e6e457792`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ca39efb9f207d4de5ab6495531fa5fbc3cfe9d73d19ccc4ca83e73a7d29e6f`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 304.3 KB (304255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca7e12a39acbba25b91d9cdab41e4c34f117c2ab0c4843b97340a0ddb97e1e`  
		Last Modified: Wed, 03 May 2023 23:17:56 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal`

```console
$ docker pull neurodebian@sha256:32657efcbe75393aa2da46975fc9ea7bebbbdc9a662f70959161666ea819a6be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:focal` - linux; amd64

```console
$ docker pull neurodebian@sha256:0e666853f7e4a618de58b520e48853965345d292ecd1931a7b71cb7d9d2fb274
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34313750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9038f4da65a7ee359dfa78434fd1b63e9938ba98825954fc79d9622ee72d7c8c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:42:04 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:42:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 18 Apr 2023 02:42:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 18 Apr 2023 02:42:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f6efd2926626473d071a223a349e2958558513cf51fde93090ea8f8883d17`  
		Last Modified: Tue, 18 Apr 2023 02:42:51 GMT  
		Size: 5.5 MB (5494338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ef84ed7d67e739f242b02ac970071100cba403cbfaa24dad8d40f190f86d53`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28598ffa8aad6fab7f3041b2006d4badce4ca24a560a48ca4cebfdcb33016029`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6472897b79c02d388e702cbf72fb1f128887d6e0f72992d276b9efd6c3fa353b`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 238.8 KB (238840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:focal` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:7e6dd01caa3656f152c63c15c2d03951352931a2cd1dbd21a8e62dc581482e5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32913188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630f2a6c42486435d7a35b2b08ac2ed21b2c7d8b905cafb81df9e9860173a5dc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:05:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:05:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 18 Apr 2023 02:05:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 18 Apr 2023 02:05:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c8f2d5b6a6ddaae0b4f84cb3ceb68eed34dfcab84b8bd8122afc877b84d7dc`  
		Last Modified: Tue, 18 Apr 2023 02:06:18 GMT  
		Size: 5.5 MB (5475094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91b40e1b81bc32ccfb31e807d1c37ff604997c2f73eb9c70b8ad2d32e23532b`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6692fe5836ed8f0bc1f41e11c59188de0c38640169128875fc695731c8a64a`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193e8a628fb21472856c5f43baaee3f05120d6d41fafd70e43931807b8c802de`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 239.7 KB (239684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal-non-free`

```console
$ docker pull neurodebian@sha256:50d69a7a5fe6275c281ae09da9a6e7ec62b90917964052cf5acd18c4c41aafd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:focal-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:117345b79c50c024801f9f60799683235ebfd8a5dfa79c45a44e339e21e38064
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34314007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab8d95f59c510bd26eac5af308b128fb87b2f5ddbf858252307dc15d19d8681`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:42:04 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:42:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 18 Apr 2023 02:42:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 18 Apr 2023 02:42:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:42:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f6efd2926626473d071a223a349e2958558513cf51fde93090ea8f8883d17`  
		Last Modified: Tue, 18 Apr 2023 02:42:51 GMT  
		Size: 5.5 MB (5494338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ef84ed7d67e739f242b02ac970071100cba403cbfaa24dad8d40f190f86d53`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28598ffa8aad6fab7f3041b2006d4badce4ca24a560a48ca4cebfdcb33016029`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6472897b79c02d388e702cbf72fb1f128887d6e0f72992d276b9efd6c3fa353b`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 238.8 KB (238840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530d1e2bbd66b9f610d9654ee50e64e8f58b3320e02d7cfd33cd055cf0dcbc96`  
		Last Modified: Tue, 18 Apr 2023 02:42:59 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:focal-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5a1bf55d2e3e46d17acea860b18164edeeedfb50863cc64366489d68d599e48a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32913444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c683e496f7e95c821943a7432fdfe2d641b5605987810896e8a4dab923c2ea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:05:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:05:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 18 Apr 2023 02:05:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 18 Apr 2023 02:05:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:05:49 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c8f2d5b6a6ddaae0b4f84cb3ceb68eed34dfcab84b8bd8122afc877b84d7dc`  
		Last Modified: Tue, 18 Apr 2023 02:06:18 GMT  
		Size: 5.5 MB (5475094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91b40e1b81bc32ccfb31e807d1c37ff604997c2f73eb9c70b8ad2d32e23532b`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6692fe5836ed8f0bc1f41e11c59188de0c38640169128875fc695731c8a64a`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193e8a628fb21472856c5f43baaee3f05120d6d41fafd70e43931807b8c802de`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 239.7 KB (239684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d2f0f07359cd0ea0074415a6b4accbc968f197484bd2872168f4707736a9c1`  
		Last Modified: Tue, 18 Apr 2023 02:06:26 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:jammy`

```console
$ docker pull neurodebian@sha256:63f8ba30ea3872358d3041e9c82f43c2540cbed3ef19f388d495af32b24fa45d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:jammy` - linux; amd64

```console
$ docker pull neurodebian@sha256:d666ee3b477274405fa2c6319d27204f720dea21a2ea159027cc0c9419d17905
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34456563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d9408f22945908b19511f7c931a9b1e4d8a77dc9223d460bead7a16cd2721b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:24:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:24:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:24:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68378f1e43a78d07ba7d4b063f86a4e752c51e3c3914a1ff9f743500f2c2f04`  
		Last Modified: Wed, 03 May 2023 21:26:39 GMT  
		Size: 3.8 MB (3765930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd168bc42e411f97adae10afe4f4653177647bfa55537a25131255844ae61492`  
		Last Modified: Wed, 03 May 2023 21:26:38 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2795c37902804d36644ab4b665f46a0a7cd526cf7843ccb4f01a084f2f61b7f7`  
		Last Modified: Wed, 03 May 2023 21:26:38 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1bb371f422afeb35fe873149a69cd084948e4a52ccd4419517b1844083c725`  
		Last Modified: Wed, 03 May 2023 21:26:39 GMT  
		Size: 258.4 KB (258401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:jammy` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:35c8d1730e274f73b120705d4aea51e53728fd1713d371325489791657df5b80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32388930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8381623266dd094df6c2fe1971091cf1277379ddd899e8ecd057d981039f6ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 19:05:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:05:46 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 19:05:47 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 19:05:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce53cea779733273cf24ec55276dac6cc9c77563b4244ce762d9679e6120250`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 3.7 MB (3738566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ed0729e8a293b6757d2d1e1f3945beb7567375d912abd1eefd688798dd1042`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daab176d4e2a4476e6e1bcef5fb4561c2b05e1c0b3913d2d61cbc02ffe5bb95f`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a285c321748b47e8da6e14e89e40a30db11775c6d6666a0dd2cc2041475d6`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 258.9 KB (258908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:jammy-non-free`

```console
$ docker pull neurodebian@sha256:21a56fb9ba3feb49b92f808c8a8417cbae38c971a650de2839d4f375035d50a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:jammy-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:972c31822cf1c906d237498983db0901dbb707f5dce3f3ff8644b1a59fc87f2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34456820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81b089e33ba1ff9d0a4c5ea7ea02ff345eecf723a5f37e77c3a5f6370d04fb6a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:24:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:24:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:24:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:03 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68378f1e43a78d07ba7d4b063f86a4e752c51e3c3914a1ff9f743500f2c2f04`  
		Last Modified: Wed, 03 May 2023 21:26:39 GMT  
		Size: 3.8 MB (3765930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd168bc42e411f97adae10afe4f4653177647bfa55537a25131255844ae61492`  
		Last Modified: Wed, 03 May 2023 21:26:38 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2795c37902804d36644ab4b665f46a0a7cd526cf7843ccb4f01a084f2f61b7f7`  
		Last Modified: Wed, 03 May 2023 21:26:38 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1bb371f422afeb35fe873149a69cd084948e4a52ccd4419517b1844083c725`  
		Last Modified: Wed, 03 May 2023 21:26:39 GMT  
		Size: 258.4 KB (258401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaaff2d156044fdfe75ec46bb7652265e374df2902b2766bb0208ff13b5cd08`  
		Last Modified: Wed, 03 May 2023 21:26:47 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:jammy-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:c0f03351042a370adc1e419ec75369af3eabf56c223100470cc142334bfdccf6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32389189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc517a41591c8a5b4fc00b1fefcff5cd72f162496949d7f5156e81b26fe48f9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 19:05:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:05:46 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 19:05:47 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 19:05:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:05:55 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce53cea779733273cf24ec55276dac6cc9c77563b4244ce762d9679e6120250`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 3.7 MB (3738566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ed0729e8a293b6757d2d1e1f3945beb7567375d912abd1eefd688798dd1042`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daab176d4e2a4476e6e1bcef5fb4561c2b05e1c0b3913d2d61cbc02ffe5bb95f`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a285c321748b47e8da6e14e89e40a30db11775c6d6666a0dd2cc2041475d6`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 258.9 KB (258908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0a9caa9aeb605ad9d4ed83546b347dcb848fd80067f47538f8cca723c5417`  
		Last Modified: Wed, 03 May 2023 19:07:46 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:d50522f5919d76c352799a16f6ee33cea1110ea1e7b1ba6f61ba4d444e4673c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:a8b160ad81cc7caee38ea9b4ecee4f76acc1063d87bccc3d4676f16b0c1cd3aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b5e10477f27ce6cbba3962cae22f891689c7f08dd7644ff9e66f4996f98de28`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:31 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b9629c74f273da9190027c7e4cc11bf7b9c6a5bc037f53f26812b96307cee1`  
		Last Modified: Wed, 03 May 2023 21:27:14 GMT  
		Size: 11.3 MB (11310941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e479d911c8ceb5e5f2c92b8d68425475e3255bf6caf9fb40846df32dd54750`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b2393d1b1e6ae558b4e42a05a8fbd0a1cb5a6deadd71a2bdaff11b3fb8691d`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103058a946030129417ba0563768d175caae3f6b41f4787c1b86b420cdb7e639`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:8e9a1ffc99ee63822e0d6d473744ca2ad41ef31639f50b2db48affd80c7cee32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65319625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a17259e4c5d36ea6062363803be00e2629bf3ed07156e49ed82adb0c75b262`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:29:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:29:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187c756d024d4e7c2776681889618e1a5149fc672ed0aac61d785f286e69cb45`  
		Last Modified: Tue, 23 May 2023 02:31:19 GMT  
		Size: 11.3 MB (11313121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0227cf7a0eaf0af3c3c1164de31c4c5555f9f5b511769db242fdc93b238f9876`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78eb1f7c1bac7ebaea871680d53583c59acee5339b44ced2f4aa3cb3e1aa6cb`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7532dbe02d3f898678b483d0df372497ea9472a859b411edd0993544bab9cd6c`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 311.9 KB (311882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; 386

```console
$ docker pull neurodebian@sha256:50ee6db1dc9787f13d68e670b76ee5bb188abdb37df2eeb108a02993ca515ddc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68050919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae6bd51d8bd61bb7ffc759874939575238eac0ebc86f65e55035ade609fde7c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:45 GMT
ADD file:59d53253d7691be0330c735eb4b57791a8fc5894572d3deaeb7138cce45132ad in / 
# Wed, 03 May 2023 00:00:46 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:16:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:16:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:16:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ac0eb37fce5e6fca952bf804df5de5ebb63724d4d44bf23abc5d5736ee32afd`  
		Last Modified: Wed, 03 May 2023 00:04:44 GMT  
		Size: 56.0 MB (56029150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c794418bd1e96a39bea1aef2c4f245b825ec4e16a1d2fa3222521c51cbe7cd8`  
		Last Modified: Wed, 03 May 2023 23:18:05 GMT  
		Size: 11.7 MB (11707936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e0e0e73c24570aa784364602cf64cd9331769082f140bfa988aad91ce79b9`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6e2c410c8e6b068d6692e30b9d8d56a1e0bf11cf420a3f030fe862b4a566f`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbe2da83496475fac6b9656e8be553e28e545fab227c1cc1c666a89f3141f1b`  
		Last Modified: Wed, 03 May 2023 23:18:04 GMT  
		Size: 311.8 KB (311820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:f23ec75f325ccd8daf51abfb2a5149de40d45fb20837f646dd63a14b24f62e7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:bfe67002364838700c76c1c3a2f8ceaf639c6a6298213f3518a0dc9635906c92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61305792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7628118084f66e224ab75edf762667e0641ead33e66b059e71a6299bd2c7eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:42 GMT
ADD file:6261ecb921e04d2b3f6fd44e5dcb5683154bc0beee4f26913c2be9395a060489 in / 
# Tue, 02 May 2023 23:47:43 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:26:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:26:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:26:08 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:26:12 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae396e350f30e1defad1bfa67a84b97389d42cf3442551e39a0e2bab6b53a50c`  
		Last Modified: Tue, 02 May 2023 23:51:56 GMT  
		Size: 49.3 MB (49299270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07001fa6af159175c58303f7752dd97019fd06951e7055bcb076e5194afa064f`  
		Last Modified: Wed, 03 May 2023 21:27:50 GMT  
		Size: 11.7 MB (11719904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdf86d32a3b26b1c1bd693d70bc6115b98a87379e31ff8b6f6b9f7ed9009fe3`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dee1f3f9a40aee303f152160ad22cf80424301d6e75afcd194d8f83d27543`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745484e4809d3b3760d3a506060c0d4454cf63ff0de190c172235e7f825eaa2f`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 284.6 KB (284611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:d63d9cec9204a1302b94dc0ebc95380ddb757f99edcab9571a3411fa6810db0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61310676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4ab96d35dc7bbfedb971394bb6ee81f1fa0c5b00bef37652c482f0bda38537c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:48 GMT
ADD file:4608b82b211b6814e5bf372be706a6c01bd7a2a4841b59ac5430ec3a3f94468d in / 
# Tue, 23 May 2023 00:43:49 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:30:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:30:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:30:36 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5842d200e3f7df637a96b64f14e82ccb2c66e201137165f2d91447fbd3248a8c`  
		Last Modified: Tue, 23 May 2023 00:47:31 GMT  
		Size: 49.3 MB (49336298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5dc20c7009c0c4fb8fcc9510272b9663f770c650ec6a79065e104de65ae083`  
		Last Modified: Tue, 23 May 2023 02:31:55 GMT  
		Size: 11.7 MB (11685804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70e50d9fe81355ff8795fe4ebe3fa83df06646ae08c427d3ce1f270d69c679c`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b1dce6b21c52e13c5410c66209fa00c80743c2703fa7deb3e2a45c521dab`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ee43739ae5dd8545181114be4dc1eda914eac3630aaf0547acfc5fd4f213a9`  
		Last Modified: Tue, 23 May 2023 02:31:54 GMT  
		Size: 286.6 KB (286566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; 386

```console
$ docker pull neurodebian@sha256:d2bf9bf510a5c7063207246fd743a970aa3f2a21bf17e4e60252263a3c93ae9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62752295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5570ba7043d26acb17e3c64bfbf3e4eb1c63eea6d8eb31e7bb571b09dcba5a71`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:59 GMT
ADD file:4abf127b0d4037b2d94457a8ef168165ed6946fec0635fdaa845ed4ee8f74681 in / 
# Wed, 03 May 2023 00:02:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:17:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:17:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:17:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:125509149936f5c9fc010cb99811f5cb23108af74e034fcf0903d3f2cc08d893`  
		Last Modified: Wed, 03 May 2023 00:06:56 GMT  
		Size: 50.3 MB (50321774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03401a139b285d7dbabf9bf47070d8513369654c65656e0c9d884753d539277f`  
		Last Modified: Wed, 03 May 2023 23:18:43 GMT  
		Size: 12.1 MB (12143791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5281eb68b6af5d72745e5c9b4b79dd83518a7577dc0fe9d915aded3a47e043`  
		Last Modified: Wed, 03 May 2023 23:18:41 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d185612295077c05c7f4013d0363a5a2d03ec6b9616cdd174458890a2a4a127b`  
		Last Modified: Wed, 03 May 2023 23:18:41 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab7c155e27703e280eaf8bb7af29a7e4811f8eff90e33735e85d08540012bcd`  
		Last Modified: Wed, 03 May 2023 23:18:42 GMT  
		Size: 284.7 KB (284722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:81280c9b90b55267fcd5d76144088664479223b24fac457ea232c971fd200fb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:3e1fda817390144cf38a8ad2261957ecaf31672324e8ebf505ea503b8c18acae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03316cf4967259749fc22171bdee854ef9b9aff3303b43444791690fb75e0d6d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:42 GMT
ADD file:6261ecb921e04d2b3f6fd44e5dcb5683154bc0beee4f26913c2be9395a060489 in / 
# Tue, 02 May 2023 23:47:43 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:26:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:26:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:26:08 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:26:12 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:26:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ae396e350f30e1defad1bfa67a84b97389d42cf3442551e39a0e2bab6b53a50c`  
		Last Modified: Tue, 02 May 2023 23:51:56 GMT  
		Size: 49.3 MB (49299270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07001fa6af159175c58303f7752dd97019fd06951e7055bcb076e5194afa064f`  
		Last Modified: Wed, 03 May 2023 21:27:50 GMT  
		Size: 11.7 MB (11719904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdf86d32a3b26b1c1bd693d70bc6115b98a87379e31ff8b6f6b9f7ed9009fe3`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dee1f3f9a40aee303f152160ad22cf80424301d6e75afcd194d8f83d27543`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745484e4809d3b3760d3a506060c0d4454cf63ff0de190c172235e7f825eaa2f`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 284.6 KB (284611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8500a41f7e728906fca7f1d637852202a87f9ea250eec4cfdf14f4a10d85694`  
		Last Modified: Wed, 03 May 2023 21:27:58 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:48c979657bcab083b5a181f205a8ba52a3218b18bed5b443ebeb4bc8cc33fafa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61311075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aa7f0542b4bfb7559aeef459dc4cc4d68c1a8b4ba610d3fafee39694f4623e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:48 GMT
ADD file:4608b82b211b6814e5bf372be706a6c01bd7a2a4841b59ac5430ec3a3f94468d in / 
# Tue, 23 May 2023 00:43:49 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:30:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:30:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:30:36 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:40 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:5842d200e3f7df637a96b64f14e82ccb2c66e201137165f2d91447fbd3248a8c`  
		Last Modified: Tue, 23 May 2023 00:47:31 GMT  
		Size: 49.3 MB (49336298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5dc20c7009c0c4fb8fcc9510272b9663f770c650ec6a79065e104de65ae083`  
		Last Modified: Tue, 23 May 2023 02:31:55 GMT  
		Size: 11.7 MB (11685804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70e50d9fe81355ff8795fe4ebe3fa83df06646ae08c427d3ce1f270d69c679c`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b1dce6b21c52e13c5410c66209fa00c80743c2703fa7deb3e2a45c521dab`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ee43739ae5dd8545181114be4dc1eda914eac3630aaf0547acfc5fd4f213a9`  
		Last Modified: Tue, 23 May 2023 02:31:54 GMT  
		Size: 286.6 KB (286566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93ad45069d23343bb6311642e0f863b5900a8b9eea8b859b2bbe1721dff1f09`  
		Last Modified: Tue, 23 May 2023 02:32:02 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:3b55d7527f746dda6b623936b102556d07bb27844f33f3b3a73f3fd4d4cc287b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62752686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a3f168461765aee166a808516f45328083a8569d9221c64fbe2fd8c2ab84650`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:59 GMT
ADD file:4abf127b0d4037b2d94457a8ef168165ed6946fec0635fdaa845ed4ee8f74681 in / 
# Wed, 03 May 2023 00:02:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:17:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:17:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:17:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:34 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:125509149936f5c9fc010cb99811f5cb23108af74e034fcf0903d3f2cc08d893`  
		Last Modified: Wed, 03 May 2023 00:06:56 GMT  
		Size: 50.3 MB (50321774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03401a139b285d7dbabf9bf47070d8513369654c65656e0c9d884753d539277f`  
		Last Modified: Wed, 03 May 2023 23:18:43 GMT  
		Size: 12.1 MB (12143791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5281eb68b6af5d72745e5c9b4b79dd83518a7577dc0fe9d915aded3a47e043`  
		Last Modified: Wed, 03 May 2023 23:18:41 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d185612295077c05c7f4013d0363a5a2d03ec6b9616cdd174458890a2a4a127b`  
		Last Modified: Wed, 03 May 2023 23:18:41 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab7c155e27703e280eaf8bb7af29a7e4811f8eff90e33735e85d08540012bcd`  
		Last Modified: Wed, 03 May 2023 23:18:42 GMT  
		Size: 284.7 KB (284722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5fa32322a1c07f34e547f4775540f6eab3c1d3464b5a006bd5c2449a0bced3`  
		Last Modified: Wed, 03 May 2023 23:18:51 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100`

```console
$ docker pull neurodebian@sha256:44b51fdc7b4248178d4ccb740761403b0b68bdd5561eb0b2c70e8d482ff1fb64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100` - linux; amd64

```console
$ docker pull neurodebian@sha256:14859d5c917b06ea663d297456f90292ba40d282f0250c3cfa738f73292630d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61259514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:477c74a581e9ea7f67ce9724de9fc8cf463e08391beb08a301ae72c534f3d88f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:07 GMT
ADD file:d176a72312205fc75b2950df98f4ed25abadd4b053b9d85bea67466a5b30220f in / 
# Tue, 02 May 2023 23:47:08 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:13 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a94073ab46f8d565f5938cc345d32f7adda10a2585e39555079da9d4ee595974`  
		Last Modified: Tue, 02 May 2023 23:50:40 GMT  
		Size: 50.4 MB (50448697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f87762e02dad34eb08994cd86e167edfd44474c49108468eb082ae17364bec7`  
		Last Modified: Wed, 03 May 2023 21:26:56 GMT  
		Size: 10.5 MB (10504492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbda83cc39ef32e5179634236082fd77e94c2021179b379bc60fc6f077b3a80`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada04c68f4b4be2aa312f558542d687e6f998884d6831a2bdee4a124b3a2cf66`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd97b4a7da61a8033aa1a379b164d4f7e19016db0f734d6f6d35ed16e42cfd4`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 304.3 KB (304318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:749db235498965a5f1361bf7f23ce1d0629d6b51d66fdbd75a817837b8169248
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60055122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0492c0aef76c50f117312fd94b88bd6ba0dc7be2214987b1ffa406bf623e5cd1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:21 GMT
ADD file:a5100e7ed3c2665c1b4dfbb32eb2b47b85783f2a6800e0ae9004db0ce021dfa5 in / 
# Tue, 23 May 2023 00:43:22 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:29:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:29:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ea482247e9a0d1ae4ed218fb0828063b9cce53822e64fd4621f587ab85a7e6d`  
		Last Modified: Tue, 23 May 2023 00:46:24 GMT  
		Size: 49.2 MB (49238292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3669f12602d08f0dbf725c5e531299324f34d80aa1333c05e17213b09f9b4f82`  
		Last Modified: Tue, 23 May 2023 02:31:02 GMT  
		Size: 10.5 MB (10510471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35875484f4c75482356db7b88ff96956756ca2ddf9fcf0db615fa7fac9e6795`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dad3d877033dd23fd3219c87d8586351dbe14d7ab3c9fe9c25296df7bbb2901`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1424958f76e02c936033580d62bee2972bde5e1f1a8b6d5c0a8781046a3b37`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 304.4 KB (304350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100` - linux; 386

```console
$ docker pull neurodebian@sha256:c0fbae788aeae82e38c9733aa4f5732ccef69a616953a913c69e2ece707a4ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62380642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90225822130b7f5284a53b778c0c2b770de586e2d8561342b384b36569cb8823`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:10 GMT
ADD file:d427d53c0d42e21426b53d60a17dd7014d2504084ae758c35f088cee043ff9ed in / 
# Wed, 03 May 2023 00:01:11 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:16:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:16:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:16:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc3c764404274f8a6e2edf459bc863892205283aa5069a204e16cce54455cb83`  
		Last Modified: Wed, 03 May 2023 00:05:33 GMT  
		Size: 51.2 MB (51206158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43844ba53e304f4440b1717d17b7f4739ebd73aaea1b850a3697ccb354ca152b`  
		Last Modified: Wed, 03 May 2023 23:17:48 GMT  
		Size: 10.9 MB (10868216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2599c7f3672a192bf65ce0684c0be96a9a476901c4f5a1f5fdad43d3f14250`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e99eacf5db7dc7bf3ebc61365890bf33ee0892276ba2c0681514f7e6e457792`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ca39efb9f207d4de5ab6495531fa5fbc3cfe9d73d19ccc4ca83e73a7d29e6f`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 304.3 KB (304255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100-non-free`

```console
$ docker pull neurodebian@sha256:f4a5c204470a35db95ee5fae5aa1924d7b8dfb31aeb46d3abba33c6af31f7965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:3c0e2236cddaca2f0f0fae30da44146a0bafc3de4555d70dbf48bdc11ffd6263
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61259872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d79f353601fa8661f09c7864b043a90ffe8c169b228b249899f3666aa4a9c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:07 GMT
ADD file:d176a72312205fc75b2950df98f4ed25abadd4b053b9d85bea67466a5b30220f in / 
# Tue, 02 May 2023 23:47:08 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:13 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a94073ab46f8d565f5938cc345d32f7adda10a2585e39555079da9d4ee595974`  
		Last Modified: Tue, 02 May 2023 23:50:40 GMT  
		Size: 50.4 MB (50448697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f87762e02dad34eb08994cd86e167edfd44474c49108468eb082ae17364bec7`  
		Last Modified: Wed, 03 May 2023 21:26:56 GMT  
		Size: 10.5 MB (10504492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbda83cc39ef32e5179634236082fd77e94c2021179b379bc60fc6f077b3a80`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada04c68f4b4be2aa312f558542d687e6f998884d6831a2bdee4a124b3a2cf66`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd97b4a7da61a8033aa1a379b164d4f7e19016db0f734d6f6d35ed16e42cfd4`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 304.3 KB (304318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b9a9a523f32160714296229f8f14f21b13da05df951a196f2f47cfa5c19b45`  
		Last Modified: Wed, 03 May 2023 21:27:04 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:d1d384571538549ef9e73096923d7672000b32b10260d4d105c910338942bcbc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60055480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:826fc2babca4e62a146037fa97738c0993582f625ae3657fc35c11f46f10fd4d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:21 GMT
ADD file:a5100e7ed3c2665c1b4dfbb32eb2b47b85783f2a6800e0ae9004db0ce021dfa5 in / 
# Tue, 23 May 2023 00:43:22 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:29:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:29:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:40 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:5ea482247e9a0d1ae4ed218fb0828063b9cce53822e64fd4621f587ab85a7e6d`  
		Last Modified: Tue, 23 May 2023 00:46:24 GMT  
		Size: 49.2 MB (49238292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3669f12602d08f0dbf725c5e531299324f34d80aa1333c05e17213b09f9b4f82`  
		Last Modified: Tue, 23 May 2023 02:31:02 GMT  
		Size: 10.5 MB (10510471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35875484f4c75482356db7b88ff96956756ca2ddf9fcf0db615fa7fac9e6795`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dad3d877033dd23fd3219c87d8586351dbe14d7ab3c9fe9c25296df7bbb2901`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1424958f76e02c936033580d62bee2972bde5e1f1a8b6d5c0a8781046a3b37`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 304.4 KB (304350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5600a1971a0e2142139cffffa014177321f94569310c622a4f530cc99eee5a72`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:b565467f94285936ab3a8d8d852cccba66345b8f508d33946bc4e40011ee2e8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62380998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c27bc0c72ef518da8e561f830d119f105da8970c80685b386314fc6d01a045`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:10 GMT
ADD file:d427d53c0d42e21426b53d60a17dd7014d2504084ae758c35f088cee043ff9ed in / 
# Wed, 03 May 2023 00:01:11 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:16:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:16:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:16:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:35 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:cc3c764404274f8a6e2edf459bc863892205283aa5069a204e16cce54455cb83`  
		Last Modified: Wed, 03 May 2023 00:05:33 GMT  
		Size: 51.2 MB (51206158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43844ba53e304f4440b1717d17b7f4739ebd73aaea1b850a3697ccb354ca152b`  
		Last Modified: Wed, 03 May 2023 23:17:48 GMT  
		Size: 10.9 MB (10868216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2599c7f3672a192bf65ce0684c0be96a9a476901c4f5a1f5fdad43d3f14250`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e99eacf5db7dc7bf3ebc61365890bf33ee0892276ba2c0681514f7e6e457792`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ca39efb9f207d4de5ab6495531fa5fbc3cfe9d73d19ccc4ca83e73a7d29e6f`  
		Last Modified: Wed, 03 May 2023 23:17:47 GMT  
		Size: 304.3 KB (304255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca7e12a39acbba25b91d9cdab41e4c34f117c2ab0c4843b97340a0ddb97e1e`  
		Last Modified: Wed, 03 May 2023 23:17:56 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110`

```console
$ docker pull neurodebian@sha256:d50522f5919d76c352799a16f6ee33cea1110ea1e7b1ba6f61ba4d444e4673c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110` - linux; amd64

```console
$ docker pull neurodebian@sha256:a8b160ad81cc7caee38ea9b4ecee4f76acc1063d87bccc3d4676f16b0c1cd3aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b5e10477f27ce6cbba3962cae22f891689c7f08dd7644ff9e66f4996f98de28`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:31 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b9629c74f273da9190027c7e4cc11bf7b9c6a5bc037f53f26812b96307cee1`  
		Last Modified: Wed, 03 May 2023 21:27:14 GMT  
		Size: 11.3 MB (11310941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e479d911c8ceb5e5f2c92b8d68425475e3255bf6caf9fb40846df32dd54750`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b2393d1b1e6ae558b4e42a05a8fbd0a1cb5a6deadd71a2bdaff11b3fb8691d`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103058a946030129417ba0563768d175caae3f6b41f4787c1b86b420cdb7e639`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:8e9a1ffc99ee63822e0d6d473744ca2ad41ef31639f50b2db48affd80c7cee32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65319625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a17259e4c5d36ea6062363803be00e2629bf3ed07156e49ed82adb0c75b262`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:29:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:29:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187c756d024d4e7c2776681889618e1a5149fc672ed0aac61d785f286e69cb45`  
		Last Modified: Tue, 23 May 2023 02:31:19 GMT  
		Size: 11.3 MB (11313121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0227cf7a0eaf0af3c3c1164de31c4c5555f9f5b511769db242fdc93b238f9876`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78eb1f7c1bac7ebaea871680d53583c59acee5339b44ced2f4aa3cb3e1aa6cb`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7532dbe02d3f898678b483d0df372497ea9472a859b411edd0993544bab9cd6c`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 311.9 KB (311882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110` - linux; 386

```console
$ docker pull neurodebian@sha256:50ee6db1dc9787f13d68e670b76ee5bb188abdb37df2eeb108a02993ca515ddc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68050919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae6bd51d8bd61bb7ffc759874939575238eac0ebc86f65e55035ade609fde7c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:45 GMT
ADD file:59d53253d7691be0330c735eb4b57791a8fc5894572d3deaeb7138cce45132ad in / 
# Wed, 03 May 2023 00:00:46 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:16:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:16:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:16:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ac0eb37fce5e6fca952bf804df5de5ebb63724d4d44bf23abc5d5736ee32afd`  
		Last Modified: Wed, 03 May 2023 00:04:44 GMT  
		Size: 56.0 MB (56029150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c794418bd1e96a39bea1aef2c4f245b825ec4e16a1d2fa3222521c51cbe7cd8`  
		Last Modified: Wed, 03 May 2023 23:18:05 GMT  
		Size: 11.7 MB (11707936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e0e0e73c24570aa784364602cf64cd9331769082f140bfa988aad91ce79b9`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6e2c410c8e6b068d6692e30b9d8d56a1e0bf11cf420a3f030fe862b4a566f`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbe2da83496475fac6b9656e8be553e28e545fab227c1cc1c666a89f3141f1b`  
		Last Modified: Wed, 03 May 2023 23:18:04 GMT  
		Size: 311.8 KB (311820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:0f540c18829c6396c0c23e747525582fa1e7cbbed1540d58be6c9b359e58f23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:0e03b2debd7a1d5f28aa746ae3e4ce140ed6790d63f39f6a5b71521e88769c50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3331ef22a29d7e47c420e4814e93b37e21973c5540cbb66fd17f4fc9a81b223`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:31 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:38 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b9629c74f273da9190027c7e4cc11bf7b9c6a5bc037f53f26812b96307cee1`  
		Last Modified: Wed, 03 May 2023 21:27:14 GMT  
		Size: 11.3 MB (11310941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e479d911c8ceb5e5f2c92b8d68425475e3255bf6caf9fb40846df32dd54750`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b2393d1b1e6ae558b4e42a05a8fbd0a1cb5a6deadd71a2bdaff11b3fb8691d`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103058a946030129417ba0563768d175caae3f6b41f4787c1b86b420cdb7e639`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a786115a54951b49a2de00541f08f3fb81963b0a9827b745be73197ea4ddb51f`  
		Last Modified: Wed, 03 May 2023 21:27:23 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:efc47b01c41eca49e029b269638c650adfd2a8f0e73807c748f9c7bc1f36cbce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65319984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4ebde6630ed604716cbd5f83c480bc3a7e5e2d8cce1d68c1355581fcfcf157`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:29:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:29:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:57 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187c756d024d4e7c2776681889618e1a5149fc672ed0aac61d785f286e69cb45`  
		Last Modified: Tue, 23 May 2023 02:31:19 GMT  
		Size: 11.3 MB (11313121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0227cf7a0eaf0af3c3c1164de31c4c5555f9f5b511769db242fdc93b238f9876`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78eb1f7c1bac7ebaea871680d53583c59acee5339b44ced2f4aa3cb3e1aa6cb`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7532dbe02d3f898678b483d0df372497ea9472a859b411edd0993544bab9cd6c`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 311.9 KB (311882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfc256c442e8e637b8a0cece189d2a76422322f8ee48f5be12c1dce583cbdd2`  
		Last Modified: Tue, 23 May 2023 02:31:28 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:fe3bde78aeb9790898d619b54ac53eb63822edbd4b7823a0984d80631bb65fed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68051278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7adfc07d9da7329f3d6d9ae824556b77b534f5b7c95c239975fbedff4eb071e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:45 GMT
ADD file:59d53253d7691be0330c735eb4b57791a8fc5894572d3deaeb7138cce45132ad in / 
# Wed, 03 May 2023 00:00:46 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:16:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:16:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:16:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:52 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:6ac0eb37fce5e6fca952bf804df5de5ebb63724d4d44bf23abc5d5736ee32afd`  
		Last Modified: Wed, 03 May 2023 00:04:44 GMT  
		Size: 56.0 MB (56029150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c794418bd1e96a39bea1aef2c4f245b825ec4e16a1d2fa3222521c51cbe7cd8`  
		Last Modified: Wed, 03 May 2023 23:18:05 GMT  
		Size: 11.7 MB (11707936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e0e0e73c24570aa784364602cf64cd9331769082f140bfa988aad91ce79b9`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6e2c410c8e6b068d6692e30b9d8d56a1e0bf11cf420a3f030fe862b4a566f`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbe2da83496475fac6b9656e8be553e28e545fab227c1cc1c666a89f3141f1b`  
		Last Modified: Wed, 03 May 2023 23:18:04 GMT  
		Size: 311.8 KB (311820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c5defbdb36be91b752ff0f2512091c04e98799ae0c1c8c8ace8eede4671471`  
		Last Modified: Wed, 03 May 2023 23:18:15 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120`

```console
$ docker pull neurodebian@sha256:6d11433337327f59e8310b362ced377bb97fadc30760c4d7150030e4a2430381
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120` - linux; amd64

```console
$ docker pull neurodebian@sha256:4bbebb1af3fa42edeb7daa76429594832677c061fbaa59f2176c8cbe40d8b607
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61305663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592dcc4b1cc3783782cfea69d58dcf8a1738781d2842c3849fd90d40df1b899a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:33 GMT
ADD file:168af20819ee8d7bc6ca3fd35873fe0b65f567f6fc4763ae2fed655e04826ef6 in / 
# Tue, 02 May 2023 23:46:33 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:879480f6969a02afb639ba9b35bc2df992fec064538a2e8af5e14cf6b6fbeac3`  
		Last Modified: Tue, 02 May 2023 23:49:26 GMT  
		Size: 49.3 MB (49299247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd09f14e055c828315e856789d20b8946366f27edf267f3902b57215e239d7ef`  
		Last Modified: Wed, 03 May 2023 21:27:34 GMT  
		Size: 11.7 MB (11719796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173622f5d1ba65e0d94854aa9998708f35b2a78b4a0c65ce6ec9cb2d772d4c39`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3666043593436d5565d087183a46b53a6ae13cb63c743b728fd872c3c48aa0e8`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f690a06a4d5ee8090896ae8454bdb93732d1e61586082cd7b596aad4aaf087`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 284.6 KB (284613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:648d84e2d1b843835b3fa399b85eeaf865c48c3be470f229543f63a4c1f56a04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61320411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a9c9e342134ca145b25d98ab14e66f984bda18bcc60e0a0f0141083df122e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:42:54 GMT
ADD file:91184714f613e1768e87fad722350f471376a88cb595664e8e23864ce5d79071 in / 
# Tue, 23 May 2023 00:42:55 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:30:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:30:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:30:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3485dc61c38c6db2e8092e9f4326fe6c51e867a1841f55346f74ec25847d7401`  
		Last Modified: Tue, 23 May 2023 00:45:14 GMT  
		Size: 49.3 MB (49347785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27205be5ff69de2ea80daf475b7d6782f5bd2c4eff02242061f43eaf6012d24`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 11.7 MB (11685619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a91d72189acf1f099b7b4f36d85c03907fb5bacd266f36caa6b04ef2e3fd7fb`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae3bb66bd12fcefd327ecdad94e32054fc3501ea2c5f23a797f919ad31b9bc9`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e899ae9f9f58a47c33891e8ef8311f802cbff074ff152ecd2f6fa34be22900d1`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 285.0 KB (284995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120` - linux; 386

```console
$ docker pull neurodebian@sha256:a8950e781f0d7e413cb43a35939504243936f723a3362cbfb4579ada1646af1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62752170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0397aab4130cfdd8b1bc6e0c4a66596c8d00e10ba6805e93f72fbdd0f7ea47b7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:17 GMT
ADD file:cd02b45138959c7ec7d466eff66efaa68d03b2e72f294b468f08c576643ac084 in / 
# Wed, 03 May 2023 00:00:18 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:17:02 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:04 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:17:04 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:17:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:028db28caf3d2a0b3bc8b8281c9f370a6ca8a97954f596e2b27e20ebf7f3b578`  
		Last Modified: Wed, 03 May 2023 00:04:07 GMT  
		Size: 50.3 MB (50321827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa3f2ae1595f6575bfc69faed0d539bf88a71f81033a72dd7cd6a6b16533a26`  
		Last Modified: Wed, 03 May 2023 23:18:26 GMT  
		Size: 12.1 MB (12143607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030d5cafe5a4885634636dec550fa431c5d4332902b7fa1e592504eb10cb4698`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc4a181c2202a0f49007cfb365321e0dc3352e79f05f6028e41b534da7b6018`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b687257037f8146aecaffcb99f883d553e938ba2d1635186ff1fde12e64952d8`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 284.7 KB (284726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120-non-free`

```console
$ docker pull neurodebian@sha256:9297ea57c8e4c3f13f28668610b9ae587a610d42b430898b1819d0b02a50f882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:d52d4af080b7f4a4e2587186062e52d88603493ad425402cf20c95c0b116a2ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3e6a45d91905bfd06f5fbdcba0eab1a5024f5f049356cec05dd240eaaf04d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:33 GMT
ADD file:168af20819ee8d7bc6ca3fd35873fe0b65f567f6fc4763ae2fed655e04826ef6 in / 
# Tue, 02 May 2023 23:46:33 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:56 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:879480f6969a02afb639ba9b35bc2df992fec064538a2e8af5e14cf6b6fbeac3`  
		Last Modified: Tue, 02 May 2023 23:49:26 GMT  
		Size: 49.3 MB (49299247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd09f14e055c828315e856789d20b8946366f27edf267f3902b57215e239d7ef`  
		Last Modified: Wed, 03 May 2023 21:27:34 GMT  
		Size: 11.7 MB (11719796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173622f5d1ba65e0d94854aa9998708f35b2a78b4a0c65ce6ec9cb2d772d4c39`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3666043593436d5565d087183a46b53a6ae13cb63c743b728fd872c3c48aa0e8`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f690a06a4d5ee8090896ae8454bdb93732d1e61586082cd7b596aad4aaf087`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 284.6 KB (284613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5ffbe0a5537ef8771e9443b26e7da93ca8f8f2a26af66c24911e7d5259053a`  
		Last Modified: Wed, 03 May 2023 21:27:41 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:b69bfc4ed29a6d42fb7f32af35e35b1635ad6ed11266fabae4dead54f1adffc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61320839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:778d928a3fee1ce61884892a6b7f775f1089f3724facee289f262e14452a8abf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:42:54 GMT
ADD file:91184714f613e1768e87fad722350f471376a88cb595664e8e23864ce5d79071 in / 
# Tue, 23 May 2023 00:42:55 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:30:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:30:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:30:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:3485dc61c38c6db2e8092e9f4326fe6c51e867a1841f55346f74ec25847d7401`  
		Last Modified: Tue, 23 May 2023 00:45:14 GMT  
		Size: 49.3 MB (49347785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27205be5ff69de2ea80daf475b7d6782f5bd2c4eff02242061f43eaf6012d24`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 11.7 MB (11685619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a91d72189acf1f099b7b4f36d85c03907fb5bacd266f36caa6b04ef2e3fd7fb`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae3bb66bd12fcefd327ecdad94e32054fc3501ea2c5f23a797f919ad31b9bc9`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e899ae9f9f58a47c33891e8ef8311f802cbff074ff152ecd2f6fa34be22900d1`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 285.0 KB (284995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f11898d17a3e3cea8f36f6751eb691a7fc506a165af741c28422a9e0b52a8e5`  
		Last Modified: Tue, 23 May 2023 02:31:46 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:16cc40944ba50beee287eba7c32319d476c46ee7c1d316ce96367ac84fb64a5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62752596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df71d0bb8af9de01eb06854a17e811ed4938dcce437ab398a47e2992b8a637d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:17 GMT
ADD file:cd02b45138959c7ec7d466eff66efaa68d03b2e72f294b468f08c576643ac084 in / 
# Wed, 03 May 2023 00:00:18 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:17:02 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:04 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:17:04 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:17:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:14 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:028db28caf3d2a0b3bc8b8281c9f370a6ca8a97954f596e2b27e20ebf7f3b578`  
		Last Modified: Wed, 03 May 2023 00:04:07 GMT  
		Size: 50.3 MB (50321827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa3f2ae1595f6575bfc69faed0d539bf88a71f81033a72dd7cd6a6b16533a26`  
		Last Modified: Wed, 03 May 2023 23:18:26 GMT  
		Size: 12.1 MB (12143607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030d5cafe5a4885634636dec550fa431c5d4332902b7fa1e592504eb10cb4698`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc4a181c2202a0f49007cfb365321e0dc3352e79f05f6028e41b534da7b6018`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b687257037f8146aecaffcb99f883d553e938ba2d1635186ff1fde12e64952d8`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 284.7 KB (284726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df75504459b747f4070dddcbeda95a33709c7b6352069c3f655621932713a20`  
		Last Modified: Wed, 03 May 2023 23:18:34 GMT  
		Size: 426.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04`

```console
$ docker pull neurodebian@sha256:e8d04969d017bf258e6f3e3823d029ffa862d189269e840eebf1773ca343ef85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd18.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:a46f35fb0fb8e1d62203cb73a8b9a35304958af2d0da86536680428b3826d6e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31778913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797d9b9af21ae983270561edc6bf2f86d96409f0fa4554d7f312bf28bc98af90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:02:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:02:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 16 May 2023 01:02:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 16 May 2023 01:02:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2372d6e43648bec4df62a3d55e7f95e72243565b07c6d5920d3406d6eefbd5a8`  
		Last Modified: Tue, 16 May 2023 01:03:22 GMT  
		Size: 4.8 MB (4821195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620a82a5993926d5580487c99ad1a0938a9b68875b3c29746a0f4374f50e4ed6`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fb021293ae8fb1060eeeb057accbc60b7390f8cf2b9edfa122e80294f3de7c`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c786576ffd5a24ecad657d482b765f09fa254580fc4d6a4ab147d457f6a89`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 240.3 KB (240297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd18.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:4d086ea47c67c213bb766b47a3728a21e11f606d760c3a61aa25575f109121cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28387601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1017979b144e550cac6c7ab43aa5f25dc69263722eddfdc4511926239bd89adf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:25:37 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:25:38 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 16 May 2023 01:25:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 16 May 2023 01:25:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592501afdaec24bcc465ef26abc1b7d532782a85c6cbe7893a7fd774b7ddb8c1`  
		Last Modified: Tue, 16 May 2023 01:26:19 GMT  
		Size: 4.4 MB (4403694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e0312aba612c00a457099681cef3a29c3e73ce54ce0e4aac34fdd08b0adfeb`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 1.7 KB (1665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fdfd9ebabe147a93ab87064e56e524fc5ae9821794b68014d92124bd1ce284`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d273709265897dc91aaf15ee076766e0c6660e13254c4aade22b856ed3e5bca`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 241.1 KB (241071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04-non-free`

```console
$ docker pull neurodebian@sha256:2740f34f475ff2fd1961eb7b2b58ae91961ef74a6f2d18ff32de78afe60def75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd18.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:dd86543f59520f317599a56451050f712c0a117c420e4e6e30cbcc1fb8db8b84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31779170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:940ae3002ffa7baadfa10c87d888bb9be5fe56c1d95565f40821ed9ff2b94bea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:41:51 GMT
ARG RELEASE
# Fri, 12 May 2023 09:41:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:41:51 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:41:52 GMT
ADD file:47682dd3869ca8e57ceb15f69a6ac7c9048d4d42c7a99a976e597cf072423c12 in / 
# Fri, 12 May 2023 09:41:53 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:02:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:02:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 16 May 2023 01:02:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 16 May 2023 01:02:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:02:42 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:c67806d7e72dd941e600bad2eabe920a17ba1852b325b63900c819ffeae646fb`  
		Last Modified: Tue, 16 May 2023 01:01:48 GMT  
		Size: 26.7 MB (26715509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2372d6e43648bec4df62a3d55e7f95e72243565b07c6d5920d3406d6eefbd5a8`  
		Last Modified: Tue, 16 May 2023 01:03:22 GMT  
		Size: 4.8 MB (4821195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620a82a5993926d5580487c99ad1a0938a9b68875b3c29746a0f4374f50e4ed6`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fb021293ae8fb1060eeeb057accbc60b7390f8cf2b9edfa122e80294f3de7c`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638c786576ffd5a24ecad657d482b765f09fa254580fc4d6a4ab147d457f6a89`  
		Last Modified: Tue, 16 May 2023 01:03:21 GMT  
		Size: 240.3 KB (240297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd3984fa38330d1b3b2590d00da5c0e2052ec84b96bd48683df7d0fd5bc299b`  
		Last Modified: Tue, 16 May 2023 01:03:29 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd18.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:51567a48e4ee4ab6244cac21df91a34de9ac8631e64cb62003c3692aaa09b61d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28387860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c879b3d4ab74022bc603e9e94dff0eec069290bf4d4a3de32a44954b0d82dd38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 12 May 2023 09:31:18 GMT
ARG RELEASE
# Fri, 12 May 2023 09:31:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 12 May 2023 09:31:18 GMT
LABEL org.opencontainers.image.version=18.04
# Fri, 12 May 2023 09:31:23 GMT
ADD file:65c814904a00832cc69b4ef05c54d1cd3b570be2c12d8891a1472a73d6534cda in / 
# Fri, 12 May 2023 09:31:24 GMT
CMD ["/bin/bash"]
# Tue, 16 May 2023 01:25:37 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:25:38 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 16 May 2023 01:25:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 16 May 2023 01:25:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 01:25:47 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:d3196e9fda85b1ae1aa48fdd42a05894cf36dbbe8d2b8b75f46691b12cba022d`  
		Last Modified: Tue, 16 May 2023 01:26:21 GMT  
		Size: 23.7 MB (23740923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592501afdaec24bcc465ef26abc1b7d532782a85c6cbe7893a7fd774b7ddb8c1`  
		Last Modified: Tue, 16 May 2023 01:26:19 GMT  
		Size: 4.4 MB (4403694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e0312aba612c00a457099681cef3a29c3e73ce54ce0e4aac34fdd08b0adfeb`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 1.7 KB (1665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fdfd9ebabe147a93ab87064e56e524fc5ae9821794b68014d92124bd1ce284`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d273709265897dc91aaf15ee076766e0c6660e13254c4aade22b856ed3e5bca`  
		Last Modified: Tue, 16 May 2023 01:26:18 GMT  
		Size: 241.1 KB (241071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2a8256b93deb2dd3244eaf3d152d923018cd4332060d4a4ec7842e728aae9b`  
		Last Modified: Tue, 16 May 2023 01:26:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04`

```console
$ docker pull neurodebian@sha256:32657efcbe75393aa2da46975fc9ea7bebbbdc9a662f70959161666ea819a6be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd20.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:0e666853f7e4a618de58b520e48853965345d292ecd1931a7b71cb7d9d2fb274
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34313750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9038f4da65a7ee359dfa78434fd1b63e9938ba98825954fc79d9622ee72d7c8c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:42:04 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:42:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 18 Apr 2023 02:42:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 18 Apr 2023 02:42:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f6efd2926626473d071a223a349e2958558513cf51fde93090ea8f8883d17`  
		Last Modified: Tue, 18 Apr 2023 02:42:51 GMT  
		Size: 5.5 MB (5494338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ef84ed7d67e739f242b02ac970071100cba403cbfaa24dad8d40f190f86d53`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28598ffa8aad6fab7f3041b2006d4badce4ca24a560a48ca4cebfdcb33016029`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6472897b79c02d388e702cbf72fb1f128887d6e0f72992d276b9efd6c3fa353b`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 238.8 KB (238840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd20.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:7e6dd01caa3656f152c63c15c2d03951352931a2cd1dbd21a8e62dc581482e5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32913188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630f2a6c42486435d7a35b2b08ac2ed21b2c7d8b905cafb81df9e9860173a5dc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:05:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:05:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 18 Apr 2023 02:05:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 18 Apr 2023 02:05:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c8f2d5b6a6ddaae0b4f84cb3ceb68eed34dfcab84b8bd8122afc877b84d7dc`  
		Last Modified: Tue, 18 Apr 2023 02:06:18 GMT  
		Size: 5.5 MB (5475094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91b40e1b81bc32ccfb31e807d1c37ff604997c2f73eb9c70b8ad2d32e23532b`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6692fe5836ed8f0bc1f41e11c59188de0c38640169128875fc695731c8a64a`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193e8a628fb21472856c5f43baaee3f05120d6d41fafd70e43931807b8c802de`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 239.7 KB (239684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04-non-free`

```console
$ docker pull neurodebian@sha256:50d69a7a5fe6275c281ae09da9a6e7ec62b90917964052cf5acd18c4c41aafd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd20.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:117345b79c50c024801f9f60799683235ebfd8a5dfa79c45a44e339e21e38064
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34314007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab8d95f59c510bd26eac5af308b128fb87b2f5ddbf858252307dc15d19d8681`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:42:04 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:42:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 18 Apr 2023 02:42:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 18 Apr 2023 02:42:11 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:42:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f6efd2926626473d071a223a349e2958558513cf51fde93090ea8f8883d17`  
		Last Modified: Tue, 18 Apr 2023 02:42:51 GMT  
		Size: 5.5 MB (5494338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ef84ed7d67e739f242b02ac970071100cba403cbfaa24dad8d40f190f86d53`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28598ffa8aad6fab7f3041b2006d4badce4ca24a560a48ca4cebfdcb33016029`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6472897b79c02d388e702cbf72fb1f128887d6e0f72992d276b9efd6c3fa353b`  
		Last Modified: Tue, 18 Apr 2023 02:42:50 GMT  
		Size: 238.8 KB (238840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530d1e2bbd66b9f610d9654ee50e64e8f58b3320e02d7cfd33cd055cf0dcbc96`  
		Last Modified: Tue, 18 Apr 2023 02:42:59 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd20.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5a1bf55d2e3e46d17acea860b18164edeeedfb50863cc64366489d68d599e48a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32913444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c683e496f7e95c821943a7432fdfe2d641b5605987810896e8a4dab923c2ea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 02:05:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:05:42 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 18 Apr 2023 02:05:43 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 18 Apr 2023 02:05:47 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 02:05:49 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c8f2d5b6a6ddaae0b4f84cb3ceb68eed34dfcab84b8bd8122afc877b84d7dc`  
		Last Modified: Tue, 18 Apr 2023 02:06:18 GMT  
		Size: 5.5 MB (5475094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91b40e1b81bc32ccfb31e807d1c37ff604997c2f73eb9c70b8ad2d32e23532b`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6692fe5836ed8f0bc1f41e11c59188de0c38640169128875fc695731c8a64a`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193e8a628fb21472856c5f43baaee3f05120d6d41fafd70e43931807b8c802de`  
		Last Modified: Tue, 18 Apr 2023 02:06:17 GMT  
		Size: 239.7 KB (239684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d2f0f07359cd0ea0074415a6b4accbc968f197484bd2872168f4707736a9c1`  
		Last Modified: Tue, 18 Apr 2023 02:06:26 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd22.04`

```console
$ docker pull neurodebian@sha256:63f8ba30ea3872358d3041e9c82f43c2540cbed3ef19f388d495af32b24fa45d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd22.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:d666ee3b477274405fa2c6319d27204f720dea21a2ea159027cc0c9419d17905
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34456563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d9408f22945908b19511f7c931a9b1e4d8a77dc9223d460bead7a16cd2721b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:24:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:24:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:24:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68378f1e43a78d07ba7d4b063f86a4e752c51e3c3914a1ff9f743500f2c2f04`  
		Last Modified: Wed, 03 May 2023 21:26:39 GMT  
		Size: 3.8 MB (3765930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd168bc42e411f97adae10afe4f4653177647bfa55537a25131255844ae61492`  
		Last Modified: Wed, 03 May 2023 21:26:38 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2795c37902804d36644ab4b665f46a0a7cd526cf7843ccb4f01a084f2f61b7f7`  
		Last Modified: Wed, 03 May 2023 21:26:38 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1bb371f422afeb35fe873149a69cd084948e4a52ccd4419517b1844083c725`  
		Last Modified: Wed, 03 May 2023 21:26:39 GMT  
		Size: 258.4 KB (258401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd22.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:35c8d1730e274f73b120705d4aea51e53728fd1713d371325489791657df5b80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32388930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8381623266dd094df6c2fe1971091cf1277379ddd899e8ecd057d981039f6ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 19:05:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:05:46 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 19:05:47 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 19:05:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce53cea779733273cf24ec55276dac6cc9c77563b4244ce762d9679e6120250`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 3.7 MB (3738566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ed0729e8a293b6757d2d1e1f3945beb7567375d912abd1eefd688798dd1042`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daab176d4e2a4476e6e1bcef5fb4561c2b05e1c0b3913d2d61cbc02ffe5bb95f`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a285c321748b47e8da6e14e89e40a30db11775c6d6666a0dd2cc2041475d6`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 258.9 KB (258908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd22.04-non-free`

```console
$ docker pull neurodebian@sha256:21a56fb9ba3feb49b92f808c8a8417cbae38c971a650de2839d4f375035d50a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd22.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:972c31822cf1c906d237498983db0901dbb707f5dce3f3ff8644b1a59fc87f2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34456820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81b089e33ba1ff9d0a4c5ea7ea02ff345eecf723a5f37e77c3a5f6370d04fb6a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 21:24:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:24:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:24:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:03 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68378f1e43a78d07ba7d4b063f86a4e752c51e3c3914a1ff9f743500f2c2f04`  
		Last Modified: Wed, 03 May 2023 21:26:39 GMT  
		Size: 3.8 MB (3765930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd168bc42e411f97adae10afe4f4653177647bfa55537a25131255844ae61492`  
		Last Modified: Wed, 03 May 2023 21:26:38 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2795c37902804d36644ab4b665f46a0a7cd526cf7843ccb4f01a084f2f61b7f7`  
		Last Modified: Wed, 03 May 2023 21:26:38 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1bb371f422afeb35fe873149a69cd084948e4a52ccd4419517b1844083c725`  
		Last Modified: Wed, 03 May 2023 21:26:39 GMT  
		Size: 258.4 KB (258401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaaff2d156044fdfe75ec46bb7652265e374df2902b2766bb0208ff13b5cd08`  
		Last Modified: Wed, 03 May 2023 21:26:47 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd22.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:c0f03351042a370adc1e419ec75369af3eabf56c223100470cc142334bfdccf6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32389189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc517a41591c8a5b4fc00b1fefcff5cd72f162496949d7f5156e81b26fe48f9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Wed, 03 May 2023 19:05:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:05:46 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 19:05:47 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 19:05:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:05:55 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce53cea779733273cf24ec55276dac6cc9c77563b4244ce762d9679e6120250`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 3.7 MB (3738566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ed0729e8a293b6757d2d1e1f3945beb7567375d912abd1eefd688798dd1042`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daab176d4e2a4476e6e1bcef5fb4561c2b05e1c0b3913d2d61cbc02ffe5bb95f`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399a285c321748b47e8da6e14e89e40a30db11775c6d6666a0dd2cc2041475d6`  
		Last Modified: Wed, 03 May 2023 19:07:38 GMT  
		Size: 258.9 KB (258908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca0a9caa9aeb605ad9d4ed83546b347dcb848fd80067f47538f8cca723c5417`  
		Last Modified: Wed, 03 May 2023 19:07:46 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:non-free`

```console
$ docker pull neurodebian@sha256:0f540c18829c6396c0c23e747525582fa1e7cbbed1540d58be6c9b359e58f23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:0e03b2debd7a1d5f28aa746ae3e4ce140ed6790d63f39f6a5b71521e88769c50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3331ef22a29d7e47c420e4814e93b37e21973c5540cbb66fd17f4fc9a81b223`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:31 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:38 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b9629c74f273da9190027c7e4cc11bf7b9c6a5bc037f53f26812b96307cee1`  
		Last Modified: Wed, 03 May 2023 21:27:14 GMT  
		Size: 11.3 MB (11310941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e479d911c8ceb5e5f2c92b8d68425475e3255bf6caf9fb40846df32dd54750`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b2393d1b1e6ae558b4e42a05a8fbd0a1cb5a6deadd71a2bdaff11b3fb8691d`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103058a946030129417ba0563768d175caae3f6b41f4787c1b86b420cdb7e639`  
		Last Modified: Wed, 03 May 2023 21:27:12 GMT  
		Size: 312.0 KB (312023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a786115a54951b49a2de00541f08f3fb81963b0a9827b745be73197ea4ddb51f`  
		Last Modified: Wed, 03 May 2023 21:27:23 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:efc47b01c41eca49e029b269638c650adfd2a8f0e73807c748f9c7bc1f36cbce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65319984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4ebde6630ed604716cbd5f83c480bc3a7e5e2d8cce1d68c1355581fcfcf157`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:29:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:29:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:57 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187c756d024d4e7c2776681889618e1a5149fc672ed0aac61d785f286e69cb45`  
		Last Modified: Tue, 23 May 2023 02:31:19 GMT  
		Size: 11.3 MB (11313121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0227cf7a0eaf0af3c3c1164de31c4c5555f9f5b511769db242fdc93b238f9876`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78eb1f7c1bac7ebaea871680d53583c59acee5339b44ced2f4aa3cb3e1aa6cb`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7532dbe02d3f898678b483d0df372497ea9472a859b411edd0993544bab9cd6c`  
		Last Modified: Tue, 23 May 2023 02:31:18 GMT  
		Size: 311.9 KB (311882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfc256c442e8e637b8a0cece189d2a76422322f8ee48f5be12c1dce583cbdd2`  
		Last Modified: Tue, 23 May 2023 02:31:28 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:fe3bde78aeb9790898d619b54ac53eb63822edbd4b7823a0984d80631bb65fed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68051278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7adfc07d9da7329f3d6d9ae824556b77b534f5b7c95c239975fbedff4eb071e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:45 GMT
ADD file:59d53253d7691be0330c735eb4b57791a8fc5894572d3deaeb7138cce45132ad in / 
# Wed, 03 May 2023 00:00:46 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:16:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:16:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:16:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:16:52 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:6ac0eb37fce5e6fca952bf804df5de5ebb63724d4d44bf23abc5d5736ee32afd`  
		Last Modified: Wed, 03 May 2023 00:04:44 GMT  
		Size: 56.0 MB (56029150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c794418bd1e96a39bea1aef2c4f245b825ec4e16a1d2fa3222521c51cbe7cd8`  
		Last Modified: Wed, 03 May 2023 23:18:05 GMT  
		Size: 11.7 MB (11707936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65e0e0e73c24570aa784364602cf64cd9331769082f140bfa988aad91ce79b9`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6e2c410c8e6b068d6692e30b9d8d56a1e0bf11cf420a3f030fe862b4a566f`  
		Last Modified: Wed, 03 May 2023 23:18:03 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbe2da83496475fac6b9656e8be553e28e545fab227c1cc1c666a89f3141f1b`  
		Last Modified: Wed, 03 May 2023 23:18:04 GMT  
		Size: 311.8 KB (311820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c5defbdb36be91b752ff0f2512091c04e98799ae0c1c8c8ace8eede4671471`  
		Last Modified: Wed, 03 May 2023 23:18:15 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:f23ec75f325ccd8daf51abfb2a5149de40d45fb20837f646dd63a14b24f62e7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:bfe67002364838700c76c1c3a2f8ceaf639c6a6298213f3518a0dc9635906c92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61305792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7628118084f66e224ab75edf762667e0641ead33e66b059e71a6299bd2c7eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:42 GMT
ADD file:6261ecb921e04d2b3f6fd44e5dcb5683154bc0beee4f26913c2be9395a060489 in / 
# Tue, 02 May 2023 23:47:43 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:26:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:26:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:26:08 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:26:12 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae396e350f30e1defad1bfa67a84b97389d42cf3442551e39a0e2bab6b53a50c`  
		Last Modified: Tue, 02 May 2023 23:51:56 GMT  
		Size: 49.3 MB (49299270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07001fa6af159175c58303f7752dd97019fd06951e7055bcb076e5194afa064f`  
		Last Modified: Wed, 03 May 2023 21:27:50 GMT  
		Size: 11.7 MB (11719904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdf86d32a3b26b1c1bd693d70bc6115b98a87379e31ff8b6f6b9f7ed9009fe3`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dee1f3f9a40aee303f152160ad22cf80424301d6e75afcd194d8f83d27543`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745484e4809d3b3760d3a506060c0d4454cf63ff0de190c172235e7f825eaa2f`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 284.6 KB (284611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:d63d9cec9204a1302b94dc0ebc95380ddb757f99edcab9571a3411fa6810db0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61310676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4ab96d35dc7bbfedb971394bb6ee81f1fa0c5b00bef37652c482f0bda38537c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:48 GMT
ADD file:4608b82b211b6814e5bf372be706a6c01bd7a2a4841b59ac5430ec3a3f94468d in / 
# Tue, 23 May 2023 00:43:49 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:30:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:30:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:30:36 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5842d200e3f7df637a96b64f14e82ccb2c66e201137165f2d91447fbd3248a8c`  
		Last Modified: Tue, 23 May 2023 00:47:31 GMT  
		Size: 49.3 MB (49336298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5dc20c7009c0c4fb8fcc9510272b9663f770c650ec6a79065e104de65ae083`  
		Last Modified: Tue, 23 May 2023 02:31:55 GMT  
		Size: 11.7 MB (11685804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70e50d9fe81355ff8795fe4ebe3fa83df06646ae08c427d3ce1f270d69c679c`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b1dce6b21c52e13c5410c66209fa00c80743c2703fa7deb3e2a45c521dab`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ee43739ae5dd8545181114be4dc1eda914eac3630aaf0547acfc5fd4f213a9`  
		Last Modified: Tue, 23 May 2023 02:31:54 GMT  
		Size: 286.6 KB (286566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; 386

```console
$ docker pull neurodebian@sha256:d2bf9bf510a5c7063207246fd743a970aa3f2a21bf17e4e60252263a3c93ae9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62752295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5570ba7043d26acb17e3c64bfbf3e4eb1c63eea6d8eb31e7bb571b09dcba5a71`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:59 GMT
ADD file:4abf127b0d4037b2d94457a8ef168165ed6946fec0635fdaa845ed4ee8f74681 in / 
# Wed, 03 May 2023 00:02:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:17:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:17:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:17:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:125509149936f5c9fc010cb99811f5cb23108af74e034fcf0903d3f2cc08d893`  
		Last Modified: Wed, 03 May 2023 00:06:56 GMT  
		Size: 50.3 MB (50321774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03401a139b285d7dbabf9bf47070d8513369654c65656e0c9d884753d539277f`  
		Last Modified: Wed, 03 May 2023 23:18:43 GMT  
		Size: 12.1 MB (12143791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5281eb68b6af5d72745e5c9b4b79dd83518a7577dc0fe9d915aded3a47e043`  
		Last Modified: Wed, 03 May 2023 23:18:41 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d185612295077c05c7f4013d0363a5a2d03ec6b9616cdd174458890a2a4a127b`  
		Last Modified: Wed, 03 May 2023 23:18:41 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab7c155e27703e280eaf8bb7af29a7e4811f8eff90e33735e85d08540012bcd`  
		Last Modified: Wed, 03 May 2023 23:18:42 GMT  
		Size: 284.7 KB (284722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:81280c9b90b55267fcd5d76144088664479223b24fac457ea232c971fd200fb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:3e1fda817390144cf38a8ad2261957ecaf31672324e8ebf505ea503b8c18acae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03316cf4967259749fc22171bdee854ef9b9aff3303b43444791690fb75e0d6d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:42 GMT
ADD file:6261ecb921e04d2b3f6fd44e5dcb5683154bc0beee4f26913c2be9395a060489 in / 
# Tue, 02 May 2023 23:47:43 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:26:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:26:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:26:08 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:26:12 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:26:15 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ae396e350f30e1defad1bfa67a84b97389d42cf3442551e39a0e2bab6b53a50c`  
		Last Modified: Tue, 02 May 2023 23:51:56 GMT  
		Size: 49.3 MB (49299270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07001fa6af159175c58303f7752dd97019fd06951e7055bcb076e5194afa064f`  
		Last Modified: Wed, 03 May 2023 21:27:50 GMT  
		Size: 11.7 MB (11719904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdf86d32a3b26b1c1bd693d70bc6115b98a87379e31ff8b6f6b9f7ed9009fe3`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dee1f3f9a40aee303f152160ad22cf80424301d6e75afcd194d8f83d27543`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745484e4809d3b3760d3a506060c0d4454cf63ff0de190c172235e7f825eaa2f`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 284.6 KB (284611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8500a41f7e728906fca7f1d637852202a87f9ea250eec4cfdf14f4a10d85694`  
		Last Modified: Wed, 03 May 2023 21:27:58 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:48c979657bcab083b5a181f205a8ba52a3218b18bed5b443ebeb4bc8cc33fafa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61311075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aa7f0542b4bfb7559aeef459dc4cc4d68c1a8b4ba610d3fafee39694f4623e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:43:48 GMT
ADD file:4608b82b211b6814e5bf372be706a6c01bd7a2a4841b59ac5430ec3a3f94468d in / 
# Tue, 23 May 2023 00:43:49 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:30:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:30:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:30:36 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:40 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:5842d200e3f7df637a96b64f14e82ccb2c66e201137165f2d91447fbd3248a8c`  
		Last Modified: Tue, 23 May 2023 00:47:31 GMT  
		Size: 49.3 MB (49336298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5dc20c7009c0c4fb8fcc9510272b9663f770c650ec6a79065e104de65ae083`  
		Last Modified: Tue, 23 May 2023 02:31:55 GMT  
		Size: 11.7 MB (11685804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70e50d9fe81355ff8795fe4ebe3fa83df06646ae08c427d3ce1f270d69c679c`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b1dce6b21c52e13c5410c66209fa00c80743c2703fa7deb3e2a45c521dab`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ee43739ae5dd8545181114be4dc1eda914eac3630aaf0547acfc5fd4f213a9`  
		Last Modified: Tue, 23 May 2023 02:31:54 GMT  
		Size: 286.6 KB (286566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93ad45069d23343bb6311642e0f863b5900a8b9eea8b859b2bbe1721dff1f09`  
		Last Modified: Tue, 23 May 2023 02:32:02 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:3b55d7527f746dda6b623936b102556d07bb27844f33f3b3a73f3fd4d4cc287b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62752686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a3f168461765aee166a808516f45328083a8569d9221c64fbe2fd8c2ab84650`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:59 GMT
ADD file:4abf127b0d4037b2d94457a8ef168165ed6946fec0635fdaa845ed4ee8f74681 in / 
# Wed, 03 May 2023 00:02:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:17:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:17:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:17:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:34 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:125509149936f5c9fc010cb99811f5cb23108af74e034fcf0903d3f2cc08d893`  
		Last Modified: Wed, 03 May 2023 00:06:56 GMT  
		Size: 50.3 MB (50321774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03401a139b285d7dbabf9bf47070d8513369654c65656e0c9d884753d539277f`  
		Last Modified: Wed, 03 May 2023 23:18:43 GMT  
		Size: 12.1 MB (12143791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5281eb68b6af5d72745e5c9b4b79dd83518a7577dc0fe9d915aded3a47e043`  
		Last Modified: Wed, 03 May 2023 23:18:41 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d185612295077c05c7f4013d0363a5a2d03ec6b9616cdd174458890a2a4a127b`  
		Last Modified: Wed, 03 May 2023 23:18:41 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab7c155e27703e280eaf8bb7af29a7e4811f8eff90e33735e85d08540012bcd`  
		Last Modified: Wed, 03 May 2023 23:18:42 GMT  
		Size: 284.7 KB (284722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5fa32322a1c07f34e547f4775540f6eab3c1d3464b5a006bd5c2449a0bced3`  
		Last Modified: Wed, 03 May 2023 23:18:51 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
