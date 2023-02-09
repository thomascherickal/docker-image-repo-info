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
$ docker pull neurodebian@sha256:e513ac1e11156aecac472db495f4a8a9289c483b45d0dc1b4a246b58da08ea53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:bionic` - linux; amd64

```console
$ docker pull neurodebian@sha256:9eaae57e6a418b8c573fc5418ad64fe129309c35c2fd161bbdbf61a529730d9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31775229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:873262071297edd49a7d33afe192f7dd416fbcb8f8329bfc9d17b220889f04e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:58:43 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:58:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:58:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:58:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c561dd565402593670454bc67f0d32877f005872b8d25d4a588ff0bd84d74582`  
		Last Modified: Tue, 31 Jan 2023 19:00:39 GMT  
		Size: 4.8 MB (4821347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3199a21fc88a38a5953a4eda7d548104c2153dbacdbeac0c1f97636aa990429d`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4dc3134d8a8ba0f045aa233e851c13346eb4ea771d8394c56cf2863567c2a8`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c014dbfdfc0e1f416ac41d8cf451e1463598f92d704b7440a38610c18f4ebe26`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 240.4 KB (240380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bionic` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5683ede91c2464e5b6ae9098e6c50ff505d17f1fa2f3e71b42ead7b3feccd26f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28382285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490edb93bb34812d94fffb01906d7d28c3e9fc0bb12c7cd49c911c949fa7ad3c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:08:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:08:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:08:44 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:08:49 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dbc19e87e6da7df7a26b73c38813e606d157ff82cead74668aa9fb1dde50fe`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 4.4 MB (4403764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b13f880e3b2e22e0f79bd577aae93628955db5dfb54dc16b5ee01d78e283612`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1536cf9d0676d119194aaac6a84cfd3883f661525fc07c8c16507232e4b0820`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455d9d3933a870d2b232e0931a36cc44e9dc946dd9f6dcdb07cc55b77f21a170`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 241.1 KB (241081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bionic-non-free`

```console
$ docker pull neurodebian@sha256:691ca2cf102d15603a0c797e930a351ed9c873489a8ee27f1e76b43eadc33e50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:bionic-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:7c10782a79f7c72117a5374ce52548ca719f89305356417c7957eef4ce83a492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31775483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6c7baace0050bff9e555573db23e79cca0226c59505907eb177d7fd551e1e6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:58:43 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:58:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:58:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:58:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:58:58 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c561dd565402593670454bc67f0d32877f005872b8d25d4a588ff0bd84d74582`  
		Last Modified: Tue, 31 Jan 2023 19:00:39 GMT  
		Size: 4.8 MB (4821347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3199a21fc88a38a5953a4eda7d548104c2153dbacdbeac0c1f97636aa990429d`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4dc3134d8a8ba0f045aa233e851c13346eb4ea771d8394c56cf2863567c2a8`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c014dbfdfc0e1f416ac41d8cf451e1463598f92d704b7440a38610c18f4ebe26`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 240.4 KB (240380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb917c28cea7ae4fa4a9d361cbbd4494ecd182af107d7ee5936bcb018641040`  
		Last Modified: Tue, 31 Jan 2023 19:00:46 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bionic-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:0106f5e71d6be760cf4fa278aa89bf7ab086e4711f5751e8c9e46031e939ba69
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28382540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15489cd4bee72086827d309d7fa524ab5f75084ac3a273f752ba9de140d3d70f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:08:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:08:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:08:44 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:08:49 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:08:53 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dbc19e87e6da7df7a26b73c38813e606d157ff82cead74668aa9fb1dde50fe`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 4.4 MB (4403764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b13f880e3b2e22e0f79bd577aae93628955db5dfb54dc16b5ee01d78e283612`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1536cf9d0676d119194aaac6a84cfd3883f661525fc07c8c16507232e4b0820`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455d9d3933a870d2b232e0931a36cc44e9dc946dd9f6dcdb07cc55b77f21a170`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 241.1 KB (241081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3633341f6970cb9798062d7a3e8b9c338cf172ef3b05cdc69e65ba08a562aee`  
		Last Modified: Tue, 31 Jan 2023 18:10:39 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm`

```console
$ docker pull neurodebian@sha256:4bf980a902cb6e7571e8beaf42bbfbbe7b1bc4dc071491be355a63c9f66ae4b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm` - linux; amd64

```console
$ docker pull neurodebian@sha256:eb5a0a012ff4ce61cf3be35916cf6c57d17003f0d54cc1e73dce0f470ec5bbca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60987077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b561be2d8127b316aaf04f6bb16054759c690801338e869278a1edc135effea`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:19:36 GMT
ADD file:99a61197d7273704581c44eae01f3342e9f3562e84fe66cc2d56ce563e58450a in / 
# Thu, 09 Feb 2023 03:19:37 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:25 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:45c04dd46fbf614b423b54561d34c6339a0376d1717729ef6dcf101dbfd20f8c`  
		Last Modified: Thu, 09 Feb 2023 03:24:14 GMT  
		Size: 49.1 MB (49054961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38236192934019393b60f6a155f92e7625f86d7040a25abc85f16331e3f20a9`  
		Last Modified: Thu, 09 Feb 2023 10:35:12 GMT  
		Size: 11.6 MB (11649251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ce3c24436d316066f2f512361cceecec6597a642758cd8a30a7e6be8045177`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389c3b6867a3b8b7a0990aed29d11f0ca7d3451728e8394e1ffd435a9860c08c`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3878ef31203d1f458f083c3adf2cefb760dd8bbc98002c0732519fe24393de`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 280.9 KB (280853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:47d7a6535244ad6e95e521fd44c18618793ed1aa080c1eead00b9dcd26032188
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60978100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d0990886517f471603003c7bff9a8442a9624b45903ac2c0307fba5b87c4eaf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:08 GMT
ADD file:b40ad920bd7dd081e20adf36435db50381b9998a1de3d2eac6b2c45734ce60b3 in / 
# Sat, 04 Feb 2023 06:17:09 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:49:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:49:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a43b5d5927a7651097e784be4430a6ade09951f5b6879cd06b0f51fc7c4812af`  
		Last Modified: Sat, 04 Feb 2023 06:20:30 GMT  
		Size: 49.1 MB (49081538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2178538c5bc5dcf98be54976e26e3643caa3a37f742386a75aeeda9818488236`  
		Last Modified: Sat, 04 Feb 2023 08:50:55 GMT  
		Size: 11.6 MB (11613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5946ba90fc15d686558f937d9db8c112910bfcc60659eae41906cab00536fbd1`  
		Last Modified: Sat, 04 Feb 2023 08:50:54 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d06715673a85e222fe91b40adfd40e6cf12abad4d8fc6b94aa1a329f289b576`  
		Last Modified: Sat, 04 Feb 2023 08:50:53 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302b2fd07b19b38ae39db22c7c35d3f8f01c22b33486483bc0f26dd2f8d1e600`  
		Last Modified: Sat, 04 Feb 2023 08:50:54 GMT  
		Size: 281.2 KB (281229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; 386

```console
$ docker pull neurodebian@sha256:e37e3580493d2c03ad895fdd2504cc02a33c83c13b2a60bc1aa72e40ced14664
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62065634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7678b3f84b1c990678feca32d4533daea648cfe711fcc0e5fc012e584c6f8689`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:11 GMT
ADD file:37cc85485a8f79a4bd5557a42685805da0b367ff061d53fdf29d5f242593ea1d in / 
# Thu, 09 Feb 2023 05:12:12 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:52 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0153a17486e7cd96c30b54f1d68ab1cffaca99de43335324f16477807b1ddb1c`  
		Last Modified: Thu, 09 Feb 2023 05:17:35 GMT  
		Size: 50.1 MB (50089500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187a90aef6870d09282470d3b592e152d72bc909d4c41fc4d2a0dc6e35d578b`  
		Last Modified: Thu, 09 Feb 2023 12:46:01 GMT  
		Size: 11.9 MB (11882490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4ad0b3bec733e0fea46c5f1aa52aba6533737fae1c7ed922601bea2dbc7dbd`  
		Last Modified: Thu, 09 Feb 2023 12:45:58 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52056b4dd31d6fd76427109e57655ab7cdb36d3cdf6287f75d9ba2f4c8dcd0f`  
		Last Modified: Thu, 09 Feb 2023 12:45:59 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8502cd76b08bed33327032c663ce30112feb1286d449672cffdf1346457ab1`  
		Last Modified: Thu, 09 Feb 2023 12:45:59 GMT  
		Size: 91.7 KB (91655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bookworm-non-free`

```console
$ docker pull neurodebian@sha256:697d553cc84b55677c1e0d69e4d0acbe64c2e0a677d1fbc0a5ceeb38a1f55c10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:c248a7d665bda19d273222a908fa5850c1f1380317d8bc4916ae925e356167d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60987511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38d056149a345cb8309ad04642bf342a4b3f0c1daab681ef1b62aadf6c4c6806`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:19:36 GMT
ADD file:99a61197d7273704581c44eae01f3342e9f3562e84fe66cc2d56ce563e58450a in / 
# Thu, 09 Feb 2023 03:19:37 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:25 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:34 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:45c04dd46fbf614b423b54561d34c6339a0376d1717729ef6dcf101dbfd20f8c`  
		Last Modified: Thu, 09 Feb 2023 03:24:14 GMT  
		Size: 49.1 MB (49054961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38236192934019393b60f6a155f92e7625f86d7040a25abc85f16331e3f20a9`  
		Last Modified: Thu, 09 Feb 2023 10:35:12 GMT  
		Size: 11.6 MB (11649251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ce3c24436d316066f2f512361cceecec6597a642758cd8a30a7e6be8045177`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389c3b6867a3b8b7a0990aed29d11f0ca7d3451728e8394e1ffd435a9860c08c`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3878ef31203d1f458f083c3adf2cefb760dd8bbc98002c0732519fe24393de`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 280.9 KB (280853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec51a2c8898f4455cebcb45cced98d389e9c9f0dfd468a9540f6529c412742a8`  
		Last Modified: Thu, 09 Feb 2023 10:35:20 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:9d38cc525233e026ed1dc6ab33d626e38579465070da1b007a4377ad7e892c38
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60978528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f457705f06d5d27f6710a5d2077f18bec766f68fff56c944f7ad6428fca9b65`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:08 GMT
ADD file:b40ad920bd7dd081e20adf36435db50381b9998a1de3d2eac6b2c45734ce60b3 in / 
# Sat, 04 Feb 2023 06:17:09 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:49:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:49:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:21 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a43b5d5927a7651097e784be4430a6ade09951f5b6879cd06b0f51fc7c4812af`  
		Last Modified: Sat, 04 Feb 2023 06:20:30 GMT  
		Size: 49.1 MB (49081538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2178538c5bc5dcf98be54976e26e3643caa3a37f742386a75aeeda9818488236`  
		Last Modified: Sat, 04 Feb 2023 08:50:55 GMT  
		Size: 11.6 MB (11613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5946ba90fc15d686558f937d9db8c112910bfcc60659eae41906cab00536fbd1`  
		Last Modified: Sat, 04 Feb 2023 08:50:54 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d06715673a85e222fe91b40adfd40e6cf12abad4d8fc6b94aa1a329f289b576`  
		Last Modified: Sat, 04 Feb 2023 08:50:53 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302b2fd07b19b38ae39db22c7c35d3f8f01c22b33486483bc0f26dd2f8d1e600`  
		Last Modified: Sat, 04 Feb 2023 08:50:54 GMT  
		Size: 281.2 KB (281229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e70a3c681969a418f4e81170b181a23350b8e71edecd45c416d7c429c37a5`  
		Last Modified: Sat, 04 Feb 2023 08:51:02 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:e493c2750ddd7876325a9c6ea61e4151508765499ed3754db677899a97357fa4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62066068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5dcb21fdd302fa0b7ef1f3c0c90c46056a0b4f1f86854e59113ff43965f7a7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:11 GMT
ADD file:37cc85485a8f79a4bd5557a42685805da0b367ff061d53fdf29d5f242593ea1d in / 
# Thu, 09 Feb 2023 05:12:12 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:52 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:44:06 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:0153a17486e7cd96c30b54f1d68ab1cffaca99de43335324f16477807b1ddb1c`  
		Last Modified: Thu, 09 Feb 2023 05:17:35 GMT  
		Size: 50.1 MB (50089500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187a90aef6870d09282470d3b592e152d72bc909d4c41fc4d2a0dc6e35d578b`  
		Last Modified: Thu, 09 Feb 2023 12:46:01 GMT  
		Size: 11.9 MB (11882490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4ad0b3bec733e0fea46c5f1aa52aba6533737fae1c7ed922601bea2dbc7dbd`  
		Last Modified: Thu, 09 Feb 2023 12:45:58 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52056b4dd31d6fd76427109e57655ab7cdb36d3cdf6287f75d9ba2f4c8dcd0f`  
		Last Modified: Thu, 09 Feb 2023 12:45:59 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8502cd76b08bed33327032c663ce30112feb1286d449672cffdf1346457ab1`  
		Last Modified: Thu, 09 Feb 2023 12:45:59 GMT  
		Size: 91.7 KB (91655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ec70962ca1ca64d913ade6eec99635035751b50e604d663e868b999958779a`  
		Last Modified: Thu, 09 Feb 2023 12:46:09 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:632446b0900714f1210ae1c5d9c7cef7ccd9afbe294a7554667fdcce66722d32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:ccd1b59aad87a7c82820e157082bac2be35db3aaeb5a21b86b72ccf0d17bc03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66671505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de330a89bf9b3656ed0d4909c39ff822d84609fe0be661455e5ef82eef9375b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6748fef26b12a93a8ea2e78ebc615a49a0a17ea28b338a2543564de8dbe7a6`  
		Last Modified: Thu, 09 Feb 2023 10:34:52 GMT  
		Size: 11.3 MB (11310827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f8febb6240b1c0efe213c5ec66b0a670a65bacc58a728ee49d9595476b44d`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab659e925660d862b7b1085bba84ab6e23e3cf0a732dd7c751b691c5450539`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b37097c0f732899899760f1a0ecf4d28df4e71f373ec4afb9bf706badbba17`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 311.9 KB (311894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:05cb95459d66a096424e07c1ed40a5be080386293e1f332d98587b154f495795
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65308759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b1dfad29a96eb0452204b34a699e432f876d5238fc40e3091e78c5e88867c1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:48:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:48:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:48:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386b993c0071d2bcf4a8f2250bfbd4fd50bcabb2d47b8fe81cff3ba3c954ad1b`  
		Last Modified: Sat, 04 Feb 2023 08:50:34 GMT  
		Size: 11.3 MB (11313033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5a3d24e8e01f6ab066d7fad4947aa0a7e70547302d3f7882dd82dda9907d2`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cb9fd8e38b57d30b04e23a8206ec76f508811e129bc4ffda4c8a0febef933`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73f1f5a7996bcea0a9b6a82d9b7384a62a8068b963ff9d707f0152657540088`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 311.8 KB (311789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye` - linux; 386

```console
$ docker pull neurodebian@sha256:ce1fbd72b2cdd70b4db22df3ec6da4ef9fbd3e19547c5d0af564a7d774eff1bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67637598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fc5eeb71cd5570608df1aec87502a7e2016fbe882237e0f216f1b8d1bcc14a3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:37 GMT
ADD file:feaff299d3310c04952143a422f0d0bdd292cd174513c54b1f50765cdbcfd401 in / 
# Thu, 09 Feb 2023 05:12:38 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9708eacca143ba8fa6c7e9a5b05456412b7b16629c20015a43f3ca391e066162`  
		Last Modified: Thu, 09 Feb 2023 05:18:13 GMT  
		Size: 56.0 MB (56030197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6553645eeab9f9390c2c8b8a61e7694834123049b6f060dbdbb11ef6b6819`  
		Last Modified: Thu, 09 Feb 2023 12:45:34 GMT  
		Size: 11.5 MB (11500078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e1e93c20ee20a385a9d97ed62c22e11afd73974b6821310c2baca0eb530970`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a06c277f46a387d7ed96bf2575c4552a533f0d45c754c0680a1d8363ffebde3`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d84f478365f04d8d680da68bd0b3ea6cc10a025630c140d289b3a0a6c8705`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 105.3 KB (105331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:bullseye-non-free`

```console
$ docker pull neurodebian@sha256:1862361da08d56105240d74ff35c75f58f9771d4a4eefb851f2bf37e3c538bdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:23260d0661d4e6523c3cf7910d025881a843462564e5fca0902506bcfc56d173
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66671865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0693ecdb52c35a1cf9714de341352d57dd8e00be2677c28cb59bbe30b1cb178`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:14 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6748fef26b12a93a8ea2e78ebc615a49a0a17ea28b338a2543564de8dbe7a6`  
		Last Modified: Thu, 09 Feb 2023 10:34:52 GMT  
		Size: 11.3 MB (11310827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f8febb6240b1c0efe213c5ec66b0a670a65bacc58a728ee49d9595476b44d`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab659e925660d862b7b1085bba84ab6e23e3cf0a732dd7c751b691c5450539`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b37097c0f732899899760f1a0ecf4d28df4e71f373ec4afb9bf706badbba17`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 311.9 KB (311894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be23a69f483739cf32a2e634572f1d3d062f6832c58c445c75f6a37363ca931c`  
		Last Modified: Thu, 09 Feb 2023 10:35:01 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:30cf133c2939a3e22c8c9c47f8a7e66b7e2ff19edf863a0431e3912e80c6d7d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65309119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28a13b8f85eea85993fd122f87cf1d2e938e7897346d1e1ad5a275adf7ef906d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:48:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:48:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:48:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:02 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386b993c0071d2bcf4a8f2250bfbd4fd50bcabb2d47b8fe81cff3ba3c954ad1b`  
		Last Modified: Sat, 04 Feb 2023 08:50:34 GMT  
		Size: 11.3 MB (11313033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5a3d24e8e01f6ab066d7fad4947aa0a7e70547302d3f7882dd82dda9907d2`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cb9fd8e38b57d30b04e23a8206ec76f508811e129bc4ffda4c8a0febef933`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73f1f5a7996bcea0a9b6a82d9b7384a62a8068b963ff9d707f0152657540088`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 311.8 KB (311789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f08233a2e298109671c3c73b17ab2cadfcf1339e4cdf03e2f98d3c5f0bb5c7`  
		Last Modified: Sat, 04 Feb 2023 08:50:44 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:82ac3daeabbbb43956bcc98ff892f14cd4e2eda9ab0677ffeda6875a104c03ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67637958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d0ff2f87b876e0b73be59b8afc1428e66a7ae42299c9f6896df1456db5bde4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:37 GMT
ADD file:feaff299d3310c04952143a422f0d0bdd292cd174513c54b1f50765cdbcfd401 in / 
# Thu, 09 Feb 2023 05:12:38 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:39 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:9708eacca143ba8fa6c7e9a5b05456412b7b16629c20015a43f3ca391e066162`  
		Last Modified: Thu, 09 Feb 2023 05:18:13 GMT  
		Size: 56.0 MB (56030197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6553645eeab9f9390c2c8b8a61e7694834123049b6f060dbdbb11ef6b6819`  
		Last Modified: Thu, 09 Feb 2023 12:45:34 GMT  
		Size: 11.5 MB (11500078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e1e93c20ee20a385a9d97ed62c22e11afd73974b6821310c2baca0eb530970`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a06c277f46a387d7ed96bf2575c4552a533f0d45c754c0680a1d8363ffebde3`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d84f478365f04d8d680da68bd0b3ea6cc10a025630c140d289b3a0a6c8705`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 105.3 KB (105331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5028dc054643bc57886786396802ac777b7d450c096930465a29c82c7004c12`  
		Last Modified: Thu, 09 Feb 2023 12:45:47 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:f6b65d4e5cbb5ea2efbd69cfe242233fb84e97ce8bc01604cc9cc57a0cd8da76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:8b7259439072b854b4b58ea410365639a35eab18c05cfb7c36fd003a9de08d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61260489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53c849b1ee4a2850d6051b704b9af212d309d9e27d8730ec6179dc41e0c7c186`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:33 GMT
ADD file:dc52371b5f4608e5887e8c657ff951d1895e0047960f44b153c4a55ebf1726d5 in / 
# Thu, 09 Feb 2023 03:20:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:32:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:32:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:32:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:32:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2404786f3febb4866f85b0c8f52b0b0b94dfdb6543e94cd65f961c68f325ff7`  
		Last Modified: Thu, 09 Feb 2023 03:25:32 GMT  
		Size: 50.4 MB (50449613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77502ab3ca1cfa948d065d90f0572b331e529eec6f234419b6ba0dd44c7e0135`  
		Last Modified: Thu, 09 Feb 2023 10:34:35 GMT  
		Size: 10.5 MB (10504538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec51aec442293416c6492307baf3e69b92abc070af15fe2f827239fb84259923`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59955829e458d6ce57c1941668246f2fcce15209bf143652918255813981e54`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258ee389ec682ceb8b472c2883f47efb2fa9bd667332c5120470649b3a98980`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 304.3 KB (304328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:dc36f118472fb5e0b20c26b75d1bfbcf49480dfc7776c2e37ace4b31486be06d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60056041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f705abad5e5e4d726795ac15eae33baf5a4e1a515ff1054f4a3774e3fccc03fa`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:45 GMT
ADD file:0241487c3fb43506be1511724644c00339c32361e6b4c21a224d7190e4e1063b in / 
# Sat, 04 Feb 2023 06:17:46 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:48:38 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:48:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:48:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e0a5a2afd38370f358c0a7154362a8d17faf709c206b40b1553a077f810c3b3`  
		Last Modified: Sat, 04 Feb 2023 06:21:43 GMT  
		Size: 49.2 MB (49239373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda0b3f7673107c2204b83097e20a33728ef30d2e731e41727e0915eb8eb7c9`  
		Last Modified: Sat, 04 Feb 2023 08:50:17 GMT  
		Size: 10.5 MB (10510366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e7e8e9562ff77a3d9a1bc9b20bcaaffb5ab25e375ce28460ba3a4018788fb`  
		Last Modified: Sat, 04 Feb 2023 08:50:16 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c8ab4aac39ddf7a0f79a2cc135d4c299bb4a80b3282626e03ba7581e2ec733`  
		Last Modified: Sat, 04 Feb 2023 08:50:16 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fc1d1a5e62555249343f0f0e4c5483c04f9b57bd28318895d6a9f14050a7e6`  
		Last Modified: Sat, 04 Feb 2023 08:50:17 GMT  
		Size: 304.3 KB (304289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; 386

```console
$ docker pull neurodebian@sha256:416d3841ac6fc65e1d4e6c0c233c294cd2fef7f92695816da69b8eca9aa1be67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61990997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b12846deb7051a30b876d4ac76a2e38df8ef0e61f7b3c86c6f343721492b7841`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:13:04 GMT
ADD file:043d1820efa588dcc60e5d9c340fd1edcd43f2988435e6284844a71d4b082dc7 in / 
# Thu, 09 Feb 2023 05:13:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:01 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:03 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:04 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ee55492a1c0f9dc3f2620641096fc2d501a92c463492dd5598f15a6634c4d8bd`  
		Last Modified: Thu, 09 Feb 2023 05:19:04 GMT  
		Size: 51.2 MB (51207786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641c4ab61efe8b684f2f70e427f740060629acab64b255865a739b677e0947ac`  
		Last Modified: Thu, 09 Feb 2023 12:45:15 GMT  
		Size: 10.7 MB (10672461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfbc65dea7c5bef81239621c61d98f3956bcf57cd5fba5d2a09920e4aed1fb2`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3ea514e731298f7c296c9efa36329cb9a29422b0290649fdaab7c8c1aca590`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252f61add039c1f47969b061f788e132a2d94ab712013ed772c1480332874361`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 108.8 KB (108760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:b6b724d93933cad4e4425f4c2488273844cc47ed104e09e4ff4800386dad5aaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:a1bdd9b45aad906eea47ee012772269bf5422c4c625d82ea9fe347f429ffba84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61260846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dfe97d2fd7b4c7dc4431ea670b0b06a22c7bd5935941b40ab11a52b5276fa4e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:33 GMT
ADD file:dc52371b5f4608e5887e8c657ff951d1895e0047960f44b153c4a55ebf1726d5 in / 
# Thu, 09 Feb 2023 03:20:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:32:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:32:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:32:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:32:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:32:55 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b2404786f3febb4866f85b0c8f52b0b0b94dfdb6543e94cd65f961c68f325ff7`  
		Last Modified: Thu, 09 Feb 2023 03:25:32 GMT  
		Size: 50.4 MB (50449613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77502ab3ca1cfa948d065d90f0572b331e529eec6f234419b6ba0dd44c7e0135`  
		Last Modified: Thu, 09 Feb 2023 10:34:35 GMT  
		Size: 10.5 MB (10504538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec51aec442293416c6492307baf3e69b92abc070af15fe2f827239fb84259923`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59955829e458d6ce57c1941668246f2fcce15209bf143652918255813981e54`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258ee389ec682ceb8b472c2883f47efb2fa9bd667332c5120470649b3a98980`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 304.3 KB (304328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf843247789a5bd789d96ea0d938767321149236fc262ca618a3848b2966ef7e`  
		Last Modified: Thu, 09 Feb 2023 10:34:42 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:9dbc4060d63354fc168ef4b4ce8d6572031d397dbd61b0240a71078697e7bc8d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60056397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e52ff1f01210e669f87eece484b274a1c9ed6dfe5aff7b6a0451113022b17b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:45 GMT
ADD file:0241487c3fb43506be1511724644c00339c32361e6b4c21a224d7190e4e1063b in / 
# Sat, 04 Feb 2023 06:17:46 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:48:38 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:48:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:48:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:46 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:8e0a5a2afd38370f358c0a7154362a8d17faf709c206b40b1553a077f810c3b3`  
		Last Modified: Sat, 04 Feb 2023 06:21:43 GMT  
		Size: 49.2 MB (49239373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda0b3f7673107c2204b83097e20a33728ef30d2e731e41727e0915eb8eb7c9`  
		Last Modified: Sat, 04 Feb 2023 08:50:17 GMT  
		Size: 10.5 MB (10510366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e7e8e9562ff77a3d9a1bc9b20bcaaffb5ab25e375ce28460ba3a4018788fb`  
		Last Modified: Sat, 04 Feb 2023 08:50:16 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c8ab4aac39ddf7a0f79a2cc135d4c299bb4a80b3282626e03ba7581e2ec733`  
		Last Modified: Sat, 04 Feb 2023 08:50:16 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fc1d1a5e62555249343f0f0e4c5483c04f9b57bd28318895d6a9f14050a7e6`  
		Last Modified: Sat, 04 Feb 2023 08:50:17 GMT  
		Size: 304.3 KB (304289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb106862c94d1d9cf42027a0b8de792e548f97d4bf206491e472fc6159c7e0e`  
		Last Modified: Sat, 04 Feb 2023 08:50:25 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:67c64ff956cb57efa4dfebe6c4c7150991d6f4fc47191cb124f5573bc5f4d027
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61991356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc45ca5c74ad14e514a7a4b704774bc433d2f3486af07bcc806487d21047ba72`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:13:04 GMT
ADD file:043d1820efa588dcc60e5d9c340fd1edcd43f2988435e6284844a71d4b082dc7 in / 
# Thu, 09 Feb 2023 05:13:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:01 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:03 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:04 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:14 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ee55492a1c0f9dc3f2620641096fc2d501a92c463492dd5598f15a6634c4d8bd`  
		Last Modified: Thu, 09 Feb 2023 05:19:04 GMT  
		Size: 51.2 MB (51207786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641c4ab61efe8b684f2f70e427f740060629acab64b255865a739b677e0947ac`  
		Last Modified: Thu, 09 Feb 2023 12:45:15 GMT  
		Size: 10.7 MB (10672461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfbc65dea7c5bef81239621c61d98f3956bcf57cd5fba5d2a09920e4aed1fb2`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3ea514e731298f7c296c9efa36329cb9a29422b0290649fdaab7c8c1aca590`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252f61add039c1f47969b061f788e132a2d94ab712013ed772c1480332874361`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 108.8 KB (108760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa7209b6e78fe409e7508dd28ec663fb4b5351bac0ef5ed20fd61ae220f65a`  
		Last Modified: Thu, 09 Feb 2023 12:45:24 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal`

```console
$ docker pull neurodebian@sha256:fc0e3f6a31571b6faef75452e7b452d8bd6b64ec637462b7dc067544e4285a3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:focal` - linux; amd64

```console
$ docker pull neurodebian@sha256:85b798bdb26eb6b1340fbc60fc0feec533e7dd20029f088b82cb4839a401cac5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34313257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fbceb465a22ad0be1c177c9fe16c5812526ba3dac6c3065f5eefbdd9efacfc1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:32:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:32:16 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 01 Feb 2023 19:32:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 01 Feb 2023 19:32:22 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340633481010cfb4323a6980ddc3fbb99c2b231c2bae539ce3adbe4323848f34`  
		Last Modified: Wed, 01 Feb 2023 19:33:24 GMT  
		Size: 5.5 MB (5494456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6a75d823acce0fa96f4fa88a59f0531577b8f2838bfe342fd493d768cbfcd`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1424e1c74c34cfbb9d0566bfa17947ded4bdff35d712e953ebe4b9a83f3483`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b985a598f6b1f9e18c76e8ff8ec2a3031cee1c84d02604bcde89fe5b75df28e4`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 238.9 KB (238907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:focal` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5f43cd8b79163c0d9d100aaf36b45be3a012257ff691d14de42300c681ff6862
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32909337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fde545e728f21aeef32f65cf9201e112821ed623b0cd56fa89b9b5024752244`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:48:36 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:48:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 01 Feb 2023 18:48:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 01 Feb 2023 18:48:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c5c02fa6b59ab2149fa6bd73b93cc90d70885b4c89395e276408e863c13469`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 5.5 MB (5474533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558f1a74caa43afa1ef7b67ba9f69563ea68ccc494931e60f17601e0d197766f`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc55772b4b9049168de57f770b06cdc6b133aad697a9d81fd887d0845d6b2e4`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64d2353b0251a8e328c31de617a38bc62b5f305270c4e614d42af92b1e1cc2b`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 239.1 KB (239055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:focal-non-free`

```console
$ docker pull neurodebian@sha256:d60d4892922515af262d9b747b2b0c64622190e73ac678135285993f68ac0b85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:focal-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:168dd889aecd1f1d598a9b69160fa460d720c310f55b50eb7f132e76a28326b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34313515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a7515b917b364356f96522dc926c5c828a4bf0df70fcf3945bd0f22f7fb7ba0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:32:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:32:16 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 01 Feb 2023 19:32:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 01 Feb 2023 19:32:22 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:32:26 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340633481010cfb4323a6980ddc3fbb99c2b231c2bae539ce3adbe4323848f34`  
		Last Modified: Wed, 01 Feb 2023 19:33:24 GMT  
		Size: 5.5 MB (5494456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6a75d823acce0fa96f4fa88a59f0531577b8f2838bfe342fd493d768cbfcd`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1424e1c74c34cfbb9d0566bfa17947ded4bdff35d712e953ebe4b9a83f3483`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b985a598f6b1f9e18c76e8ff8ec2a3031cee1c84d02604bcde89fe5b75df28e4`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 238.9 KB (238907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dbb4dc6c7f0965eb4d15b6c9b5762a70d0caf0e9fca5b9eb8c5dbe3211b746`  
		Last Modified: Wed, 01 Feb 2023 19:33:31 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:focal-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:757707483fe2ff4d1589194906a99b162fc40a8b19fe18f56b7e989510aae4c1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32909592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e032ef358f0f25a08aba8f3214453113a399a57680920f1d06b130156139f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:48:36 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:48:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 01 Feb 2023 18:48:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 01 Feb 2023 18:48:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:48:44 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c5c02fa6b59ab2149fa6bd73b93cc90d70885b4c89395e276408e863c13469`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 5.5 MB (5474533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558f1a74caa43afa1ef7b67ba9f69563ea68ccc494931e60f17601e0d197766f`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc55772b4b9049168de57f770b06cdc6b133aad697a9d81fd887d0845d6b2e4`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64d2353b0251a8e328c31de617a38bc62b5f305270c4e614d42af92b1e1cc2b`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 239.1 KB (239055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3479d262aebc44602af32ef7336be8974c16ae723c6ab77fba1e7f9149483d`  
		Last Modified: Wed, 01 Feb 2023 18:49:53 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:jammy`

```console
$ docker pull neurodebian@sha256:91558095dc8910356f23d8076b9e5bf353defc04223d3ee7a18400505ca71261
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:jammy` - linux; amd64

```console
$ docker pull neurodebian@sha256:cada10ba69f57f775b9a16faf888565f07d1b296414c488e3fca9431c22eb82e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34455516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b792d6fc44f8bc39ec8ca5d656529a5b8e1492d6cf4d082b0cd49d8488881de`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:59:37 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:59:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:59:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:59:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400062d61da6ac9d18eda99b4de78dbf1a9cea47ada42fb59417bd7d3940966f`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 3.8 MB (3766134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50dda20f552df25b1a3c041dc92181af9b5119500b13a52cde52648c6017d94c`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3f682ee0399a91bfe1c17e2e5ab2568e45560917037011fec50f7d71e38f73`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cac7bfc4ecfa33e13fd29c32d5dcca6e240446d22389f2b5f5acfa67a23ebd`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 258.4 KB (258366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:jammy` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:4da522322b179b93738a554ff42291674f410633468302dd3d7bd78301252a47
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32386337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f27e0b58fd465ae00b00a9699e5f6d77c96a7ad58c71aaba7095dc9079d9128a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:09:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:09:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:09:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:09:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c38043ccc25501401b9d77af23fd531bac15eb599f37aa73c2942390f0f89`  
		Last Modified: Tue, 31 Jan 2023 18:11:05 GMT  
		Size: 3.7 MB (3739627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80411de25d3f2eee928df25a78042197af878bcef13d3d216f05d002d204251a`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0062cb70e52c57d65210d9b388e6d54a802a2fe89c07a377d86c4ef4502ff590`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b27a9557ed3f80818b8a9ec76450e885b5ffe64974f8eb88642d67dd3319fff`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 259.7 KB (259722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:jammy-non-free`

```console
$ docker pull neurodebian@sha256:ccb27ac7137a1b4182dd842114c37428a600b752e0a730e9c549e04c9532a2d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:jammy-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:db0328bfc73471afc6ea3959e9064784e0dd65fb33221f8f8521acec39130003
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34455776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b38aceba7f88d45ed89bf01fcb40220c82e24b6d334c9b0b89d08767fd5b80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:59:37 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:59:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:59:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:59:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:59:47 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400062d61da6ac9d18eda99b4de78dbf1a9cea47ada42fb59417bd7d3940966f`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 3.8 MB (3766134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50dda20f552df25b1a3c041dc92181af9b5119500b13a52cde52648c6017d94c`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3f682ee0399a91bfe1c17e2e5ab2568e45560917037011fec50f7d71e38f73`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cac7bfc4ecfa33e13fd29c32d5dcca6e240446d22389f2b5f5acfa67a23ebd`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 258.4 KB (258366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f11ca7c2dee167ced8c8ec1ceff5bc630ac061bdd9f59ed00071722ab7e4070`  
		Last Modified: Tue, 31 Jan 2023 19:01:18 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:jammy-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5b770230161b71f7a2138e112d463c38b90dffd6594d2f302b7a18d1b4ec02ae
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32386596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f059c6b605395fae939c68fffd06ebbdf64ae2b55e1622515c21d759152063`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:09:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:09:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:09:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:09:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:09:33 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c38043ccc25501401b9d77af23fd531bac15eb599f37aa73c2942390f0f89`  
		Last Modified: Tue, 31 Jan 2023 18:11:05 GMT  
		Size: 3.7 MB (3739627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80411de25d3f2eee928df25a78042197af878bcef13d3d216f05d002d204251a`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0062cb70e52c57d65210d9b388e6d54a802a2fe89c07a377d86c4ef4502ff590`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b27a9557ed3f80818b8a9ec76450e885b5ffe64974f8eb88642d67dd3319fff`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 259.7 KB (259722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d03b38e66b4a534e50a16c431fd0aef94dc19cf45e0e60da70a12541a9870f1`  
		Last Modified: Tue, 31 Jan 2023 18:11:12 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:632446b0900714f1210ae1c5d9c7cef7ccd9afbe294a7554667fdcce66722d32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:ccd1b59aad87a7c82820e157082bac2be35db3aaeb5a21b86b72ccf0d17bc03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66671505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de330a89bf9b3656ed0d4909c39ff822d84609fe0be661455e5ef82eef9375b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6748fef26b12a93a8ea2e78ebc615a49a0a17ea28b338a2543564de8dbe7a6`  
		Last Modified: Thu, 09 Feb 2023 10:34:52 GMT  
		Size: 11.3 MB (11310827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f8febb6240b1c0efe213c5ec66b0a670a65bacc58a728ee49d9595476b44d`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab659e925660d862b7b1085bba84ab6e23e3cf0a732dd7c751b691c5450539`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b37097c0f732899899760f1a0ecf4d28df4e71f373ec4afb9bf706badbba17`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 311.9 KB (311894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:05cb95459d66a096424e07c1ed40a5be080386293e1f332d98587b154f495795
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65308759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b1dfad29a96eb0452204b34a699e432f876d5238fc40e3091e78c5e88867c1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:48:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:48:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:48:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386b993c0071d2bcf4a8f2250bfbd4fd50bcabb2d47b8fe81cff3ba3c954ad1b`  
		Last Modified: Sat, 04 Feb 2023 08:50:34 GMT  
		Size: 11.3 MB (11313033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5a3d24e8e01f6ab066d7fad4947aa0a7e70547302d3f7882dd82dda9907d2`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cb9fd8e38b57d30b04e23a8206ec76f508811e129bc4ffda4c8a0febef933`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73f1f5a7996bcea0a9b6a82d9b7384a62a8068b963ff9d707f0152657540088`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 311.8 KB (311789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; 386

```console
$ docker pull neurodebian@sha256:ce1fbd72b2cdd70b4db22df3ec6da4ef9fbd3e19547c5d0af564a7d774eff1bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67637598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fc5eeb71cd5570608df1aec87502a7e2016fbe882237e0f216f1b8d1bcc14a3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:37 GMT
ADD file:feaff299d3310c04952143a422f0d0bdd292cd174513c54b1f50765cdbcfd401 in / 
# Thu, 09 Feb 2023 05:12:38 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9708eacca143ba8fa6c7e9a5b05456412b7b16629c20015a43f3ca391e066162`  
		Last Modified: Thu, 09 Feb 2023 05:18:13 GMT  
		Size: 56.0 MB (56030197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6553645eeab9f9390c2c8b8a61e7694834123049b6f060dbdbb11ef6b6819`  
		Last Modified: Thu, 09 Feb 2023 12:45:34 GMT  
		Size: 11.5 MB (11500078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e1e93c20ee20a385a9d97ed62c22e11afd73974b6821310c2baca0eb530970`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a06c277f46a387d7ed96bf2575c4552a533f0d45c754c0680a1d8363ffebde3`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d84f478365f04d8d680da68bd0b3ea6cc10a025630c140d289b3a0a6c8705`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 105.3 KB (105331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:f61756a89ca0ae78a787ad5f097acbadc619d848eb89219f2ca55cf110fff99a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:5fe7da4512a60b0d04da2d0b934e3144b590651ef535f1f137a7aae63521eabe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61218765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3d8df3b4f832d39637ae30c01c22c727ef4adef9f5cb69891c3e416104e81e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:21:29 GMT
ADD file:b3a4ee0f0fbf2d8fbbab0aefd91aa4d658c41b09c8a2beea1024bfce5e7d3fca in / 
# Thu, 09 Feb 2023 03:21:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca2c7deeb5af7aa8a0aa3358218901c07b10bb98573151782e5e7af0ab03009c`  
		Last Modified: Thu, 09 Feb 2023 03:26:46 GMT  
		Size: 49.2 MB (49234515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8364caf5a58b2deb6126067cb35d010bad611576893cd5016c15f73077ed6`  
		Last Modified: Thu, 09 Feb 2023 10:35:29 GMT  
		Size: 11.7 MB (11700970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d427fbbb2b26c4a76ad11c5aca1a15a6e3a3ce0ebed9bb368ac16aa4b0a201c4`  
		Last Modified: Thu, 09 Feb 2023 10:35:27 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaccf87aac953e023363d8b331021aa3544b998ea3b8a32099f54494bf17268`  
		Last Modified: Thu, 09 Feb 2023 10:35:27 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d98dcb68c6cd5f7564faf602448779dafa9193a157852d3d9b0cb9194ff14a`  
		Last Modified: Thu, 09 Feb 2023 10:35:28 GMT  
		Size: 281.3 KB (281270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:6eb274643631939f13097c755fe3b8cf92bd7086309a009a638fbe6cd4c943a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60961349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d679ee54e61884acbc26f2ffce51aa67f4d41315ba0d0987a72d5f37fe00d5a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:18:18 GMT
ADD file:e0f39d8fee93f482160beca25b949b1de50ecc55ac86b1c276bed0b5c9955393 in / 
# Sat, 04 Feb 2023 06:18:19 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:49:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:49:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:541de84dec560e0a7dc13f9e5246f1a165b0955a6aefdc92d0bc46a50138a249`  
		Last Modified: Sat, 04 Feb 2023 06:22:53 GMT  
		Size: 49.1 MB (49064951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feef954a467cdbd9442f76eae26dcce65b43e942cf51fb0fc9932a2ce11a37a5`  
		Last Modified: Sat, 04 Feb 2023 08:51:11 GMT  
		Size: 11.6 MB (11613149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1fb0ddc7c21670259cb7fa6d33e4a66293440c6bb9ac9b12014f6ad578ba76`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b3ab955b5154981b3ebc74d79cacb2c050f8b3045d9e3b9bb5d5b3c6d69a3a`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e036d4fa82c2440e6b7a89404b4a9cdf679911cccfc91b67183e47fac4bfe42`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 281.2 KB (281241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; 386

```console
$ docker pull neurodebian@sha256:455b44b7e0c1d17689080417db8ac9f52f60cd492c355412ffe920270cfddaa2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62312627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aedf8b33e399cc416b854b13b947b342c26e5a35866973353a64f6ccc306a737`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:14:01 GMT
ADD file:9ac1978405b6f0a95e33d1c34f01be82bbc11fcce2878747e4f688335279964c in / 
# Thu, 09 Feb 2023 05:14:02 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:44:18 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:44:19 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:44:20 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:44:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e58ae2871ac91256d220f3da2b9736b2afb1a06906579876546cfae103647f95`  
		Last Modified: Thu, 09 Feb 2023 05:20:31 GMT  
		Size: 50.3 MB (50285434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2a120090af691fd4e5ade938037157e5d29f3d11e3c3fd540b83e8f5a65011`  
		Last Modified: Thu, 09 Feb 2023 12:46:22 GMT  
		Size: 11.9 MB (11933559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93706304552ccb0d7cebc8928c9d0832dbd0daca00da28c190209bade85501`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065c687c96091f2284561bb5a43d98da272ed8a551560f9d647cf28c84137b8`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe14b41a09e2614c0ecf5a7a46afa8824cb42dd8a5503453498ba712306cc7b8`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 91.6 KB (91647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:e49be3797df78950663c99383b242ecdb280aac33088c95d854db1b4cd93eb04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:1d4623f580034954fb9ae2a6581693e907b81515de59dbce4828b3fa0f7c237b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61219162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014f69502a0fadd5f7f6eeacbf6b145d2391afe2b7afeb3d39bdccf6f6453351`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:21:29 GMT
ADD file:b3a4ee0f0fbf2d8fbbab0aefd91aa4d658c41b09c8a2beea1024bfce5e7d3fca in / 
# Thu, 09 Feb 2023 03:21:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:54 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ca2c7deeb5af7aa8a0aa3358218901c07b10bb98573151782e5e7af0ab03009c`  
		Last Modified: Thu, 09 Feb 2023 03:26:46 GMT  
		Size: 49.2 MB (49234515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8364caf5a58b2deb6126067cb35d010bad611576893cd5016c15f73077ed6`  
		Last Modified: Thu, 09 Feb 2023 10:35:29 GMT  
		Size: 11.7 MB (11700970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d427fbbb2b26c4a76ad11c5aca1a15a6e3a3ce0ebed9bb368ac16aa4b0a201c4`  
		Last Modified: Thu, 09 Feb 2023 10:35:27 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaccf87aac953e023363d8b331021aa3544b998ea3b8a32099f54494bf17268`  
		Last Modified: Thu, 09 Feb 2023 10:35:27 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d98dcb68c6cd5f7564faf602448779dafa9193a157852d3d9b0cb9194ff14a`  
		Last Modified: Thu, 09 Feb 2023 10:35:28 GMT  
		Size: 281.3 KB (281270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d986c1719d280776ecb8e97d8c6f14bd2def0d6f2263214410856de069a22796`  
		Last Modified: Thu, 09 Feb 2023 10:35:37 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:0dfc6d72a79ebae3679ff6b7311d814ad650c536b908466f05bfedab09c0c447
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60961744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f8d4407ad794329f99fbc45860becd38ed0ebb95f343004673e640cc94f0e34`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:18:18 GMT
ADD file:e0f39d8fee93f482160beca25b949b1de50ecc55ac86b1c276bed0b5c9955393 in / 
# Sat, 04 Feb 2023 06:18:19 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:49:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:49:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:37 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:541de84dec560e0a7dc13f9e5246f1a165b0955a6aefdc92d0bc46a50138a249`  
		Last Modified: Sat, 04 Feb 2023 06:22:53 GMT  
		Size: 49.1 MB (49064951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feef954a467cdbd9442f76eae26dcce65b43e942cf51fb0fc9932a2ce11a37a5`  
		Last Modified: Sat, 04 Feb 2023 08:51:11 GMT  
		Size: 11.6 MB (11613149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1fb0ddc7c21670259cb7fa6d33e4a66293440c6bb9ac9b12014f6ad578ba76`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b3ab955b5154981b3ebc74d79cacb2c050f8b3045d9e3b9bb5d5b3c6d69a3a`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e036d4fa82c2440e6b7a89404b4a9cdf679911cccfc91b67183e47fac4bfe42`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 281.2 KB (281241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69955de265518b9a0350d0446a8659f1d17fbd7262785ae52dae2c7b501b6e42`  
		Last Modified: Sat, 04 Feb 2023 08:51:19 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:a7055efcfe63c64c27f2d87abf8735eb755fb868a8741acf37a3d7f454513e92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62313023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9887da48d9004339e187c7ffcab2d5c6c4ca7fbc748db978d079cfb9ac1777a2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:14:01 GMT
ADD file:9ac1978405b6f0a95e33d1c34f01be82bbc11fcce2878747e4f688335279964c in / 
# Thu, 09 Feb 2023 05:14:02 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:44:18 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:44:19 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:44:20 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:44:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:44:30 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:e58ae2871ac91256d220f3da2b9736b2afb1a06906579876546cfae103647f95`  
		Last Modified: Thu, 09 Feb 2023 05:20:31 GMT  
		Size: 50.3 MB (50285434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2a120090af691fd4e5ade938037157e5d29f3d11e3c3fd540b83e8f5a65011`  
		Last Modified: Thu, 09 Feb 2023 12:46:22 GMT  
		Size: 11.9 MB (11933559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93706304552ccb0d7cebc8928c9d0832dbd0daca00da28c190209bade85501`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065c687c96091f2284561bb5a43d98da272ed8a551560f9d647cf28c84137b8`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe14b41a09e2614c0ecf5a7a46afa8824cb42dd8a5503453498ba712306cc7b8`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 91.6 KB (91647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992b26ef35e55050f48421f0d0441414650d88f959be0fe5cc0f64dc9aa920b2`  
		Last Modified: Thu, 09 Feb 2023 12:46:31 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100`

```console
$ docker pull neurodebian@sha256:f6b65d4e5cbb5ea2efbd69cfe242233fb84e97ce8bc01604cc9cc57a0cd8da76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100` - linux; amd64

```console
$ docker pull neurodebian@sha256:8b7259439072b854b4b58ea410365639a35eab18c05cfb7c36fd003a9de08d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61260489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53c849b1ee4a2850d6051b704b9af212d309d9e27d8730ec6179dc41e0c7c186`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:33 GMT
ADD file:dc52371b5f4608e5887e8c657ff951d1895e0047960f44b153c4a55ebf1726d5 in / 
# Thu, 09 Feb 2023 03:20:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:32:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:32:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:32:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:32:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2404786f3febb4866f85b0c8f52b0b0b94dfdb6543e94cd65f961c68f325ff7`  
		Last Modified: Thu, 09 Feb 2023 03:25:32 GMT  
		Size: 50.4 MB (50449613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77502ab3ca1cfa948d065d90f0572b331e529eec6f234419b6ba0dd44c7e0135`  
		Last Modified: Thu, 09 Feb 2023 10:34:35 GMT  
		Size: 10.5 MB (10504538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec51aec442293416c6492307baf3e69b92abc070af15fe2f827239fb84259923`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59955829e458d6ce57c1941668246f2fcce15209bf143652918255813981e54`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258ee389ec682ceb8b472c2883f47efb2fa9bd667332c5120470649b3a98980`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 304.3 KB (304328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:dc36f118472fb5e0b20c26b75d1bfbcf49480dfc7776c2e37ace4b31486be06d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60056041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f705abad5e5e4d726795ac15eae33baf5a4e1a515ff1054f4a3774e3fccc03fa`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:45 GMT
ADD file:0241487c3fb43506be1511724644c00339c32361e6b4c21a224d7190e4e1063b in / 
# Sat, 04 Feb 2023 06:17:46 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:48:38 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:48:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:48:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e0a5a2afd38370f358c0a7154362a8d17faf709c206b40b1553a077f810c3b3`  
		Last Modified: Sat, 04 Feb 2023 06:21:43 GMT  
		Size: 49.2 MB (49239373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda0b3f7673107c2204b83097e20a33728ef30d2e731e41727e0915eb8eb7c9`  
		Last Modified: Sat, 04 Feb 2023 08:50:17 GMT  
		Size: 10.5 MB (10510366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e7e8e9562ff77a3d9a1bc9b20bcaaffb5ab25e375ce28460ba3a4018788fb`  
		Last Modified: Sat, 04 Feb 2023 08:50:16 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c8ab4aac39ddf7a0f79a2cc135d4c299bb4a80b3282626e03ba7581e2ec733`  
		Last Modified: Sat, 04 Feb 2023 08:50:16 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fc1d1a5e62555249343f0f0e4c5483c04f9b57bd28318895d6a9f14050a7e6`  
		Last Modified: Sat, 04 Feb 2023 08:50:17 GMT  
		Size: 304.3 KB (304289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100` - linux; 386

```console
$ docker pull neurodebian@sha256:416d3841ac6fc65e1d4e6c0c233c294cd2fef7f92695816da69b8eca9aa1be67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61990997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b12846deb7051a30b876d4ac76a2e38df8ef0e61f7b3c86c6f343721492b7841`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:13:04 GMT
ADD file:043d1820efa588dcc60e5d9c340fd1edcd43f2988435e6284844a71d4b082dc7 in / 
# Thu, 09 Feb 2023 05:13:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:01 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:03 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:04 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ee55492a1c0f9dc3f2620641096fc2d501a92c463492dd5598f15a6634c4d8bd`  
		Last Modified: Thu, 09 Feb 2023 05:19:04 GMT  
		Size: 51.2 MB (51207786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641c4ab61efe8b684f2f70e427f740060629acab64b255865a739b677e0947ac`  
		Last Modified: Thu, 09 Feb 2023 12:45:15 GMT  
		Size: 10.7 MB (10672461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfbc65dea7c5bef81239621c61d98f3956bcf57cd5fba5d2a09920e4aed1fb2`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3ea514e731298f7c296c9efa36329cb9a29422b0290649fdaab7c8c1aca590`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252f61add039c1f47969b061f788e132a2d94ab712013ed772c1480332874361`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 108.8 KB (108760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd100-non-free`

```console
$ docker pull neurodebian@sha256:b6b724d93933cad4e4425f4c2488273844cc47ed104e09e4ff4800386dad5aaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:a1bdd9b45aad906eea47ee012772269bf5422c4c625d82ea9fe347f429ffba84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61260846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dfe97d2fd7b4c7dc4431ea670b0b06a22c7bd5935941b40ab11a52b5276fa4e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:33 GMT
ADD file:dc52371b5f4608e5887e8c657ff951d1895e0047960f44b153c4a55ebf1726d5 in / 
# Thu, 09 Feb 2023 03:20:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:32:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:32:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:32:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:32:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:32:55 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b2404786f3febb4866f85b0c8f52b0b0b94dfdb6543e94cd65f961c68f325ff7`  
		Last Modified: Thu, 09 Feb 2023 03:25:32 GMT  
		Size: 50.4 MB (50449613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77502ab3ca1cfa948d065d90f0572b331e529eec6f234419b6ba0dd44c7e0135`  
		Last Modified: Thu, 09 Feb 2023 10:34:35 GMT  
		Size: 10.5 MB (10504538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec51aec442293416c6492307baf3e69b92abc070af15fe2f827239fb84259923`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59955829e458d6ce57c1941668246f2fcce15209bf143652918255813981e54`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258ee389ec682ceb8b472c2883f47efb2fa9bd667332c5120470649b3a98980`  
		Last Modified: Thu, 09 Feb 2023 10:34:34 GMT  
		Size: 304.3 KB (304328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf843247789a5bd789d96ea0d938767321149236fc262ca618a3848b2966ef7e`  
		Last Modified: Thu, 09 Feb 2023 10:34:42 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:9dbc4060d63354fc168ef4b4ce8d6572031d397dbd61b0240a71078697e7bc8d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60056397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e52ff1f01210e669f87eece484b274a1c9ed6dfe5aff7b6a0451113022b17b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:45 GMT
ADD file:0241487c3fb43506be1511724644c00339c32361e6b4c21a224d7190e4e1063b in / 
# Sat, 04 Feb 2023 06:17:46 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:48:38 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:48:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:48:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:46 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:8e0a5a2afd38370f358c0a7154362a8d17faf709c206b40b1553a077f810c3b3`  
		Last Modified: Sat, 04 Feb 2023 06:21:43 GMT  
		Size: 49.2 MB (49239373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda0b3f7673107c2204b83097e20a33728ef30d2e731e41727e0915eb8eb7c9`  
		Last Modified: Sat, 04 Feb 2023 08:50:17 GMT  
		Size: 10.5 MB (10510366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e7e8e9562ff77a3d9a1bc9b20bcaaffb5ab25e375ce28460ba3a4018788fb`  
		Last Modified: Sat, 04 Feb 2023 08:50:16 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c8ab4aac39ddf7a0f79a2cc135d4c299bb4a80b3282626e03ba7581e2ec733`  
		Last Modified: Sat, 04 Feb 2023 08:50:16 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fc1d1a5e62555249343f0f0e4c5483c04f9b57bd28318895d6a9f14050a7e6`  
		Last Modified: Sat, 04 Feb 2023 08:50:17 GMT  
		Size: 304.3 KB (304289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb106862c94d1d9cf42027a0b8de792e548f97d4bf206491e472fc6159c7e0e`  
		Last Modified: Sat, 04 Feb 2023 08:50:25 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:67c64ff956cb57efa4dfebe6c4c7150991d6f4fc47191cb124f5573bc5f4d027
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61991356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc45ca5c74ad14e514a7a4b704774bc433d2f3486af07bcc806487d21047ba72`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:13:04 GMT
ADD file:043d1820efa588dcc60e5d9c340fd1edcd43f2988435e6284844a71d4b082dc7 in / 
# Thu, 09 Feb 2023 05:13:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:01 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:03 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:04 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:14 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ee55492a1c0f9dc3f2620641096fc2d501a92c463492dd5598f15a6634c4d8bd`  
		Last Modified: Thu, 09 Feb 2023 05:19:04 GMT  
		Size: 51.2 MB (51207786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641c4ab61efe8b684f2f70e427f740060629acab64b255865a739b677e0947ac`  
		Last Modified: Thu, 09 Feb 2023 12:45:15 GMT  
		Size: 10.7 MB (10672461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfbc65dea7c5bef81239621c61d98f3956bcf57cd5fba5d2a09920e4aed1fb2`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3ea514e731298f7c296c9efa36329cb9a29422b0290649fdaab7c8c1aca590`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252f61add039c1f47969b061f788e132a2d94ab712013ed772c1480332874361`  
		Last Modified: Thu, 09 Feb 2023 12:45:13 GMT  
		Size: 108.8 KB (108760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa7209b6e78fe409e7508dd28ec663fb4b5351bac0ef5ed20fd61ae220f65a`  
		Last Modified: Thu, 09 Feb 2023 12:45:24 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110`

```console
$ docker pull neurodebian@sha256:632446b0900714f1210ae1c5d9c7cef7ccd9afbe294a7554667fdcce66722d32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110` - linux; amd64

```console
$ docker pull neurodebian@sha256:ccd1b59aad87a7c82820e157082bac2be35db3aaeb5a21b86b72ccf0d17bc03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66671505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de330a89bf9b3656ed0d4909c39ff822d84609fe0be661455e5ef82eef9375b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6748fef26b12a93a8ea2e78ebc615a49a0a17ea28b338a2543564de8dbe7a6`  
		Last Modified: Thu, 09 Feb 2023 10:34:52 GMT  
		Size: 11.3 MB (11310827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f8febb6240b1c0efe213c5ec66b0a670a65bacc58a728ee49d9595476b44d`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab659e925660d862b7b1085bba84ab6e23e3cf0a732dd7c751b691c5450539`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b37097c0f732899899760f1a0ecf4d28df4e71f373ec4afb9bf706badbba17`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 311.9 KB (311894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:05cb95459d66a096424e07c1ed40a5be080386293e1f332d98587b154f495795
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65308759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b1dfad29a96eb0452204b34a699e432f876d5238fc40e3091e78c5e88867c1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:48:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:48:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:48:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386b993c0071d2bcf4a8f2250bfbd4fd50bcabb2d47b8fe81cff3ba3c954ad1b`  
		Last Modified: Sat, 04 Feb 2023 08:50:34 GMT  
		Size: 11.3 MB (11313033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5a3d24e8e01f6ab066d7fad4947aa0a7e70547302d3f7882dd82dda9907d2`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cb9fd8e38b57d30b04e23a8206ec76f508811e129bc4ffda4c8a0febef933`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73f1f5a7996bcea0a9b6a82d9b7384a62a8068b963ff9d707f0152657540088`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 311.8 KB (311789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110` - linux; 386

```console
$ docker pull neurodebian@sha256:ce1fbd72b2cdd70b4db22df3ec6da4ef9fbd3e19547c5d0af564a7d774eff1bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67637598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fc5eeb71cd5570608df1aec87502a7e2016fbe882237e0f216f1b8d1bcc14a3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:37 GMT
ADD file:feaff299d3310c04952143a422f0d0bdd292cd174513c54b1f50765cdbcfd401 in / 
# Thu, 09 Feb 2023 05:12:38 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9708eacca143ba8fa6c7e9a5b05456412b7b16629c20015a43f3ca391e066162`  
		Last Modified: Thu, 09 Feb 2023 05:18:13 GMT  
		Size: 56.0 MB (56030197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6553645eeab9f9390c2c8b8a61e7694834123049b6f060dbdbb11ef6b6819`  
		Last Modified: Thu, 09 Feb 2023 12:45:34 GMT  
		Size: 11.5 MB (11500078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e1e93c20ee20a385a9d97ed62c22e11afd73974b6821310c2baca0eb530970`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a06c277f46a387d7ed96bf2575c4552a533f0d45c754c0680a1d8363ffebde3`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d84f478365f04d8d680da68bd0b3ea6cc10a025630c140d289b3a0a6c8705`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 105.3 KB (105331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:1862361da08d56105240d74ff35c75f58f9771d4a4eefb851f2bf37e3c538bdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:23260d0661d4e6523c3cf7910d025881a843462564e5fca0902506bcfc56d173
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66671865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0693ecdb52c35a1cf9714de341352d57dd8e00be2677c28cb59bbe30b1cb178`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:14 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6748fef26b12a93a8ea2e78ebc615a49a0a17ea28b338a2543564de8dbe7a6`  
		Last Modified: Thu, 09 Feb 2023 10:34:52 GMT  
		Size: 11.3 MB (11310827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f8febb6240b1c0efe213c5ec66b0a670a65bacc58a728ee49d9595476b44d`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab659e925660d862b7b1085bba84ab6e23e3cf0a732dd7c751b691c5450539`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b37097c0f732899899760f1a0ecf4d28df4e71f373ec4afb9bf706badbba17`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 311.9 KB (311894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be23a69f483739cf32a2e634572f1d3d062f6832c58c445c75f6a37363ca931c`  
		Last Modified: Thu, 09 Feb 2023 10:35:01 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:30cf133c2939a3e22c8c9c47f8a7e66b7e2ff19edf863a0431e3912e80c6d7d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65309119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28a13b8f85eea85993fd122f87cf1d2e938e7897346d1e1ad5a275adf7ef906d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:48:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:48:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:48:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:02 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386b993c0071d2bcf4a8f2250bfbd4fd50bcabb2d47b8fe81cff3ba3c954ad1b`  
		Last Modified: Sat, 04 Feb 2023 08:50:34 GMT  
		Size: 11.3 MB (11313033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5a3d24e8e01f6ab066d7fad4947aa0a7e70547302d3f7882dd82dda9907d2`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cb9fd8e38b57d30b04e23a8206ec76f508811e129bc4ffda4c8a0febef933`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73f1f5a7996bcea0a9b6a82d9b7384a62a8068b963ff9d707f0152657540088`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 311.8 KB (311789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f08233a2e298109671c3c73b17ab2cadfcf1339e4cdf03e2f98d3c5f0bb5c7`  
		Last Modified: Sat, 04 Feb 2023 08:50:44 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:82ac3daeabbbb43956bcc98ff892f14cd4e2eda9ab0677ffeda6875a104c03ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67637958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d0ff2f87b876e0b73be59b8afc1428e66a7ae42299c9f6896df1456db5bde4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:37 GMT
ADD file:feaff299d3310c04952143a422f0d0bdd292cd174513c54b1f50765cdbcfd401 in / 
# Thu, 09 Feb 2023 05:12:38 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:39 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:9708eacca143ba8fa6c7e9a5b05456412b7b16629c20015a43f3ca391e066162`  
		Last Modified: Thu, 09 Feb 2023 05:18:13 GMT  
		Size: 56.0 MB (56030197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6553645eeab9f9390c2c8b8a61e7694834123049b6f060dbdbb11ef6b6819`  
		Last Modified: Thu, 09 Feb 2023 12:45:34 GMT  
		Size: 11.5 MB (11500078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e1e93c20ee20a385a9d97ed62c22e11afd73974b6821310c2baca0eb530970`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a06c277f46a387d7ed96bf2575c4552a533f0d45c754c0680a1d8363ffebde3`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d84f478365f04d8d680da68bd0b3ea6cc10a025630c140d289b3a0a6c8705`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 105.3 KB (105331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5028dc054643bc57886786396802ac777b7d450c096930465a29c82c7004c12`  
		Last Modified: Thu, 09 Feb 2023 12:45:47 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120`

```console
$ docker pull neurodebian@sha256:4bf980a902cb6e7571e8beaf42bbfbbe7b1bc4dc071491be355a63c9f66ae4b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120` - linux; amd64

```console
$ docker pull neurodebian@sha256:eb5a0a012ff4ce61cf3be35916cf6c57d17003f0d54cc1e73dce0f470ec5bbca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60987077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b561be2d8127b316aaf04f6bb16054759c690801338e869278a1edc135effea`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:19:36 GMT
ADD file:99a61197d7273704581c44eae01f3342e9f3562e84fe66cc2d56ce563e58450a in / 
# Thu, 09 Feb 2023 03:19:37 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:25 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:45c04dd46fbf614b423b54561d34c6339a0376d1717729ef6dcf101dbfd20f8c`  
		Last Modified: Thu, 09 Feb 2023 03:24:14 GMT  
		Size: 49.1 MB (49054961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38236192934019393b60f6a155f92e7625f86d7040a25abc85f16331e3f20a9`  
		Last Modified: Thu, 09 Feb 2023 10:35:12 GMT  
		Size: 11.6 MB (11649251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ce3c24436d316066f2f512361cceecec6597a642758cd8a30a7e6be8045177`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389c3b6867a3b8b7a0990aed29d11f0ca7d3451728e8394e1ffd435a9860c08c`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3878ef31203d1f458f083c3adf2cefb760dd8bbc98002c0732519fe24393de`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 280.9 KB (280853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:47d7a6535244ad6e95e521fd44c18618793ed1aa080c1eead00b9dcd26032188
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60978100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d0990886517f471603003c7bff9a8442a9624b45903ac2c0307fba5b87c4eaf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:08 GMT
ADD file:b40ad920bd7dd081e20adf36435db50381b9998a1de3d2eac6b2c45734ce60b3 in / 
# Sat, 04 Feb 2023 06:17:09 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:49:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:49:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a43b5d5927a7651097e784be4430a6ade09951f5b6879cd06b0f51fc7c4812af`  
		Last Modified: Sat, 04 Feb 2023 06:20:30 GMT  
		Size: 49.1 MB (49081538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2178538c5bc5dcf98be54976e26e3643caa3a37f742386a75aeeda9818488236`  
		Last Modified: Sat, 04 Feb 2023 08:50:55 GMT  
		Size: 11.6 MB (11613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5946ba90fc15d686558f937d9db8c112910bfcc60659eae41906cab00536fbd1`  
		Last Modified: Sat, 04 Feb 2023 08:50:54 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d06715673a85e222fe91b40adfd40e6cf12abad4d8fc6b94aa1a329f289b576`  
		Last Modified: Sat, 04 Feb 2023 08:50:53 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302b2fd07b19b38ae39db22c7c35d3f8f01c22b33486483bc0f26dd2f8d1e600`  
		Last Modified: Sat, 04 Feb 2023 08:50:54 GMT  
		Size: 281.2 KB (281229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120` - linux; 386

```console
$ docker pull neurodebian@sha256:e37e3580493d2c03ad895fdd2504cc02a33c83c13b2a60bc1aa72e40ced14664
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62065634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7678b3f84b1c990678feca32d4533daea648cfe711fcc0e5fc012e584c6f8689`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:11 GMT
ADD file:37cc85485a8f79a4bd5557a42685805da0b367ff061d53fdf29d5f242593ea1d in / 
# Thu, 09 Feb 2023 05:12:12 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:52 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0153a17486e7cd96c30b54f1d68ab1cffaca99de43335324f16477807b1ddb1c`  
		Last Modified: Thu, 09 Feb 2023 05:17:35 GMT  
		Size: 50.1 MB (50089500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187a90aef6870d09282470d3b592e152d72bc909d4c41fc4d2a0dc6e35d578b`  
		Last Modified: Thu, 09 Feb 2023 12:46:01 GMT  
		Size: 11.9 MB (11882490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4ad0b3bec733e0fea46c5f1aa52aba6533737fae1c7ed922601bea2dbc7dbd`  
		Last Modified: Thu, 09 Feb 2023 12:45:58 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52056b4dd31d6fd76427109e57655ab7cdb36d3cdf6287f75d9ba2f4c8dcd0f`  
		Last Modified: Thu, 09 Feb 2023 12:45:59 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8502cd76b08bed33327032c663ce30112feb1286d449672cffdf1346457ab1`  
		Last Modified: Thu, 09 Feb 2023 12:45:59 GMT  
		Size: 91.7 KB (91655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd120-non-free`

```console
$ docker pull neurodebian@sha256:697d553cc84b55677c1e0d69e4d0acbe64c2e0a677d1fbc0a5ceeb38a1f55c10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:c248a7d665bda19d273222a908fa5850c1f1380317d8bc4916ae925e356167d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60987511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38d056149a345cb8309ad04642bf342a4b3f0c1daab681ef1b62aadf6c4c6806`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:19:36 GMT
ADD file:99a61197d7273704581c44eae01f3342e9f3562e84fe66cc2d56ce563e58450a in / 
# Thu, 09 Feb 2023 03:19:37 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:25 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:34 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:45c04dd46fbf614b423b54561d34c6339a0376d1717729ef6dcf101dbfd20f8c`  
		Last Modified: Thu, 09 Feb 2023 03:24:14 GMT  
		Size: 49.1 MB (49054961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38236192934019393b60f6a155f92e7625f86d7040a25abc85f16331e3f20a9`  
		Last Modified: Thu, 09 Feb 2023 10:35:12 GMT  
		Size: 11.6 MB (11649251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ce3c24436d316066f2f512361cceecec6597a642758cd8a30a7e6be8045177`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389c3b6867a3b8b7a0990aed29d11f0ca7d3451728e8394e1ffd435a9860c08c`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3878ef31203d1f458f083c3adf2cefb760dd8bbc98002c0732519fe24393de`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 280.9 KB (280853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec51a2c8898f4455cebcb45cced98d389e9c9f0dfd468a9540f6529c412742a8`  
		Last Modified: Thu, 09 Feb 2023 10:35:20 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:9d38cc525233e026ed1dc6ab33d626e38579465070da1b007a4377ad7e892c38
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60978528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f457705f06d5d27f6710a5d2077f18bec766f68fff56c944f7ad6428fca9b65`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:08 GMT
ADD file:b40ad920bd7dd081e20adf36435db50381b9998a1de3d2eac6b2c45734ce60b3 in / 
# Sat, 04 Feb 2023 06:17:09 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:49:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:49:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:21 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a43b5d5927a7651097e784be4430a6ade09951f5b6879cd06b0f51fc7c4812af`  
		Last Modified: Sat, 04 Feb 2023 06:20:30 GMT  
		Size: 49.1 MB (49081538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2178538c5bc5dcf98be54976e26e3643caa3a37f742386a75aeeda9818488236`  
		Last Modified: Sat, 04 Feb 2023 08:50:55 GMT  
		Size: 11.6 MB (11613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5946ba90fc15d686558f937d9db8c112910bfcc60659eae41906cab00536fbd1`  
		Last Modified: Sat, 04 Feb 2023 08:50:54 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d06715673a85e222fe91b40adfd40e6cf12abad4d8fc6b94aa1a329f289b576`  
		Last Modified: Sat, 04 Feb 2023 08:50:53 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302b2fd07b19b38ae39db22c7c35d3f8f01c22b33486483bc0f26dd2f8d1e600`  
		Last Modified: Sat, 04 Feb 2023 08:50:54 GMT  
		Size: 281.2 KB (281229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596e70a3c681969a418f4e81170b181a23350b8e71edecd45c416d7c429c37a5`  
		Last Modified: Sat, 04 Feb 2023 08:51:02 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:e493c2750ddd7876325a9c6ea61e4151508765499ed3754db677899a97357fa4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62066068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5dcb21fdd302fa0b7ef1f3c0c90c46056a0b4f1f86854e59113ff43965f7a7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:11 GMT
ADD file:37cc85485a8f79a4bd5557a42685805da0b367ff061d53fdf29d5f242593ea1d in / 
# Thu, 09 Feb 2023 05:12:12 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:52 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:44:06 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:0153a17486e7cd96c30b54f1d68ab1cffaca99de43335324f16477807b1ddb1c`  
		Last Modified: Thu, 09 Feb 2023 05:17:35 GMT  
		Size: 50.1 MB (50089500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187a90aef6870d09282470d3b592e152d72bc909d4c41fc4d2a0dc6e35d578b`  
		Last Modified: Thu, 09 Feb 2023 12:46:01 GMT  
		Size: 11.9 MB (11882490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4ad0b3bec733e0fea46c5f1aa52aba6533737fae1c7ed922601bea2dbc7dbd`  
		Last Modified: Thu, 09 Feb 2023 12:45:58 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52056b4dd31d6fd76427109e57655ab7cdb36d3cdf6287f75d9ba2f4c8dcd0f`  
		Last Modified: Thu, 09 Feb 2023 12:45:59 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8502cd76b08bed33327032c663ce30112feb1286d449672cffdf1346457ab1`  
		Last Modified: Thu, 09 Feb 2023 12:45:59 GMT  
		Size: 91.7 KB (91655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ec70962ca1ca64d913ade6eec99635035751b50e604d663e868b999958779a`  
		Last Modified: Thu, 09 Feb 2023 12:46:09 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04`

```console
$ docker pull neurodebian@sha256:e513ac1e11156aecac472db495f4a8a9289c483b45d0dc1b4a246b58da08ea53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd18.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:9eaae57e6a418b8c573fc5418ad64fe129309c35c2fd161bbdbf61a529730d9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31775229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:873262071297edd49a7d33afe192f7dd416fbcb8f8329bfc9d17b220889f04e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:58:43 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:58:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:58:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:58:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c561dd565402593670454bc67f0d32877f005872b8d25d4a588ff0bd84d74582`  
		Last Modified: Tue, 31 Jan 2023 19:00:39 GMT  
		Size: 4.8 MB (4821347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3199a21fc88a38a5953a4eda7d548104c2153dbacdbeac0c1f97636aa990429d`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4dc3134d8a8ba0f045aa233e851c13346eb4ea771d8394c56cf2863567c2a8`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c014dbfdfc0e1f416ac41d8cf451e1463598f92d704b7440a38610c18f4ebe26`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 240.4 KB (240380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd18.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5683ede91c2464e5b6ae9098e6c50ff505d17f1fa2f3e71b42ead7b3feccd26f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28382285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490edb93bb34812d94fffb01906d7d28c3e9fc0bb12c7cd49c911c949fa7ad3c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:08:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:08:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:08:44 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:08:49 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dbc19e87e6da7df7a26b73c38813e606d157ff82cead74668aa9fb1dde50fe`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 4.4 MB (4403764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b13f880e3b2e22e0f79bd577aae93628955db5dfb54dc16b5ee01d78e283612`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1536cf9d0676d119194aaac6a84cfd3883f661525fc07c8c16507232e4b0820`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455d9d3933a870d2b232e0931a36cc44e9dc946dd9f6dcdb07cc55b77f21a170`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 241.1 KB (241081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd18.04-non-free`

```console
$ docker pull neurodebian@sha256:691ca2cf102d15603a0c797e930a351ed9c873489a8ee27f1e76b43eadc33e50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd18.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:7c10782a79f7c72117a5374ce52548ca719f89305356417c7957eef4ce83a492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31775483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6c7baace0050bff9e555573db23e79cca0226c59505907eb177d7fd551e1e6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:58:43 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:58:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:58:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:58:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:58:58 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c561dd565402593670454bc67f0d32877f005872b8d25d4a588ff0bd84d74582`  
		Last Modified: Tue, 31 Jan 2023 19:00:39 GMT  
		Size: 4.8 MB (4821347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3199a21fc88a38a5953a4eda7d548104c2153dbacdbeac0c1f97636aa990429d`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4dc3134d8a8ba0f045aa233e851c13346eb4ea771d8394c56cf2863567c2a8`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c014dbfdfc0e1f416ac41d8cf451e1463598f92d704b7440a38610c18f4ebe26`  
		Last Modified: Tue, 31 Jan 2023 19:00:38 GMT  
		Size: 240.4 KB (240380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb917c28cea7ae4fa4a9d361cbbd4494ecd182af107d7ee5936bcb018641040`  
		Last Modified: Tue, 31 Jan 2023 19:00:46 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd18.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:0106f5e71d6be760cf4fa278aa89bf7ab086e4711f5751e8c9e46031e939ba69
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28382540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15489cd4bee72086827d309d7fa524ab5f75084ac3a273f752ba9de140d3d70f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:08:42 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:08:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:08:44 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:08:49 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:08:53 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:c58359f0ed0774e1ace1315b1a5c48c0d40a2519a5d69c92eb49fab69b4ff6b8`  
		Last Modified: Tue, 31 Jan 2023 18:07:50 GMT  
		Size: 23.7 MB (23735530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dbc19e87e6da7df7a26b73c38813e606d157ff82cead74668aa9fb1dde50fe`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 4.4 MB (4403764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b13f880e3b2e22e0f79bd577aae93628955db5dfb54dc16b5ee01d78e283612`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1536cf9d0676d119194aaac6a84cfd3883f661525fc07c8c16507232e4b0820`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455d9d3933a870d2b232e0931a36cc44e9dc946dd9f6dcdb07cc55b77f21a170`  
		Last Modified: Tue, 31 Jan 2023 18:10:28 GMT  
		Size: 241.1 KB (241081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3633341f6970cb9798062d7a3e8b9c338cf172ef3b05cdc69e65ba08a562aee`  
		Last Modified: Tue, 31 Jan 2023 18:10:39 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04`

```console
$ docker pull neurodebian@sha256:fc0e3f6a31571b6faef75452e7b452d8bd6b64ec637462b7dc067544e4285a3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd20.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:85b798bdb26eb6b1340fbc60fc0feec533e7dd20029f088b82cb4839a401cac5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34313257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fbceb465a22ad0be1c177c9fe16c5812526ba3dac6c3065f5eefbdd9efacfc1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:32:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:32:16 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 01 Feb 2023 19:32:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 01 Feb 2023 19:32:22 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340633481010cfb4323a6980ddc3fbb99c2b231c2bae539ce3adbe4323848f34`  
		Last Modified: Wed, 01 Feb 2023 19:33:24 GMT  
		Size: 5.5 MB (5494456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6a75d823acce0fa96f4fa88a59f0531577b8f2838bfe342fd493d768cbfcd`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1424e1c74c34cfbb9d0566bfa17947ded4bdff35d712e953ebe4b9a83f3483`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b985a598f6b1f9e18c76e8ff8ec2a3031cee1c84d02604bcde89fe5b75df28e4`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 238.9 KB (238907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd20.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5f43cd8b79163c0d9d100aaf36b45be3a012257ff691d14de42300c681ff6862
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32909337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fde545e728f21aeef32f65cf9201e112821ed623b0cd56fa89b9b5024752244`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:48:36 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:48:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 01 Feb 2023 18:48:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 01 Feb 2023 18:48:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c5c02fa6b59ab2149fa6bd73b93cc90d70885b4c89395e276408e863c13469`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 5.5 MB (5474533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558f1a74caa43afa1ef7b67ba9f69563ea68ccc494931e60f17601e0d197766f`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc55772b4b9049168de57f770b06cdc6b133aad697a9d81fd887d0845d6b2e4`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64d2353b0251a8e328c31de617a38bc62b5f305270c4e614d42af92b1e1cc2b`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 239.1 KB (239055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd20.04-non-free`

```console
$ docker pull neurodebian@sha256:d60d4892922515af262d9b747b2b0c64622190e73ac678135285993f68ac0b85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd20.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:168dd889aecd1f1d598a9b69160fa460d720c310f55b50eb7f132e76a28326b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34313515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a7515b917b364356f96522dc926c5c828a4bf0df70fcf3945bd0f22f7fb7ba0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:32:14 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:32:16 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 01 Feb 2023 19:32:16 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 01 Feb 2023 19:32:22 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:32:26 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340633481010cfb4323a6980ddc3fbb99c2b231c2bae539ce3adbe4323848f34`  
		Last Modified: Wed, 01 Feb 2023 19:33:24 GMT  
		Size: 5.5 MB (5494456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6a75d823acce0fa96f4fa88a59f0531577b8f2838bfe342fd493d768cbfcd`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1424e1c74c34cfbb9d0566bfa17947ded4bdff35d712e953ebe4b9a83f3483`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b985a598f6b1f9e18c76e8ff8ec2a3031cee1c84d02604bcde89fe5b75df28e4`  
		Last Modified: Wed, 01 Feb 2023 19:33:23 GMT  
		Size: 238.9 KB (238907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dbb4dc6c7f0965eb4d15b6c9b5762a70d0caf0e9fca5b9eb8c5dbe3211b746`  
		Last Modified: Wed, 01 Feb 2023 19:33:31 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd20.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:757707483fe2ff4d1589194906a99b162fc40a8b19fe18f56b7e989510aae4c1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32909592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e032ef358f0f25a08aba8f3214453113a399a57680920f1d06b130156139f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:48:36 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:48:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 01 Feb 2023 18:48:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 01 Feb 2023 18:48:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:48:44 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c5c02fa6b59ab2149fa6bd73b93cc90d70885b4c89395e276408e863c13469`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 5.5 MB (5474533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558f1a74caa43afa1ef7b67ba9f69563ea68ccc494931e60f17601e0d197766f`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc55772b4b9049168de57f770b06cdc6b133aad697a9d81fd887d0845d6b2e4`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64d2353b0251a8e328c31de617a38bc62b5f305270c4e614d42af92b1e1cc2b`  
		Last Modified: Wed, 01 Feb 2023 18:49:45 GMT  
		Size: 239.1 KB (239055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3479d262aebc44602af32ef7336be8974c16ae723c6ab77fba1e7f9149483d`  
		Last Modified: Wed, 01 Feb 2023 18:49:53 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd22.04`

```console
$ docker pull neurodebian@sha256:91558095dc8910356f23d8076b9e5bf353defc04223d3ee7a18400505ca71261
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd22.04` - linux; amd64

```console
$ docker pull neurodebian@sha256:cada10ba69f57f775b9a16faf888565f07d1b296414c488e3fca9431c22eb82e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34455516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b792d6fc44f8bc39ec8ca5d656529a5b8e1492d6cf4d082b0cd49d8488881de`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:59:37 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:59:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:59:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:59:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400062d61da6ac9d18eda99b4de78dbf1a9cea47ada42fb59417bd7d3940966f`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 3.8 MB (3766134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50dda20f552df25b1a3c041dc92181af9b5119500b13a52cde52648c6017d94c`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3f682ee0399a91bfe1c17e2e5ab2568e45560917037011fec50f7d71e38f73`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cac7bfc4ecfa33e13fd29c32d5dcca6e240446d22389f2b5f5acfa67a23ebd`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 258.4 KB (258366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd22.04` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:4da522322b179b93738a554ff42291674f410633468302dd3d7bd78301252a47
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32386337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f27e0b58fd465ae00b00a9699e5f6d77c96a7ad58c71aaba7095dc9079d9128a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:09:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:09:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:09:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:09:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c38043ccc25501401b9d77af23fd531bac15eb599f37aa73c2942390f0f89`  
		Last Modified: Tue, 31 Jan 2023 18:11:05 GMT  
		Size: 3.7 MB (3739627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80411de25d3f2eee928df25a78042197af878bcef13d3d216f05d002d204251a`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0062cb70e52c57d65210d9b388e6d54a802a2fe89c07a377d86c4ef4502ff590`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b27a9557ed3f80818b8a9ec76450e885b5ffe64974f8eb88642d67dd3319fff`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 259.7 KB (259722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:nd22.04-non-free`

```console
$ docker pull neurodebian@sha256:ccb27ac7137a1b4182dd842114c37428a600b752e0a730e9c549e04c9532a2d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:nd22.04-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:db0328bfc73471afc6ea3959e9064784e0dd65fb33221f8f8521acec39130003
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34455776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b38aceba7f88d45ed89bf01fcb40220c82e24b6d334c9b0b89d08767fd5b80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:59:37 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:59:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:59:39 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:59:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:59:47 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400062d61da6ac9d18eda99b4de78dbf1a9cea47ada42fb59417bd7d3940966f`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 3.8 MB (3766134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50dda20f552df25b1a3c041dc92181af9b5119500b13a52cde52648c6017d94c`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3f682ee0399a91bfe1c17e2e5ab2568e45560917037011fec50f7d71e38f73`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cac7bfc4ecfa33e13fd29c32d5dcca6e240446d22389f2b5f5acfa67a23ebd`  
		Last Modified: Tue, 31 Jan 2023 19:01:10 GMT  
		Size: 258.4 KB (258366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f11ca7c2dee167ced8c8ec1ceff5bc630ac061bdd9f59ed00071722ab7e4070`  
		Last Modified: Tue, 31 Jan 2023 19:01:18 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd22.04-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:5b770230161b71f7a2138e112d463c38b90dffd6594d2f302b7a18d1b4ec02ae
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32386596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f059c6b605395fae939c68fffd06ebbdf64ae2b55e1622515c21d759152063`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:09:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:09:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 31 Jan 2023 18:09:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jammy main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jammy main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 31 Jan 2023 18:09:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:09:33 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c38043ccc25501401b9d77af23fd531bac15eb599f37aa73c2942390f0f89`  
		Last Modified: Tue, 31 Jan 2023 18:11:05 GMT  
		Size: 3.7 MB (3739627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80411de25d3f2eee928df25a78042197af878bcef13d3d216f05d002d204251a`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0062cb70e52c57d65210d9b388e6d54a802a2fe89c07a377d86c4ef4502ff590`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b27a9557ed3f80818b8a9ec76450e885b5ffe64974f8eb88642d67dd3319fff`  
		Last Modified: Tue, 31 Jan 2023 18:11:04 GMT  
		Size: 259.7 KB (259722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d03b38e66b4a534e50a16c431fd0aef94dc19cf45e0e60da70a12541a9870f1`  
		Last Modified: Tue, 31 Jan 2023 18:11:12 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:non-free`

```console
$ docker pull neurodebian@sha256:1862361da08d56105240d74ff35c75f58f9771d4a4eefb851f2bf37e3c538bdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:23260d0661d4e6523c3cf7910d025881a843462564e5fca0902506bcfc56d173
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66671865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0693ecdb52c35a1cf9714de341352d57dd8e00be2677c28cb59bbe30b1cb178`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:14 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6748fef26b12a93a8ea2e78ebc615a49a0a17ea28b338a2543564de8dbe7a6`  
		Last Modified: Thu, 09 Feb 2023 10:34:52 GMT  
		Size: 11.3 MB (11310827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38f8febb6240b1c0efe213c5ec66b0a670a65bacc58a728ee49d9595476b44d`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab659e925660d862b7b1085bba84ab6e23e3cf0a732dd7c751b691c5450539`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b37097c0f732899899760f1a0ecf4d28df4e71f373ec4afb9bf706badbba17`  
		Last Modified: Thu, 09 Feb 2023 10:34:50 GMT  
		Size: 311.9 KB (311894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be23a69f483739cf32a2e634572f1d3d062f6832c58c445c75f6a37363ca931c`  
		Last Modified: Thu, 09 Feb 2023 10:35:01 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:30cf133c2939a3e22c8c9c47f8a7e66b7e2ff19edf863a0431e3912e80c6d7d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65309119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28a13b8f85eea85993fd122f87cf1d2e938e7897346d1e1ad5a275adf7ef906d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:48:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:48:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:48:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:48:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:02 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386b993c0071d2bcf4a8f2250bfbd4fd50bcabb2d47b8fe81cff3ba3c954ad1b`  
		Last Modified: Sat, 04 Feb 2023 08:50:34 GMT  
		Size: 11.3 MB (11313033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5a3d24e8e01f6ab066d7fad4947aa0a7e70547302d3f7882dd82dda9907d2`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cb9fd8e38b57d30b04e23a8206ec76f508811e129bc4ffda4c8a0febef933`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73f1f5a7996bcea0a9b6a82d9b7384a62a8068b963ff9d707f0152657540088`  
		Last Modified: Sat, 04 Feb 2023 08:50:33 GMT  
		Size: 311.8 KB (311789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f08233a2e298109671c3c73b17ab2cadfcf1339e4cdf03e2f98d3c5f0bb5c7`  
		Last Modified: Sat, 04 Feb 2023 08:50:44 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:82ac3daeabbbb43956bcc98ff892f14cd4e2eda9ab0677ffeda6875a104c03ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67637958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d0ff2f87b876e0b73be59b8afc1428e66a7ae42299c9f6896df1456db5bde4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:37 GMT
ADD file:feaff299d3310c04952143a422f0d0bdd292cd174513c54b1f50765cdbcfd401 in / 
# Thu, 09 Feb 2023 05:12:38 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:28 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:39 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:9708eacca143ba8fa6c7e9a5b05456412b7b16629c20015a43f3ca391e066162`  
		Last Modified: Thu, 09 Feb 2023 05:18:13 GMT  
		Size: 56.0 MB (56030197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6553645eeab9f9390c2c8b8a61e7694834123049b6f060dbdbb11ef6b6819`  
		Last Modified: Thu, 09 Feb 2023 12:45:34 GMT  
		Size: 11.5 MB (11500078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e1e93c20ee20a385a9d97ed62c22e11afd73974b6821310c2baca0eb530970`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a06c277f46a387d7ed96bf2575c4552a533f0d45c754c0680a1d8363ffebde3`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d84f478365f04d8d680da68bd0b3ea6cc10a025630c140d289b3a0a6c8705`  
		Last Modified: Thu, 09 Feb 2023 12:45:33 GMT  
		Size: 105.3 KB (105331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5028dc054643bc57886786396802ac777b7d450c096930465a29c82c7004c12`  
		Last Modified: Thu, 09 Feb 2023 12:45:47 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:f61756a89ca0ae78a787ad5f097acbadc619d848eb89219f2ca55cf110fff99a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:5fe7da4512a60b0d04da2d0b934e3144b590651ef535f1f137a7aae63521eabe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61218765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3d8df3b4f832d39637ae30c01c22c727ef4adef9f5cb69891c3e416104e81e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:21:29 GMT
ADD file:b3a4ee0f0fbf2d8fbbab0aefd91aa4d658c41b09c8a2beea1024bfce5e7d3fca in / 
# Thu, 09 Feb 2023 03:21:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca2c7deeb5af7aa8a0aa3358218901c07b10bb98573151782e5e7af0ab03009c`  
		Last Modified: Thu, 09 Feb 2023 03:26:46 GMT  
		Size: 49.2 MB (49234515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8364caf5a58b2deb6126067cb35d010bad611576893cd5016c15f73077ed6`  
		Last Modified: Thu, 09 Feb 2023 10:35:29 GMT  
		Size: 11.7 MB (11700970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d427fbbb2b26c4a76ad11c5aca1a15a6e3a3ce0ebed9bb368ac16aa4b0a201c4`  
		Last Modified: Thu, 09 Feb 2023 10:35:27 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaccf87aac953e023363d8b331021aa3544b998ea3b8a32099f54494bf17268`  
		Last Modified: Thu, 09 Feb 2023 10:35:27 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d98dcb68c6cd5f7564faf602448779dafa9193a157852d3d9b0cb9194ff14a`  
		Last Modified: Thu, 09 Feb 2023 10:35:28 GMT  
		Size: 281.3 KB (281270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:6eb274643631939f13097c755fe3b8cf92bd7086309a009a638fbe6cd4c943a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60961349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d679ee54e61884acbc26f2ffce51aa67f4d41315ba0d0987a72d5f37fe00d5a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:18:18 GMT
ADD file:e0f39d8fee93f482160beca25b949b1de50ecc55ac86b1c276bed0b5c9955393 in / 
# Sat, 04 Feb 2023 06:18:19 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:49:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:49:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:541de84dec560e0a7dc13f9e5246f1a165b0955a6aefdc92d0bc46a50138a249`  
		Last Modified: Sat, 04 Feb 2023 06:22:53 GMT  
		Size: 49.1 MB (49064951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feef954a467cdbd9442f76eae26dcce65b43e942cf51fb0fc9932a2ce11a37a5`  
		Last Modified: Sat, 04 Feb 2023 08:51:11 GMT  
		Size: 11.6 MB (11613149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1fb0ddc7c21670259cb7fa6d33e4a66293440c6bb9ac9b12014f6ad578ba76`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b3ab955b5154981b3ebc74d79cacb2c050f8b3045d9e3b9bb5d5b3c6d69a3a`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e036d4fa82c2440e6b7a89404b4a9cdf679911cccfc91b67183e47fac4bfe42`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 281.2 KB (281241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid` - linux; 386

```console
$ docker pull neurodebian@sha256:455b44b7e0c1d17689080417db8ac9f52f60cd492c355412ffe920270cfddaa2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62312627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aedf8b33e399cc416b854b13b947b342c26e5a35866973353a64f6ccc306a737`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:14:01 GMT
ADD file:9ac1978405b6f0a95e33d1c34f01be82bbc11fcce2878747e4f688335279964c in / 
# Thu, 09 Feb 2023 05:14:02 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:44:18 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:44:19 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:44:20 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:44:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e58ae2871ac91256d220f3da2b9736b2afb1a06906579876546cfae103647f95`  
		Last Modified: Thu, 09 Feb 2023 05:20:31 GMT  
		Size: 50.3 MB (50285434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2a120090af691fd4e5ade938037157e5d29f3d11e3c3fd540b83e8f5a65011`  
		Last Modified: Thu, 09 Feb 2023 12:46:22 GMT  
		Size: 11.9 MB (11933559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93706304552ccb0d7cebc8928c9d0832dbd0daca00da28c190209bade85501`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065c687c96091f2284561bb5a43d98da272ed8a551560f9d647cf28c84137b8`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe14b41a09e2614c0ecf5a7a46afa8824cb42dd8a5503453498ba712306cc7b8`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 91.6 KB (91647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:e49be3797df78950663c99383b242ecdb280aac33088c95d854db1b4cd93eb04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:1d4623f580034954fb9ae2a6581693e907b81515de59dbce4828b3fa0f7c237b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61219162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014f69502a0fadd5f7f6eeacbf6b145d2391afe2b7afeb3d39bdccf6f6453351`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:21:29 GMT
ADD file:b3a4ee0f0fbf2d8fbbab0aefd91aa4d658c41b09c8a2beea1024bfce5e7d3fca in / 
# Thu, 09 Feb 2023 03:21:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:44 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:46 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:54 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ca2c7deeb5af7aa8a0aa3358218901c07b10bb98573151782e5e7af0ab03009c`  
		Last Modified: Thu, 09 Feb 2023 03:26:46 GMT  
		Size: 49.2 MB (49234515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8364caf5a58b2deb6126067cb35d010bad611576893cd5016c15f73077ed6`  
		Last Modified: Thu, 09 Feb 2023 10:35:29 GMT  
		Size: 11.7 MB (11700970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d427fbbb2b26c4a76ad11c5aca1a15a6e3a3ce0ebed9bb368ac16aa4b0a201c4`  
		Last Modified: Thu, 09 Feb 2023 10:35:27 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaccf87aac953e023363d8b331021aa3544b998ea3b8a32099f54494bf17268`  
		Last Modified: Thu, 09 Feb 2023 10:35:27 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d98dcb68c6cd5f7564faf602448779dafa9193a157852d3d9b0cb9194ff14a`  
		Last Modified: Thu, 09 Feb 2023 10:35:28 GMT  
		Size: 281.3 KB (281270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d986c1719d280776ecb8e97d8c6f14bd2def0d6f2263214410856de069a22796`  
		Last Modified: Thu, 09 Feb 2023 10:35:37 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:0dfc6d72a79ebae3679ff6b7311d814ad650c536b908466f05bfedab09c0c447
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60961744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f8d4407ad794329f99fbc45860becd38ed0ebb95f343004673e640cc94f0e34`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:18:18 GMT
ADD file:e0f39d8fee93f482160beca25b949b1de50ecc55ac86b1c276bed0b5c9955393 in / 
# Sat, 04 Feb 2023 06:18:19 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:49:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:49:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:37 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:541de84dec560e0a7dc13f9e5246f1a165b0955a6aefdc92d0bc46a50138a249`  
		Last Modified: Sat, 04 Feb 2023 06:22:53 GMT  
		Size: 49.1 MB (49064951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feef954a467cdbd9442f76eae26dcce65b43e942cf51fb0fc9932a2ce11a37a5`  
		Last Modified: Sat, 04 Feb 2023 08:51:11 GMT  
		Size: 11.6 MB (11613149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1fb0ddc7c21670259cb7fa6d33e4a66293440c6bb9ac9b12014f6ad578ba76`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b3ab955b5154981b3ebc74d79cacb2c050f8b3045d9e3b9bb5d5b3c6d69a3a`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e036d4fa82c2440e6b7a89404b4a9cdf679911cccfc91b67183e47fac4bfe42`  
		Last Modified: Sat, 04 Feb 2023 08:51:10 GMT  
		Size: 281.2 KB (281241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69955de265518b9a0350d0446a8659f1d17fbd7262785ae52dae2c7b501b6e42`  
		Last Modified: Sat, 04 Feb 2023 08:51:19 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:sid-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:a7055efcfe63c64c27f2d87abf8735eb755fb868a8741acf37a3d7f454513e92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62313023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9887da48d9004339e187c7ffcab2d5c6c4ca7fbc748db978d079cfb9ac1777a2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:14:01 GMT
ADD file:9ac1978405b6f0a95e33d1c34f01be82bbc11fcce2878747e4f688335279964c in / 
# Thu, 09 Feb 2023 05:14:02 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:44:18 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:44:19 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:44:20 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:44:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:44:30 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:e58ae2871ac91256d220f3da2b9736b2afb1a06906579876546cfae103647f95`  
		Last Modified: Thu, 09 Feb 2023 05:20:31 GMT  
		Size: 50.3 MB (50285434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2a120090af691fd4e5ade938037157e5d29f3d11e3c3fd540b83e8f5a65011`  
		Last Modified: Thu, 09 Feb 2023 12:46:22 GMT  
		Size: 11.9 MB (11933559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a93706304552ccb0d7cebc8928c9d0832dbd0daca00da28c190209bade85501`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065c687c96091f2284561bb5a43d98da272ed8a551560f9d647cf28c84137b8`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe14b41a09e2614c0ecf5a7a46afa8824cb42dd8a5503453498ba712306cc7b8`  
		Last Modified: Thu, 09 Feb 2023 12:46:21 GMT  
		Size: 91.6 KB (91647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992b26ef35e55050f48421f0d0441414650d88f959be0fe5cc0f64dc9aa920b2`  
		Last Modified: Thu, 09 Feb 2023 12:46:31 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
