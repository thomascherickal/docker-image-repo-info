<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `julia`

-	[`julia:1`](#julia1)
-	[`julia:1-alpine`](#julia1-alpine)
-	[`julia:1-alpine3.13`](#julia1-alpine313)
-	[`julia:1-buster`](#julia1-buster)
-	[`julia:1-windowsservercore-1809`](#julia1-windowsservercore-1809)
-	[`julia:1-windowsservercore-ltsc2016`](#julia1-windowsservercore-ltsc2016)
-	[`julia:1.0`](#julia10)
-	[`julia:1.0-buster`](#julia10-buster)
-	[`julia:1.0-stretch`](#julia10-stretch)
-	[`julia:1.0-windowsservercore-1809`](#julia10-windowsservercore-1809)
-	[`julia:1.0-windowsservercore-ltsc2016`](#julia10-windowsservercore-ltsc2016)
-	[`julia:1.0.5`](#julia105)
-	[`julia:1.0.5-buster`](#julia105-buster)
-	[`julia:1.0.5-stretch`](#julia105-stretch)
-	[`julia:1.0.5-windowsservercore-1809`](#julia105-windowsservercore-1809)
-	[`julia:1.0.5-windowsservercore-ltsc2016`](#julia105-windowsservercore-ltsc2016)
-	[`julia:1.6`](#julia16)
-	[`julia:1.6-alpine`](#julia16-alpine)
-	[`julia:1.6-alpine3.13`](#julia16-alpine313)
-	[`julia:1.6-buster`](#julia16-buster)
-	[`julia:1.6-windowsservercore-1809`](#julia16-windowsservercore-1809)
-	[`julia:1.6-windowsservercore-ltsc2016`](#julia16-windowsservercore-ltsc2016)
-	[`julia:1.6.1`](#julia161)
-	[`julia:1.6.1-alpine`](#julia161-alpine)
-	[`julia:1.6.1-alpine3.13`](#julia161-alpine313)
-	[`julia:1.6.1-buster`](#julia161-buster)
-	[`julia:1.6.1-windowsservercore-1809`](#julia161-windowsservercore-1809)
-	[`julia:1.6.1-windowsservercore-ltsc2016`](#julia161-windowsservercore-ltsc2016)
-	[`julia:alpine`](#juliaalpine)
-	[`julia:alpine3.13`](#juliaalpine313)
-	[`julia:buster`](#juliabuster)
-	[`julia:latest`](#julialatest)
-	[`julia:windowsservercore-1809`](#juliawindowsservercore-1809)
-	[`julia:windowsservercore-ltsc2016`](#juliawindowsservercore-ltsc2016)

## `julia:1`

```console
$ docker pull julia@sha256:ce3a3fe709ac7e242b4d8fd081a13f1e7cd160f7cabb592b9552bf563fa8f5a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `julia:1` - linux; amd64

```console
$ docker pull julia@sha256:9e0a7e7f671ff4249101208df5150945e3b15d4a712ec068a1ca82afb8e70833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152635667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5406d71f1cccd07971d3759be41a3e4ea3c0f52a740b246d40da57684cfa077`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:08 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 19:38:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc393e77a75f632f581added9733180f506256f659d50247f42862153b44a2d`  
		Last Modified: Mon, 26 Apr 2021 19:39:41 GMT  
		Size: 121.0 MB (121038297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm variant v7

```console
$ docker pull julia@sha256:a03e9e70fd6d73b842cbeca5112acc107bbd4c6fbd63c5b56c708a266224807d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138668730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9dea7467a9211b67e60854de9e2ebd34d257b065ecf56ef47446445fafc80bc`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 20:10:16 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:16:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:16:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacce62cd0061e689b2f6a7abf6ba0372808efc29bf5fcfd302a8e07825dd29`  
		Last Modified: Mon, 10 May 2021 21:17:40 GMT  
		Size: 112.1 MB (112123457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0b1bb0aa54548f67f8027615d6cd9f28629f9428e3d7775b543669d7a63a7370
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145159457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb777f8f3d4ca2313ecc47b6894705e9265ca1410009749d73d7902ab846e46f`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:02:48 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:14:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:14:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42476a9f7e3bcac4810c863cd8d19cf0eb4eb627c0e90c934c09796844599dd`  
		Last Modified: Mon, 10 May 2021 21:15:33 GMT  
		Size: 114.9 MB (114916446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:03edae6d5bfcebbd136b888b8d94a7fd71fc752db39d60319dbc52c2cf277955
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151020856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779d82018ac27ee00e27417a817b697d39aa87594ab4607303be7416871c7bcb`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 18:54:54 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 18:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 18:55:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcd3467ae1a05da8d7c83b3c276e92778b61d6b90c5913785049f463745b39d`  
		Last Modified: Mon, 26 Apr 2021 18:56:23 GMT  
		Size: 118.6 MB (118621282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; ppc64le

```console
$ docker pull julia@sha256:34f2b72bbab5bb60259559e69c3e31a388e502db98d0a360088c271b39a04118
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141797926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142a7fd70412cc059bddf7a9c1b19ae16fce2caa33bf8689e959f3f38171b1fe`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:44:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 14:44:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 14:44:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 21:34:17 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:36:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 21:37:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de5cbe49ae47809605d7676cf919113b9fcd0039eeeb96d8a990491cb6e266e`  
		Last Modified: Sat, 10 Apr 2021 14:47:08 GMT  
		Size: 4.9 MB (4853557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b7e6fa0abc963aba7a4fc0f66f88960593b6afdf11c1a264e40403924f737`  
		Last Modified: Mon, 26 Apr 2021 21:38:02 GMT  
		Size: 106.4 MB (106398436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:e75466db30b85df9499b4547b8800e7e7755a324c3ee303f978990c2a83a625e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2607668952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415cc2c3e6325cbf96ebb79033925c33d584618fd11a8b0d73ea7ccbf4f4bd2c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:02:47 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:02:48 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:04:26 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:04:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d62f536b5a512c7dda3dfa351ff2a7113f409efe61f18feebd3fe3739927bc`  
		Last Modified: Mon, 26 Apr 2021 21:08:03 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001c92228b8dfe3a318ea88fa0c4f005aab8ac0bc0a4a7b17daacb3b11a01ea`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a5006275da11a373e2da6e690d7567700b3e040322583e596a2e968e34153`  
		Last Modified: Mon, 26 Apr 2021 21:08:36 GMT  
		Size: 137.9 MB (137909420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d6a3269b15f3d75f3292fcaa599df92e864d530a71ac1d5a0827b4a6120e71`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:8c989761b1dc748646817175b7623754f784aaea26070852701f14184040bd6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937855117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261a028fcf019c1cc5a1103c3359767ecff911c002d73e53c132f2e77ce27f84`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:04:45 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:04:46 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:07:09 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:07:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b8ff0cbb14542ed03b2c1fdb5d6e4b1787e9af6ac9a33fb06dbc7b119d9e69`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b526113b3aa441415c74b9d97a76dbb51fc93a620e2cf7d3570565f00da19`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a952cc9a0bfa19a13f0a4e8394c838a67a56d8fe4f61a601f28bb258db138f1`  
		Last Modified: Mon, 26 Apr 2021 21:09:26 GMT  
		Size: 143.0 MB (142965626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b17799f8a1b7ae1f6d125d71b7b27be62cbfc5d3e8d5fb83ebacd72df660fa`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine`

```console
$ docker pull julia@sha256:36052a38d8ce24173a714e6f45e15217fc5f6db83f6e3362bea1e9b330e602f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1-alpine` - linux; amd64

```console
$ docker pull julia@sha256:ca3709087833add7942f34806d4ca65ccd2ab5e59126a9c6c4cae85a20fe36e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123108120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e8f10e31159b593f38f63d8737617466ba087325f6a24c7dee6fef1f502de3`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 14 Apr 2021 23:02:59 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:28 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='492514c93c97e7012b8124a959a9f5569231e52b14f992e74a977fffd7b8961b' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 26 Apr 2021 19:38:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f83c49c066b01cd3dbd841541c23568ea47df8d53902a4cbf122f3865476478`  
		Last Modified: Mon, 26 Apr 2021 19:40:22 GMT  
		Size: 120.3 MB (120296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.13`

```console
$ docker pull julia@sha256:36052a38d8ce24173a714e6f45e15217fc5f6db83f6e3362bea1e9b330e602f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:ca3709087833add7942f34806d4ca65ccd2ab5e59126a9c6c4cae85a20fe36e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123108120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e8f10e31159b593f38f63d8737617466ba087325f6a24c7dee6fef1f502de3`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 14 Apr 2021 23:02:59 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:28 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='492514c93c97e7012b8124a959a9f5569231e52b14f992e74a977fffd7b8961b' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 26 Apr 2021 19:38:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f83c49c066b01cd3dbd841541c23568ea47df8d53902a4cbf122f3865476478`  
		Last Modified: Mon, 26 Apr 2021 19:40:22 GMT  
		Size: 120.3 MB (120296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-buster`

```console
$ docker pull julia@sha256:bbd5234fe0bf8904dd3374e84b81f9f14a7e5e754ef7e3c2a0a93edaa259eaac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1-buster` - linux; amd64

```console
$ docker pull julia@sha256:9e0a7e7f671ff4249101208df5150945e3b15d4a712ec068a1ca82afb8e70833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152635667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5406d71f1cccd07971d3759be41a3e4ea3c0f52a740b246d40da57684cfa077`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:08 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 19:38:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc393e77a75f632f581added9733180f506256f659d50247f42862153b44a2d`  
		Last Modified: Mon, 26 Apr 2021 19:39:41 GMT  
		Size: 121.0 MB (121038297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:a03e9e70fd6d73b842cbeca5112acc107bbd4c6fbd63c5b56c708a266224807d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138668730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9dea7467a9211b67e60854de9e2ebd34d257b065ecf56ef47446445fafc80bc`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 20:10:16 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:16:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:16:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacce62cd0061e689b2f6a7abf6ba0372808efc29bf5fcfd302a8e07825dd29`  
		Last Modified: Mon, 10 May 2021 21:17:40 GMT  
		Size: 112.1 MB (112123457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0b1bb0aa54548f67f8027615d6cd9f28629f9428e3d7775b543669d7a63a7370
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145159457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb777f8f3d4ca2313ecc47b6894705e9265ca1410009749d73d7902ab846e46f`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:02:48 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:14:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:14:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42476a9f7e3bcac4810c863cd8d19cf0eb4eb627c0e90c934c09796844599dd`  
		Last Modified: Mon, 10 May 2021 21:15:33 GMT  
		Size: 114.9 MB (114916446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; 386

```console
$ docker pull julia@sha256:03edae6d5bfcebbd136b888b8d94a7fd71fc752db39d60319dbc52c2cf277955
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151020856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779d82018ac27ee00e27417a817b697d39aa87594ab4607303be7416871c7bcb`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 18:54:54 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 18:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 18:55:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcd3467ae1a05da8d7c83b3c276e92778b61d6b90c5913785049f463745b39d`  
		Last Modified: Mon, 26 Apr 2021 18:56:23 GMT  
		Size: 118.6 MB (118621282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:34f2b72bbab5bb60259559e69c3e31a388e502db98d0a360088c271b39a04118
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141797926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142a7fd70412cc059bddf7a9c1b19ae16fce2caa33bf8689e959f3f38171b1fe`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:44:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 14:44:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 14:44:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 21:34:17 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:36:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 21:37:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de5cbe49ae47809605d7676cf919113b9fcd0039eeeb96d8a990491cb6e266e`  
		Last Modified: Sat, 10 Apr 2021 14:47:08 GMT  
		Size: 4.9 MB (4853557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b7e6fa0abc963aba7a4fc0f66f88960593b6afdf11c1a264e40403924f737`  
		Last Modified: Mon, 26 Apr 2021 21:38:02 GMT  
		Size: 106.4 MB (106398436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:3ecf65224dc411f7db10f3a2e8db36c39b9f426df607227cc15b556e6ea95bb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:e75466db30b85df9499b4547b8800e7e7755a324c3ee303f978990c2a83a625e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2607668952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415cc2c3e6325cbf96ebb79033925c33d584618fd11a8b0d73ea7ccbf4f4bd2c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:02:47 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:02:48 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:04:26 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:04:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d62f536b5a512c7dda3dfa351ff2a7113f409efe61f18feebd3fe3739927bc`  
		Last Modified: Mon, 26 Apr 2021 21:08:03 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001c92228b8dfe3a318ea88fa0c4f005aab8ac0bc0a4a7b17daacb3b11a01ea`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a5006275da11a373e2da6e690d7567700b3e040322583e596a2e968e34153`  
		Last Modified: Mon, 26 Apr 2021 21:08:36 GMT  
		Size: 137.9 MB (137909420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d6a3269b15f3d75f3292fcaa599df92e864d530a71ac1d5a0827b4a6120e71`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:7aad9a78ec1bdf5b8abb4347a01c01565fb80df6be36878a82af9ac6c38f7191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `julia:1-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:8c989761b1dc748646817175b7623754f784aaea26070852701f14184040bd6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937855117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261a028fcf019c1cc5a1103c3359767ecff911c002d73e53c132f2e77ce27f84`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:04:45 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:04:46 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:07:09 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:07:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b8ff0cbb14542ed03b2c1fdb5d6e4b1787e9af6ac9a33fb06dbc7b119d9e69`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b526113b3aa441415c74b9d97a76dbb51fc93a620e2cf7d3570565f00da19`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a952cc9a0bfa19a13f0a4e8394c838a67a56d8fe4f61a601f28bb258db138f1`  
		Last Modified: Mon, 26 Apr 2021 21:09:26 GMT  
		Size: 143.0 MB (142965626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b17799f8a1b7ae1f6d125d71b7b27be62cbfc5d3e8d5fb83ebacd72df660fa`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0`

```console
$ docker pull julia@sha256:f20f2d7f981f975531d55ea4996a2aa69d08e89e3a9b666061e84f9dae48a2fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `julia:1.0` - linux; amd64

```console
$ docker pull julia@sha256:e7356fa28d6a4987c58a1f6f7dc440849c266f9851ed4d82c72d7d5f3a5ccd20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127160873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4192a3c04950b2540fec11a7e4f46d7ed5cafa83febbae85735b870b911d1d61`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 06:56:03 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 06:56:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 06:56:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee451d4af2607b4456153f80c701f2b07f6b2fb2e4535f60ec164946959056e3`  
		Last Modified: Sat, 10 Apr 2021 06:59:02 GMT  
		Size: 95.6 MB (95563503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm variant v7

```console
$ docker pull julia@sha256:b7b693f60c5d785a868d16dca933c6ac99b0360fa57b726c357d980533dfb8af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113674320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f140293da2b06b3e5460c1c72efd536d05b5d060e2a59d3ed66b7e51414d88`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 08:55:12 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 08:55:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 08:55:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa554dc4868f92de9c870bb30ba3a5d6438103c7fd39d714385113f85075a4c`  
		Last Modified: Sat, 10 Apr 2021 08:57:37 GMT  
		Size: 87.1 MB (87129047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:04b7bb606de1dc1f5bb6b48bdd089bd14288566aca2472caea620f6351e40bf3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110134162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cd94e1c43336431e3edb09481c9fe0bea378557c1abb6a7f0d07d7e0e8c28ad`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 04:45:30 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 04:45:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 04:45:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a98972b50a270632f45130eaf2a99a8ca57b42592e61c6d1c51e65bc8b3c8b7`  
		Last Modified: Sat, 10 Apr 2021 04:48:22 GMT  
		Size: 79.9 MB (79891151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; 386

```console
$ docker pull julia@sha256:5c51d1c767d30d534240ac82620bbc6f770f0659c5949118e97c09c1ca0c9214
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124898681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c8b41521f9ce8188648d7c9c1ced0704812aacf5c3dce6ff0b037c3caed669`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 15:29:43 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 15:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 15:30:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a76dba200a60a7d2968f11ec92dfc01fe29ff348cbf2e09d95ec5c938ed35d`  
		Last Modified: Sat, 10 Apr 2021 15:32:55 GMT  
		Size: 92.5 MB (92499107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:82d2ae1cd51760ea862bd8eee305e9c7231cfbc535b660463436e59a88cd5485
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572774166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17fe8ceff799289ef3a2ceeca81252224a93120e1e68c03bdc3ad4f53e28bc65`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 15:50:16 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 14 Apr 2021 15:50:17 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 14 Apr 2021 15:52:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Apr 2021 15:52:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b379fdee058a5aa9179d46735bb9d73290d2499b786ab8063381d5f816e2ef26`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a6abc879c6c64433953bbe571693b7f5be337a70b5de6916805cc57a182e68`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb0e571d1600f3adaede46e989f366787363679618538be7faf3dea7190e23c`  
		Last Modified: Wed, 14 Apr 2021 15:59:46 GMT  
		Size: 103.0 MB (103014581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40b8a693ca496d377520699151bb3bba4bcbffff1b1d023b418eedd84d20d72`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:b8b6347c526a55532ca135c5c7cf24aa3c362a21f6b23c25ff8c6460ca856987
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5902979674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e447aea075faae1061db97891dd5a655487db2914a1ba943ab81b355ccc8cf14`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 15:52:14 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 14 Apr 2021 15:52:15 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 14 Apr 2021 15:54:41 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Apr 2021 15:54:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc627fcb8c9e01f8f86383d21dc94c420ac05eb3431ba6b498711359f82f9e4`  
		Last Modified: Wed, 14 Apr 2021 15:59:56 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e084b169dd53aaf422f1ba6f611651235b10e508af06413fe34dcfc80d057f`  
		Last Modified: Wed, 14 Apr 2021 15:59:57 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4323aa0b17e9a9e2455a9fe73125e3d6b9d951efd598de618b76a5af8d7bfd9`  
		Last Modified: Wed, 14 Apr 2021 16:01:56 GMT  
		Size: 108.1 MB (108090124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d275978bd26d80ff9e58c7fd86afdbdbad668cbf576a3d447175a0d04409b495`  
		Last Modified: Wed, 14 Apr 2021 15:59:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-buster`

```console
$ docker pull julia@sha256:9f102c5680e01ea277a2c51fbb96cd1f0b5acd446ebc6fa857c42f35854e04bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:e7356fa28d6a4987c58a1f6f7dc440849c266f9851ed4d82c72d7d5f3a5ccd20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127160873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4192a3c04950b2540fec11a7e4f46d7ed5cafa83febbae85735b870b911d1d61`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 06:56:03 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 06:56:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 06:56:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee451d4af2607b4456153f80c701f2b07f6b2fb2e4535f60ec164946959056e3`  
		Last Modified: Sat, 10 Apr 2021 06:59:02 GMT  
		Size: 95.6 MB (95563503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:b7b693f60c5d785a868d16dca933c6ac99b0360fa57b726c357d980533dfb8af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113674320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f140293da2b06b3e5460c1c72efd536d05b5d060e2a59d3ed66b7e51414d88`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 08:55:12 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 08:55:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 08:55:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa554dc4868f92de9c870bb30ba3a5d6438103c7fd39d714385113f85075a4c`  
		Last Modified: Sat, 10 Apr 2021 08:57:37 GMT  
		Size: 87.1 MB (87129047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:04b7bb606de1dc1f5bb6b48bdd089bd14288566aca2472caea620f6351e40bf3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110134162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cd94e1c43336431e3edb09481c9fe0bea378557c1abb6a7f0d07d7e0e8c28ad`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 04:45:30 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 04:45:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 04:45:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a98972b50a270632f45130eaf2a99a8ca57b42592e61c6d1c51e65bc8b3c8b7`  
		Last Modified: Sat, 10 Apr 2021 04:48:22 GMT  
		Size: 79.9 MB (79891151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; 386

```console
$ docker pull julia@sha256:5c51d1c767d30d534240ac82620bbc6f770f0659c5949118e97c09c1ca0c9214
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124898681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c8b41521f9ce8188648d7c9c1ced0704812aacf5c3dce6ff0b037c3caed669`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 15:29:43 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 15:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 15:30:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a76dba200a60a7d2968f11ec92dfc01fe29ff348cbf2e09d95ec5c938ed35d`  
		Last Modified: Sat, 10 Apr 2021 15:32:55 GMT  
		Size: 92.5 MB (92499107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-stretch`

```console
$ docker pull julia@sha256:1a561d55c022704c54441c9bdd0f4f70fdba0ef365b96723ecd921faee4e64f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-stretch` - linux; amd64

```console
$ docker pull julia@sha256:b7bc060bed0838c22a2407f23d016049af38d1df98b18a2af856cc983b0937eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150445658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16bee941776445f5620265e0c74899c5be987b44ad1aace7e54982fab9cba7a8`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:57:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:57:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:57:03 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:57:03 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 06:57:04 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 06:57:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 06:57:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9817a0383dcc1e6c9dcabd07fd653f1bc8cf5ae5aa6e6f995f3c9944b10072`  
		Last Modified: Sat, 10 Apr 2021 06:59:16 GMT  
		Size: 9.5 MB (9491891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1eaab0bbb8428691964935bbc21efdd26cae8137c57777caae673f7bc562b79`  
		Last Modified: Sat, 10 Apr 2021 06:59:37 GMT  
		Size: 95.6 MB (95573730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:2440654f6965d8cdf3e15891977ffc3d3ea49727462017d7fcc031a200a338fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137464367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b8ec2022ed5088ed98962b636d48fa9801ed23daba2439696703a40407d087`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:02:42 GMT
ADD file:4c101c517b88a8d25a4997ab4d938ea50aaa265c7f88a4e63edaaed37d89a288 in / 
# Sat, 10 Apr 2021 01:02:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:56:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:56:14 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:56:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:56:16 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 08:56:16 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 08:56:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 08:56:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:533b099902e847172558070703785f6c70f0c6912fefcfd283f3b0e3ebc306c5`  
		Last Modified: Sat, 10 Apr 2021 01:10:12 GMT  
		Size: 42.1 MB (42120304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3236614b6770231b3e4d178dba0fbe1b1b9e67f8cb3ace6c99110904677072`  
		Last Modified: Sat, 10 Apr 2021 08:57:45 GMT  
		Size: 8.2 MB (8206321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc039437dff145f61282a1b7c0fd122f75517d6115eda0798c530140f81c50d`  
		Last Modified: Sat, 10 Apr 2021 08:58:12 GMT  
		Size: 87.1 MB (87137742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:78ae5df7a30d43dce65efd0a97e0b6de4bef7d64def6ea3116f66ee2026515ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131538177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b96c8aba8ceb45ddb5ba5276c52bfc49d4e2fd0edbad8bbc71c75de908d1c58`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:43:48 GMT
ADD file:64990d14743657dbcbe885739e43ac964a0239a63e4693e6401b0884ab96e09b in / 
# Sat, 10 Apr 2021 00:43:50 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:46:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:46:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:46:27 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:46:28 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 04:46:29 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 04:46:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 04:46:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:30bd672115ff6f225cb98d2d7f1ed62feb72c2612297b2ac615e762e436c64ec`  
		Last Modified: Sat, 10 Apr 2021 00:49:51 GMT  
		Size: 43.2 MB (43177772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97057139e5283acaafb8f75491790de4bb25aeedba170457e6ddce162bfb8854`  
		Last Modified: Sat, 10 Apr 2021 04:48:31 GMT  
		Size: 8.5 MB (8451279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fedd46f41add1b8d01d4d6a58cd64c4692eded6146da1868862ab94b92b277`  
		Last Modified: Sat, 10 Apr 2021 04:48:57 GMT  
		Size: 79.9 MB (79909126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; 386

```console
$ docker pull julia@sha256:f89cc0a87c27c3676879adb66f2e2b8d8059c28532fac7f023d22b135eb4fd94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148093960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79678704daf76040195474cd181d60d6ffaedf07861edc8f67c9c0f43d309602`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:14 GMT
ADD file:cebeeb1ed904e9433778c60c09ed31939334fd4f1c9550cce191b3bff4df0272 in / 
# Sat, 10 Apr 2021 00:41:14 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:30:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:30:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:30:17 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:30:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 15:30:17 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 15:30:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 15:30:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f8270215e0f4bee2960e85333265840385530ee75e6f553f8cfc3e5b0534bf0e`  
		Last Modified: Sat, 10 Apr 2021 00:48:47 GMT  
		Size: 46.1 MB (46098724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce70ef388d53064dd5ac189f0b483a807420ac35a313065e3ca18ffd85ee7b`  
		Last Modified: Sat, 10 Apr 2021 15:33:14 GMT  
		Size: 9.5 MB (9493333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5665e375e21cd9ae3261b08d73be71330fdec65d9152464482642b5b676eab`  
		Last Modified: Sat, 10 Apr 2021 15:33:42 GMT  
		Size: 92.5 MB (92501903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:5bfe6f9401a1126200bdfd419841beb466b9ba6fd8e8f359a8f188559008d20a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `julia:1.0-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:82d2ae1cd51760ea862bd8eee305e9c7231cfbc535b660463436e59a88cd5485
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572774166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17fe8ceff799289ef3a2ceeca81252224a93120e1e68c03bdc3ad4f53e28bc65`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 15:50:16 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 14 Apr 2021 15:50:17 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 14 Apr 2021 15:52:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Apr 2021 15:52:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b379fdee058a5aa9179d46735bb9d73290d2499b786ab8063381d5f816e2ef26`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a6abc879c6c64433953bbe571693b7f5be337a70b5de6916805cc57a182e68`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb0e571d1600f3adaede46e989f366787363679618538be7faf3dea7190e23c`  
		Last Modified: Wed, 14 Apr 2021 15:59:46 GMT  
		Size: 103.0 MB (103014581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40b8a693ca496d377520699151bb3bba4bcbffff1b1d023b418eedd84d20d72`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:fb23b0037012a52e8be649c28834ee043fc35836889e76fa9ca9b46a39d90e7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `julia:1.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:b8b6347c526a55532ca135c5c7cf24aa3c362a21f6b23c25ff8c6460ca856987
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5902979674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e447aea075faae1061db97891dd5a655487db2914a1ba943ab81b355ccc8cf14`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 15:52:14 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 14 Apr 2021 15:52:15 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 14 Apr 2021 15:54:41 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Apr 2021 15:54:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc627fcb8c9e01f8f86383d21dc94c420ac05eb3431ba6b498711359f82f9e4`  
		Last Modified: Wed, 14 Apr 2021 15:59:56 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e084b169dd53aaf422f1ba6f611651235b10e508af06413fe34dcfc80d057f`  
		Last Modified: Wed, 14 Apr 2021 15:59:57 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4323aa0b17e9a9e2455a9fe73125e3d6b9d951efd598de618b76a5af8d7bfd9`  
		Last Modified: Wed, 14 Apr 2021 16:01:56 GMT  
		Size: 108.1 MB (108090124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d275978bd26d80ff9e58c7fd86afdbdbad668cbf576a3d447175a0d04409b495`  
		Last Modified: Wed, 14 Apr 2021 15:59:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5`

```console
$ docker pull julia@sha256:f20f2d7f981f975531d55ea4996a2aa69d08e89e3a9b666061e84f9dae48a2fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `julia:1.0.5` - linux; amd64

```console
$ docker pull julia@sha256:e7356fa28d6a4987c58a1f6f7dc440849c266f9851ed4d82c72d7d5f3a5ccd20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127160873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4192a3c04950b2540fec11a7e4f46d7ed5cafa83febbae85735b870b911d1d61`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 06:56:03 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 06:56:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 06:56:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee451d4af2607b4456153f80c701f2b07f6b2fb2e4535f60ec164946959056e3`  
		Last Modified: Sat, 10 Apr 2021 06:59:02 GMT  
		Size: 95.6 MB (95563503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm variant v7

```console
$ docker pull julia@sha256:b7b693f60c5d785a868d16dca933c6ac99b0360fa57b726c357d980533dfb8af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113674320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f140293da2b06b3e5460c1c72efd536d05b5d060e2a59d3ed66b7e51414d88`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 08:55:12 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 08:55:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 08:55:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa554dc4868f92de9c870bb30ba3a5d6438103c7fd39d714385113f85075a4c`  
		Last Modified: Sat, 10 Apr 2021 08:57:37 GMT  
		Size: 87.1 MB (87129047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:04b7bb606de1dc1f5bb6b48bdd089bd14288566aca2472caea620f6351e40bf3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110134162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cd94e1c43336431e3edb09481c9fe0bea378557c1abb6a7f0d07d7e0e8c28ad`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 04:45:30 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 04:45:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 04:45:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a98972b50a270632f45130eaf2a99a8ca57b42592e61c6d1c51e65bc8b3c8b7`  
		Last Modified: Sat, 10 Apr 2021 04:48:22 GMT  
		Size: 79.9 MB (79891151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; 386

```console
$ docker pull julia@sha256:5c51d1c767d30d534240ac82620bbc6f770f0659c5949118e97c09c1ca0c9214
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124898681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c8b41521f9ce8188648d7c9c1ced0704812aacf5c3dce6ff0b037c3caed669`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 15:29:43 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 15:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 15:30:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a76dba200a60a7d2968f11ec92dfc01fe29ff348cbf2e09d95ec5c938ed35d`  
		Last Modified: Sat, 10 Apr 2021 15:32:55 GMT  
		Size: 92.5 MB (92499107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:82d2ae1cd51760ea862bd8eee305e9c7231cfbc535b660463436e59a88cd5485
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572774166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17fe8ceff799289ef3a2ceeca81252224a93120e1e68c03bdc3ad4f53e28bc65`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 15:50:16 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 14 Apr 2021 15:50:17 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 14 Apr 2021 15:52:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Apr 2021 15:52:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b379fdee058a5aa9179d46735bb9d73290d2499b786ab8063381d5f816e2ef26`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a6abc879c6c64433953bbe571693b7f5be337a70b5de6916805cc57a182e68`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb0e571d1600f3adaede46e989f366787363679618538be7faf3dea7190e23c`  
		Last Modified: Wed, 14 Apr 2021 15:59:46 GMT  
		Size: 103.0 MB (103014581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40b8a693ca496d377520699151bb3bba4bcbffff1b1d023b418eedd84d20d72`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:b8b6347c526a55532ca135c5c7cf24aa3c362a21f6b23c25ff8c6460ca856987
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5902979674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e447aea075faae1061db97891dd5a655487db2914a1ba943ab81b355ccc8cf14`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 15:52:14 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 14 Apr 2021 15:52:15 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 14 Apr 2021 15:54:41 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Apr 2021 15:54:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc627fcb8c9e01f8f86383d21dc94c420ac05eb3431ba6b498711359f82f9e4`  
		Last Modified: Wed, 14 Apr 2021 15:59:56 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e084b169dd53aaf422f1ba6f611651235b10e508af06413fe34dcfc80d057f`  
		Last Modified: Wed, 14 Apr 2021 15:59:57 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4323aa0b17e9a9e2455a9fe73125e3d6b9d951efd598de618b76a5af8d7bfd9`  
		Last Modified: Wed, 14 Apr 2021 16:01:56 GMT  
		Size: 108.1 MB (108090124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d275978bd26d80ff9e58c7fd86afdbdbad668cbf576a3d447175a0d04409b495`  
		Last Modified: Wed, 14 Apr 2021 15:59:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-buster`

```console
$ docker pull julia@sha256:9f102c5680e01ea277a2c51fbb96cd1f0b5acd446ebc6fa857c42f35854e04bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-buster` - linux; amd64

```console
$ docker pull julia@sha256:e7356fa28d6a4987c58a1f6f7dc440849c266f9851ed4d82c72d7d5f3a5ccd20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127160873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4192a3c04950b2540fec11a7e4f46d7ed5cafa83febbae85735b870b911d1d61`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 06:56:03 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 06:56:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 06:56:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee451d4af2607b4456153f80c701f2b07f6b2fb2e4535f60ec164946959056e3`  
		Last Modified: Sat, 10 Apr 2021 06:59:02 GMT  
		Size: 95.6 MB (95563503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:b7b693f60c5d785a868d16dca933c6ac99b0360fa57b726c357d980533dfb8af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113674320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f140293da2b06b3e5460c1c72efd536d05b5d060e2a59d3ed66b7e51414d88`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 08:55:12 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 08:55:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 08:55:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa554dc4868f92de9c870bb30ba3a5d6438103c7fd39d714385113f85075a4c`  
		Last Modified: Sat, 10 Apr 2021 08:57:37 GMT  
		Size: 87.1 MB (87129047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:04b7bb606de1dc1f5bb6b48bdd089bd14288566aca2472caea620f6351e40bf3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110134162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cd94e1c43336431e3edb09481c9fe0bea378557c1abb6a7f0d07d7e0e8c28ad`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 04:45:30 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 04:45:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 04:45:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a98972b50a270632f45130eaf2a99a8ca57b42592e61c6d1c51e65bc8b3c8b7`  
		Last Modified: Sat, 10 Apr 2021 04:48:22 GMT  
		Size: 79.9 MB (79891151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; 386

```console
$ docker pull julia@sha256:5c51d1c767d30d534240ac82620bbc6f770f0659c5949118e97c09c1ca0c9214
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124898681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c8b41521f9ce8188648d7c9c1ced0704812aacf5c3dce6ff0b037c3caed669`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 15:29:43 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 15:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 15:30:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a76dba200a60a7d2968f11ec92dfc01fe29ff348cbf2e09d95ec5c938ed35d`  
		Last Modified: Sat, 10 Apr 2021 15:32:55 GMT  
		Size: 92.5 MB (92499107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-stretch`

```console
$ docker pull julia@sha256:1a561d55c022704c54441c9bdd0f4f70fdba0ef365b96723ecd921faee4e64f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-stretch` - linux; amd64

```console
$ docker pull julia@sha256:b7bc060bed0838c22a2407f23d016049af38d1df98b18a2af856cc983b0937eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150445658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16bee941776445f5620265e0c74899c5be987b44ad1aace7e54982fab9cba7a8`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:57:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:57:03 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:57:03 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:57:03 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 06:57:04 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 06:57:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 06:57:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9817a0383dcc1e6c9dcabd07fd653f1bc8cf5ae5aa6e6f995f3c9944b10072`  
		Last Modified: Sat, 10 Apr 2021 06:59:16 GMT  
		Size: 9.5 MB (9491891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1eaab0bbb8428691964935bbc21efdd26cae8137c57777caae673f7bc562b79`  
		Last Modified: Sat, 10 Apr 2021 06:59:37 GMT  
		Size: 95.6 MB (95573730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:2440654f6965d8cdf3e15891977ffc3d3ea49727462017d7fcc031a200a338fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137464367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b8ec2022ed5088ed98962b636d48fa9801ed23daba2439696703a40407d087`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:02:42 GMT
ADD file:4c101c517b88a8d25a4997ab4d938ea50aaa265c7f88a4e63edaaed37d89a288 in / 
# Sat, 10 Apr 2021 01:02:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:56:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:56:14 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:56:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:56:16 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 08:56:16 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 08:56:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 08:56:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:533b099902e847172558070703785f6c70f0c6912fefcfd283f3b0e3ebc306c5`  
		Last Modified: Sat, 10 Apr 2021 01:10:12 GMT  
		Size: 42.1 MB (42120304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3236614b6770231b3e4d178dba0fbe1b1b9e67f8cb3ace6c99110904677072`  
		Last Modified: Sat, 10 Apr 2021 08:57:45 GMT  
		Size: 8.2 MB (8206321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc039437dff145f61282a1b7c0fd122f75517d6115eda0798c530140f81c50d`  
		Last Modified: Sat, 10 Apr 2021 08:58:12 GMT  
		Size: 87.1 MB (87137742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:78ae5df7a30d43dce65efd0a97e0b6de4bef7d64def6ea3116f66ee2026515ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131538177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b96c8aba8ceb45ddb5ba5276c52bfc49d4e2fd0edbad8bbc71c75de908d1c58`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:43:48 GMT
ADD file:64990d14743657dbcbe885739e43ac964a0239a63e4693e6401b0884ab96e09b in / 
# Sat, 10 Apr 2021 00:43:50 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:46:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:46:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:46:27 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:46:28 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 04:46:29 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 04:46:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 04:46:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:30bd672115ff6f225cb98d2d7f1ed62feb72c2612297b2ac615e762e436c64ec`  
		Last Modified: Sat, 10 Apr 2021 00:49:51 GMT  
		Size: 43.2 MB (43177772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97057139e5283acaafb8f75491790de4bb25aeedba170457e6ddce162bfb8854`  
		Last Modified: Sat, 10 Apr 2021 04:48:31 GMT  
		Size: 8.5 MB (8451279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fedd46f41add1b8d01d4d6a58cd64c4692eded6146da1868862ab94b92b277`  
		Last Modified: Sat, 10 Apr 2021 04:48:57 GMT  
		Size: 79.9 MB (79909126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; 386

```console
$ docker pull julia@sha256:f89cc0a87c27c3676879adb66f2e2b8d8059c28532fac7f023d22b135eb4fd94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148093960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79678704daf76040195474cd181d60d6ffaedf07861edc8f67c9c0f43d309602`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:14 GMT
ADD file:cebeeb1ed904e9433778c60c09ed31939334fd4f1c9550cce191b3bff4df0272 in / 
# Sat, 10 Apr 2021 00:41:14 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:30:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:30:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:30:17 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:30:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 10 Apr 2021 15:30:17 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 10 Apr 2021 15:30:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 10 Apr 2021 15:30:38 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f8270215e0f4bee2960e85333265840385530ee75e6f553f8cfc3e5b0534bf0e`  
		Last Modified: Sat, 10 Apr 2021 00:48:47 GMT  
		Size: 46.1 MB (46098724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce70ef388d53064dd5ac189f0b483a807420ac35a313065e3ca18ffd85ee7b`  
		Last Modified: Sat, 10 Apr 2021 15:33:14 GMT  
		Size: 9.5 MB (9493333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5665e375e21cd9ae3261b08d73be71330fdec65d9152464482642b5b676eab`  
		Last Modified: Sat, 10 Apr 2021 15:33:42 GMT  
		Size: 92.5 MB (92501903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-1809`

```console
$ docker pull julia@sha256:5bfe6f9401a1126200bdfd419841beb466b9ba6fd8e8f359a8f188559008d20a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `julia:1.0.5-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:82d2ae1cd51760ea862bd8eee305e9c7231cfbc535b660463436e59a88cd5485
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2572774166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17fe8ceff799289ef3a2ceeca81252224a93120e1e68c03bdc3ad4f53e28bc65`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 15:50:16 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 14 Apr 2021 15:50:17 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 14 Apr 2021 15:52:05 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Apr 2021 15:52:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b379fdee058a5aa9179d46735bb9d73290d2499b786ab8063381d5f816e2ef26`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a6abc879c6c64433953bbe571693b7f5be337a70b5de6916805cc57a182e68`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb0e571d1600f3adaede46e989f366787363679618538be7faf3dea7190e23c`  
		Last Modified: Wed, 14 Apr 2021 15:59:46 GMT  
		Size: 103.0 MB (103014581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40b8a693ca496d377520699151bb3bba4bcbffff1b1d023b418eedd84d20d72`  
		Last Modified: Wed, 14 Apr 2021 15:59:22 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:fb23b0037012a52e8be649c28834ee043fc35836889e76fa9ca9b46a39d90e7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `julia:1.0.5-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:b8b6347c526a55532ca135c5c7cf24aa3c362a21f6b23c25ff8c6460ca856987
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5902979674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e447aea075faae1061db97891dd5a655487db2914a1ba943ab81b355ccc8cf14`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 15:52:14 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 14 Apr 2021 15:52:15 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 14 Apr 2021 15:54:41 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Apr 2021 15:54:43 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc627fcb8c9e01f8f86383d21dc94c420ac05eb3431ba6b498711359f82f9e4`  
		Last Modified: Wed, 14 Apr 2021 15:59:56 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e084b169dd53aaf422f1ba6f611651235b10e508af06413fe34dcfc80d057f`  
		Last Modified: Wed, 14 Apr 2021 15:59:57 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4323aa0b17e9a9e2455a9fe73125e3d6b9d951efd598de618b76a5af8d7bfd9`  
		Last Modified: Wed, 14 Apr 2021 16:01:56 GMT  
		Size: 108.1 MB (108090124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d275978bd26d80ff9e58c7fd86afdbdbad668cbf576a3d447175a0d04409b495`  
		Last Modified: Wed, 14 Apr 2021 15:59:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6`

```console
$ docker pull julia@sha256:ce3a3fe709ac7e242b4d8fd081a13f1e7cd160f7cabb592b9552bf563fa8f5a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `julia:1.6` - linux; amd64

```console
$ docker pull julia@sha256:9e0a7e7f671ff4249101208df5150945e3b15d4a712ec068a1ca82afb8e70833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152635667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5406d71f1cccd07971d3759be41a3e4ea3c0f52a740b246d40da57684cfa077`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:08 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 19:38:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc393e77a75f632f581added9733180f506256f659d50247f42862153b44a2d`  
		Last Modified: Mon, 26 Apr 2021 19:39:41 GMT  
		Size: 121.0 MB (121038297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm variant v7

```console
$ docker pull julia@sha256:a03e9e70fd6d73b842cbeca5112acc107bbd4c6fbd63c5b56c708a266224807d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138668730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9dea7467a9211b67e60854de9e2ebd34d257b065ecf56ef47446445fafc80bc`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 20:10:16 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:16:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:16:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacce62cd0061e689b2f6a7abf6ba0372808efc29bf5fcfd302a8e07825dd29`  
		Last Modified: Mon, 10 May 2021 21:17:40 GMT  
		Size: 112.1 MB (112123457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0b1bb0aa54548f67f8027615d6cd9f28629f9428e3d7775b543669d7a63a7370
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145159457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb777f8f3d4ca2313ecc47b6894705e9265ca1410009749d73d7902ab846e46f`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:02:48 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:14:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:14:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42476a9f7e3bcac4810c863cd8d19cf0eb4eb627c0e90c934c09796844599dd`  
		Last Modified: Mon, 10 May 2021 21:15:33 GMT  
		Size: 114.9 MB (114916446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; 386

```console
$ docker pull julia@sha256:03edae6d5bfcebbd136b888b8d94a7fd71fc752db39d60319dbc52c2cf277955
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151020856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779d82018ac27ee00e27417a817b697d39aa87594ab4607303be7416871c7bcb`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 18:54:54 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 18:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 18:55:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcd3467ae1a05da8d7c83b3c276e92778b61d6b90c5913785049f463745b39d`  
		Last Modified: Mon, 26 Apr 2021 18:56:23 GMT  
		Size: 118.6 MB (118621282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; ppc64le

```console
$ docker pull julia@sha256:34f2b72bbab5bb60259559e69c3e31a388e502db98d0a360088c271b39a04118
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141797926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142a7fd70412cc059bddf7a9c1b19ae16fce2caa33bf8689e959f3f38171b1fe`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:44:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 14:44:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 14:44:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 21:34:17 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:36:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 21:37:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de5cbe49ae47809605d7676cf919113b9fcd0039eeeb96d8a990491cb6e266e`  
		Last Modified: Sat, 10 Apr 2021 14:47:08 GMT  
		Size: 4.9 MB (4853557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b7e6fa0abc963aba7a4fc0f66f88960593b6afdf11c1a264e40403924f737`  
		Last Modified: Mon, 26 Apr 2021 21:38:02 GMT  
		Size: 106.4 MB (106398436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:e75466db30b85df9499b4547b8800e7e7755a324c3ee303f978990c2a83a625e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2607668952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415cc2c3e6325cbf96ebb79033925c33d584618fd11a8b0d73ea7ccbf4f4bd2c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:02:47 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:02:48 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:04:26 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:04:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d62f536b5a512c7dda3dfa351ff2a7113f409efe61f18feebd3fe3739927bc`  
		Last Modified: Mon, 26 Apr 2021 21:08:03 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001c92228b8dfe3a318ea88fa0c4f005aab8ac0bc0a4a7b17daacb3b11a01ea`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a5006275da11a373e2da6e690d7567700b3e040322583e596a2e968e34153`  
		Last Modified: Mon, 26 Apr 2021 21:08:36 GMT  
		Size: 137.9 MB (137909420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d6a3269b15f3d75f3292fcaa599df92e864d530a71ac1d5a0827b4a6120e71`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:8c989761b1dc748646817175b7623754f784aaea26070852701f14184040bd6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937855117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261a028fcf019c1cc5a1103c3359767ecff911c002d73e53c132f2e77ce27f84`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:04:45 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:04:46 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:07:09 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:07:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b8ff0cbb14542ed03b2c1fdb5d6e4b1787e9af6ac9a33fb06dbc7b119d9e69`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b526113b3aa441415c74b9d97a76dbb51fc93a620e2cf7d3570565f00da19`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a952cc9a0bfa19a13f0a4e8394c838a67a56d8fe4f61a601f28bb258db138f1`  
		Last Modified: Mon, 26 Apr 2021 21:09:26 GMT  
		Size: 143.0 MB (142965626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b17799f8a1b7ae1f6d125d71b7b27be62cbfc5d3e8d5fb83ebacd72df660fa`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine`

```console
$ docker pull julia@sha256:36052a38d8ce24173a714e6f45e15217fc5f6db83f6e3362bea1e9b330e602f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.6-alpine` - linux; amd64

```console
$ docker pull julia@sha256:ca3709087833add7942f34806d4ca65ccd2ab5e59126a9c6c4cae85a20fe36e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123108120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e8f10e31159b593f38f63d8737617466ba087325f6a24c7dee6fef1f502de3`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 14 Apr 2021 23:02:59 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:28 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='492514c93c97e7012b8124a959a9f5569231e52b14f992e74a977fffd7b8961b' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 26 Apr 2021 19:38:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f83c49c066b01cd3dbd841541c23568ea47df8d53902a4cbf122f3865476478`  
		Last Modified: Mon, 26 Apr 2021 19:40:22 GMT  
		Size: 120.3 MB (120296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine3.13`

```console
$ docker pull julia@sha256:36052a38d8ce24173a714e6f45e15217fc5f6db83f6e3362bea1e9b330e602f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.6-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:ca3709087833add7942f34806d4ca65ccd2ab5e59126a9c6c4cae85a20fe36e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123108120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e8f10e31159b593f38f63d8737617466ba087325f6a24c7dee6fef1f502de3`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 14 Apr 2021 23:02:59 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:28 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='492514c93c97e7012b8124a959a9f5569231e52b14f992e74a977fffd7b8961b' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 26 Apr 2021 19:38:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f83c49c066b01cd3dbd841541c23568ea47df8d53902a4cbf122f3865476478`  
		Last Modified: Mon, 26 Apr 2021 19:40:22 GMT  
		Size: 120.3 MB (120296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-buster`

```console
$ docker pull julia@sha256:bbd5234fe0bf8904dd3374e84b81f9f14a7e5e754ef7e3c2a0a93edaa259eaac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6-buster` - linux; amd64

```console
$ docker pull julia@sha256:9e0a7e7f671ff4249101208df5150945e3b15d4a712ec068a1ca82afb8e70833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152635667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5406d71f1cccd07971d3759be41a3e4ea3c0f52a740b246d40da57684cfa077`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:08 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 19:38:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc393e77a75f632f581added9733180f506256f659d50247f42862153b44a2d`  
		Last Modified: Mon, 26 Apr 2021 19:39:41 GMT  
		Size: 121.0 MB (121038297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:a03e9e70fd6d73b842cbeca5112acc107bbd4c6fbd63c5b56c708a266224807d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138668730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9dea7467a9211b67e60854de9e2ebd34d257b065ecf56ef47446445fafc80bc`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 20:10:16 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:16:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:16:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacce62cd0061e689b2f6a7abf6ba0372808efc29bf5fcfd302a8e07825dd29`  
		Last Modified: Mon, 10 May 2021 21:17:40 GMT  
		Size: 112.1 MB (112123457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0b1bb0aa54548f67f8027615d6cd9f28629f9428e3d7775b543669d7a63a7370
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145159457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb777f8f3d4ca2313ecc47b6894705e9265ca1410009749d73d7902ab846e46f`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:02:48 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:14:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:14:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42476a9f7e3bcac4810c863cd8d19cf0eb4eb627c0e90c934c09796844599dd`  
		Last Modified: Mon, 10 May 2021 21:15:33 GMT  
		Size: 114.9 MB (114916446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; 386

```console
$ docker pull julia@sha256:03edae6d5bfcebbd136b888b8d94a7fd71fc752db39d60319dbc52c2cf277955
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151020856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779d82018ac27ee00e27417a817b697d39aa87594ab4607303be7416871c7bcb`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 18:54:54 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 18:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 18:55:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcd3467ae1a05da8d7c83b3c276e92778b61d6b90c5913785049f463745b39d`  
		Last Modified: Mon, 26 Apr 2021 18:56:23 GMT  
		Size: 118.6 MB (118621282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:34f2b72bbab5bb60259559e69c3e31a388e502db98d0a360088c271b39a04118
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141797926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142a7fd70412cc059bddf7a9c1b19ae16fce2caa33bf8689e959f3f38171b1fe`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:44:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 14:44:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 14:44:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 21:34:17 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:36:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 21:37:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de5cbe49ae47809605d7676cf919113b9fcd0039eeeb96d8a990491cb6e266e`  
		Last Modified: Sat, 10 Apr 2021 14:47:08 GMT  
		Size: 4.9 MB (4853557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b7e6fa0abc963aba7a4fc0f66f88960593b6afdf11c1a264e40403924f737`  
		Last Modified: Mon, 26 Apr 2021 21:38:02 GMT  
		Size: 106.4 MB (106398436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-1809`

```console
$ docker pull julia@sha256:3ecf65224dc411f7db10f3a2e8db36c39b9f426df607227cc15b556e6ea95bb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `julia:1.6-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:e75466db30b85df9499b4547b8800e7e7755a324c3ee303f978990c2a83a625e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2607668952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415cc2c3e6325cbf96ebb79033925c33d584618fd11a8b0d73ea7ccbf4f4bd2c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:02:47 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:02:48 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:04:26 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:04:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d62f536b5a512c7dda3dfa351ff2a7113f409efe61f18feebd3fe3739927bc`  
		Last Modified: Mon, 26 Apr 2021 21:08:03 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001c92228b8dfe3a318ea88fa0c4f005aab8ac0bc0a4a7b17daacb3b11a01ea`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a5006275da11a373e2da6e690d7567700b3e040322583e596a2e968e34153`  
		Last Modified: Mon, 26 Apr 2021 21:08:36 GMT  
		Size: 137.9 MB (137909420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d6a3269b15f3d75f3292fcaa599df92e864d530a71ac1d5a0827b4a6120e71`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:7aad9a78ec1bdf5b8abb4347a01c01565fb80df6be36878a82af9ac6c38f7191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `julia:1.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:8c989761b1dc748646817175b7623754f784aaea26070852701f14184040bd6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937855117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261a028fcf019c1cc5a1103c3359767ecff911c002d73e53c132f2e77ce27f84`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:04:45 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:04:46 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:07:09 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:07:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b8ff0cbb14542ed03b2c1fdb5d6e4b1787e9af6ac9a33fb06dbc7b119d9e69`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b526113b3aa441415c74b9d97a76dbb51fc93a620e2cf7d3570565f00da19`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a952cc9a0bfa19a13f0a4e8394c838a67a56d8fe4f61a601f28bb258db138f1`  
		Last Modified: Mon, 26 Apr 2021 21:09:26 GMT  
		Size: 143.0 MB (142965626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b17799f8a1b7ae1f6d125d71b7b27be62cbfc5d3e8d5fb83ebacd72df660fa`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.1`

```console
$ docker pull julia@sha256:ce3a3fe709ac7e242b4d8fd081a13f1e7cd160f7cabb592b9552bf563fa8f5a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `julia:1.6.1` - linux; amd64

```console
$ docker pull julia@sha256:9e0a7e7f671ff4249101208df5150945e3b15d4a712ec068a1ca82afb8e70833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152635667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5406d71f1cccd07971d3759be41a3e4ea3c0f52a740b246d40da57684cfa077`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:08 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 19:38:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc393e77a75f632f581added9733180f506256f659d50247f42862153b44a2d`  
		Last Modified: Mon, 26 Apr 2021 19:39:41 GMT  
		Size: 121.0 MB (121038297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1` - linux; arm variant v7

```console
$ docker pull julia@sha256:a03e9e70fd6d73b842cbeca5112acc107bbd4c6fbd63c5b56c708a266224807d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138668730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9dea7467a9211b67e60854de9e2ebd34d257b065ecf56ef47446445fafc80bc`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 20:10:16 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:16:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:16:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacce62cd0061e689b2f6a7abf6ba0372808efc29bf5fcfd302a8e07825dd29`  
		Last Modified: Mon, 10 May 2021 21:17:40 GMT  
		Size: 112.1 MB (112123457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0b1bb0aa54548f67f8027615d6cd9f28629f9428e3d7775b543669d7a63a7370
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145159457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb777f8f3d4ca2313ecc47b6894705e9265ca1410009749d73d7902ab846e46f`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:02:48 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:14:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:14:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42476a9f7e3bcac4810c863cd8d19cf0eb4eb627c0e90c934c09796844599dd`  
		Last Modified: Mon, 10 May 2021 21:15:33 GMT  
		Size: 114.9 MB (114916446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1` - linux; 386

```console
$ docker pull julia@sha256:03edae6d5bfcebbd136b888b8d94a7fd71fc752db39d60319dbc52c2cf277955
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151020856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779d82018ac27ee00e27417a817b697d39aa87594ab4607303be7416871c7bcb`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 18:54:54 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 18:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 18:55:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcd3467ae1a05da8d7c83b3c276e92778b61d6b90c5913785049f463745b39d`  
		Last Modified: Mon, 26 Apr 2021 18:56:23 GMT  
		Size: 118.6 MB (118621282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1` - linux; ppc64le

```console
$ docker pull julia@sha256:34f2b72bbab5bb60259559e69c3e31a388e502db98d0a360088c271b39a04118
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141797926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142a7fd70412cc059bddf7a9c1b19ae16fce2caa33bf8689e959f3f38171b1fe`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:44:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 14:44:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 14:44:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 21:34:17 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:36:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 21:37:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de5cbe49ae47809605d7676cf919113b9fcd0039eeeb96d8a990491cb6e266e`  
		Last Modified: Sat, 10 Apr 2021 14:47:08 GMT  
		Size: 4.9 MB (4853557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b7e6fa0abc963aba7a4fc0f66f88960593b6afdf11c1a264e40403924f737`  
		Last Modified: Mon, 26 Apr 2021 21:38:02 GMT  
		Size: 106.4 MB (106398436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:e75466db30b85df9499b4547b8800e7e7755a324c3ee303f978990c2a83a625e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2607668952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415cc2c3e6325cbf96ebb79033925c33d584618fd11a8b0d73ea7ccbf4f4bd2c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:02:47 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:02:48 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:04:26 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:04:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d62f536b5a512c7dda3dfa351ff2a7113f409efe61f18feebd3fe3739927bc`  
		Last Modified: Mon, 26 Apr 2021 21:08:03 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001c92228b8dfe3a318ea88fa0c4f005aab8ac0bc0a4a7b17daacb3b11a01ea`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a5006275da11a373e2da6e690d7567700b3e040322583e596a2e968e34153`  
		Last Modified: Mon, 26 Apr 2021 21:08:36 GMT  
		Size: 137.9 MB (137909420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d6a3269b15f3d75f3292fcaa599df92e864d530a71ac1d5a0827b4a6120e71`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:8c989761b1dc748646817175b7623754f784aaea26070852701f14184040bd6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937855117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261a028fcf019c1cc5a1103c3359767ecff911c002d73e53c132f2e77ce27f84`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:04:45 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:04:46 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:07:09 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:07:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b8ff0cbb14542ed03b2c1fdb5d6e4b1787e9af6ac9a33fb06dbc7b119d9e69`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b526113b3aa441415c74b9d97a76dbb51fc93a620e2cf7d3570565f00da19`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a952cc9a0bfa19a13f0a4e8394c838a67a56d8fe4f61a601f28bb258db138f1`  
		Last Modified: Mon, 26 Apr 2021 21:09:26 GMT  
		Size: 143.0 MB (142965626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b17799f8a1b7ae1f6d125d71b7b27be62cbfc5d3e8d5fb83ebacd72df660fa`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.1-alpine`

```console
$ docker pull julia@sha256:36052a38d8ce24173a714e6f45e15217fc5f6db83f6e3362bea1e9b330e602f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.6.1-alpine` - linux; amd64

```console
$ docker pull julia@sha256:ca3709087833add7942f34806d4ca65ccd2ab5e59126a9c6c4cae85a20fe36e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123108120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e8f10e31159b593f38f63d8737617466ba087325f6a24c7dee6fef1f502de3`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 14 Apr 2021 23:02:59 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:28 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='492514c93c97e7012b8124a959a9f5569231e52b14f992e74a977fffd7b8961b' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 26 Apr 2021 19:38:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f83c49c066b01cd3dbd841541c23568ea47df8d53902a4cbf122f3865476478`  
		Last Modified: Mon, 26 Apr 2021 19:40:22 GMT  
		Size: 120.3 MB (120296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.1-alpine3.13`

```console
$ docker pull julia@sha256:36052a38d8ce24173a714e6f45e15217fc5f6db83f6e3362bea1e9b330e602f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1.6.1-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:ca3709087833add7942f34806d4ca65ccd2ab5e59126a9c6c4cae85a20fe36e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123108120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e8f10e31159b593f38f63d8737617466ba087325f6a24c7dee6fef1f502de3`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 14 Apr 2021 23:02:59 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:28 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='492514c93c97e7012b8124a959a9f5569231e52b14f992e74a977fffd7b8961b' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 26 Apr 2021 19:38:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f83c49c066b01cd3dbd841541c23568ea47df8d53902a4cbf122f3865476478`  
		Last Modified: Mon, 26 Apr 2021 19:40:22 GMT  
		Size: 120.3 MB (120296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.1-buster`

```console
$ docker pull julia@sha256:bbd5234fe0bf8904dd3374e84b81f9f14a7e5e754ef7e3c2a0a93edaa259eaac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6.1-buster` - linux; amd64

```console
$ docker pull julia@sha256:9e0a7e7f671ff4249101208df5150945e3b15d4a712ec068a1ca82afb8e70833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152635667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5406d71f1cccd07971d3759be41a3e4ea3c0f52a740b246d40da57684cfa077`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:08 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 19:38:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc393e77a75f632f581added9733180f506256f659d50247f42862153b44a2d`  
		Last Modified: Mon, 26 Apr 2021 19:39:41 GMT  
		Size: 121.0 MB (121038297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:a03e9e70fd6d73b842cbeca5112acc107bbd4c6fbd63c5b56c708a266224807d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138668730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9dea7467a9211b67e60854de9e2ebd34d257b065ecf56ef47446445fafc80bc`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 20:10:16 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:16:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:16:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacce62cd0061e689b2f6a7abf6ba0372808efc29bf5fcfd302a8e07825dd29`  
		Last Modified: Mon, 10 May 2021 21:17:40 GMT  
		Size: 112.1 MB (112123457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0b1bb0aa54548f67f8027615d6cd9f28629f9428e3d7775b543669d7a63a7370
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145159457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb777f8f3d4ca2313ecc47b6894705e9265ca1410009749d73d7902ab846e46f`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:02:48 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:14:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:14:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42476a9f7e3bcac4810c863cd8d19cf0eb4eb627c0e90c934c09796844599dd`  
		Last Modified: Mon, 10 May 2021 21:15:33 GMT  
		Size: 114.9 MB (114916446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1-buster` - linux; 386

```console
$ docker pull julia@sha256:03edae6d5bfcebbd136b888b8d94a7fd71fc752db39d60319dbc52c2cf277955
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151020856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779d82018ac27ee00e27417a817b697d39aa87594ab4607303be7416871c7bcb`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 18:54:54 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 18:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 18:55:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcd3467ae1a05da8d7c83b3c276e92778b61d6b90c5913785049f463745b39d`  
		Last Modified: Mon, 26 Apr 2021 18:56:23 GMT  
		Size: 118.6 MB (118621282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:34f2b72bbab5bb60259559e69c3e31a388e502db98d0a360088c271b39a04118
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141797926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142a7fd70412cc059bddf7a9c1b19ae16fce2caa33bf8689e959f3f38171b1fe`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:44:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 14:44:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 14:44:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 21:34:17 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:36:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 21:37:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de5cbe49ae47809605d7676cf919113b9fcd0039eeeb96d8a990491cb6e266e`  
		Last Modified: Sat, 10 Apr 2021 14:47:08 GMT  
		Size: 4.9 MB (4853557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b7e6fa0abc963aba7a4fc0f66f88960593b6afdf11c1a264e40403924f737`  
		Last Modified: Mon, 26 Apr 2021 21:38:02 GMT  
		Size: 106.4 MB (106398436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.1-windowsservercore-1809`

```console
$ docker pull julia@sha256:3ecf65224dc411f7db10f3a2e8db36c39b9f426df607227cc15b556e6ea95bb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `julia:1.6.1-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:e75466db30b85df9499b4547b8800e7e7755a324c3ee303f978990c2a83a625e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2607668952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415cc2c3e6325cbf96ebb79033925c33d584618fd11a8b0d73ea7ccbf4f4bd2c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:02:47 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:02:48 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:04:26 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:04:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d62f536b5a512c7dda3dfa351ff2a7113f409efe61f18feebd3fe3739927bc`  
		Last Modified: Mon, 26 Apr 2021 21:08:03 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001c92228b8dfe3a318ea88fa0c4f005aab8ac0bc0a4a7b17daacb3b11a01ea`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a5006275da11a373e2da6e690d7567700b3e040322583e596a2e968e34153`  
		Last Modified: Mon, 26 Apr 2021 21:08:36 GMT  
		Size: 137.9 MB (137909420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d6a3269b15f3d75f3292fcaa599df92e864d530a71ac1d5a0827b4a6120e71`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:7aad9a78ec1bdf5b8abb4347a01c01565fb80df6be36878a82af9ac6c38f7191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `julia:1.6.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:8c989761b1dc748646817175b7623754f784aaea26070852701f14184040bd6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937855117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261a028fcf019c1cc5a1103c3359767ecff911c002d73e53c132f2e77ce27f84`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:04:45 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:04:46 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:07:09 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:07:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b8ff0cbb14542ed03b2c1fdb5d6e4b1787e9af6ac9a33fb06dbc7b119d9e69`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b526113b3aa441415c74b9d97a76dbb51fc93a620e2cf7d3570565f00da19`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a952cc9a0bfa19a13f0a4e8394c838a67a56d8fe4f61a601f28bb258db138f1`  
		Last Modified: Mon, 26 Apr 2021 21:09:26 GMT  
		Size: 143.0 MB (142965626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b17799f8a1b7ae1f6d125d71b7b27be62cbfc5d3e8d5fb83ebacd72df660fa`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine`

```console
$ docker pull julia@sha256:36052a38d8ce24173a714e6f45e15217fc5f6db83f6e3362bea1e9b330e602f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:alpine` - linux; amd64

```console
$ docker pull julia@sha256:ca3709087833add7942f34806d4ca65ccd2ab5e59126a9c6c4cae85a20fe36e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123108120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e8f10e31159b593f38f63d8737617466ba087325f6a24c7dee6fef1f502de3`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 14 Apr 2021 23:02:59 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:28 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='492514c93c97e7012b8124a959a9f5569231e52b14f992e74a977fffd7b8961b' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 26 Apr 2021 19:38:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f83c49c066b01cd3dbd841541c23568ea47df8d53902a4cbf122f3865476478`  
		Last Modified: Mon, 26 Apr 2021 19:40:22 GMT  
		Size: 120.3 MB (120296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.13`

```console
$ docker pull julia@sha256:36052a38d8ce24173a714e6f45e15217fc5f6db83f6e3362bea1e9b330e602f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:ca3709087833add7942f34806d4ca65ccd2ab5e59126a9c6c4cae85a20fe36e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123108120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e8f10e31159b593f38f63d8737617466ba087325f6a24c7dee6fef1f502de3`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 14 Apr 2021 23:02:59 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Apr 2021 23:02:59 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:28 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='492514c93c97e7012b8124a959a9f5569231e52b14f992e74a977fffd7b8961b' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 26 Apr 2021 19:38:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f83c49c066b01cd3dbd841541c23568ea47df8d53902a4cbf122f3865476478`  
		Last Modified: Mon, 26 Apr 2021 19:40:22 GMT  
		Size: 120.3 MB (120296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:buster`

```console
$ docker pull julia@sha256:bbd5234fe0bf8904dd3374e84b81f9f14a7e5e754ef7e3c2a0a93edaa259eaac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:9e0a7e7f671ff4249101208df5150945e3b15d4a712ec068a1ca82afb8e70833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152635667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5406d71f1cccd07971d3759be41a3e4ea3c0f52a740b246d40da57684cfa077`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:08 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 19:38:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc393e77a75f632f581added9733180f506256f659d50247f42862153b44a2d`  
		Last Modified: Mon, 26 Apr 2021 19:39:41 GMT  
		Size: 121.0 MB (121038297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:a03e9e70fd6d73b842cbeca5112acc107bbd4c6fbd63c5b56c708a266224807d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138668730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9dea7467a9211b67e60854de9e2ebd34d257b065ecf56ef47446445fafc80bc`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 20:10:16 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:16:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:16:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacce62cd0061e689b2f6a7abf6ba0372808efc29bf5fcfd302a8e07825dd29`  
		Last Modified: Mon, 10 May 2021 21:17:40 GMT  
		Size: 112.1 MB (112123457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0b1bb0aa54548f67f8027615d6cd9f28629f9428e3d7775b543669d7a63a7370
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145159457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb777f8f3d4ca2313ecc47b6894705e9265ca1410009749d73d7902ab846e46f`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:02:48 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:14:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:14:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42476a9f7e3bcac4810c863cd8d19cf0eb4eb627c0e90c934c09796844599dd`  
		Last Modified: Mon, 10 May 2021 21:15:33 GMT  
		Size: 114.9 MB (114916446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:03edae6d5bfcebbd136b888b8d94a7fd71fc752db39d60319dbc52c2cf277955
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151020856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779d82018ac27ee00e27417a817b697d39aa87594ab4607303be7416871c7bcb`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 18:54:54 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 18:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 18:55:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcd3467ae1a05da8d7c83b3c276e92778b61d6b90c5913785049f463745b39d`  
		Last Modified: Mon, 26 Apr 2021 18:56:23 GMT  
		Size: 118.6 MB (118621282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; ppc64le

```console
$ docker pull julia@sha256:34f2b72bbab5bb60259559e69c3e31a388e502db98d0a360088c271b39a04118
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141797926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142a7fd70412cc059bddf7a9c1b19ae16fce2caa33bf8689e959f3f38171b1fe`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:44:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 14:44:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 14:44:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 21:34:17 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:36:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 21:37:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de5cbe49ae47809605d7676cf919113b9fcd0039eeeb96d8a990491cb6e266e`  
		Last Modified: Sat, 10 Apr 2021 14:47:08 GMT  
		Size: 4.9 MB (4853557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b7e6fa0abc963aba7a4fc0f66f88960593b6afdf11c1a264e40403924f737`  
		Last Modified: Mon, 26 Apr 2021 21:38:02 GMT  
		Size: 106.4 MB (106398436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:ce3a3fe709ac7e242b4d8fd081a13f1e7cd160f7cabb592b9552bf563fa8f5a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:9e0a7e7f671ff4249101208df5150945e3b15d4a712ec068a1ca82afb8e70833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152635667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5406d71f1cccd07971d3759be41a3e4ea3c0f52a740b246d40da57684cfa077`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:55:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:55:18 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 06:55:19 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 06:55:19 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:38:08 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 19:38:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 19:38:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f91229f9c8886c99154152d2b89193390ef02de463be9079d60a98c9b9934`  
		Last Modified: Sat, 10 Apr 2021 06:57:57 GMT  
		Size: 4.5 MB (4457997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc393e77a75f632f581added9733180f506256f659d50247f42862153b44a2d`  
		Last Modified: Mon, 26 Apr 2021 19:39:41 GMT  
		Size: 121.0 MB (121038297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm variant v7

```console
$ docker pull julia@sha256:a03e9e70fd6d73b842cbeca5112acc107bbd4c6fbd63c5b56c708a266224807d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138668730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9dea7467a9211b67e60854de9e2ebd34d257b065ecf56ef47446445fafc80bc`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:55:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 08:55:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 08:55:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 08:55:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 20:10:16 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:16:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:16:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf06015707f9a6e13b12da6305bd938e2ccb25fb513cf0cfcd286bb44f4331`  
		Last Modified: Sat, 10 Apr 2021 08:57:09 GMT  
		Size: 3.8 MB (3805472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacce62cd0061e689b2f6a7abf6ba0372808efc29bf5fcfd302a8e07825dd29`  
		Last Modified: Mon, 10 May 2021 21:17:40 GMT  
		Size: 112.1 MB (112123457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:0b1bb0aa54548f67f8027615d6cd9f28629f9428e3d7775b543669d7a63a7370
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145159457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb777f8f3d4ca2313ecc47b6894705e9265ca1410009749d73d7902ab846e46f`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:44:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 04:44:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 04:44:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 04:44:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 19:02:48 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 10 May 2021 21:14:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 10 May 2021 21:14:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50efa104be575ecdac5e5c9a088c46c41a22ab286646b5831164ef61a3f0799e`  
		Last Modified: Sat, 10 Apr 2021 04:47:21 GMT  
		Size: 4.3 MB (4338429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42476a9f7e3bcac4810c863cd8d19cf0eb4eb627c0e90c934c09796844599dd`  
		Last Modified: Mon, 10 May 2021 21:15:33 GMT  
		Size: 114.9 MB (114916446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:03edae6d5bfcebbd136b888b8d94a7fd71fc752db39d60319dbc52c2cf277955
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151020856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779d82018ac27ee00e27417a817b697d39aa87594ab4607303be7416871c7bcb`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 15:29:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 15:29:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:29:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 18:54:54 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 18:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 18:55:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736f834e1ba502d6c1a7780d13032b1d8d992c44ecefa53d1c9afb4019e1d69`  
		Last Modified: Sat, 10 Apr 2021 15:31:38 GMT  
		Size: 4.6 MB (4610587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcd3467ae1a05da8d7c83b3c276e92778b61d6b90c5913785049f463745b39d`  
		Last Modified: Mon, 26 Apr 2021 18:56:23 GMT  
		Size: 118.6 MB (118621282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; ppc64le

```console
$ docker pull julia@sha256:34f2b72bbab5bb60259559e69c3e31a388e502db98d0a360088c271b39a04118
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141797926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142a7fd70412cc059bddf7a9c1b19ae16fce2caa33bf8689e959f3f38171b1fe`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:44:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 10 Apr 2021 14:44:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 14:44:33 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 26 Apr 2021 21:34:17 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:36:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 26 Apr 2021 21:37:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de5cbe49ae47809605d7676cf919113b9fcd0039eeeb96d8a990491cb6e266e`  
		Last Modified: Sat, 10 Apr 2021 14:47:08 GMT  
		Size: 4.9 MB (4853557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b7e6fa0abc963aba7a4fc0f66f88960593b6afdf11c1a264e40403924f737`  
		Last Modified: Mon, 26 Apr 2021 21:38:02 GMT  
		Size: 106.4 MB (106398436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:e75466db30b85df9499b4547b8800e7e7755a324c3ee303f978990c2a83a625e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2607668952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415cc2c3e6325cbf96ebb79033925c33d584618fd11a8b0d73ea7ccbf4f4bd2c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:02:47 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:02:48 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:04:26 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:04:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d62f536b5a512c7dda3dfa351ff2a7113f409efe61f18feebd3fe3739927bc`  
		Last Modified: Mon, 26 Apr 2021 21:08:03 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001c92228b8dfe3a318ea88fa0c4f005aab8ac0bc0a4a7b17daacb3b11a01ea`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a5006275da11a373e2da6e690d7567700b3e040322583e596a2e968e34153`  
		Last Modified: Mon, 26 Apr 2021 21:08:36 GMT  
		Size: 137.9 MB (137909420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d6a3269b15f3d75f3292fcaa599df92e864d530a71ac1d5a0827b4a6120e71`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:8c989761b1dc748646817175b7623754f784aaea26070852701f14184040bd6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937855117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261a028fcf019c1cc5a1103c3359767ecff911c002d73e53c132f2e77ce27f84`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:04:45 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:04:46 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:07:09 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:07:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b8ff0cbb14542ed03b2c1fdb5d6e4b1787e9af6ac9a33fb06dbc7b119d9e69`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b526113b3aa441415c74b9d97a76dbb51fc93a620e2cf7d3570565f00da19`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a952cc9a0bfa19a13f0a4e8394c838a67a56d8fe4f61a601f28bb258db138f1`  
		Last Modified: Mon, 26 Apr 2021 21:09:26 GMT  
		Size: 143.0 MB (142965626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b17799f8a1b7ae1f6d125d71b7b27be62cbfc5d3e8d5fb83ebacd72df660fa`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:3ecf65224dc411f7db10f3a2e8db36c39b9f426df607227cc15b556e6ea95bb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull julia@sha256:e75466db30b85df9499b4547b8800e7e7755a324c3ee303f978990c2a83a625e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2607668952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415cc2c3e6325cbf96ebb79033925c33d584618fd11a8b0d73ea7ccbf4f4bd2c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:02:47 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:02:48 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:04:26 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:04:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d62f536b5a512c7dda3dfa351ff2a7113f409efe61f18feebd3fe3739927bc`  
		Last Modified: Mon, 26 Apr 2021 21:08:03 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001c92228b8dfe3a318ea88fa0c4f005aab8ac0bc0a4a7b17daacb3b11a01ea`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a5006275da11a373e2da6e690d7567700b3e040322583e596a2e968e34153`  
		Last Modified: Mon, 26 Apr 2021 21:08:36 GMT  
		Size: 137.9 MB (137909420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d6a3269b15f3d75f3292fcaa599df92e864d530a71ac1d5a0827b4a6120e71`  
		Last Modified: Mon, 26 Apr 2021 21:08:02 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:7aad9a78ec1bdf5b8abb4347a01c01565fb80df6be36878a82af9ac6c38f7191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `julia:windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull julia@sha256:8c989761b1dc748646817175b7623754f784aaea26070852701f14184040bd6c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937855117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261a028fcf019c1cc5a1103c3359767ecff911c002d73e53c132f2e77ce27f84`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 26 Apr 2021 21:04:45 GMT
ENV JULIA_VERSION=1.6.1
# Mon, 26 Apr 2021 21:04:46 GMT
ENV JULIA_SHA256=953a7715cd0a0eed1fdaee1f2c2886b9581da89f56675b79cf095672fcdc8d6b
# Mon, 26 Apr 2021 21:07:09 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Mon, 26 Apr 2021 21:07:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b8ff0cbb14542ed03b2c1fdb5d6e4b1787e9af6ac9a33fb06dbc7b119d9e69`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b526113b3aa441415c74b9d97a76dbb51fc93a620e2cf7d3570565f00da19`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a952cc9a0bfa19a13f0a4e8394c838a67a56d8fe4f61a601f28bb258db138f1`  
		Last Modified: Mon, 26 Apr 2021 21:09:26 GMT  
		Size: 143.0 MB (142965626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b17799f8a1b7ae1f6d125d71b7b27be62cbfc5d3e8d5fb83ebacd72df660fa`  
		Last Modified: Mon, 26 Apr 2021 21:08:57 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
