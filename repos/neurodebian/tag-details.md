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
$ docker pull neurodebian@sha256:b69b9cebdfd8b83213c9c6932c85b7c7923cee9a49ba2b9a3b702ee8ad38359b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm` - linux; amd64

```console
$ docker pull neurodebian@sha256:baabb08f7f35eece8fe86b5cca134eb909f7605d48b5070fc38ff2584518df2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61307789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f47799e2bf3d6bb22f8204885da1e8a33389ad6326faf0f6abdb17224ff07f3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:19:36 GMT
ADD file:aea4560c39a3a877086fc63afdf218ba3600a05abef7c44563f788e8b60c04ef in / 
# Tue, 23 May 2023 01:19:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:23:01 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:02 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:23:03 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:23:06 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c98dda1b0e97e7fa61fa33cea43f85bb1a36a4f6f65c7b8430cae442b76ece09`  
		Last Modified: Tue, 23 May 2023 01:23:14 GMT  
		Size: 49.3 MB (49301275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33627279e466d7f7d1e2299fc1f1ef0aba016364269114db58eefb5bc4f174fe`  
		Last Modified: Tue, 23 May 2023 04:24:30 GMT  
		Size: 11.7 MB (11719838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc38d23881ba02c585bb2b72b06f955689ebf8e30cce25285d5c6ded4b79550`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179908f928b0af97bceaffff9a265d97bffd58aa45ff6ec4b2b6595b33b7bb3d`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b52941f1978acefe1f1b3a5493124b6927d21693f82780f76726caab179a1b9`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 284.7 KB (284664 bytes)  
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
$ docker pull neurodebian@sha256:8764e75acf0b0d9877c509c66f2decc88573d88ddba2da984c14c771b505d3e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62753602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:525bc620b64464f1c6f7d5fafe4c31be7f124b8a9cd79ce2422d9335855f5138`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:38:43 GMT
ADD file:4d14207b5cf935fa2b9de70132f41a0eb90a8b5200ed3d27e60b766fc6131e13 in / 
# Tue, 23 May 2023 00:38:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:43:10 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:43:12 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:43:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22e40771358829b6817b47cb2d682b51257385478c18bb1ec96251a68a9c75e4`  
		Last Modified: Tue, 23 May 2023 00:43:23 GMT  
		Size: 50.3 MB (50323189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c247d5ed731b6493a71fa628813b52b9d64900d688cef945f8c5b85ed9b2690`  
		Last Modified: Tue, 23 May 2023 05:44:33 GMT  
		Size: 12.1 MB (12143667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4ef75fcb9af10a6ff980ed195a464fff7047d4905d4d99184bd7f27a313cde`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fab7974bae62c89adabeae697146cde0caf8f16c854425dfd1aadafebeb2b12`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d4b90c50e699685d80e5102a8756309b6103a931798615b13c4ed4b16df39`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 284.7 KB (284735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm-non-free`

```console
$ docker pull neurodebian@sha256:b402dbf57d17caed337237f154a5cdd1ad740cda0a99babda118d593197a86be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:9e34ce5c236de895d1aee892e0aadae7d75a19c75fe0d4544fe642c97ce44b28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61308217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf96f115f3a71ad93f74b628601aba8b6460282524cf285a40ae9a784ae7ae48`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:19:36 GMT
ADD file:aea4560c39a3a877086fc63afdf218ba3600a05abef7c44563f788e8b60c04ef in / 
# Tue, 23 May 2023 01:19:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:23:01 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:02 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:23:03 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:23:06 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:10 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c98dda1b0e97e7fa61fa33cea43f85bb1a36a4f6f65c7b8430cae442b76ece09`  
		Last Modified: Tue, 23 May 2023 01:23:14 GMT  
		Size: 49.3 MB (49301275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33627279e466d7f7d1e2299fc1f1ef0aba016364269114db58eefb5bc4f174fe`  
		Last Modified: Tue, 23 May 2023 04:24:30 GMT  
		Size: 11.7 MB (11719838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc38d23881ba02c585bb2b72b06f955689ebf8e30cce25285d5c6ded4b79550`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179908f928b0af97bceaffff9a265d97bffd58aa45ff6ec4b2b6595b33b7bb3d`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b52941f1978acefe1f1b3a5493124b6927d21693f82780f76726caab179a1b9`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 284.7 KB (284664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6363d30de594fa89c4fafd1a441b7ea23b4a565e0f0902e4d226e73c22c5edf0`  
		Last Modified: Tue, 23 May 2023 04:24:38 GMT  
		Size: 428.0 B  
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
$ docker pull neurodebian@sha256:25200d6048a13ef9220e62f845de1441b53e5ce2d49f5642b3174eda494a1975
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62754031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fb8a1cffbdfa3a0dc9916920eacf40dfdfa74532919c0059d8b6ad8cb5b20c3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:38:43 GMT
ADD file:4d14207b5cf935fa2b9de70132f41a0eb90a8b5200ed3d27e60b766fc6131e13 in / 
# Tue, 23 May 2023 00:38:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:43:10 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:43:12 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:43:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:21 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:22e40771358829b6817b47cb2d682b51257385478c18bb1ec96251a68a9c75e4`  
		Last Modified: Tue, 23 May 2023 00:43:23 GMT  
		Size: 50.3 MB (50323189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c247d5ed731b6493a71fa628813b52b9d64900d688cef945f8c5b85ed9b2690`  
		Last Modified: Tue, 23 May 2023 05:44:33 GMT  
		Size: 12.1 MB (12143667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4ef75fcb9af10a6ff980ed195a464fff7047d4905d4d99184bd7f27a313cde`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fab7974bae62c89adabeae697146cde0caf8f16c854425dfd1aadafebeb2b12`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d4b90c50e699685d80e5102a8756309b6103a931798615b13c4ed4b16df39`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 284.7 KB (284735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e868cd6c65860bf552879c80292c1c5c5d73ee61bc17eaab036c8fc0231f0a5`  
		Last Modified: Tue, 23 May 2023 05:44:41 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:58ede793451b5dcd9b8484cdf7a4d96286b7ca6dd4cd7691b09bcee139a37c03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:7f15da2016b618ea07c99f0db53a7d4d811f7d3a1e07b3dcfc62aa706a62d14b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d3c77884c39fcf8c8197b0e9da8509b340aac50f30d7d6f7927089ca89bbbc2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:22:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:22:42 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:22:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c8f317bbcc308a1e6f1fac03e1e3a9f2a39fc82e936c0570d59117b539f98b`  
		Last Modified: Tue, 23 May 2023 04:24:10 GMT  
		Size: 11.3 MB (11310985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339b1ccbf456e866652af2b8427b66dc919fc8ff09b50fc20bbadf9864f1299e`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec272ec7995fd0da0e4007df35052366ac83178183bc9be766a7c07054484d`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b179b6be05eca9ee18ca837dfeafb6f09c1357d864b810f767c3b8c7e6150efa`  
		Last Modified: Tue, 23 May 2023 04:24:09 GMT  
		Size: 312.0 KB (311996 bytes)  
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
$ docker pull neurodebian@sha256:e013ecaa24d4606f907599811071f8b27f5c368a4f3b70509ff650713c26f7f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68050980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b877fcd3514ab2d8dc777764b898ba9ff9a8029ad45de0c1312ca006cec9a203`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:14 GMT
ADD file:acdf45f51b991111aa6c929fedd4e8de03e5d42578cca2f895f74697c3c66e33 in / 
# Tue, 23 May 2023 00:39:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:42:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:42:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:42:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c377769761bd9f2bd79d27a4f6dfa29be1047f4e6e8df1653027ef5262e020bb`  
		Last Modified: Tue, 23 May 2023 00:44:01 GMT  
		Size: 56.0 MB (56029173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaae1eed722697680293151e7092e07fa7042893bd549883ec3cc9b401babf0`  
		Last Modified: Tue, 23 May 2023 05:44:13 GMT  
		Size: 11.7 MB (11707960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c029d5297bd9708c2063123e4843df78700aa651c8968e98d0bb366528c3a761`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf405f235e316c73593fa6527a595699f0597ddcd7b09a16cf17b7c645e3b76`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a472eab1c6eb96814a14e198ebc46c183ff9b9b7a4b5244cd7133a8db20481`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 311.8 KB (311833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye-non-free`

```console
$ docker pull neurodebian@sha256:c7e4e9212de829ff29050399e6e4223a7a0940a9e224e39068f2aafa3fb0870c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:58b179e8710e5d072a22ab3c4c24817c15d3b73a6a48cb1906158618473afd50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7403edb772c4b84cae3e2436b127af6bff49d8bd52c824a2369855ab5f1e48ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:22:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:22:42 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:22:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:48 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c8f317bbcc308a1e6f1fac03e1e3a9f2a39fc82e936c0570d59117b539f98b`  
		Last Modified: Tue, 23 May 2023 04:24:10 GMT  
		Size: 11.3 MB (11310985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339b1ccbf456e866652af2b8427b66dc919fc8ff09b50fc20bbadf9864f1299e`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec272ec7995fd0da0e4007df35052366ac83178183bc9be766a7c07054484d`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b179b6be05eca9ee18ca837dfeafb6f09c1357d864b810f767c3b8c7e6150efa`  
		Last Modified: Tue, 23 May 2023 04:24:09 GMT  
		Size: 312.0 KB (311996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6846656eb9c3c17db60e2ba659abb84645043fa6fbdaac726e3f617c4afb4c09`  
		Last Modified: Tue, 23 May 2023 04:24:19 GMT  
		Size: 360.0 B  
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
$ docker pull neurodebian@sha256:317b5120cde566e6c15f029bb71d9b2dc8824edd485de316291dd44741f169f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68051343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:156c0f22d08a31852143fea310856afdb1ab248f648e45cf25dcc9b45aec549b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:14 GMT
ADD file:acdf45f51b991111aa6c929fedd4e8de03e5d42578cca2f895f74697c3c66e33 in / 
# Tue, 23 May 2023 00:39:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:42:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:42:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:42:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:56 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c377769761bd9f2bd79d27a4f6dfa29be1047f4e6e8df1653027ef5262e020bb`  
		Last Modified: Tue, 23 May 2023 00:44:01 GMT  
		Size: 56.0 MB (56029173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaae1eed722697680293151e7092e07fa7042893bd549883ec3cc9b401babf0`  
		Last Modified: Tue, 23 May 2023 05:44:13 GMT  
		Size: 11.7 MB (11707960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c029d5297bd9708c2063123e4843df78700aa651c8968e98d0bb366528c3a761`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf405f235e316c73593fa6527a595699f0597ddcd7b09a16cf17b7c645e3b76`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a472eab1c6eb96814a14e198ebc46c183ff9b9b7a4b5244cd7133a8db20481`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 311.8 KB (311833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10c00d49702288a28d1849a812fd1703827069b7342dc19848b5859eb83a678`  
		Last Modified: Tue, 23 May 2023 05:44:22 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:be0623771211bf72794bc7a4e5ba4445cc041529b2195f01063e59ddaa06655c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:a54a0e6a43c82ac92956cc38be35595d319d742722e9b8b047949498d504ab89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61259662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486e428db546a885e4035ba89a4f616b68f09845e5e4516434534d8d05c05a06`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:24 GMT
ADD file:9d769df745075dbc4cd2c01ca784571a0df008f6b650b895a7f92d3281132807 in / 
# Tue, 23 May 2023 01:20:25 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:22:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:22:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:22:30 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c722db24a050621ee87ea07acd5d066d3d6a94737c32012f27d73a1ad5cc645c`  
		Last Modified: Tue, 23 May 2023 01:24:26 GMT  
		Size: 50.4 MB (50448716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5580aa8b086cc8c6dc3c839df2b54e92d4785fc4e9b824c0da7819479aa00`  
		Last Modified: Tue, 23 May 2023 04:23:53 GMT  
		Size: 10.5 MB (10504489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fae9d7e648f7f5be8b0df37a4284949621932cbe6f4f3ad8a51c76867b82d1`  
		Last Modified: Tue, 23 May 2023 04:23:52 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09094d5b9484661a6878ceaf9f02e2d901afebadcdb601e0deb31411ce74c26`  
		Last Modified: Tue, 23 May 2023 04:23:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee599431be61d0a5ed744c9cb86ef6b4d02c23e602e36f5a2ac021111dca7ca`  
		Last Modified: Tue, 23 May 2023 04:23:53 GMT  
		Size: 304.5 KB (304451 bytes)  
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
$ docker pull neurodebian@sha256:6f8924222996b6666b244ad59ffa72cd53789c28367bc6c4c5516ac65ec23933
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62380281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cab147f8daa11258c7e63b95ad5170ed4d51e503ff0cbb25c526c509ed920b9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:45 GMT
ADD file:d82a514985e1c8796d6c5572290d84fdff0dc1c748d7d2e469d3066ac0344c5f in / 
# Tue, 23 May 2023 00:39:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:42:25 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:26 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:42:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:42:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a48e9012f51ff679af95460521da76c7184da775e3adaa39fed65c912ce0a57`  
		Last Modified: Tue, 23 May 2023 00:44:49 GMT  
		Size: 51.2 MB (51205678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4226282d9c19402a2492d1ec19244689e7600cc6b9fc41325278c52d8b5b9e0`  
		Last Modified: Tue, 23 May 2023 05:43:56 GMT  
		Size: 10.9 MB (10868296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542327d6541db55160c5e48c276b22429d6e27856e8d86a7d00da85d2b3b8cda`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3e74af901c5e67254d5cdc0ff3c41bef80b4b9cabfd174697af611d6406377`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cf355598094ecd630526aed002e391ba7365154fd960d40bdc635d92a68585`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 304.3 KB (304298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:132b8fa6f0a9fac5455b659b41bc620720fe7f602757e2800f2092a7aa1f4ae2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:44806c8d2020d66ae467d0812cde42ad45fddb5e0a8ff7b427793a23d6a447b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61260017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7823c1a9101821c016ca63cf774e6a8ccd0cc61aa8d9a1099d7a61f8b7e71f0d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:24 GMT
ADD file:9d769df745075dbc4cd2c01ca784571a0df008f6b650b895a7f92d3281132807 in / 
# Tue, 23 May 2023 01:20:25 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:22:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:22:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:22:30 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:32 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c722db24a050621ee87ea07acd5d066d3d6a94737c32012f27d73a1ad5cc645c`  
		Last Modified: Tue, 23 May 2023 01:24:26 GMT  
		Size: 50.4 MB (50448716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5580aa8b086cc8c6dc3c839df2b54e92d4785fc4e9b824c0da7819479aa00`  
		Last Modified: Tue, 23 May 2023 04:23:53 GMT  
		Size: 10.5 MB (10504489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fae9d7e648f7f5be8b0df37a4284949621932cbe6f4f3ad8a51c76867b82d1`  
		Last Modified: Tue, 23 May 2023 04:23:52 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09094d5b9484661a6878ceaf9f02e2d901afebadcdb601e0deb31411ce74c26`  
		Last Modified: Tue, 23 May 2023 04:23:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee599431be61d0a5ed744c9cb86ef6b4d02c23e602e36f5a2ac021111dca7ca`  
		Last Modified: Tue, 23 May 2023 04:23:53 GMT  
		Size: 304.5 KB (304451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd539f4479d039165c3dd5ad7548b8840bfb1e87810c63a90fd25f2c4cc371`  
		Last Modified: Tue, 23 May 2023 04:24:01 GMT  
		Size: 355.0 B  
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
$ docker pull neurodebian@sha256:d8a746880aac51b323612d7e3af5bd6a1f7a1090a55f7ac5a75776ea460b884d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62380639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f60a1dc4fd3e415746e9d747980bcd556aa03b22d84fa99454e480123069fd97`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:45 GMT
ADD file:d82a514985e1c8796d6c5572290d84fdff0dc1c748d7d2e469d3066ac0344c5f in / 
# Tue, 23 May 2023 00:39:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:42:25 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:26 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:42:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:42:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:35 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:5a48e9012f51ff679af95460521da76c7184da775e3adaa39fed65c912ce0a57`  
		Last Modified: Tue, 23 May 2023 00:44:49 GMT  
		Size: 51.2 MB (51205678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4226282d9c19402a2492d1ec19244689e7600cc6b9fc41325278c52d8b5b9e0`  
		Last Modified: Tue, 23 May 2023 05:43:56 GMT  
		Size: 10.9 MB (10868296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542327d6541db55160c5e48c276b22429d6e27856e8d86a7d00da85d2b3b8cda`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3e74af901c5e67254d5cdc0ff3c41bef80b4b9cabfd174697af611d6406377`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cf355598094ecd630526aed002e391ba7365154fd960d40bdc635d92a68585`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 304.3 KB (304298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f216b2323999a15c9f3d04e270325018173befad613dffa8ccba0696305277d1`  
		Last Modified: Tue, 23 May 2023 05:44:04 GMT  
		Size: 358.0 B  
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
$ docker pull neurodebian@sha256:58ede793451b5dcd9b8484cdf7a4d96286b7ca6dd4cd7691b09bcee139a37c03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:7f15da2016b618ea07c99f0db53a7d4d811f7d3a1e07b3dcfc62aa706a62d14b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d3c77884c39fcf8c8197b0e9da8509b340aac50f30d7d6f7927089ca89bbbc2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:22:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:22:42 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:22:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c8f317bbcc308a1e6f1fac03e1e3a9f2a39fc82e936c0570d59117b539f98b`  
		Last Modified: Tue, 23 May 2023 04:24:10 GMT  
		Size: 11.3 MB (11310985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339b1ccbf456e866652af2b8427b66dc919fc8ff09b50fc20bbadf9864f1299e`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec272ec7995fd0da0e4007df35052366ac83178183bc9be766a7c07054484d`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b179b6be05eca9ee18ca837dfeafb6f09c1357d864b810f767c3b8c7e6150efa`  
		Last Modified: Tue, 23 May 2023 04:24:09 GMT  
		Size: 312.0 KB (311996 bytes)  
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
$ docker pull neurodebian@sha256:e013ecaa24d4606f907599811071f8b27f5c368a4f3b70509ff650713c26f7f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68050980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b877fcd3514ab2d8dc777764b898ba9ff9a8029ad45de0c1312ca006cec9a203`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:14 GMT
ADD file:acdf45f51b991111aa6c929fedd4e8de03e5d42578cca2f895f74697c3c66e33 in / 
# Tue, 23 May 2023 00:39:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:42:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:42:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:42:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c377769761bd9f2bd79d27a4f6dfa29be1047f4e6e8df1653027ef5262e020bb`  
		Last Modified: Tue, 23 May 2023 00:44:01 GMT  
		Size: 56.0 MB (56029173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaae1eed722697680293151e7092e07fa7042893bd549883ec3cc9b401babf0`  
		Last Modified: Tue, 23 May 2023 05:44:13 GMT  
		Size: 11.7 MB (11707960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c029d5297bd9708c2063123e4843df78700aa651c8968e98d0bb366528c3a761`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf405f235e316c73593fa6527a595699f0597ddcd7b09a16cf17b7c645e3b76`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a472eab1c6eb96814a14e198ebc46c183ff9b9b7a4b5244cd7133a8db20481`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 311.8 KB (311833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:b7eabe01fca7074e04d46dd14d8dc8b6b1cdf141a0c35821b83235e913ea4b88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:d4373ee7bb59ea1b6932dff39a08917c9ecea36de486c81c414c786c4695120b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61299586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac725a56cfb49d044c98bc06afd02334e0c25d27aac6c54eaadc6d18dd114da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:21:12 GMT
ADD file:3b942ada2dbba1c073e568411a383d6ab987c117af5bbb011afd46549d64c4dc in / 
# Tue, 23 May 2023 01:21:12 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:23:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:23:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:23:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8285c3e1284db51d7096ff9c9434e138a00153495c655a040787b10e562b7515`  
		Last Modified: Tue, 23 May 2023 01:25:36 GMT  
		Size: 49.3 MB (49289184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158a1759b167defe3ac364f8157c49f063c470a5a956e0d702fc47b0a929f38`  
		Last Modified: Tue, 23 May 2023 04:24:47 GMT  
		Size: 11.7 MB (11722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f37d696beaa9b72a35a3d14f54f0b856dcc0621888c8afb8cc7ddda831e3310`  
		Last Modified: Tue, 23 May 2023 04:24:45 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e94a7d5efaab58c44a59d954d27135a86f8e445818b065a841ac08f6f00544`  
		Last Modified: Tue, 23 May 2023 04:24:45 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b33126a764321fb1a50ada00da1192641da6f41c03432c227137e50acd8357`  
		Last Modified: Tue, 23 May 2023 04:24:46 GMT  
		Size: 286.3 KB (286314 bytes)  
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
$ docker pull neurodebian@sha256:ca6fb83db48276fe96ae643fd4c1acaf9846431386d9ab11596e85fb2acbb08d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.7 MB (62745155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:435d9c6d98412b4bdf45e80888addecd13eb835ab8cdb7eef2b256c5a8554ee6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:40:47 GMT
ADD file:33dd3eb2725f92170606ce015e99cc9496d244630b3f4844cb8f3f61b16e2eb0 in / 
# Tue, 23 May 2023 00:40:48 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:43:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:43:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:43:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1034171b4bde64cf8e4ff854704a3bf68000eddcceb63b481197082dced785ba`  
		Last Modified: Tue, 23 May 2023 00:46:09 GMT  
		Size: 50.3 MB (50311497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb94666b190ba95be7fadf283441a70d7afa10a0b07170b8674ec2678968d429`  
		Last Modified: Tue, 23 May 2023 05:44:50 GMT  
		Size: 12.1 MB (12145347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf7364560006b36553ea625f2134dc9718506f9939d605cf9bbeffa03222aa8`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e68c126603fa53d236ac3cef352fb8266303d1f60ea86c338b5a104baa5a545`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fef25ab16b5c30aa387e5e2d002d54aff3c430bb03a10607bffcb018bc94d4`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 286.3 KB (286305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:60a78434fdd546c8d2fc025282e6431fa3a5a5ec5dfb00ab19c7bf2c532572c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:c3cd2902ff137d947cf1183caee8e2e881476148001aea0c106652a0982d3310
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61299977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:757103b2b0ac7345e1a0dcb71a788028ccd7ab37e1a27cf53cb423724f8f4ab2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:21:12 GMT
ADD file:3b942ada2dbba1c073e568411a383d6ab987c117af5bbb011afd46549d64c4dc in / 
# Tue, 23 May 2023 01:21:12 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:23:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:23:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:23:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:29 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:8285c3e1284db51d7096ff9c9434e138a00153495c655a040787b10e562b7515`  
		Last Modified: Tue, 23 May 2023 01:25:36 GMT  
		Size: 49.3 MB (49289184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158a1759b167defe3ac364f8157c49f063c470a5a956e0d702fc47b0a929f38`  
		Last Modified: Tue, 23 May 2023 04:24:47 GMT  
		Size: 11.7 MB (11722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f37d696beaa9b72a35a3d14f54f0b856dcc0621888c8afb8cc7ddda831e3310`  
		Last Modified: Tue, 23 May 2023 04:24:45 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e94a7d5efaab58c44a59d954d27135a86f8e445818b065a841ac08f6f00544`  
		Last Modified: Tue, 23 May 2023 04:24:45 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b33126a764321fb1a50ada00da1192641da6f41c03432c227137e50acd8357`  
		Last Modified: Tue, 23 May 2023 04:24:46 GMT  
		Size: 286.3 KB (286314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c80b51ea09266240fd930629cb4fb877838167da0961769224e46b9843a810`  
		Last Modified: Tue, 23 May 2023 04:24:56 GMT  
		Size: 391.0 B  
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
$ docker pull neurodebian@sha256:6753b469ed406da38695358a52a1c87e179ebe14d42c59b452a6cf03dc178c54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.7 MB (62745547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d6d3c089bd7ecb7dece0a9305fb5900887130cddead11f80b1b13b0fb57b418`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:40:47 GMT
ADD file:33dd3eb2725f92170606ce015e99cc9496d244630b3f4844cb8f3f61b16e2eb0 in / 
# Tue, 23 May 2023 00:40:48 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:43:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:43:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:43:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:42 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:1034171b4bde64cf8e4ff854704a3bf68000eddcceb63b481197082dced785ba`  
		Last Modified: Tue, 23 May 2023 00:46:09 GMT  
		Size: 50.3 MB (50311497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb94666b190ba95be7fadf283441a70d7afa10a0b07170b8674ec2678968d429`  
		Last Modified: Tue, 23 May 2023 05:44:50 GMT  
		Size: 12.1 MB (12145347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf7364560006b36553ea625f2134dc9718506f9939d605cf9bbeffa03222aa8`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e68c126603fa53d236ac3cef352fb8266303d1f60ea86c338b5a104baa5a545`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fef25ab16b5c30aa387e5e2d002d54aff3c430bb03a10607bffcb018bc94d4`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 286.3 KB (286305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da399a07548054d441160ab6c71e0f30793cf8071685057f199a0590aba9ad84`  
		Last Modified: Tue, 23 May 2023 05:44:57 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100`

```console
$ docker pull neurodebian@sha256:be0623771211bf72794bc7a4e5ba4445cc041529b2195f01063e59ddaa06655c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100` - linux; amd64

```console
$ docker pull neurodebian@sha256:a54a0e6a43c82ac92956cc38be35595d319d742722e9b8b047949498d504ab89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61259662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486e428db546a885e4035ba89a4f616b68f09845e5e4516434534d8d05c05a06`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:24 GMT
ADD file:9d769df745075dbc4cd2c01ca784571a0df008f6b650b895a7f92d3281132807 in / 
# Tue, 23 May 2023 01:20:25 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:22:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:22:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:22:30 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c722db24a050621ee87ea07acd5d066d3d6a94737c32012f27d73a1ad5cc645c`  
		Last Modified: Tue, 23 May 2023 01:24:26 GMT  
		Size: 50.4 MB (50448716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5580aa8b086cc8c6dc3c839df2b54e92d4785fc4e9b824c0da7819479aa00`  
		Last Modified: Tue, 23 May 2023 04:23:53 GMT  
		Size: 10.5 MB (10504489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fae9d7e648f7f5be8b0df37a4284949621932cbe6f4f3ad8a51c76867b82d1`  
		Last Modified: Tue, 23 May 2023 04:23:52 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09094d5b9484661a6878ceaf9f02e2d901afebadcdb601e0deb31411ce74c26`  
		Last Modified: Tue, 23 May 2023 04:23:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee599431be61d0a5ed744c9cb86ef6b4d02c23e602e36f5a2ac021111dca7ca`  
		Last Modified: Tue, 23 May 2023 04:23:53 GMT  
		Size: 304.5 KB (304451 bytes)  
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
$ docker pull neurodebian@sha256:6f8924222996b6666b244ad59ffa72cd53789c28367bc6c4c5516ac65ec23933
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62380281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cab147f8daa11258c7e63b95ad5170ed4d51e503ff0cbb25c526c509ed920b9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:45 GMT
ADD file:d82a514985e1c8796d6c5572290d84fdff0dc1c748d7d2e469d3066ac0344c5f in / 
# Tue, 23 May 2023 00:39:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:42:25 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:26 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:42:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:42:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a48e9012f51ff679af95460521da76c7184da775e3adaa39fed65c912ce0a57`  
		Last Modified: Tue, 23 May 2023 00:44:49 GMT  
		Size: 51.2 MB (51205678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4226282d9c19402a2492d1ec19244689e7600cc6b9fc41325278c52d8b5b9e0`  
		Last Modified: Tue, 23 May 2023 05:43:56 GMT  
		Size: 10.9 MB (10868296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542327d6541db55160c5e48c276b22429d6e27856e8d86a7d00da85d2b3b8cda`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3e74af901c5e67254d5cdc0ff3c41bef80b4b9cabfd174697af611d6406377`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cf355598094ecd630526aed002e391ba7365154fd960d40bdc635d92a68585`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 304.3 KB (304298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100-non-free`

```console
$ docker pull neurodebian@sha256:132b8fa6f0a9fac5455b659b41bc620720fe7f602757e2800f2092a7aa1f4ae2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:44806c8d2020d66ae467d0812cde42ad45fddb5e0a8ff7b427793a23d6a447b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61260017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7823c1a9101821c016ca63cf774e6a8ccd0cc61aa8d9a1099d7a61f8b7e71f0d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:24 GMT
ADD file:9d769df745075dbc4cd2c01ca784571a0df008f6b650b895a7f92d3281132807 in / 
# Tue, 23 May 2023 01:20:25 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:22:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:22:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:22:30 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:32 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c722db24a050621ee87ea07acd5d066d3d6a94737c32012f27d73a1ad5cc645c`  
		Last Modified: Tue, 23 May 2023 01:24:26 GMT  
		Size: 50.4 MB (50448716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5580aa8b086cc8c6dc3c839df2b54e92d4785fc4e9b824c0da7819479aa00`  
		Last Modified: Tue, 23 May 2023 04:23:53 GMT  
		Size: 10.5 MB (10504489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fae9d7e648f7f5be8b0df37a4284949621932cbe6f4f3ad8a51c76867b82d1`  
		Last Modified: Tue, 23 May 2023 04:23:52 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09094d5b9484661a6878ceaf9f02e2d901afebadcdb601e0deb31411ce74c26`  
		Last Modified: Tue, 23 May 2023 04:23:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee599431be61d0a5ed744c9cb86ef6b4d02c23e602e36f5a2ac021111dca7ca`  
		Last Modified: Tue, 23 May 2023 04:23:53 GMT  
		Size: 304.5 KB (304451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd539f4479d039165c3dd5ad7548b8840bfb1e87810c63a90fd25f2c4cc371`  
		Last Modified: Tue, 23 May 2023 04:24:01 GMT  
		Size: 355.0 B  
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
$ docker pull neurodebian@sha256:d8a746880aac51b323612d7e3af5bd6a1f7a1090a55f7ac5a75776ea460b884d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62380639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f60a1dc4fd3e415746e9d747980bcd556aa03b22d84fa99454e480123069fd97`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:45 GMT
ADD file:d82a514985e1c8796d6c5572290d84fdff0dc1c748d7d2e469d3066ac0344c5f in / 
# Tue, 23 May 2023 00:39:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:42:25 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:26 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:42:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:42:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:35 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:5a48e9012f51ff679af95460521da76c7184da775e3adaa39fed65c912ce0a57`  
		Last Modified: Tue, 23 May 2023 00:44:49 GMT  
		Size: 51.2 MB (51205678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4226282d9c19402a2492d1ec19244689e7600cc6b9fc41325278c52d8b5b9e0`  
		Last Modified: Tue, 23 May 2023 05:43:56 GMT  
		Size: 10.9 MB (10868296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542327d6541db55160c5e48c276b22429d6e27856e8d86a7d00da85d2b3b8cda`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3e74af901c5e67254d5cdc0ff3c41bef80b4b9cabfd174697af611d6406377`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cf355598094ecd630526aed002e391ba7365154fd960d40bdc635d92a68585`  
		Last Modified: Tue, 23 May 2023 05:43:54 GMT  
		Size: 304.3 KB (304298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f216b2323999a15c9f3d04e270325018173befad613dffa8ccba0696305277d1`  
		Last Modified: Tue, 23 May 2023 05:44:04 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110`

```console
$ docker pull neurodebian@sha256:58ede793451b5dcd9b8484cdf7a4d96286b7ca6dd4cd7691b09bcee139a37c03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110` - linux; amd64

```console
$ docker pull neurodebian@sha256:7f15da2016b618ea07c99f0db53a7d4d811f7d3a1e07b3dcfc62aa706a62d14b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d3c77884c39fcf8c8197b0e9da8509b340aac50f30d7d6f7927089ca89bbbc2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:22:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:22:42 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:22:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c8f317bbcc308a1e6f1fac03e1e3a9f2a39fc82e936c0570d59117b539f98b`  
		Last Modified: Tue, 23 May 2023 04:24:10 GMT  
		Size: 11.3 MB (11310985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339b1ccbf456e866652af2b8427b66dc919fc8ff09b50fc20bbadf9864f1299e`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec272ec7995fd0da0e4007df35052366ac83178183bc9be766a7c07054484d`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b179b6be05eca9ee18ca837dfeafb6f09c1357d864b810f767c3b8c7e6150efa`  
		Last Modified: Tue, 23 May 2023 04:24:09 GMT  
		Size: 312.0 KB (311996 bytes)  
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
$ docker pull neurodebian@sha256:e013ecaa24d4606f907599811071f8b27f5c368a4f3b70509ff650713c26f7f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68050980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b877fcd3514ab2d8dc777764b898ba9ff9a8029ad45de0c1312ca006cec9a203`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:14 GMT
ADD file:acdf45f51b991111aa6c929fedd4e8de03e5d42578cca2f895f74697c3c66e33 in / 
# Tue, 23 May 2023 00:39:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:42:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:42:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:42:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c377769761bd9f2bd79d27a4f6dfa29be1047f4e6e8df1653027ef5262e020bb`  
		Last Modified: Tue, 23 May 2023 00:44:01 GMT  
		Size: 56.0 MB (56029173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaae1eed722697680293151e7092e07fa7042893bd549883ec3cc9b401babf0`  
		Last Modified: Tue, 23 May 2023 05:44:13 GMT  
		Size: 11.7 MB (11707960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c029d5297bd9708c2063123e4843df78700aa651c8968e98d0bb366528c3a761`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf405f235e316c73593fa6527a595699f0597ddcd7b09a16cf17b7c645e3b76`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a472eab1c6eb96814a14e198ebc46c183ff9b9b7a4b5244cd7133a8db20481`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 311.8 KB (311833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:c7e4e9212de829ff29050399e6e4223a7a0940a9e224e39068f2aafa3fb0870c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:58b179e8710e5d072a22ab3c4c24817c15d3b73a6a48cb1906158618473afd50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7403edb772c4b84cae3e2436b127af6bff49d8bd52c824a2369855ab5f1e48ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:22:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:22:42 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:22:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:48 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c8f317bbcc308a1e6f1fac03e1e3a9f2a39fc82e936c0570d59117b539f98b`  
		Last Modified: Tue, 23 May 2023 04:24:10 GMT  
		Size: 11.3 MB (11310985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339b1ccbf456e866652af2b8427b66dc919fc8ff09b50fc20bbadf9864f1299e`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec272ec7995fd0da0e4007df35052366ac83178183bc9be766a7c07054484d`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b179b6be05eca9ee18ca837dfeafb6f09c1357d864b810f767c3b8c7e6150efa`  
		Last Modified: Tue, 23 May 2023 04:24:09 GMT  
		Size: 312.0 KB (311996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6846656eb9c3c17db60e2ba659abb84645043fa6fbdaac726e3f617c4afb4c09`  
		Last Modified: Tue, 23 May 2023 04:24:19 GMT  
		Size: 360.0 B  
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
$ docker pull neurodebian@sha256:317b5120cde566e6c15f029bb71d9b2dc8824edd485de316291dd44741f169f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68051343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:156c0f22d08a31852143fea310856afdb1ab248f648e45cf25dcc9b45aec549b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:14 GMT
ADD file:acdf45f51b991111aa6c929fedd4e8de03e5d42578cca2f895f74697c3c66e33 in / 
# Tue, 23 May 2023 00:39:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:42:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:42:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:42:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:56 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c377769761bd9f2bd79d27a4f6dfa29be1047f4e6e8df1653027ef5262e020bb`  
		Last Modified: Tue, 23 May 2023 00:44:01 GMT  
		Size: 56.0 MB (56029173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaae1eed722697680293151e7092e07fa7042893bd549883ec3cc9b401babf0`  
		Last Modified: Tue, 23 May 2023 05:44:13 GMT  
		Size: 11.7 MB (11707960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c029d5297bd9708c2063123e4843df78700aa651c8968e98d0bb366528c3a761`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf405f235e316c73593fa6527a595699f0597ddcd7b09a16cf17b7c645e3b76`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a472eab1c6eb96814a14e198ebc46c183ff9b9b7a4b5244cd7133a8db20481`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 311.8 KB (311833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10c00d49702288a28d1849a812fd1703827069b7342dc19848b5859eb83a678`  
		Last Modified: Tue, 23 May 2023 05:44:22 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120`

```console
$ docker pull neurodebian@sha256:b69b9cebdfd8b83213c9c6932c85b7c7923cee9a49ba2b9a3b702ee8ad38359b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120` - linux; amd64

```console
$ docker pull neurodebian@sha256:baabb08f7f35eece8fe86b5cca134eb909f7605d48b5070fc38ff2584518df2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61307789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f47799e2bf3d6bb22f8204885da1e8a33389ad6326faf0f6abdb17224ff07f3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:19:36 GMT
ADD file:aea4560c39a3a877086fc63afdf218ba3600a05abef7c44563f788e8b60c04ef in / 
# Tue, 23 May 2023 01:19:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:23:01 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:02 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:23:03 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:23:06 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c98dda1b0e97e7fa61fa33cea43f85bb1a36a4f6f65c7b8430cae442b76ece09`  
		Last Modified: Tue, 23 May 2023 01:23:14 GMT  
		Size: 49.3 MB (49301275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33627279e466d7f7d1e2299fc1f1ef0aba016364269114db58eefb5bc4f174fe`  
		Last Modified: Tue, 23 May 2023 04:24:30 GMT  
		Size: 11.7 MB (11719838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc38d23881ba02c585bb2b72b06f955689ebf8e30cce25285d5c6ded4b79550`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179908f928b0af97bceaffff9a265d97bffd58aa45ff6ec4b2b6595b33b7bb3d`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b52941f1978acefe1f1b3a5493124b6927d21693f82780f76726caab179a1b9`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 284.7 KB (284664 bytes)  
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
$ docker pull neurodebian@sha256:8764e75acf0b0d9877c509c66f2decc88573d88ddba2da984c14c771b505d3e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62753602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:525bc620b64464f1c6f7d5fafe4c31be7f124b8a9cd79ce2422d9335855f5138`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:38:43 GMT
ADD file:4d14207b5cf935fa2b9de70132f41a0eb90a8b5200ed3d27e60b766fc6131e13 in / 
# Tue, 23 May 2023 00:38:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:43:10 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:43:12 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:43:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22e40771358829b6817b47cb2d682b51257385478c18bb1ec96251a68a9c75e4`  
		Last Modified: Tue, 23 May 2023 00:43:23 GMT  
		Size: 50.3 MB (50323189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c247d5ed731b6493a71fa628813b52b9d64900d688cef945f8c5b85ed9b2690`  
		Last Modified: Tue, 23 May 2023 05:44:33 GMT  
		Size: 12.1 MB (12143667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4ef75fcb9af10a6ff980ed195a464fff7047d4905d4d99184bd7f27a313cde`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fab7974bae62c89adabeae697146cde0caf8f16c854425dfd1aadafebeb2b12`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d4b90c50e699685d80e5102a8756309b6103a931798615b13c4ed4b16df39`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 284.7 KB (284735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120-non-free`

```console
$ docker pull neurodebian@sha256:b402dbf57d17caed337237f154a5cdd1ad740cda0a99babda118d593197a86be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:9e34ce5c236de895d1aee892e0aadae7d75a19c75fe0d4544fe642c97ce44b28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61308217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf96f115f3a71ad93f74b628601aba8b6460282524cf285a40ae9a784ae7ae48`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:19:36 GMT
ADD file:aea4560c39a3a877086fc63afdf218ba3600a05abef7c44563f788e8b60c04ef in / 
# Tue, 23 May 2023 01:19:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:23:01 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:02 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:23:03 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:23:06 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:10 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c98dda1b0e97e7fa61fa33cea43f85bb1a36a4f6f65c7b8430cae442b76ece09`  
		Last Modified: Tue, 23 May 2023 01:23:14 GMT  
		Size: 49.3 MB (49301275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33627279e466d7f7d1e2299fc1f1ef0aba016364269114db58eefb5bc4f174fe`  
		Last Modified: Tue, 23 May 2023 04:24:30 GMT  
		Size: 11.7 MB (11719838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc38d23881ba02c585bb2b72b06f955689ebf8e30cce25285d5c6ded4b79550`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179908f928b0af97bceaffff9a265d97bffd58aa45ff6ec4b2b6595b33b7bb3d`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b52941f1978acefe1f1b3a5493124b6927d21693f82780f76726caab179a1b9`  
		Last Modified: Tue, 23 May 2023 04:24:29 GMT  
		Size: 284.7 KB (284664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6363d30de594fa89c4fafd1a441b7ea23b4a565e0f0902e4d226e73c22c5edf0`  
		Last Modified: Tue, 23 May 2023 04:24:38 GMT  
		Size: 428.0 B  
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
$ docker pull neurodebian@sha256:25200d6048a13ef9220e62f845de1441b53e5ce2d49f5642b3174eda494a1975
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62754031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fb8a1cffbdfa3a0dc9916920eacf40dfdfa74532919c0059d8b6ad8cb5b20c3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:38:43 GMT
ADD file:4d14207b5cf935fa2b9de70132f41a0eb90a8b5200ed3d27e60b766fc6131e13 in / 
# Tue, 23 May 2023 00:38:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:43:10 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:43:12 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:43:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:21 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:22e40771358829b6817b47cb2d682b51257385478c18bb1ec96251a68a9c75e4`  
		Last Modified: Tue, 23 May 2023 00:43:23 GMT  
		Size: 50.3 MB (50323189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c247d5ed731b6493a71fa628813b52b9d64900d688cef945f8c5b85ed9b2690`  
		Last Modified: Tue, 23 May 2023 05:44:33 GMT  
		Size: 12.1 MB (12143667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4ef75fcb9af10a6ff980ed195a464fff7047d4905d4d99184bd7f27a313cde`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fab7974bae62c89adabeae697146cde0caf8f16c854425dfd1aadafebeb2b12`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d4b90c50e699685d80e5102a8756309b6103a931798615b13c4ed4b16df39`  
		Last Modified: Tue, 23 May 2023 05:44:31 GMT  
		Size: 284.7 KB (284735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e868cd6c65860bf552879c80292c1c5c5d73ee61bc17eaab036c8fc0231f0a5`  
		Last Modified: Tue, 23 May 2023 05:44:41 GMT  
		Size: 429.0 B  
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
$ docker pull neurodebian@sha256:c7e4e9212de829ff29050399e6e4223a7a0940a9e224e39068f2aafa3fb0870c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:58b179e8710e5d072a22ab3c4c24817c15d3b73a6a48cb1906158618473afd50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66674382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7403edb772c4b84cae3e2436b127af6bff49d8bd52c824a2369855ab5f1e48ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:22:40 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:22:42 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:22:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:22:48 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c8f317bbcc308a1e6f1fac03e1e3a9f2a39fc82e936c0570d59117b539f98b`  
		Last Modified: Tue, 23 May 2023 04:24:10 GMT  
		Size: 11.3 MB (11310985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339b1ccbf456e866652af2b8427b66dc919fc8ff09b50fc20bbadf9864f1299e`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec272ec7995fd0da0e4007df35052366ac83178183bc9be766a7c07054484d`  
		Last Modified: Tue, 23 May 2023 04:24:08 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b179b6be05eca9ee18ca837dfeafb6f09c1357d864b810f767c3b8c7e6150efa`  
		Last Modified: Tue, 23 May 2023 04:24:09 GMT  
		Size: 312.0 KB (311996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6846656eb9c3c17db60e2ba659abb84645043fa6fbdaac726e3f617c4afb4c09`  
		Last Modified: Tue, 23 May 2023 04:24:19 GMT  
		Size: 360.0 B  
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
$ docker pull neurodebian@sha256:317b5120cde566e6c15f029bb71d9b2dc8824edd485de316291dd44741f169f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68051343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:156c0f22d08a31852143fea310856afdb1ab248f648e45cf25dcc9b45aec549b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:39:14 GMT
ADD file:acdf45f51b991111aa6c929fedd4e8de03e5d42578cca2f895f74697c3c66e33 in / 
# Tue, 23 May 2023 00:39:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:42:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:42:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:42:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:42:56 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c377769761bd9f2bd79d27a4f6dfa29be1047f4e6e8df1653027ef5262e020bb`  
		Last Modified: Tue, 23 May 2023 00:44:01 GMT  
		Size: 56.0 MB (56029173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaae1eed722697680293151e7092e07fa7042893bd549883ec3cc9b401babf0`  
		Last Modified: Tue, 23 May 2023 05:44:13 GMT  
		Size: 11.7 MB (11707960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c029d5297bd9708c2063123e4843df78700aa651c8968e98d0bb366528c3a761`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf405f235e316c73593fa6527a595699f0597ddcd7b09a16cf17b7c645e3b76`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a472eab1c6eb96814a14e198ebc46c183ff9b9b7a4b5244cd7133a8db20481`  
		Last Modified: Tue, 23 May 2023 05:44:11 GMT  
		Size: 311.8 KB (311833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10c00d49702288a28d1849a812fd1703827069b7342dc19848b5859eb83a678`  
		Last Modified: Tue, 23 May 2023 05:44:22 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:b7eabe01fca7074e04d46dd14d8dc8b6b1cdf141a0c35821b83235e913ea4b88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:d4373ee7bb59ea1b6932dff39a08917c9ecea36de486c81c414c786c4695120b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61299586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac725a56cfb49d044c98bc06afd02334e0c25d27aac6c54eaadc6d18dd114da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:21:12 GMT
ADD file:3b942ada2dbba1c073e568411a383d6ab987c117af5bbb011afd46549d64c4dc in / 
# Tue, 23 May 2023 01:21:12 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:23:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:23:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:23:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8285c3e1284db51d7096ff9c9434e138a00153495c655a040787b10e562b7515`  
		Last Modified: Tue, 23 May 2023 01:25:36 GMT  
		Size: 49.3 MB (49289184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158a1759b167defe3ac364f8157c49f063c470a5a956e0d702fc47b0a929f38`  
		Last Modified: Tue, 23 May 2023 04:24:47 GMT  
		Size: 11.7 MB (11722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f37d696beaa9b72a35a3d14f54f0b856dcc0621888c8afb8cc7ddda831e3310`  
		Last Modified: Tue, 23 May 2023 04:24:45 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e94a7d5efaab58c44a59d954d27135a86f8e445818b065a841ac08f6f00544`  
		Last Modified: Tue, 23 May 2023 04:24:45 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b33126a764321fb1a50ada00da1192641da6f41c03432c227137e50acd8357`  
		Last Modified: Tue, 23 May 2023 04:24:46 GMT  
		Size: 286.3 KB (286314 bytes)  
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
$ docker pull neurodebian@sha256:ca6fb83db48276fe96ae643fd4c1acaf9846431386d9ab11596e85fb2acbb08d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.7 MB (62745155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:435d9c6d98412b4bdf45e80888addecd13eb835ab8cdb7eef2b256c5a8554ee6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:40:47 GMT
ADD file:33dd3eb2725f92170606ce015e99cc9496d244630b3f4844cb8f3f61b16e2eb0 in / 
# Tue, 23 May 2023 00:40:48 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:43:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:43:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:43:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1034171b4bde64cf8e4ff854704a3bf68000eddcceb63b481197082dced785ba`  
		Last Modified: Tue, 23 May 2023 00:46:09 GMT  
		Size: 50.3 MB (50311497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb94666b190ba95be7fadf283441a70d7afa10a0b07170b8674ec2678968d429`  
		Last Modified: Tue, 23 May 2023 05:44:50 GMT  
		Size: 12.1 MB (12145347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf7364560006b36553ea625f2134dc9718506f9939d605cf9bbeffa03222aa8`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e68c126603fa53d236ac3cef352fb8266303d1f60ea86c338b5a104baa5a545`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fef25ab16b5c30aa387e5e2d002d54aff3c430bb03a10607bffcb018bc94d4`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 286.3 KB (286305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:60a78434fdd546c8d2fc025282e6431fa3a5a5ec5dfb00ab19c7bf2c532572c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:c3cd2902ff137d947cf1183caee8e2e881476148001aea0c106652a0982d3310
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61299977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:757103b2b0ac7345e1a0dcb71a788028ccd7ab37e1a27cf53cb423724f8f4ab2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:21:12 GMT
ADD file:3b942ada2dbba1c073e568411a383d6ab987c117af5bbb011afd46549d64c4dc in / 
# Tue, 23 May 2023 01:21:12 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:23:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:21 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 04:23:21 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 04:23:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:23:29 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:8285c3e1284db51d7096ff9c9434e138a00153495c655a040787b10e562b7515`  
		Last Modified: Tue, 23 May 2023 01:25:36 GMT  
		Size: 49.3 MB (49289184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158a1759b167defe3ac364f8157c49f063c470a5a956e0d702fc47b0a929f38`  
		Last Modified: Tue, 23 May 2023 04:24:47 GMT  
		Size: 11.7 MB (11722081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f37d696beaa9b72a35a3d14f54f0b856dcc0621888c8afb8cc7ddda831e3310`  
		Last Modified: Tue, 23 May 2023 04:24:45 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e94a7d5efaab58c44a59d954d27135a86f8e445818b065a841ac08f6f00544`  
		Last Modified: Tue, 23 May 2023 04:24:45 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b33126a764321fb1a50ada00da1192641da6f41c03432c227137e50acd8357`  
		Last Modified: Tue, 23 May 2023 04:24:46 GMT  
		Size: 286.3 KB (286314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c80b51ea09266240fd930629cb4fb877838167da0961769224e46b9843a810`  
		Last Modified: Tue, 23 May 2023 04:24:56 GMT  
		Size: 391.0 B  
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
$ docker pull neurodebian@sha256:6753b469ed406da38695358a52a1c87e179ebe14d42c59b452a6cf03dc178c54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.7 MB (62745547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d6d3c089bd7ecb7dece0a9305fb5900887130cddead11f80b1b13b0fb57b418`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:40:47 GMT
ADD file:33dd3eb2725f92170606ce015e99cc9496d244630b3f4844cb8f3f61b16e2eb0 in / 
# Tue, 23 May 2023 00:40:48 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:43:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 05:43:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 05:43:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:43:42 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:1034171b4bde64cf8e4ff854704a3bf68000eddcceb63b481197082dced785ba`  
		Last Modified: Tue, 23 May 2023 00:46:09 GMT  
		Size: 50.3 MB (50311497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb94666b190ba95be7fadf283441a70d7afa10a0b07170b8674ec2678968d429`  
		Last Modified: Tue, 23 May 2023 05:44:50 GMT  
		Size: 12.1 MB (12145347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf7364560006b36553ea625f2134dc9718506f9939d605cf9bbeffa03222aa8`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e68c126603fa53d236ac3cef352fb8266303d1f60ea86c338b5a104baa5a545`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fef25ab16b5c30aa387e5e2d002d54aff3c430bb03a10607bffcb018bc94d4`  
		Last Modified: Tue, 23 May 2023 05:44:48 GMT  
		Size: 286.3 KB (286305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da399a07548054d441160ab6c71e0f30793cf8071685057f199a0590aba9ad84`  
		Last Modified: Tue, 23 May 2023 05:44:57 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
