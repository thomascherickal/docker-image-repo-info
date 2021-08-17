<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `julia`

-	[`julia:1`](#julia1)
-	[`julia:1-alpine`](#julia1-alpine)
-	[`julia:1-alpine3.13`](#julia1-alpine313)
-	[`julia:1-alpine3.14`](#julia1-alpine314)
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
-	[`julia:1.6-alpine3.14`](#julia16-alpine314)
-	[`julia:1.6-buster`](#julia16-buster)
-	[`julia:1.6-windowsservercore-1809`](#julia16-windowsservercore-1809)
-	[`julia:1.6-windowsservercore-ltsc2016`](#julia16-windowsservercore-ltsc2016)
-	[`julia:1.6.2`](#julia162)
-	[`julia:1.6.2-alpine`](#julia162-alpine)
-	[`julia:1.6.2-alpine3.13`](#julia162-alpine313)
-	[`julia:1.6.2-alpine3.14`](#julia162-alpine314)
-	[`julia:1.6.2-buster`](#julia162-buster)
-	[`julia:1.6.2-windowsservercore-1809`](#julia162-windowsservercore-1809)
-	[`julia:1.6.2-windowsservercore-ltsc2016`](#julia162-windowsservercore-ltsc2016)
-	[`julia:alpine`](#juliaalpine)
-	[`julia:alpine3.13`](#juliaalpine313)
-	[`julia:alpine3.14`](#juliaalpine314)
-	[`julia:buster`](#juliabuster)
-	[`julia:latest`](#julialatest)
-	[`julia:windowsservercore-1809`](#juliawindowsservercore-1809)
-	[`julia:windowsservercore-ltsc2016`](#juliawindowsservercore-ltsc2016)

## `julia:1`

```console
$ docker pull julia@sha256:b18d280fdffecb0a8e721ee6ddd9fcac90e5105971a27a807955028fd0a40351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `julia:1` - linux; amd64

```console
$ docker pull julia@sha256:bcb46263bd3c3f722ff0d0499dba259e63c4559eb90a263fb95d4630b97f9e8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.8 MB (152842070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306354d242a718dac2a913c2eddd0d85a25b9cb7c7e4785c2af862a19c3c47db`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:35:39 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 11:35:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:35:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e7adc69a5e3c4289c70204f1a0c48c949894094a578301d6f2752c07ab2eb6`  
		Last Modified: Tue, 17 Aug 2021 11:38:26 GMT  
		Size: 121.2 MB (121238091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm variant v7

```console
$ docker pull julia@sha256:8227526b538f3c5722c33b95347831e594dc786e092d2da4e4f0301f458931cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138995918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6a92fd63ee0ccae5b2580375b577fde954069fbb13aefc7aaf2271847d34c0`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 08:12:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:12:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441056932b57179a6f22c0b15f1612f326bc0f2caaf4f408d4ecd47eccdfc26c`  
		Last Modified: Thu, 22 Jul 2021 08:16:54 GMT  
		Size: 112.4 MB (112444514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a4f890ca489344c7eddc9b6aea274d4f4a967d251e2a9f817855b7b8360c1692
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145412296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bef4d46929877e22a4e338f64810cf8a866ad8d3ff5b8b0336c7d767bd82e2d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 09:05:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a5737827d37b8a0745903244a9bb5e3d3cf692a3a77e43fee84fa36165fcde`  
		Last Modified: Tue, 17 Aug 2021 09:06:53 GMT  
		Size: 115.2 MB (115158876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:8884b0d2a81dbce90d25e54832481a3143a0e7a9f252d5c1de20183b193f79fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151312378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b1d83d85c635ba8894cadf08a55105aed29bb3cdb242b97972e8a8165d301a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 12:35:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e64774c01c9e59daab48784fb86986780e0d4c30a87f2546d2c41d4fa6243ef`  
		Last Modified: Tue, 17 Aug 2021 12:38:54 GMT  
		Size: 118.9 MB (118904136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; ppc64le

```console
$ docker pull julia@sha256:0a4bbd735273e267514717a187cca1475366ddc6c930df4f7fecdadca9f0fc69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142009834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dbceb35c27bc3d1bff37fc2825c6182e91c37dcd483a6ea53d391694269c65b`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 07:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 07:55:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 07:56:03 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 07:56:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 07:56:11 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 07:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 07:57:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7030c44b136c8de83d74ae09b565174756f2f3ff2dee55885b458f3319d805`  
		Last Modified: Thu, 22 Jul 2021 07:58:32 GMT  
		Size: 4.9 MB (4853473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15b7a7b1631f7a8a140572b774d44aa1929a8d0b6ea4d2d49848acd0da77230`  
		Last Modified: Thu, 22 Jul 2021 07:58:50 GMT  
		Size: 106.6 MB (106602652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:4864ef25c972c714afbc5d30293956a403639e17d278bcd8209a3d46944d48e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2819461834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c15e4cf688eccdbea4a0c8ad51488f19e2e288357238008067f7ab93af8b10`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:31:53 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:31:56 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:34:08 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:34:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c078c711fb6c8ce9576f8dd2c9a5bc7b27c4028c2cc4ecf73fa51496dfddb37`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3f3a64fffd4a6b075410687ff920992b8d532eee734f01a23c8b4acd6eeee`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf511001abbb952897431c950e3ce3c8767038aa724abbc790a05b468dcfbb4`  
		Last Modified: Wed, 11 Aug 2021 16:43:52 GMT  
		Size: 133.5 MB (133458221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d79499293ab2e6910164de236be148ac8a632bf1a159adc08f9c30dedfcb80`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:44f4d3bfb9ba8c20d0f791831e0317e698bddf73b22c54bc48951ac0bf399fe8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408877306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9866121315e46465b3db7d8253e9835d6b32ff8810ee9b62e6c8f2f40a9165a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:34:22 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:34:26 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:37:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:37:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf4d37a068724cf088d64b143f952d057279607a5ea96202c171ccc235e0d10`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7527903790dab1fed6f1b33403b2f51147576eba5f0e57003265456f301d580e`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beab471f1cddf276909b1df5e600fcf90f396cf1992ce340206ac53a217204dc`  
		Last Modified: Wed, 11 Aug 2021 16:46:54 GMT  
		Size: 137.9 MB (137905576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347992b07a31f90c28cc76bdb461185c0c4b6788d9531dc59d27d832312174f5`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine`

```console
$ docker pull julia@sha256:d0980478df718600aaf0ea15f78de9bd7a32ad6fddea792796a8be128df40294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine` - linux; amd64

```console
$ docker pull julia@sha256:5ce902a963bfbd5b4814a6d54ae2a1295cae317355c023b7dc8f39c4fb4f0a7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123230502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c518e06864bb2a5a90a14c2cae95a954f545973c12542a6712a8516e70c9dcb`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 06 Aug 2021 22:47:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 06 Aug 2021 22:47:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 06 Aug 2021 22:47:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb037792c1fc4339d5cfa5b7748d2eb3f44ee3bddc835af017da3f591cf272d`  
		Last Modified: Fri, 06 Aug 2021 22:48:43 GMT  
		Size: 120.4 MB (120417496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.13`

```console
$ docker pull julia@sha256:6f857ff264a0a7daefcf384c8a3890c8dfc01ebb2547870a5f609a17ef13b067
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:86fcdf28ffa781bc68aa60aadda06696b81b3f342b7970da9d3fa5e2bec143c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123227540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cf72173a4e6f83f28bd49525dfccad7429be1d2bd8707e8c5bc4f304a83f980`
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
# Thu, 15 Jul 2021 17:20:46 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 15 Jul 2021 17:20:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 15 Jul 2021 17:20:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08adf7967e3b7e49fa5006ecb084bf6a3b40503e41b7f308a404ebb5539a1a7`  
		Last Modified: Thu, 15 Jul 2021 17:23:47 GMT  
		Size: 120.4 MB (120415571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.14`

```console
$ docker pull julia@sha256:d0980478df718600aaf0ea15f78de9bd7a32ad6fddea792796a8be128df40294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:5ce902a963bfbd5b4814a6d54ae2a1295cae317355c023b7dc8f39c4fb4f0a7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123230502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c518e06864bb2a5a90a14c2cae95a954f545973c12542a6712a8516e70c9dcb`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 06 Aug 2021 22:47:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 06 Aug 2021 22:47:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 06 Aug 2021 22:47:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb037792c1fc4339d5cfa5b7748d2eb3f44ee3bddc835af017da3f591cf272d`  
		Last Modified: Fri, 06 Aug 2021 22:48:43 GMT  
		Size: 120.4 MB (120417496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-buster`

```console
$ docker pull julia@sha256:3bc83d78f37700068c6d3121ba3288c4ad4e637cac68a33d996b0f5eeef11121
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1-buster` - linux; amd64

```console
$ docker pull julia@sha256:bcb46263bd3c3f722ff0d0499dba259e63c4559eb90a263fb95d4630b97f9e8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.8 MB (152842070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306354d242a718dac2a913c2eddd0d85a25b9cb7c7e4785c2af862a19c3c47db`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:35:39 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 11:35:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:35:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e7adc69a5e3c4289c70204f1a0c48c949894094a578301d6f2752c07ab2eb6`  
		Last Modified: Tue, 17 Aug 2021 11:38:26 GMT  
		Size: 121.2 MB (121238091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:8227526b538f3c5722c33b95347831e594dc786e092d2da4e4f0301f458931cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138995918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6a92fd63ee0ccae5b2580375b577fde954069fbb13aefc7aaf2271847d34c0`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 08:12:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:12:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441056932b57179a6f22c0b15f1612f326bc0f2caaf4f408d4ecd47eccdfc26c`  
		Last Modified: Thu, 22 Jul 2021 08:16:54 GMT  
		Size: 112.4 MB (112444514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a4f890ca489344c7eddc9b6aea274d4f4a967d251e2a9f817855b7b8360c1692
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145412296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bef4d46929877e22a4e338f64810cf8a866ad8d3ff5b8b0336c7d767bd82e2d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 09:05:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a5737827d37b8a0745903244a9bb5e3d3cf692a3a77e43fee84fa36165fcde`  
		Last Modified: Tue, 17 Aug 2021 09:06:53 GMT  
		Size: 115.2 MB (115158876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; 386

```console
$ docker pull julia@sha256:8884b0d2a81dbce90d25e54832481a3143a0e7a9f252d5c1de20183b193f79fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151312378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b1d83d85c635ba8894cadf08a55105aed29bb3cdb242b97972e8a8165d301a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 12:35:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e64774c01c9e59daab48784fb86986780e0d4c30a87f2546d2c41d4fa6243ef`  
		Last Modified: Tue, 17 Aug 2021 12:38:54 GMT  
		Size: 118.9 MB (118904136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:0a4bbd735273e267514717a187cca1475366ddc6c930df4f7fecdadca9f0fc69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142009834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dbceb35c27bc3d1bff37fc2825c6182e91c37dcd483a6ea53d391694269c65b`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 07:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 07:55:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 07:56:03 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 07:56:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 07:56:11 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 07:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 07:57:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7030c44b136c8de83d74ae09b565174756f2f3ff2dee55885b458f3319d805`  
		Last Modified: Thu, 22 Jul 2021 07:58:32 GMT  
		Size: 4.9 MB (4853473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15b7a7b1631f7a8a140572b774d44aa1929a8d0b6ea4d2d49848acd0da77230`  
		Last Modified: Thu, 22 Jul 2021 07:58:50 GMT  
		Size: 106.6 MB (106602652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:887c0908564800a3e262dd192eafcdf59d122ed2a8846e2006aad90b64c79658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:4864ef25c972c714afbc5d30293956a403639e17d278bcd8209a3d46944d48e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2819461834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c15e4cf688eccdbea4a0c8ad51488f19e2e288357238008067f7ab93af8b10`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:31:53 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:31:56 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:34:08 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:34:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c078c711fb6c8ce9576f8dd2c9a5bc7b27c4028c2cc4ecf73fa51496dfddb37`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3f3a64fffd4a6b075410687ff920992b8d532eee734f01a23c8b4acd6eeee`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf511001abbb952897431c950e3ce3c8767038aa724abbc790a05b468dcfbb4`  
		Last Modified: Wed, 11 Aug 2021 16:43:52 GMT  
		Size: 133.5 MB (133458221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d79499293ab2e6910164de236be148ac8a632bf1a159adc08f9c30dedfcb80`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:618c3ee48853b47e4e32cfa9e19030156d259020ca9c43a31a495711ae5be225
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `julia:1-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:44f4d3bfb9ba8c20d0f791831e0317e698bddf73b22c54bc48951ac0bf399fe8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408877306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9866121315e46465b3db7d8253e9835d6b32ff8810ee9b62e6c8f2f40a9165a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:34:22 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:34:26 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:37:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:37:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf4d37a068724cf088d64b143f952d057279607a5ea96202c171ccc235e0d10`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7527903790dab1fed6f1b33403b2f51147576eba5f0e57003265456f301d580e`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beab471f1cddf276909b1df5e600fcf90f396cf1992ce340206ac53a217204dc`  
		Last Modified: Wed, 11 Aug 2021 16:46:54 GMT  
		Size: 137.9 MB (137905576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347992b07a31f90c28cc76bdb461185c0c4b6788d9531dc59d27d832312174f5`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0`

```console
$ docker pull julia@sha256:58c0901c62df626d5de1ef0b60e637a2e28238928d9993dca3679a871d0e3cbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `julia:1.0` - linux; amd64

```console
$ docker pull julia@sha256:8a8fe77d4a2389a87f7aba73135c911c52fc853cae4727324ca514051b83274f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127167456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57b0dfe4583acb1166daa0473237e89f0f835955eb2943ada543d4e4946a643a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:36:08 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 11:36:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:36:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b6ff3cc10f84a86d49c539694b48ebcb908467bf748351ebc85a6c5bc1ee15`  
		Last Modified: Tue, 17 Aug 2021 11:39:09 GMT  
		Size: 95.6 MB (95563477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm variant v7

```console
$ docker pull julia@sha256:01eb2eff1167bc8a4b51f9a40980a18a8f80848035b53d51fea660fa9b6516b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113680326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d74578d98f09be172e5d57597eb8f886314be22bcbf3c0437f0f42897dd068d`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:12:40 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 22 Jul 2021 08:13:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:13:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665929fdf633b1bcdbb4471d7d658ec299fdaef9af2f6c2317334b3629a0b49f`  
		Last Modified: Thu, 22 Jul 2021 08:18:15 GMT  
		Size: 87.1 MB (87128922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a1ae79b23bc1ff73ecc1035e7bbf520cf7c8333425e265fe49079df8da9c22f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110144499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca078a450efb0b58ea6c8e78fa48a0cb9456d7bf33ba254cbd1c7b8bcc05325`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:05:18 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 09:05:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4ba659453226ddc28b3e73ccfbd8756cfb9762f7b5956662c3a2b9ecbbca0`  
		Last Modified: Tue, 17 Aug 2021 09:07:25 GMT  
		Size: 79.9 MB (79891079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; 386

```console
$ docker pull julia@sha256:030b82b0e64d2524d329e62adccdd8a9ed22458c9ce1dfa95dfd293616c0abf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124907307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36663257914bb0ad9627f5aa8c7c99f6c8e7586f541f140009333addd841e4c0`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:36:10 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 12:36:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da3e28cfaa9b4b1dd617fab44fd7c5ac2d8a6cce818ee5799a70d3c8e15f757`  
		Last Modified: Tue, 17 Aug 2021 12:39:43 GMT  
		Size: 92.5 MB (92499065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:0afcea1c6804e40d1df58fa605c94eb8d7c5f055e2411345616a7391b6e92cfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784302662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db0ce69d581def17ed160eb7163def1a0c5715b06b1383a79e8895525e81459`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:37:34 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Aug 2021 16:37:37 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Aug 2021 16:39:36 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:39:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21184c08f79288263e9c4d36a99550db755ece6e9d3c25c924dddc6bac179a7d`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19f3bc85a6702672270a830e745ff9315a85fd5513cb4eea7dd350d916e3bb2`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b6076d45223f46974be8f22cbb27aedd70a4f2371c787a6545f5bf9df72299`  
		Last Modified: Wed, 11 Aug 2021 16:47:32 GMT  
		Size: 98.3 MB (98299008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d0a7b2513a1ff7afe315483232683e5deea57eebe1d4c5b0196ac22e559e91`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:7d89024602e90e913be3eff0bba217db0a4f5a968f6873147f6c0ed583ac8200
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6373727967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8682fe79aefe9620a165d8ea58e6e94e85b945acca868841aa6de61f7f9c0b8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:40:02 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Aug 2021 16:40:04 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Aug 2021 16:42:38 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:42:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5223186be1fa84d7b74bef621e5416915d8fdcb7e99392fa6bc0b23c753d5`  
		Last Modified: Wed, 11 Aug 2021 16:47:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59696a8f2091dbed2381e8b17fef468b8c991932aa183ba33fbebfc509fed34b`  
		Last Modified: Wed, 11 Aug 2021 16:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec78a1576c834c87be7d6cc04070b02a48e396c0b481bf78abf1caf0464ab07`  
		Last Modified: Wed, 11 Aug 2021 16:48:06 GMT  
		Size: 102.8 MB (102756279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf246f8eb19fd850ee2024654493afe4ee73056293d8a97da8272b27b73d870`  
		Last Modified: Wed, 11 Aug 2021 16:47:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-buster`

```console
$ docker pull julia@sha256:b97e0330045bd1c9b81ed9ec17dbde54a627e7a966a161cd5eea56a3a0a07a70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:8a8fe77d4a2389a87f7aba73135c911c52fc853cae4727324ca514051b83274f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127167456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57b0dfe4583acb1166daa0473237e89f0f835955eb2943ada543d4e4946a643a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:36:08 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 11:36:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:36:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b6ff3cc10f84a86d49c539694b48ebcb908467bf748351ebc85a6c5bc1ee15`  
		Last Modified: Tue, 17 Aug 2021 11:39:09 GMT  
		Size: 95.6 MB (95563477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:01eb2eff1167bc8a4b51f9a40980a18a8f80848035b53d51fea660fa9b6516b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113680326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d74578d98f09be172e5d57597eb8f886314be22bcbf3c0437f0f42897dd068d`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:12:40 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 22 Jul 2021 08:13:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:13:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665929fdf633b1bcdbb4471d7d658ec299fdaef9af2f6c2317334b3629a0b49f`  
		Last Modified: Thu, 22 Jul 2021 08:18:15 GMT  
		Size: 87.1 MB (87128922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a1ae79b23bc1ff73ecc1035e7bbf520cf7c8333425e265fe49079df8da9c22f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110144499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca078a450efb0b58ea6c8e78fa48a0cb9456d7bf33ba254cbd1c7b8bcc05325`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:05:18 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 09:05:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4ba659453226ddc28b3e73ccfbd8756cfb9762f7b5956662c3a2b9ecbbca0`  
		Last Modified: Tue, 17 Aug 2021 09:07:25 GMT  
		Size: 79.9 MB (79891079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; 386

```console
$ docker pull julia@sha256:030b82b0e64d2524d329e62adccdd8a9ed22458c9ce1dfa95dfd293616c0abf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124907307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36663257914bb0ad9627f5aa8c7c99f6c8e7586f541f140009333addd841e4c0`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:36:10 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 12:36:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da3e28cfaa9b4b1dd617fab44fd7c5ac2d8a6cce818ee5799a70d3c8e15f757`  
		Last Modified: Tue, 17 Aug 2021 12:39:43 GMT  
		Size: 92.5 MB (92499065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-stretch`

```console
$ docker pull julia@sha256:d589659fa0441ccd4aafdb36bb8505b92a88c92771e97b11dd9186dc639dcc0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-stretch` - linux; amd64

```console
$ docker pull julia@sha256:1eb418c409be6cac028ad6c786eae6d99d833849ed80e2ad10d1be25ca75b049
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150447415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863efdee75acef9f461f86536cf66a1c3bbd3c0f01355ffd5b05dba2b64fea1`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:56 GMT
ADD file:0d0aa1ebd07b0f301aaf1077d1e9f2e9be1859510dd8535e143571b347a2a379 in / 
# Tue, 17 Aug 2021 01:25:56 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:36:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:36:50 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:36:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:36:51 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:36:51 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 11:37:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:37:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:eb18d230e067c240479c6a3f842e7f9d4ff1088e3072d0a3245829c4e356623f`  
		Last Modified: Tue, 17 Aug 2021 01:33:03 GMT  
		Size: 45.4 MB (45379966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62db5ad1a57b18349c59434948289d846c9251c2a1e7de99d926f214a00d3d6`  
		Last Modified: Tue, 17 Aug 2021 11:39:23 GMT  
		Size: 9.5 MB (9493699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a3677f04ac89a4814196de877e6111509d1ca8427b84c2b91adb54c6a5cfc0`  
		Last Modified: Tue, 17 Aug 2021 11:39:43 GMT  
		Size: 95.6 MB (95573750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:216290dd6fd3c56783dadb8169bc65096387799f185995c091213ab412331fe1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137470007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6837784e126e46bea71ac8109a2aaf7cf798b0b970a051df4940bb17703425`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:06:56 GMT
ADD file:544c40297b94c3ecc6561cf7bfef1cdf9763a18ce5e24b6841a1b70d0516d41d in / 
# Thu, 22 Jul 2021 02:06:57 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:13:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:13:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:13:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:13:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:13:53 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 22 Jul 2021 08:14:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:14:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b3cc5e47308fe8ded537d7ffdcaba46fcdf803cfe9878bd9264754a50eaa128b`  
		Last Modified: Thu, 22 Jul 2021 02:20:37 GMT  
		Size: 42.1 MB (42120108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ac0ee690289a5577347cb1385e4d2289a6cf36c8305fd663d325369f64f5`  
		Last Modified: Thu, 22 Jul 2021 08:18:31 GMT  
		Size: 8.2 MB (8212142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891f0dd2cab5e2517db0cee6175896e687b0fcdba20ec868ce02df90e7b6326d`  
		Last Modified: Thu, 22 Jul 2021 08:19:25 GMT  
		Size: 87.1 MB (87137757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:21f8ae51b0d0241f7edabc5c2c302cf25f33d98fade358919844ff9058983fc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131547401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9ace85496553eaed67dfdea0dbf808b4b350da15cceecd304f9c5a6cba99839`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:17 GMT
ADD file:79e0d0ec943ec405612e2310514d8f0c72cf83483eea6d5f1a7c28b36fa21cf8 in / 
# Tue, 17 Aug 2021 01:48:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:05:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:05:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:05:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:05:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:05:47 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 09:05:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:06:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a410f7a7fb8af899e64ef008ec59cc8062766e91abbf21ba5cee65faac7ba3fa`  
		Last Modified: Tue, 17 Aug 2021 01:57:32 GMT  
		Size: 43.2 MB (43177652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea3b35608d51cdf5a5e4cc6a8f3329bcdda234e8fc7aa8b2d2c7146b68749e2`  
		Last Modified: Tue, 17 Aug 2021 09:07:38 GMT  
		Size: 8.5 MB (8460777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85b0e115535bdde9a12fbb505abb9d6cc01a9c367739131d471d18519f4e7f8`  
		Last Modified: Tue, 17 Aug 2021 09:07:51 GMT  
		Size: 79.9 MB (79908972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; 386

```console
$ docker pull julia@sha256:696ea674e88f989aab9e63fe95f69b70e93d9faa1f2938d28c1ca3081c81597b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148101744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9f2dcd836a0ede0678fa31beb3255a9ae95cd34b60ad7210c769b9cf60ad781`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:43:45 GMT
ADD file:e05a48da77b08cb5622f87152f4378e29fbb9bc65a76c762d45e488e30adb647 in / 
# Tue, 17 Aug 2021 01:43:46 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:37:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:37:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:37:02 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:37:02 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:37:02 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 12:37:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:37:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fd774782ceed955e627fdc8415668afabdebb5525036f0dc871ec023eb317787`  
		Last Modified: Tue, 17 Aug 2021 01:54:38 GMT  
		Size: 46.1 MB (46097220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48a28b5aec238a885bd766ce996d3c7fe148703af53533605e3c8726aa787a8`  
		Last Modified: Tue, 17 Aug 2021 12:39:59 GMT  
		Size: 9.5 MB (9502509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120d424bfb5b5478b2bf3c7b15473a31194cf4224010cf08d62ab67d9c5ca7b8`  
		Last Modified: Tue, 17 Aug 2021 12:40:19 GMT  
		Size: 92.5 MB (92502015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:f44536f58cbd7d14cc0612d6aadc48ed1bdee85257586d2409ecc2e380aa767b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `julia:1.0-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:0afcea1c6804e40d1df58fa605c94eb8d7c5f055e2411345616a7391b6e92cfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784302662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db0ce69d581def17ed160eb7163def1a0c5715b06b1383a79e8895525e81459`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:37:34 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Aug 2021 16:37:37 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Aug 2021 16:39:36 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:39:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21184c08f79288263e9c4d36a99550db755ece6e9d3c25c924dddc6bac179a7d`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19f3bc85a6702672270a830e745ff9315a85fd5513cb4eea7dd350d916e3bb2`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b6076d45223f46974be8f22cbb27aedd70a4f2371c787a6545f5bf9df72299`  
		Last Modified: Wed, 11 Aug 2021 16:47:32 GMT  
		Size: 98.3 MB (98299008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d0a7b2513a1ff7afe315483232683e5deea57eebe1d4c5b0196ac22e559e91`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:6c7bdbf372b7fd6257b903b8aebf61685f9c3f0f399cfc3fb7ca485c1c7aa92b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `julia:1.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:7d89024602e90e913be3eff0bba217db0a4f5a968f6873147f6c0ed583ac8200
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6373727967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8682fe79aefe9620a165d8ea58e6e94e85b945acca868841aa6de61f7f9c0b8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:40:02 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Aug 2021 16:40:04 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Aug 2021 16:42:38 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:42:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5223186be1fa84d7b74bef621e5416915d8fdcb7e99392fa6bc0b23c753d5`  
		Last Modified: Wed, 11 Aug 2021 16:47:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59696a8f2091dbed2381e8b17fef468b8c991932aa183ba33fbebfc509fed34b`  
		Last Modified: Wed, 11 Aug 2021 16:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec78a1576c834c87be7d6cc04070b02a48e396c0b481bf78abf1caf0464ab07`  
		Last Modified: Wed, 11 Aug 2021 16:48:06 GMT  
		Size: 102.8 MB (102756279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf246f8eb19fd850ee2024654493afe4ee73056293d8a97da8272b27b73d870`  
		Last Modified: Wed, 11 Aug 2021 16:47:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5`

```console
$ docker pull julia@sha256:58c0901c62df626d5de1ef0b60e637a2e28238928d9993dca3679a871d0e3cbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `julia:1.0.5` - linux; amd64

```console
$ docker pull julia@sha256:8a8fe77d4a2389a87f7aba73135c911c52fc853cae4727324ca514051b83274f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127167456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57b0dfe4583acb1166daa0473237e89f0f835955eb2943ada543d4e4946a643a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:36:08 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 11:36:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:36:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b6ff3cc10f84a86d49c539694b48ebcb908467bf748351ebc85a6c5bc1ee15`  
		Last Modified: Tue, 17 Aug 2021 11:39:09 GMT  
		Size: 95.6 MB (95563477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm variant v7

```console
$ docker pull julia@sha256:01eb2eff1167bc8a4b51f9a40980a18a8f80848035b53d51fea660fa9b6516b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113680326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d74578d98f09be172e5d57597eb8f886314be22bcbf3c0437f0f42897dd068d`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:12:40 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 22 Jul 2021 08:13:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:13:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665929fdf633b1bcdbb4471d7d658ec299fdaef9af2f6c2317334b3629a0b49f`  
		Last Modified: Thu, 22 Jul 2021 08:18:15 GMT  
		Size: 87.1 MB (87128922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a1ae79b23bc1ff73ecc1035e7bbf520cf7c8333425e265fe49079df8da9c22f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110144499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca078a450efb0b58ea6c8e78fa48a0cb9456d7bf33ba254cbd1c7b8bcc05325`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:05:18 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 09:05:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4ba659453226ddc28b3e73ccfbd8756cfb9762f7b5956662c3a2b9ecbbca0`  
		Last Modified: Tue, 17 Aug 2021 09:07:25 GMT  
		Size: 79.9 MB (79891079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; 386

```console
$ docker pull julia@sha256:030b82b0e64d2524d329e62adccdd8a9ed22458c9ce1dfa95dfd293616c0abf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124907307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36663257914bb0ad9627f5aa8c7c99f6c8e7586f541f140009333addd841e4c0`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:36:10 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 12:36:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da3e28cfaa9b4b1dd617fab44fd7c5ac2d8a6cce818ee5799a70d3c8e15f757`  
		Last Modified: Tue, 17 Aug 2021 12:39:43 GMT  
		Size: 92.5 MB (92499065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:0afcea1c6804e40d1df58fa605c94eb8d7c5f055e2411345616a7391b6e92cfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784302662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db0ce69d581def17ed160eb7163def1a0c5715b06b1383a79e8895525e81459`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:37:34 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Aug 2021 16:37:37 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Aug 2021 16:39:36 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:39:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21184c08f79288263e9c4d36a99550db755ece6e9d3c25c924dddc6bac179a7d`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19f3bc85a6702672270a830e745ff9315a85fd5513cb4eea7dd350d916e3bb2`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b6076d45223f46974be8f22cbb27aedd70a4f2371c787a6545f5bf9df72299`  
		Last Modified: Wed, 11 Aug 2021 16:47:32 GMT  
		Size: 98.3 MB (98299008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d0a7b2513a1ff7afe315483232683e5deea57eebe1d4c5b0196ac22e559e91`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:7d89024602e90e913be3eff0bba217db0a4f5a968f6873147f6c0ed583ac8200
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6373727967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8682fe79aefe9620a165d8ea58e6e94e85b945acca868841aa6de61f7f9c0b8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:40:02 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Aug 2021 16:40:04 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Aug 2021 16:42:38 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:42:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5223186be1fa84d7b74bef621e5416915d8fdcb7e99392fa6bc0b23c753d5`  
		Last Modified: Wed, 11 Aug 2021 16:47:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59696a8f2091dbed2381e8b17fef468b8c991932aa183ba33fbebfc509fed34b`  
		Last Modified: Wed, 11 Aug 2021 16:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec78a1576c834c87be7d6cc04070b02a48e396c0b481bf78abf1caf0464ab07`  
		Last Modified: Wed, 11 Aug 2021 16:48:06 GMT  
		Size: 102.8 MB (102756279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf246f8eb19fd850ee2024654493afe4ee73056293d8a97da8272b27b73d870`  
		Last Modified: Wed, 11 Aug 2021 16:47:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-buster`

```console
$ docker pull julia@sha256:b97e0330045bd1c9b81ed9ec17dbde54a627e7a966a161cd5eea56a3a0a07a70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-buster` - linux; amd64

```console
$ docker pull julia@sha256:8a8fe77d4a2389a87f7aba73135c911c52fc853cae4727324ca514051b83274f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127167456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57b0dfe4583acb1166daa0473237e89f0f835955eb2943ada543d4e4946a643a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:36:08 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 11:36:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:36:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b6ff3cc10f84a86d49c539694b48ebcb908467bf748351ebc85a6c5bc1ee15`  
		Last Modified: Tue, 17 Aug 2021 11:39:09 GMT  
		Size: 95.6 MB (95563477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:01eb2eff1167bc8a4b51f9a40980a18a8f80848035b53d51fea660fa9b6516b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113680326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d74578d98f09be172e5d57597eb8f886314be22bcbf3c0437f0f42897dd068d`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:12:40 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 22 Jul 2021 08:13:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:13:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665929fdf633b1bcdbb4471d7d658ec299fdaef9af2f6c2317334b3629a0b49f`  
		Last Modified: Thu, 22 Jul 2021 08:18:15 GMT  
		Size: 87.1 MB (87128922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a1ae79b23bc1ff73ecc1035e7bbf520cf7c8333425e265fe49079df8da9c22f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110144499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca078a450efb0b58ea6c8e78fa48a0cb9456d7bf33ba254cbd1c7b8bcc05325`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:05:18 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 09:05:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4ba659453226ddc28b3e73ccfbd8756cfb9762f7b5956662c3a2b9ecbbca0`  
		Last Modified: Tue, 17 Aug 2021 09:07:25 GMT  
		Size: 79.9 MB (79891079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; 386

```console
$ docker pull julia@sha256:030b82b0e64d2524d329e62adccdd8a9ed22458c9ce1dfa95dfd293616c0abf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124907307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36663257914bb0ad9627f5aa8c7c99f6c8e7586f541f140009333addd841e4c0`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:36:10 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 12:36:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da3e28cfaa9b4b1dd617fab44fd7c5ac2d8a6cce818ee5799a70d3c8e15f757`  
		Last Modified: Tue, 17 Aug 2021 12:39:43 GMT  
		Size: 92.5 MB (92499065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-stretch`

```console
$ docker pull julia@sha256:d589659fa0441ccd4aafdb36bb8505b92a88c92771e97b11dd9186dc639dcc0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-stretch` - linux; amd64

```console
$ docker pull julia@sha256:1eb418c409be6cac028ad6c786eae6d99d833849ed80e2ad10d1be25ca75b049
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150447415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863efdee75acef9f461f86536cf66a1c3bbd3c0f01355ffd5b05dba2b64fea1`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:56 GMT
ADD file:0d0aa1ebd07b0f301aaf1077d1e9f2e9be1859510dd8535e143571b347a2a379 in / 
# Tue, 17 Aug 2021 01:25:56 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:36:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:36:50 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:36:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:36:51 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:36:51 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 11:37:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:37:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:eb18d230e067c240479c6a3f842e7f9d4ff1088e3072d0a3245829c4e356623f`  
		Last Modified: Tue, 17 Aug 2021 01:33:03 GMT  
		Size: 45.4 MB (45379966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62db5ad1a57b18349c59434948289d846c9251c2a1e7de99d926f214a00d3d6`  
		Last Modified: Tue, 17 Aug 2021 11:39:23 GMT  
		Size: 9.5 MB (9493699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a3677f04ac89a4814196de877e6111509d1ca8427b84c2b91adb54c6a5cfc0`  
		Last Modified: Tue, 17 Aug 2021 11:39:43 GMT  
		Size: 95.6 MB (95573750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:216290dd6fd3c56783dadb8169bc65096387799f185995c091213ab412331fe1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137470007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6837784e126e46bea71ac8109a2aaf7cf798b0b970a051df4940bb17703425`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:06:56 GMT
ADD file:544c40297b94c3ecc6561cf7bfef1cdf9763a18ce5e24b6841a1b70d0516d41d in / 
# Thu, 22 Jul 2021 02:06:57 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:13:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:13:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:13:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:13:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:13:53 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 22 Jul 2021 08:14:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:14:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b3cc5e47308fe8ded537d7ffdcaba46fcdf803cfe9878bd9264754a50eaa128b`  
		Last Modified: Thu, 22 Jul 2021 02:20:37 GMT  
		Size: 42.1 MB (42120108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ac0ee690289a5577347cb1385e4d2289a6cf36c8305fd663d325369f64f5`  
		Last Modified: Thu, 22 Jul 2021 08:18:31 GMT  
		Size: 8.2 MB (8212142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891f0dd2cab5e2517db0cee6175896e687b0fcdba20ec868ce02df90e7b6326d`  
		Last Modified: Thu, 22 Jul 2021 08:19:25 GMT  
		Size: 87.1 MB (87137757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:21f8ae51b0d0241f7edabc5c2c302cf25f33d98fade358919844ff9058983fc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131547401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9ace85496553eaed67dfdea0dbf808b4b350da15cceecd304f9c5a6cba99839`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:17 GMT
ADD file:79e0d0ec943ec405612e2310514d8f0c72cf83483eea6d5f1a7c28b36fa21cf8 in / 
# Tue, 17 Aug 2021 01:48:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:05:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:05:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:05:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:05:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:05:47 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 09:05:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:06:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a410f7a7fb8af899e64ef008ec59cc8062766e91abbf21ba5cee65faac7ba3fa`  
		Last Modified: Tue, 17 Aug 2021 01:57:32 GMT  
		Size: 43.2 MB (43177652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea3b35608d51cdf5a5e4cc6a8f3329bcdda234e8fc7aa8b2d2c7146b68749e2`  
		Last Modified: Tue, 17 Aug 2021 09:07:38 GMT  
		Size: 8.5 MB (8460777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85b0e115535bdde9a12fbb505abb9d6cc01a9c367739131d471d18519f4e7f8`  
		Last Modified: Tue, 17 Aug 2021 09:07:51 GMT  
		Size: 79.9 MB (79908972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; 386

```console
$ docker pull julia@sha256:696ea674e88f989aab9e63fe95f69b70e93d9faa1f2938d28c1ca3081c81597b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148101744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9f2dcd836a0ede0678fa31beb3255a9ae95cd34b60ad7210c769b9cf60ad781`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:43:45 GMT
ADD file:e05a48da77b08cb5622f87152f4378e29fbb9bc65a76c762d45e488e30adb647 in / 
# Tue, 17 Aug 2021 01:43:46 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:37:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:37:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:37:02 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:37:02 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:37:02 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 17 Aug 2021 12:37:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:37:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fd774782ceed955e627fdc8415668afabdebb5525036f0dc871ec023eb317787`  
		Last Modified: Tue, 17 Aug 2021 01:54:38 GMT  
		Size: 46.1 MB (46097220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48a28b5aec238a885bd766ce996d3c7fe148703af53533605e3c8726aa787a8`  
		Last Modified: Tue, 17 Aug 2021 12:39:59 GMT  
		Size: 9.5 MB (9502509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120d424bfb5b5478b2bf3c7b15473a31194cf4224010cf08d62ab67d9c5ca7b8`  
		Last Modified: Tue, 17 Aug 2021 12:40:19 GMT  
		Size: 92.5 MB (92502015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-1809`

```console
$ docker pull julia@sha256:f44536f58cbd7d14cc0612d6aadc48ed1bdee85257586d2409ecc2e380aa767b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `julia:1.0.5-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:0afcea1c6804e40d1df58fa605c94eb8d7c5f055e2411345616a7391b6e92cfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784302662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db0ce69d581def17ed160eb7163def1a0c5715b06b1383a79e8895525e81459`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:37:34 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Aug 2021 16:37:37 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Aug 2021 16:39:36 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:39:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21184c08f79288263e9c4d36a99550db755ece6e9d3c25c924dddc6bac179a7d`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19f3bc85a6702672270a830e745ff9315a85fd5513cb4eea7dd350d916e3bb2`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b6076d45223f46974be8f22cbb27aedd70a4f2371c787a6545f5bf9df72299`  
		Last Modified: Wed, 11 Aug 2021 16:47:32 GMT  
		Size: 98.3 MB (98299008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d0a7b2513a1ff7afe315483232683e5deea57eebe1d4c5b0196ac22e559e91`  
		Last Modified: Wed, 11 Aug 2021 16:47:10 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:6c7bdbf372b7fd6257b903b8aebf61685f9c3f0f399cfc3fb7ca485c1c7aa92b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `julia:1.0.5-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:7d89024602e90e913be3eff0bba217db0a4f5a968f6873147f6c0ed583ac8200
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6373727967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8682fe79aefe9620a165d8ea58e6e94e85b945acca868841aa6de61f7f9c0b8`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:40:02 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Aug 2021 16:40:04 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Aug 2021 16:42:38 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:42:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5223186be1fa84d7b74bef621e5416915d8fdcb7e99392fa6bc0b23c753d5`  
		Last Modified: Wed, 11 Aug 2021 16:47:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59696a8f2091dbed2381e8b17fef468b8c991932aa183ba33fbebfc509fed34b`  
		Last Modified: Wed, 11 Aug 2021 16:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec78a1576c834c87be7d6cc04070b02a48e396c0b481bf78abf1caf0464ab07`  
		Last Modified: Wed, 11 Aug 2021 16:48:06 GMT  
		Size: 102.8 MB (102756279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf246f8eb19fd850ee2024654493afe4ee73056293d8a97da8272b27b73d870`  
		Last Modified: Wed, 11 Aug 2021 16:47:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6`

```console
$ docker pull julia@sha256:b18d280fdffecb0a8e721ee6ddd9fcac90e5105971a27a807955028fd0a40351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `julia:1.6` - linux; amd64

```console
$ docker pull julia@sha256:bcb46263bd3c3f722ff0d0499dba259e63c4559eb90a263fb95d4630b97f9e8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.8 MB (152842070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306354d242a718dac2a913c2eddd0d85a25b9cb7c7e4785c2af862a19c3c47db`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:35:39 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 11:35:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:35:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e7adc69a5e3c4289c70204f1a0c48c949894094a578301d6f2752c07ab2eb6`  
		Last Modified: Tue, 17 Aug 2021 11:38:26 GMT  
		Size: 121.2 MB (121238091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm variant v7

```console
$ docker pull julia@sha256:8227526b538f3c5722c33b95347831e594dc786e092d2da4e4f0301f458931cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138995918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6a92fd63ee0ccae5b2580375b577fde954069fbb13aefc7aaf2271847d34c0`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 08:12:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:12:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441056932b57179a6f22c0b15f1612f326bc0f2caaf4f408d4ecd47eccdfc26c`  
		Last Modified: Thu, 22 Jul 2021 08:16:54 GMT  
		Size: 112.4 MB (112444514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a4f890ca489344c7eddc9b6aea274d4f4a967d251e2a9f817855b7b8360c1692
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145412296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bef4d46929877e22a4e338f64810cf8a866ad8d3ff5b8b0336c7d767bd82e2d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 09:05:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a5737827d37b8a0745903244a9bb5e3d3cf692a3a77e43fee84fa36165fcde`  
		Last Modified: Tue, 17 Aug 2021 09:06:53 GMT  
		Size: 115.2 MB (115158876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; 386

```console
$ docker pull julia@sha256:8884b0d2a81dbce90d25e54832481a3143a0e7a9f252d5c1de20183b193f79fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151312378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b1d83d85c635ba8894cadf08a55105aed29bb3cdb242b97972e8a8165d301a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 12:35:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e64774c01c9e59daab48784fb86986780e0d4c30a87f2546d2c41d4fa6243ef`  
		Last Modified: Tue, 17 Aug 2021 12:38:54 GMT  
		Size: 118.9 MB (118904136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; ppc64le

```console
$ docker pull julia@sha256:0a4bbd735273e267514717a187cca1475366ddc6c930df4f7fecdadca9f0fc69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142009834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dbceb35c27bc3d1bff37fc2825c6182e91c37dcd483a6ea53d391694269c65b`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 07:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 07:55:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 07:56:03 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 07:56:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 07:56:11 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 07:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 07:57:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7030c44b136c8de83d74ae09b565174756f2f3ff2dee55885b458f3319d805`  
		Last Modified: Thu, 22 Jul 2021 07:58:32 GMT  
		Size: 4.9 MB (4853473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15b7a7b1631f7a8a140572b774d44aa1929a8d0b6ea4d2d49848acd0da77230`  
		Last Modified: Thu, 22 Jul 2021 07:58:50 GMT  
		Size: 106.6 MB (106602652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:4864ef25c972c714afbc5d30293956a403639e17d278bcd8209a3d46944d48e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2819461834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c15e4cf688eccdbea4a0c8ad51488f19e2e288357238008067f7ab93af8b10`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:31:53 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:31:56 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:34:08 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:34:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c078c711fb6c8ce9576f8dd2c9a5bc7b27c4028c2cc4ecf73fa51496dfddb37`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3f3a64fffd4a6b075410687ff920992b8d532eee734f01a23c8b4acd6eeee`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf511001abbb952897431c950e3ce3c8767038aa724abbc790a05b468dcfbb4`  
		Last Modified: Wed, 11 Aug 2021 16:43:52 GMT  
		Size: 133.5 MB (133458221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d79499293ab2e6910164de236be148ac8a632bf1a159adc08f9c30dedfcb80`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:44f4d3bfb9ba8c20d0f791831e0317e698bddf73b22c54bc48951ac0bf399fe8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408877306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9866121315e46465b3db7d8253e9835d6b32ff8810ee9b62e6c8f2f40a9165a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:34:22 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:34:26 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:37:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:37:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf4d37a068724cf088d64b143f952d057279607a5ea96202c171ccc235e0d10`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7527903790dab1fed6f1b33403b2f51147576eba5f0e57003265456f301d580e`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beab471f1cddf276909b1df5e600fcf90f396cf1992ce340206ac53a217204dc`  
		Last Modified: Wed, 11 Aug 2021 16:46:54 GMT  
		Size: 137.9 MB (137905576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347992b07a31f90c28cc76bdb461185c0c4b6788d9531dc59d27d832312174f5`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine`

```console
$ docker pull julia@sha256:d0980478df718600aaf0ea15f78de9bd7a32ad6fddea792796a8be128df40294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine` - linux; amd64

```console
$ docker pull julia@sha256:5ce902a963bfbd5b4814a6d54ae2a1295cae317355c023b7dc8f39c4fb4f0a7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123230502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c518e06864bb2a5a90a14c2cae95a954f545973c12542a6712a8516e70c9dcb`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 06 Aug 2021 22:47:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 06 Aug 2021 22:47:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 06 Aug 2021 22:47:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb037792c1fc4339d5cfa5b7748d2eb3f44ee3bddc835af017da3f591cf272d`  
		Last Modified: Fri, 06 Aug 2021 22:48:43 GMT  
		Size: 120.4 MB (120417496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine3.13`

```console
$ docker pull julia@sha256:6f857ff264a0a7daefcf384c8a3890c8dfc01ebb2547870a5f609a17ef13b067
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:86fcdf28ffa781bc68aa60aadda06696b81b3f342b7970da9d3fa5e2bec143c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123227540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cf72173a4e6f83f28bd49525dfccad7429be1d2bd8707e8c5bc4f304a83f980`
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
# Thu, 15 Jul 2021 17:20:46 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 15 Jul 2021 17:20:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 15 Jul 2021 17:20:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08adf7967e3b7e49fa5006ecb084bf6a3b40503e41b7f308a404ebb5539a1a7`  
		Last Modified: Thu, 15 Jul 2021 17:23:47 GMT  
		Size: 120.4 MB (120415571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine3.14`

```console
$ docker pull julia@sha256:d0980478df718600aaf0ea15f78de9bd7a32ad6fddea792796a8be128df40294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:5ce902a963bfbd5b4814a6d54ae2a1295cae317355c023b7dc8f39c4fb4f0a7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123230502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c518e06864bb2a5a90a14c2cae95a954f545973c12542a6712a8516e70c9dcb`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 06 Aug 2021 22:47:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 06 Aug 2021 22:47:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 06 Aug 2021 22:47:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb037792c1fc4339d5cfa5b7748d2eb3f44ee3bddc835af017da3f591cf272d`  
		Last Modified: Fri, 06 Aug 2021 22:48:43 GMT  
		Size: 120.4 MB (120417496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-buster`

```console
$ docker pull julia@sha256:3bc83d78f37700068c6d3121ba3288c4ad4e637cac68a33d996b0f5eeef11121
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6-buster` - linux; amd64

```console
$ docker pull julia@sha256:bcb46263bd3c3f722ff0d0499dba259e63c4559eb90a263fb95d4630b97f9e8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.8 MB (152842070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306354d242a718dac2a913c2eddd0d85a25b9cb7c7e4785c2af862a19c3c47db`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:35:39 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 11:35:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:35:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e7adc69a5e3c4289c70204f1a0c48c949894094a578301d6f2752c07ab2eb6`  
		Last Modified: Tue, 17 Aug 2021 11:38:26 GMT  
		Size: 121.2 MB (121238091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:8227526b538f3c5722c33b95347831e594dc786e092d2da4e4f0301f458931cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138995918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6a92fd63ee0ccae5b2580375b577fde954069fbb13aefc7aaf2271847d34c0`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 08:12:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:12:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441056932b57179a6f22c0b15f1612f326bc0f2caaf4f408d4ecd47eccdfc26c`  
		Last Modified: Thu, 22 Jul 2021 08:16:54 GMT  
		Size: 112.4 MB (112444514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a4f890ca489344c7eddc9b6aea274d4f4a967d251e2a9f817855b7b8360c1692
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145412296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bef4d46929877e22a4e338f64810cf8a866ad8d3ff5b8b0336c7d767bd82e2d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 09:05:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a5737827d37b8a0745903244a9bb5e3d3cf692a3a77e43fee84fa36165fcde`  
		Last Modified: Tue, 17 Aug 2021 09:06:53 GMT  
		Size: 115.2 MB (115158876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; 386

```console
$ docker pull julia@sha256:8884b0d2a81dbce90d25e54832481a3143a0e7a9f252d5c1de20183b193f79fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151312378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b1d83d85c635ba8894cadf08a55105aed29bb3cdb242b97972e8a8165d301a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 12:35:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e64774c01c9e59daab48784fb86986780e0d4c30a87f2546d2c41d4fa6243ef`  
		Last Modified: Tue, 17 Aug 2021 12:38:54 GMT  
		Size: 118.9 MB (118904136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:0a4bbd735273e267514717a187cca1475366ddc6c930df4f7fecdadca9f0fc69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142009834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dbceb35c27bc3d1bff37fc2825c6182e91c37dcd483a6ea53d391694269c65b`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 07:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 07:55:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 07:56:03 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 07:56:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 07:56:11 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 07:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 07:57:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7030c44b136c8de83d74ae09b565174756f2f3ff2dee55885b458f3319d805`  
		Last Modified: Thu, 22 Jul 2021 07:58:32 GMT  
		Size: 4.9 MB (4853473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15b7a7b1631f7a8a140572b774d44aa1929a8d0b6ea4d2d49848acd0da77230`  
		Last Modified: Thu, 22 Jul 2021 07:58:50 GMT  
		Size: 106.6 MB (106602652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-1809`

```console
$ docker pull julia@sha256:887c0908564800a3e262dd192eafcdf59d122ed2a8846e2006aad90b64c79658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `julia:1.6-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:4864ef25c972c714afbc5d30293956a403639e17d278bcd8209a3d46944d48e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2819461834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c15e4cf688eccdbea4a0c8ad51488f19e2e288357238008067f7ab93af8b10`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:31:53 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:31:56 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:34:08 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:34:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c078c711fb6c8ce9576f8dd2c9a5bc7b27c4028c2cc4ecf73fa51496dfddb37`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3f3a64fffd4a6b075410687ff920992b8d532eee734f01a23c8b4acd6eeee`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf511001abbb952897431c950e3ce3c8767038aa724abbc790a05b468dcfbb4`  
		Last Modified: Wed, 11 Aug 2021 16:43:52 GMT  
		Size: 133.5 MB (133458221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d79499293ab2e6910164de236be148ac8a632bf1a159adc08f9c30dedfcb80`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:618c3ee48853b47e4e32cfa9e19030156d259020ca9c43a31a495711ae5be225
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `julia:1.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:44f4d3bfb9ba8c20d0f791831e0317e698bddf73b22c54bc48951ac0bf399fe8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408877306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9866121315e46465b3db7d8253e9835d6b32ff8810ee9b62e6c8f2f40a9165a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:34:22 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:34:26 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:37:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:37:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf4d37a068724cf088d64b143f952d057279607a5ea96202c171ccc235e0d10`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7527903790dab1fed6f1b33403b2f51147576eba5f0e57003265456f301d580e`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beab471f1cddf276909b1df5e600fcf90f396cf1992ce340206ac53a217204dc`  
		Last Modified: Wed, 11 Aug 2021 16:46:54 GMT  
		Size: 137.9 MB (137905576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347992b07a31f90c28cc76bdb461185c0c4b6788d9531dc59d27d832312174f5`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.2`

```console
$ docker pull julia@sha256:b18d280fdffecb0a8e721ee6ddd9fcac90e5105971a27a807955028fd0a40351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `julia:1.6.2` - linux; amd64

```console
$ docker pull julia@sha256:bcb46263bd3c3f722ff0d0499dba259e63c4559eb90a263fb95d4630b97f9e8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.8 MB (152842070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306354d242a718dac2a913c2eddd0d85a25b9cb7c7e4785c2af862a19c3c47db`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:35:39 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 11:35:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:35:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e7adc69a5e3c4289c70204f1a0c48c949894094a578301d6f2752c07ab2eb6`  
		Last Modified: Tue, 17 Aug 2021 11:38:26 GMT  
		Size: 121.2 MB (121238091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.2` - linux; arm variant v7

```console
$ docker pull julia@sha256:8227526b538f3c5722c33b95347831e594dc786e092d2da4e4f0301f458931cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138995918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6a92fd63ee0ccae5b2580375b577fde954069fbb13aefc7aaf2271847d34c0`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 08:12:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:12:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441056932b57179a6f22c0b15f1612f326bc0f2caaf4f408d4ecd47eccdfc26c`  
		Last Modified: Thu, 22 Jul 2021 08:16:54 GMT  
		Size: 112.4 MB (112444514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.2` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a4f890ca489344c7eddc9b6aea274d4f4a967d251e2a9f817855b7b8360c1692
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145412296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bef4d46929877e22a4e338f64810cf8a866ad8d3ff5b8b0336c7d767bd82e2d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 09:05:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a5737827d37b8a0745903244a9bb5e3d3cf692a3a77e43fee84fa36165fcde`  
		Last Modified: Tue, 17 Aug 2021 09:06:53 GMT  
		Size: 115.2 MB (115158876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.2` - linux; 386

```console
$ docker pull julia@sha256:8884b0d2a81dbce90d25e54832481a3143a0e7a9f252d5c1de20183b193f79fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151312378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b1d83d85c635ba8894cadf08a55105aed29bb3cdb242b97972e8a8165d301a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 12:35:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e64774c01c9e59daab48784fb86986780e0d4c30a87f2546d2c41d4fa6243ef`  
		Last Modified: Tue, 17 Aug 2021 12:38:54 GMT  
		Size: 118.9 MB (118904136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.2` - linux; ppc64le

```console
$ docker pull julia@sha256:0a4bbd735273e267514717a187cca1475366ddc6c930df4f7fecdadca9f0fc69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142009834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dbceb35c27bc3d1bff37fc2825c6182e91c37dcd483a6ea53d391694269c65b`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 07:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 07:55:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 07:56:03 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 07:56:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 07:56:11 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 07:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 07:57:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7030c44b136c8de83d74ae09b565174756f2f3ff2dee55885b458f3319d805`  
		Last Modified: Thu, 22 Jul 2021 07:58:32 GMT  
		Size: 4.9 MB (4853473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15b7a7b1631f7a8a140572b774d44aa1929a8d0b6ea4d2d49848acd0da77230`  
		Last Modified: Thu, 22 Jul 2021 07:58:50 GMT  
		Size: 106.6 MB (106602652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.2` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:4864ef25c972c714afbc5d30293956a403639e17d278bcd8209a3d46944d48e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2819461834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c15e4cf688eccdbea4a0c8ad51488f19e2e288357238008067f7ab93af8b10`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:31:53 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:31:56 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:34:08 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:34:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c078c711fb6c8ce9576f8dd2c9a5bc7b27c4028c2cc4ecf73fa51496dfddb37`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3f3a64fffd4a6b075410687ff920992b8d532eee734f01a23c8b4acd6eeee`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf511001abbb952897431c950e3ce3c8767038aa724abbc790a05b468dcfbb4`  
		Last Modified: Wed, 11 Aug 2021 16:43:52 GMT  
		Size: 133.5 MB (133458221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d79499293ab2e6910164de236be148ac8a632bf1a159adc08f9c30dedfcb80`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.2` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:44f4d3bfb9ba8c20d0f791831e0317e698bddf73b22c54bc48951ac0bf399fe8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408877306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9866121315e46465b3db7d8253e9835d6b32ff8810ee9b62e6c8f2f40a9165a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:34:22 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:34:26 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:37:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:37:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf4d37a068724cf088d64b143f952d057279607a5ea96202c171ccc235e0d10`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7527903790dab1fed6f1b33403b2f51147576eba5f0e57003265456f301d580e`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beab471f1cddf276909b1df5e600fcf90f396cf1992ce340206ac53a217204dc`  
		Last Modified: Wed, 11 Aug 2021 16:46:54 GMT  
		Size: 137.9 MB (137905576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347992b07a31f90c28cc76bdb461185c0c4b6788d9531dc59d27d832312174f5`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.2-alpine`

```console
$ docker pull julia@sha256:d0980478df718600aaf0ea15f78de9bd7a32ad6fddea792796a8be128df40294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.2-alpine` - linux; amd64

```console
$ docker pull julia@sha256:5ce902a963bfbd5b4814a6d54ae2a1295cae317355c023b7dc8f39c4fb4f0a7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123230502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c518e06864bb2a5a90a14c2cae95a954f545973c12542a6712a8516e70c9dcb`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 06 Aug 2021 22:47:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 06 Aug 2021 22:47:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 06 Aug 2021 22:47:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb037792c1fc4339d5cfa5b7748d2eb3f44ee3bddc835af017da3f591cf272d`  
		Last Modified: Fri, 06 Aug 2021 22:48:43 GMT  
		Size: 120.4 MB (120417496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.2-alpine3.13`

```console
$ docker pull julia@sha256:6f857ff264a0a7daefcf384c8a3890c8dfc01ebb2547870a5f609a17ef13b067
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.2-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:86fcdf28ffa781bc68aa60aadda06696b81b3f342b7970da9d3fa5e2bec143c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123227540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cf72173a4e6f83f28bd49525dfccad7429be1d2bd8707e8c5bc4f304a83f980`
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
# Thu, 15 Jul 2021 17:20:46 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 15 Jul 2021 17:20:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 15 Jul 2021 17:20:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08adf7967e3b7e49fa5006ecb084bf6a3b40503e41b7f308a404ebb5539a1a7`  
		Last Modified: Thu, 15 Jul 2021 17:23:47 GMT  
		Size: 120.4 MB (120415571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.2-alpine3.14`

```console
$ docker pull julia@sha256:d0980478df718600aaf0ea15f78de9bd7a32ad6fddea792796a8be128df40294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.2-alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:5ce902a963bfbd5b4814a6d54ae2a1295cae317355c023b7dc8f39c4fb4f0a7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123230502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c518e06864bb2a5a90a14c2cae95a954f545973c12542a6712a8516e70c9dcb`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 06 Aug 2021 22:47:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 06 Aug 2021 22:47:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 06 Aug 2021 22:47:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb037792c1fc4339d5cfa5b7748d2eb3f44ee3bddc835af017da3f591cf272d`  
		Last Modified: Fri, 06 Aug 2021 22:48:43 GMT  
		Size: 120.4 MB (120417496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.2-buster`

```console
$ docker pull julia@sha256:3bc83d78f37700068c6d3121ba3288c4ad4e637cac68a33d996b0f5eeef11121
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.6.2-buster` - linux; amd64

```console
$ docker pull julia@sha256:bcb46263bd3c3f722ff0d0499dba259e63c4559eb90a263fb95d4630b97f9e8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.8 MB (152842070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306354d242a718dac2a913c2eddd0d85a25b9cb7c7e4785c2af862a19c3c47db`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:35:39 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 11:35:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:35:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e7adc69a5e3c4289c70204f1a0c48c949894094a578301d6f2752c07ab2eb6`  
		Last Modified: Tue, 17 Aug 2021 11:38:26 GMT  
		Size: 121.2 MB (121238091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.2-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:8227526b538f3c5722c33b95347831e594dc786e092d2da4e4f0301f458931cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138995918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6a92fd63ee0ccae5b2580375b577fde954069fbb13aefc7aaf2271847d34c0`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 08:12:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:12:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441056932b57179a6f22c0b15f1612f326bc0f2caaf4f408d4ecd47eccdfc26c`  
		Last Modified: Thu, 22 Jul 2021 08:16:54 GMT  
		Size: 112.4 MB (112444514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.2-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a4f890ca489344c7eddc9b6aea274d4f4a967d251e2a9f817855b7b8360c1692
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145412296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bef4d46929877e22a4e338f64810cf8a866ad8d3ff5b8b0336c7d767bd82e2d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 09:05:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a5737827d37b8a0745903244a9bb5e3d3cf692a3a77e43fee84fa36165fcde`  
		Last Modified: Tue, 17 Aug 2021 09:06:53 GMT  
		Size: 115.2 MB (115158876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.2-buster` - linux; 386

```console
$ docker pull julia@sha256:8884b0d2a81dbce90d25e54832481a3143a0e7a9f252d5c1de20183b193f79fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151312378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b1d83d85c635ba8894cadf08a55105aed29bb3cdb242b97972e8a8165d301a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 12:35:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e64774c01c9e59daab48784fb86986780e0d4c30a87f2546d2c41d4fa6243ef`  
		Last Modified: Tue, 17 Aug 2021 12:38:54 GMT  
		Size: 118.9 MB (118904136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.2-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:0a4bbd735273e267514717a187cca1475366ddc6c930df4f7fecdadca9f0fc69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142009834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dbceb35c27bc3d1bff37fc2825c6182e91c37dcd483a6ea53d391694269c65b`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 07:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 07:55:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 07:56:03 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 07:56:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 07:56:11 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 07:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 07:57:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7030c44b136c8de83d74ae09b565174756f2f3ff2dee55885b458f3319d805`  
		Last Modified: Thu, 22 Jul 2021 07:58:32 GMT  
		Size: 4.9 MB (4853473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15b7a7b1631f7a8a140572b774d44aa1929a8d0b6ea4d2d49848acd0da77230`  
		Last Modified: Thu, 22 Jul 2021 07:58:50 GMT  
		Size: 106.6 MB (106602652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.2-windowsservercore-1809`

```console
$ docker pull julia@sha256:887c0908564800a3e262dd192eafcdf59d122ed2a8846e2006aad90b64c79658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `julia:1.6.2-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:4864ef25c972c714afbc5d30293956a403639e17d278bcd8209a3d46944d48e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2819461834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c15e4cf688eccdbea4a0c8ad51488f19e2e288357238008067f7ab93af8b10`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:31:53 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:31:56 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:34:08 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:34:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c078c711fb6c8ce9576f8dd2c9a5bc7b27c4028c2cc4ecf73fa51496dfddb37`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3f3a64fffd4a6b075410687ff920992b8d532eee734f01a23c8b4acd6eeee`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf511001abbb952897431c950e3ce3c8767038aa724abbc790a05b468dcfbb4`  
		Last Modified: Wed, 11 Aug 2021 16:43:52 GMT  
		Size: 133.5 MB (133458221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d79499293ab2e6910164de236be148ac8a632bf1a159adc08f9c30dedfcb80`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.2-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:618c3ee48853b47e4e32cfa9e19030156d259020ca9c43a31a495711ae5be225
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `julia:1.6.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:44f4d3bfb9ba8c20d0f791831e0317e698bddf73b22c54bc48951ac0bf399fe8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408877306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9866121315e46465b3db7d8253e9835d6b32ff8810ee9b62e6c8f2f40a9165a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:34:22 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:34:26 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:37:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:37:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf4d37a068724cf088d64b143f952d057279607a5ea96202c171ccc235e0d10`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7527903790dab1fed6f1b33403b2f51147576eba5f0e57003265456f301d580e`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beab471f1cddf276909b1df5e600fcf90f396cf1992ce340206ac53a217204dc`  
		Last Modified: Wed, 11 Aug 2021 16:46:54 GMT  
		Size: 137.9 MB (137905576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347992b07a31f90c28cc76bdb461185c0c4b6788d9531dc59d27d832312174f5`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine`

```console
$ docker pull julia@sha256:d0980478df718600aaf0ea15f78de9bd7a32ad6fddea792796a8be128df40294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine` - linux; amd64

```console
$ docker pull julia@sha256:5ce902a963bfbd5b4814a6d54ae2a1295cae317355c023b7dc8f39c4fb4f0a7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123230502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c518e06864bb2a5a90a14c2cae95a954f545973c12542a6712a8516e70c9dcb`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 06 Aug 2021 22:47:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 06 Aug 2021 22:47:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 06 Aug 2021 22:47:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb037792c1fc4339d5cfa5b7748d2eb3f44ee3bddc835af017da3f591cf272d`  
		Last Modified: Fri, 06 Aug 2021 22:48:43 GMT  
		Size: 120.4 MB (120417496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.13`

```console
$ docker pull julia@sha256:6f857ff264a0a7daefcf384c8a3890c8dfc01ebb2547870a5f609a17ef13b067
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:86fcdf28ffa781bc68aa60aadda06696b81b3f342b7970da9d3fa5e2bec143c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123227540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cf72173a4e6f83f28bd49525dfccad7429be1d2bd8707e8c5bc4f304a83f980`
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
# Thu, 15 Jul 2021 17:20:46 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 15 Jul 2021 17:20:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 15 Jul 2021 17:20:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08adf7967e3b7e49fa5006ecb084bf6a3b40503e41b7f308a404ebb5539a1a7`  
		Last Modified: Thu, 15 Jul 2021 17:23:47 GMT  
		Size: 120.4 MB (120415571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.14`

```console
$ docker pull julia@sha256:d0980478df718600aaf0ea15f78de9bd7a32ad6fddea792796a8be128df40294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:5ce902a963bfbd5b4814a6d54ae2a1295cae317355c023b7dc8f39c4fb4f0a7a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123230502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c518e06864bb2a5a90a14c2cae95a954f545973c12542a6712a8516e70c9dcb`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 06 Aug 2021 22:47:29 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 06 Aug 2021 22:47:29 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 06 Aug 2021 22:47:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='5ff279bc733a99a9582fd9b39eb3d18a3fa77b9d3d2733039279a250c8c5d49c' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 06 Aug 2021 22:47:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb037792c1fc4339d5cfa5b7748d2eb3f44ee3bddc835af017da3f591cf272d`  
		Last Modified: Fri, 06 Aug 2021 22:48:43 GMT  
		Size: 120.4 MB (120417496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:buster`

```console
$ docker pull julia@sha256:3bc83d78f37700068c6d3121ba3288c4ad4e637cac68a33d996b0f5eeef11121
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:bcb46263bd3c3f722ff0d0499dba259e63c4559eb90a263fb95d4630b97f9e8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.8 MB (152842070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306354d242a718dac2a913c2eddd0d85a25b9cb7c7e4785c2af862a19c3c47db`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:35:39 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 11:35:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:35:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e7adc69a5e3c4289c70204f1a0c48c949894094a578301d6f2752c07ab2eb6`  
		Last Modified: Tue, 17 Aug 2021 11:38:26 GMT  
		Size: 121.2 MB (121238091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:8227526b538f3c5722c33b95347831e594dc786e092d2da4e4f0301f458931cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138995918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6a92fd63ee0ccae5b2580375b577fde954069fbb13aefc7aaf2271847d34c0`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 08:12:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:12:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441056932b57179a6f22c0b15f1612f326bc0f2caaf4f408d4ecd47eccdfc26c`  
		Last Modified: Thu, 22 Jul 2021 08:16:54 GMT  
		Size: 112.4 MB (112444514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a4f890ca489344c7eddc9b6aea274d4f4a967d251e2a9f817855b7b8360c1692
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145412296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bef4d46929877e22a4e338f64810cf8a866ad8d3ff5b8b0336c7d767bd82e2d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 09:05:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a5737827d37b8a0745903244a9bb5e3d3cf692a3a77e43fee84fa36165fcde`  
		Last Modified: Tue, 17 Aug 2021 09:06:53 GMT  
		Size: 115.2 MB (115158876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:8884b0d2a81dbce90d25e54832481a3143a0e7a9f252d5c1de20183b193f79fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151312378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b1d83d85c635ba8894cadf08a55105aed29bb3cdb242b97972e8a8165d301a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 12:35:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e64774c01c9e59daab48784fb86986780e0d4c30a87f2546d2c41d4fa6243ef`  
		Last Modified: Tue, 17 Aug 2021 12:38:54 GMT  
		Size: 118.9 MB (118904136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; ppc64le

```console
$ docker pull julia@sha256:0a4bbd735273e267514717a187cca1475366ddc6c930df4f7fecdadca9f0fc69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142009834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dbceb35c27bc3d1bff37fc2825c6182e91c37dcd483a6ea53d391694269c65b`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 07:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 07:55:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 07:56:03 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 07:56:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 07:56:11 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 07:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 07:57:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7030c44b136c8de83d74ae09b565174756f2f3ff2dee55885b458f3319d805`  
		Last Modified: Thu, 22 Jul 2021 07:58:32 GMT  
		Size: 4.9 MB (4853473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15b7a7b1631f7a8a140572b774d44aa1929a8d0b6ea4d2d49848acd0da77230`  
		Last Modified: Thu, 22 Jul 2021 07:58:50 GMT  
		Size: 106.6 MB (106602652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:b18d280fdffecb0a8e721ee6ddd9fcac90e5105971a27a807955028fd0a40351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:bcb46263bd3c3f722ff0d0499dba259e63c4559eb90a263fb95d4630b97f9e8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.8 MB (152842070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306354d242a718dac2a913c2eddd0d85a25b9cb7c7e4785c2af862a19c3c47db`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 11:35:38 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 11:35:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 11:35:39 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 11:35:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 11:35:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d64765c97dd29814ade4b391dd66832fad7568132cc3ad687489b48ca104054`  
		Last Modified: Tue, 17 Aug 2021 11:38:01 GMT  
		Size: 4.5 MB (4457994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e7adc69a5e3c4289c70204f1a0c48c949894094a578301d6f2752c07ab2eb6`  
		Last Modified: Tue, 17 Aug 2021 11:38:26 GMT  
		Size: 121.2 MB (121238091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm variant v7

```console
$ docker pull julia@sha256:8227526b538f3c5722c33b95347831e594dc786e092d2da4e4f0301f458931cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138995918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6a92fd63ee0ccae5b2580375b577fde954069fbb13aefc7aaf2271847d34c0`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 08:11:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:11:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 08:11:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 08:11:41 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 08:12:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 08:12:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6baaf097f768b56fe00e83538f3de53e4e8d0daa34ad79793afcf7d6ceeded`  
		Last Modified: Thu, 22 Jul 2021 08:15:43 GMT  
		Size: 3.8 MB (3805430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441056932b57179a6f22c0b15f1612f326bc0f2caaf4f408d4ecd47eccdfc26c`  
		Last Modified: Thu, 22 Jul 2021 08:16:54 GMT  
		Size: 112.4 MB (112444514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a4f890ca489344c7eddc9b6aea274d4f4a967d251e2a9f817855b7b8360c1692
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145412296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bef4d46929877e22a4e338f64810cf8a866ad8d3ff5b8b0336c7d767bd82e2d`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:04:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 09:04:53 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 09:04:53 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 09:05:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 09:05:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad85c89ab52b41e4be5bdfa38af68d8abb81d766eba92b20832fceabaa500681`  
		Last Modified: Tue, 17 Aug 2021 09:06:35 GMT  
		Size: 4.3 MB (4338348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a5737827d37b8a0745903244a9bb5e3d3cf692a3a77e43fee84fa36165fcde`  
		Last Modified: Tue, 17 Aug 2021 09:06:53 GMT  
		Size: 115.2 MB (115158876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:8884b0d2a81dbce90d25e54832481a3143a0e7a9f252d5c1de20183b193f79fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151312378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b1d83d85c635ba8894cadf08a55105aed29bb3cdb242b97972e8a8165d301a`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:35:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 17 Aug 2021 12:35:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 17 Aug 2021 12:35:36 GMT
ENV JULIA_VERSION=1.6.2
# Tue, 17 Aug 2021 12:35:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 17 Aug 2021 12:36:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f8f02eaa9da30d8a91ca45dcd548542a27a707c227e350e22bd16297e2df8c`  
		Last Modified: Tue, 17 Aug 2021 12:38:20 GMT  
		Size: 4.6 MB (4610615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e64774c01c9e59daab48784fb86986780e0d4c30a87f2546d2c41d4fa6243ef`  
		Last Modified: Tue, 17 Aug 2021 12:38:54 GMT  
		Size: 118.9 MB (118904136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; ppc64le

```console
$ docker pull julia@sha256:0a4bbd735273e267514717a187cca1475366ddc6c930df4f7fecdadca9f0fc69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142009834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dbceb35c27bc3d1bff37fc2825c6182e91c37dcd483a6ea53d391694269c65b`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 07:55:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 07:55:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 22 Jul 2021 07:56:03 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 07:56:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 22 Jul 2021 07:56:11 GMT
ENV JULIA_VERSION=1.6.2
# Thu, 22 Jul 2021 07:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 22 Jul 2021 07:57:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7030c44b136c8de83d74ae09b565174756f2f3ff2dee55885b458f3319d805`  
		Last Modified: Thu, 22 Jul 2021 07:58:32 GMT  
		Size: 4.9 MB (4853473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15b7a7b1631f7a8a140572b774d44aa1929a8d0b6ea4d2d49848acd0da77230`  
		Last Modified: Thu, 22 Jul 2021 07:58:50 GMT  
		Size: 106.6 MB (106602652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:4864ef25c972c714afbc5d30293956a403639e17d278bcd8209a3d46944d48e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2819461834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c15e4cf688eccdbea4a0c8ad51488f19e2e288357238008067f7ab93af8b10`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:31:53 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:31:56 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:34:08 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:34:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c078c711fb6c8ce9576f8dd2c9a5bc7b27c4028c2cc4ecf73fa51496dfddb37`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3f3a64fffd4a6b075410687ff920992b8d532eee734f01a23c8b4acd6eeee`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf511001abbb952897431c950e3ce3c8767038aa724abbc790a05b468dcfbb4`  
		Last Modified: Wed, 11 Aug 2021 16:43:52 GMT  
		Size: 133.5 MB (133458221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d79499293ab2e6910164de236be148ac8a632bf1a159adc08f9c30dedfcb80`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:44f4d3bfb9ba8c20d0f791831e0317e698bddf73b22c54bc48951ac0bf399fe8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408877306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9866121315e46465b3db7d8253e9835d6b32ff8810ee9b62e6c8f2f40a9165a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:34:22 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:34:26 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:37:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:37:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf4d37a068724cf088d64b143f952d057279607a5ea96202c171ccc235e0d10`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7527903790dab1fed6f1b33403b2f51147576eba5f0e57003265456f301d580e`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beab471f1cddf276909b1df5e600fcf90f396cf1992ce340206ac53a217204dc`  
		Last Modified: Wed, 11 Aug 2021 16:46:54 GMT  
		Size: 137.9 MB (137905576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347992b07a31f90c28cc76bdb461185c0c4b6788d9531dc59d27d832312174f5`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:887c0908564800a3e262dd192eafcdf59d122ed2a8846e2006aad90b64c79658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull julia@sha256:4864ef25c972c714afbc5d30293956a403639e17d278bcd8209a3d46944d48e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2819461834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c15e4cf688eccdbea4a0c8ad51488f19e2e288357238008067f7ab93af8b10`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:31:53 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:31:56 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:34:08 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:34:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c078c711fb6c8ce9576f8dd2c9a5bc7b27c4028c2cc4ecf73fa51496dfddb37`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3f3a64fffd4a6b075410687ff920992b8d532eee734f01a23c8b4acd6eeee`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf511001abbb952897431c950e3ce3c8767038aa724abbc790a05b468dcfbb4`  
		Last Modified: Wed, 11 Aug 2021 16:43:52 GMT  
		Size: 133.5 MB (133458221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d79499293ab2e6910164de236be148ac8a632bf1a159adc08f9c30dedfcb80`  
		Last Modified: Wed, 11 Aug 2021 16:43:22 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:618c3ee48853b47e4e32cfa9e19030156d259020ca9c43a31a495711ae5be225
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `julia:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull julia@sha256:44f4d3bfb9ba8c20d0f791831e0317e698bddf73b22c54bc48951ac0bf399fe8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6408877306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9866121315e46465b3db7d8253e9835d6b32ff8810ee9b62e6c8f2f40a9165a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 16:34:22 GMT
ENV JULIA_VERSION=1.6.2
# Wed, 11 Aug 2021 16:34:26 GMT
ENV JULIA_SHA256=380115d80e2f0bebe1885b80f67cf9330b659722f50608495962ab3a00e02977
# Wed, 11 Aug 2021 16:37:12 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 16:37:16 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf4d37a068724cf088d64b143f952d057279607a5ea96202c171ccc235e0d10`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7527903790dab1fed6f1b33403b2f51147576eba5f0e57003265456f301d580e`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beab471f1cddf276909b1df5e600fcf90f396cf1992ce340206ac53a217204dc`  
		Last Modified: Wed, 11 Aug 2021 16:46:54 GMT  
		Size: 137.9 MB (137905576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347992b07a31f90c28cc76bdb461185c0c4b6788d9531dc59d27d832312174f5`  
		Last Modified: Wed, 11 Aug 2021 16:44:08 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
