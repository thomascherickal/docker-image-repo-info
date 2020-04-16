<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `julia`

-	[`julia:1`](#julia1)
-	[`julia:1.0`](#julia10)
-	[`julia:1.0.5`](#julia105)
-	[`julia:1.0.5-buster`](#julia105-buster)
-	[`julia:1.0.5-stretch`](#julia105-stretch)
-	[`julia:1.0.5-windowsservercore-1809`](#julia105-windowsservercore-1809)
-	[`julia:1.0.5-windowsservercore-ltsc2016`](#julia105-windowsservercore-ltsc2016)
-	[`julia:1.0-buster`](#julia10-buster)
-	[`julia:1.0-stretch`](#julia10-stretch)
-	[`julia:1.0-windowsservercore-1809`](#julia10-windowsservercore-1809)
-	[`julia:1.0-windowsservercore-ltsc2016`](#julia10-windowsservercore-ltsc2016)
-	[`julia:1.4`](#julia14)
-	[`julia:1.4.0`](#julia140)
-	[`julia:1.4.0-buster`](#julia140-buster)
-	[`julia:1.4.0-windowsservercore-1809`](#julia140-windowsservercore-1809)
-	[`julia:1.4.0-windowsservercore-ltsc2016`](#julia140-windowsservercore-ltsc2016)
-	[`julia:1.4-buster`](#julia14-buster)
-	[`julia:1.4-windowsservercore-1809`](#julia14-windowsservercore-1809)
-	[`julia:1.4-windowsservercore-ltsc2016`](#julia14-windowsservercore-ltsc2016)
-	[`julia:1-buster`](#julia1-buster)
-	[`julia:1-windowsservercore-1809`](#julia1-windowsservercore-1809)
-	[`julia:1-windowsservercore-ltsc2016`](#julia1-windowsservercore-ltsc2016)
-	[`julia:buster`](#juliabuster)
-	[`julia:latest`](#julialatest)
-	[`julia:windowsservercore-1809`](#juliawindowsservercore-1809)
-	[`julia:windowsservercore-ltsc2016`](#juliawindowsservercore-ltsc2016)

## `julia:1`

```console
$ docker pull julia@sha256:d041f4a94d00a7b0e2634045cd422b7fa97edef601a48894ab045c55b31f1ae9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `julia:1` - linux; amd64

```console
$ docker pull julia@sha256:98b9f4174aee469d83a3d6c8c46d0fd9c1a6ef95f7fcf0a3e8e1b20aa01d4988
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138323266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18183d0f0d8119399633e1baabfd1092b030b9b48d98290b15676c3cfa06b283`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:09:46 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:20:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364e671b6375d1b6ec0a9a1d40cdab37905fa8dfaa094127586381c6f867ae36`  
		Last Modified: Mon, 06 Apr 2020 23:20:50 GMT  
		Size: 106.8 MB (106794820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm variant v7

```console
$ docker pull julia@sha256:0ac7eb3ba05168cd26791bb2e36436f2fa132b37f0776a9b39fb36214bb93f47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123503508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f5de0dda095868608104228885ffc09b658a247d7720b16fc63282f0f26238`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:25:49 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 04:26:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:26:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0230b466eb1f16bd472b786b23f9da3b9174ac5b23eab9e862321830d0c2d0e`  
		Last Modified: Thu, 16 Apr 2020 04:29:15 GMT  
		Size: 97.0 MB (97014701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a10a693db14af0d554aa7b98379fc4b4c8717d239186ea58c5f36f999e038229
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119875470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102fa2b9dd57d9ddb7762e531e4757d83f221990dee3606caa028c6839c2908f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:01:25 GMT
ENV JULIA_VERSION=1.4.0
# Tue, 07 Apr 2020 00:44:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Apr 2020 00:44:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e431814eaafc5d057cf00cdcafa51c860fb428bf78ff92489102a2e0f9712c8`  
		Last Modified: Tue, 07 Apr 2020 00:45:18 GMT  
		Size: 89.7 MB (89708315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:fb09607a2c0f0ff09e2ca51ffe314721d2708313b20bb41d05edbbad1b0285ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135745740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d0a3d12891fdd339b3bb182b7db7ecfc83e0979dc3ad4f6a914ae74a3f96f6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:27 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:38:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:38:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f23a5e87a61c1beb0e0fbcbd325e86d325f9d2737b674c120dd486c8699396`  
		Last Modified: Mon, 06 Apr 2020 23:39:33 GMT  
		Size: 103.4 MB (103411717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:73899dda58739417bedc7db11486dc30cdb3da1f37fb14d5b21473d11e609b13
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5862126325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a2078b38cb3b41f4a03539a1f6c4b3004fa67d2ca6b5594c396da81e1c2c0b`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:33:36 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:33:37 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 15:36:28 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 15:36:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f038398c36fe8c9f122b2c320286deb8340ad4bfb15151c7f0003b30a446a5`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc10fd05f63ed1f8c894e879f5b7e265e57eba8c14fd15dec49febcc9d9a4c50`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdbe481149c0c0461929bedd602d9e61479caa109e234b517e2b5ab9fe67a5`  
		Last Modified: Wed, 15 Apr 2020 16:17:45 GMT  
		Size: 134.1 MB (134054202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df348e63ef1f9d6be06ba680c38dd8277df605185deb68d67a49e0ae50436a1a`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:1e33b6e7007a2f411de49d7b1a0f7e803fb903c85fae39b26a499bd7627bb628
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2404042630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c55b7e7389c5a36e6037e0e789d97bef87e8e8036194f157e4a1848622b4c0c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:36:48 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:36:49 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 16:09:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:09:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef82f9deae85c127a0081ef3def77db201036d2e40fc3c59d76d5a9479ffe8`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2578c185ed18752b07b8d9a71d93a1fdb3707a17661f7e9aca7dc773371628a9`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb745a5e60aaa23fe0b0860d65adf83ee9f0415022f23f35d34dd993877b06`  
		Last Modified: Wed, 15 Apr 2020 16:18:29 GMT  
		Size: 133.3 MB (133330862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842173cc65f3b5379978f761a13c39c00bc69db010d3f1475329c69a8f6dec0`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0`

```console
$ docker pull julia@sha256:7f9ebb2f9852aec8a8b895a04fc781c3996795fea2f4c1bcde44b7cf36bc8138
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `julia:1.0` - linux; amd64

```console
$ docker pull julia@sha256:2a06370da23d782108c0732072af7f9bd8b7e4637fb3c566518eadab25ad1452
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127091567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2b45ef2aee5caef759cec3135a8fe45aadd3622a3b0f32b3a64ab1f5f8fcff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:10:06 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 03:10:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 03:10:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47628d6c8460c838b670244642769e16d3fda363aaa38e3a15ace69770d32ae7`  
		Last Modified: Tue, 31 Mar 2020 03:12:47 GMT  
		Size: 95.6 MB (95563121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm variant v7

```console
$ docker pull julia@sha256:75b7ce521343f133276fe003ec3f45049c28229c3917d2a87a04df5a11ee6e56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113617564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d520aea8b3e10328c36ed39bff20260c9a2c5f325dada3bee03825bdfd85b3`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:26:42 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 16 Apr 2020 04:27:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:27:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f84f27cb050c6c80eaa3f030e663d1f379434c7eb723ecd961960cca94ce23`  
		Last Modified: Thu, 16 Apr 2020 04:29:56 GMT  
		Size: 87.1 MB (87128757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:e51be36c62c43437e8545d96dca91a4d8ffcfa69de20ca8a194d2a188ce4f284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110058209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db7f8cac7240d993e5a99a10e525f4dbe9252c4fd0893af10a821803c0ff0a2f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:02:15 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 05:02:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 05:02:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0331b401a52b08506234031b6eee798966f847554f590eeeb5ecca88f452ee9d`  
		Last Modified: Tue, 31 Mar 2020 05:05:01 GMT  
		Size: 79.9 MB (79891054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; 386

```console
$ docker pull julia@sha256:4d1091e0130d722328e51323bd017ae3123bffb54c505947b83080016f58d5c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124832456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2a2be245b976227c78c02e70504f280bb9d531a8e7d23c72bc42d187240f32`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:50 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 01:06:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 01:06:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c736f77b2c39c0a7d673f69702b484cd32fd0ae06a2c41afbfdd09bd67a26a3f`  
		Last Modified: Tue, 31 Mar 2020 01:07:46 GMT  
		Size: 92.5 MB (92498433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:1674bdb64a13be8dd0ba1ed1ae5297600c359090114cf479e7ee78ad8a97c0a4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5835909745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38c7621840a1341adc13f5dc96a174c9049ae25e090a50762bbc848046035f7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 16:09:36 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Apr 2020 16:09:37 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 15 Apr 2020 16:12:19 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:12:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9783a626bfc6c492e88d93634cd51b0db5500193ddc79fec9e60483a136fd44f`  
		Last Modified: Wed, 15 Apr 2020 16:18:46 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f74b39daa13501d036cac058e6e9ba589ecf851154e194d38a0e5513398e5d5`  
		Last Modified: Wed, 15 Apr 2020 16:18:47 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8731473ab072a405f24c4d785b331ca3426e5a6ee4530c4a4c8db95238ab8f`  
		Last Modified: Wed, 15 Apr 2020 16:20:49 GMT  
		Size: 107.8 MB (107837593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e106b6892877a7ece24dc8a1b93d6558d7f4291002d73b115629e6468a367f`  
		Last Modified: Wed, 15 Apr 2020 16:18:46 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:6d1fcd8c3852d82ed2106a3864f1988f4c2b5abb9468d39c21949b747acc078a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2373324090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c557ea613ed973fefc9515f7d983425cb0aa38a06022753a4a33c4dfde3229c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 16:12:31 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Apr 2020 16:12:32 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 15 Apr 2020 16:14:40 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:14:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c87e61e215534fa0ea052587f742ba88472509be46c78a7cc75d7ed0053b17`  
		Last Modified: Wed, 15 Apr 2020 16:21:01 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bcde73013f768a9f44196664367e81b4f43c0b882e570853af0bf59948fe5a`  
		Last Modified: Wed, 15 Apr 2020 16:21:01 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb83cc8dbfc7bab88eb17aa225d5613c093fb8b5710136f27532a8c834b84c5`  
		Last Modified: Wed, 15 Apr 2020 16:21:24 GMT  
		Size: 102.6 MB (102612307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1827d03c2ba71b8c71cac7bdcc334d9a0ef28fa9f624767395c9ed6901f2189`  
		Last Modified: Wed, 15 Apr 2020 16:21:00 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5`

```console
$ docker pull julia@sha256:7f9ebb2f9852aec8a8b895a04fc781c3996795fea2f4c1bcde44b7cf36bc8138
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `julia:1.0.5` - linux; amd64

```console
$ docker pull julia@sha256:2a06370da23d782108c0732072af7f9bd8b7e4637fb3c566518eadab25ad1452
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127091567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2b45ef2aee5caef759cec3135a8fe45aadd3622a3b0f32b3a64ab1f5f8fcff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:10:06 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 03:10:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 03:10:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47628d6c8460c838b670244642769e16d3fda363aaa38e3a15ace69770d32ae7`  
		Last Modified: Tue, 31 Mar 2020 03:12:47 GMT  
		Size: 95.6 MB (95563121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm variant v7

```console
$ docker pull julia@sha256:75b7ce521343f133276fe003ec3f45049c28229c3917d2a87a04df5a11ee6e56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113617564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d520aea8b3e10328c36ed39bff20260c9a2c5f325dada3bee03825bdfd85b3`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:26:42 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 16 Apr 2020 04:27:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:27:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f84f27cb050c6c80eaa3f030e663d1f379434c7eb723ecd961960cca94ce23`  
		Last Modified: Thu, 16 Apr 2020 04:29:56 GMT  
		Size: 87.1 MB (87128757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:e51be36c62c43437e8545d96dca91a4d8ffcfa69de20ca8a194d2a188ce4f284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110058209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db7f8cac7240d993e5a99a10e525f4dbe9252c4fd0893af10a821803c0ff0a2f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:02:15 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 05:02:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 05:02:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0331b401a52b08506234031b6eee798966f847554f590eeeb5ecca88f452ee9d`  
		Last Modified: Tue, 31 Mar 2020 05:05:01 GMT  
		Size: 79.9 MB (79891054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; 386

```console
$ docker pull julia@sha256:4d1091e0130d722328e51323bd017ae3123bffb54c505947b83080016f58d5c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124832456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2a2be245b976227c78c02e70504f280bb9d531a8e7d23c72bc42d187240f32`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:50 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 01:06:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 01:06:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c736f77b2c39c0a7d673f69702b484cd32fd0ae06a2c41afbfdd09bd67a26a3f`  
		Last Modified: Tue, 31 Mar 2020 01:07:46 GMT  
		Size: 92.5 MB (92498433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:1674bdb64a13be8dd0ba1ed1ae5297600c359090114cf479e7ee78ad8a97c0a4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5835909745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38c7621840a1341adc13f5dc96a174c9049ae25e090a50762bbc848046035f7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 16:09:36 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Apr 2020 16:09:37 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 15 Apr 2020 16:12:19 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:12:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9783a626bfc6c492e88d93634cd51b0db5500193ddc79fec9e60483a136fd44f`  
		Last Modified: Wed, 15 Apr 2020 16:18:46 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f74b39daa13501d036cac058e6e9ba589ecf851154e194d38a0e5513398e5d5`  
		Last Modified: Wed, 15 Apr 2020 16:18:47 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8731473ab072a405f24c4d785b331ca3426e5a6ee4530c4a4c8db95238ab8f`  
		Last Modified: Wed, 15 Apr 2020 16:20:49 GMT  
		Size: 107.8 MB (107837593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e106b6892877a7ece24dc8a1b93d6558d7f4291002d73b115629e6468a367f`  
		Last Modified: Wed, 15 Apr 2020 16:18:46 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:6d1fcd8c3852d82ed2106a3864f1988f4c2b5abb9468d39c21949b747acc078a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2373324090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c557ea613ed973fefc9515f7d983425cb0aa38a06022753a4a33c4dfde3229c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 16:12:31 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Apr 2020 16:12:32 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 15 Apr 2020 16:14:40 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:14:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c87e61e215534fa0ea052587f742ba88472509be46c78a7cc75d7ed0053b17`  
		Last Modified: Wed, 15 Apr 2020 16:21:01 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bcde73013f768a9f44196664367e81b4f43c0b882e570853af0bf59948fe5a`  
		Last Modified: Wed, 15 Apr 2020 16:21:01 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb83cc8dbfc7bab88eb17aa225d5613c093fb8b5710136f27532a8c834b84c5`  
		Last Modified: Wed, 15 Apr 2020 16:21:24 GMT  
		Size: 102.6 MB (102612307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1827d03c2ba71b8c71cac7bdcc334d9a0ef28fa9f624767395c9ed6901f2189`  
		Last Modified: Wed, 15 Apr 2020 16:21:00 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-buster`

```console
$ docker pull julia@sha256:c955f5236d77d2f7e64ef68db2e437339ce90bf02e5797c47e858e505e9da4a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-buster` - linux; amd64

```console
$ docker pull julia@sha256:2a06370da23d782108c0732072af7f9bd8b7e4637fb3c566518eadab25ad1452
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127091567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2b45ef2aee5caef759cec3135a8fe45aadd3622a3b0f32b3a64ab1f5f8fcff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:10:06 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 03:10:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 03:10:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47628d6c8460c838b670244642769e16d3fda363aaa38e3a15ace69770d32ae7`  
		Last Modified: Tue, 31 Mar 2020 03:12:47 GMT  
		Size: 95.6 MB (95563121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:75b7ce521343f133276fe003ec3f45049c28229c3917d2a87a04df5a11ee6e56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113617564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d520aea8b3e10328c36ed39bff20260c9a2c5f325dada3bee03825bdfd85b3`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:26:42 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 16 Apr 2020 04:27:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:27:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f84f27cb050c6c80eaa3f030e663d1f379434c7eb723ecd961960cca94ce23`  
		Last Modified: Thu, 16 Apr 2020 04:29:56 GMT  
		Size: 87.1 MB (87128757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:e51be36c62c43437e8545d96dca91a4d8ffcfa69de20ca8a194d2a188ce4f284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110058209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db7f8cac7240d993e5a99a10e525f4dbe9252c4fd0893af10a821803c0ff0a2f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:02:15 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 05:02:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 05:02:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0331b401a52b08506234031b6eee798966f847554f590eeeb5ecca88f452ee9d`  
		Last Modified: Tue, 31 Mar 2020 05:05:01 GMT  
		Size: 79.9 MB (79891054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; 386

```console
$ docker pull julia@sha256:4d1091e0130d722328e51323bd017ae3123bffb54c505947b83080016f58d5c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124832456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2a2be245b976227c78c02e70504f280bb9d531a8e7d23c72bc42d187240f32`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:50 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 01:06:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 01:06:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c736f77b2c39c0a7d673f69702b484cd32fd0ae06a2c41afbfdd09bd67a26a3f`  
		Last Modified: Tue, 31 Mar 2020 01:07:46 GMT  
		Size: 92.5 MB (92498433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-stretch`

```console
$ docker pull julia@sha256:707b42a3b6299cb939fb060e8c8b68d56b1809f81a09d813bbdb7dc0ade6b335
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-stretch` - linux; amd64

```console
$ docker pull julia@sha256:2b2bdfdbb79c80f4b6c5429255e030fc43a3c22bd9211da35451f1c401ab1bd9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150462359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab155a20c23e928df7f77391605a2dcb28b670fb8a69443fd76e58c3f66adc24`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:23:50 GMT
ADD file:774b5e2033bb42ad97daa64267a5f041124cc0b05ec0198f1b5578ceea5a48e4 in / 
# Tue, 31 Mar 2020 01:23:51 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:10:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:10:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:10:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:10:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:10:52 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 03:11:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 03:11:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:56da78ce36e97a8ba1f860575bb1422d1cb6ab4dade70b06ddf1651302dde955`  
		Last Modified: Tue, 31 Mar 2020 01:29:15 GMT  
		Size: 45.4 MB (45375928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caae116d1f2e04bd2bb34f461207f1678ffbd1055cac4261fc47c26bfd09ecec`  
		Last Modified: Tue, 31 Mar 2020 03:12:54 GMT  
		Size: 9.5 MB (9512490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc4ee952d08081e65a7a25f118cda93d54cd4e1095f51399fca929ce8af4ec7`  
		Last Modified: Tue, 31 Mar 2020 03:13:16 GMT  
		Size: 95.6 MB (95573941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:5b84a10f822b25848ea3fabc8bc6086581128ecd3b156c1f54b856ece255c213
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137475536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ed8e99447aa20809833a8be698edfaddce2888aa9b42cab044b3c7aca1beea`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 01:04:37 GMT
ADD file:b83ed4f9f7c8b10eba728f85030722a771b39336afd7ff9eef2eb6b94791533e in / 
# Thu, 16 Apr 2020 01:04:40 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:27:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:27:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:27:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:27:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:27:54 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 16 Apr 2020 04:28:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:28:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:37d8a5aac9ec54f7757e1243cff051c8372be0cf907e086fba2607e08d2a4135`  
		Last Modified: Thu, 16 Apr 2020 01:12:16 GMT  
		Size: 42.1 MB (42101227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef7d5f25fea236330cff3e861fb0b9ba3fea72a068f04f41052cdf983b4b6ea`  
		Last Modified: Thu, 16 Apr 2020 04:30:04 GMT  
		Size: 8.2 MB (8236420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33e6e0c3d457486bd1bbaa1293f5284cae17e122303e00c6c0f3688c2682bef`  
		Last Modified: Thu, 16 Apr 2020 04:30:33 GMT  
		Size: 87.1 MB (87137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:64780dcf9dde72ea1d13eeb38426159f503c66f5c8cb5fc89fb7e3b1dd03714b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131542888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50141ed73b125c08cdb905970f9814272b2233356ef817714b774e2b1ef434ad`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:08:11 GMT
ADD file:ab80e35f9496440fac439083c9c9c18cd80521039d4bc4f4082e8e84a5e9fcda in / 
# Tue, 31 Mar 2020 02:08:15 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:03:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:03:14 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:03:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:03:15 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:03:16 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 05:03:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 05:03:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:84582781a9f06ad84225307f9cf89d5f77f6e5610281e6ca088fc8c2e9a1d027`  
		Last Modified: Tue, 31 Mar 2020 02:14:13 GMT  
		Size: 43.2 MB (43158116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070099fd0c601859f7343963cb68e812f0a3f9d28f51692f4b6724163810f797`  
		Last Modified: Tue, 31 Mar 2020 05:05:12 GMT  
		Size: 8.5 MB (8475542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d14b70fb1b508a370e075af661c60d29bf03f87d88f83f12315aa274e5c93b`  
		Last Modified: Tue, 31 Mar 2020 05:05:35 GMT  
		Size: 79.9 MB (79909230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; 386

```console
$ docker pull julia@sha256:11951e55331a4ab948ae1d2251e1d4b984a80f51dc18e3deb4a13e7356082a91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148115515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:516139a7db9645d481dc83d3de07d0b66641a7be8d61f6feae38c167a4856902`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:42:34 GMT
ADD file:a2d15d4f5721611194d2e75c068cf76220a1fd273b28e60afc9d97c41920f37b in / 
# Tue, 31 Mar 2020 00:42:34 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:06:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:06:22 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:06:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:06:23 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:06:23 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 01:06:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 01:06:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e23f42c0de4ea650702adc216b9d71349a24439e774c0bbbb00d2ad19aa304df`  
		Last Modified: Tue, 31 Mar 2020 00:48:31 GMT  
		Size: 46.1 MB (46095182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94b8e22825a1c08e3ff89c71100144c828d6ce65a471c0dbe8436d1bae4a95`  
		Last Modified: Tue, 31 Mar 2020 01:07:54 GMT  
		Size: 9.5 MB (9518564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de53669bf41db847593fe23c9add4ef17c241fc3907cf637acaf9b9856b9eac6`  
		Last Modified: Tue, 31 Mar 2020 01:08:13 GMT  
		Size: 92.5 MB (92501769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-1809`

```console
$ docker pull julia@sha256:fcf962fbc743de075477cea3ea12b929d74c96a66c2f81e3d5f7820e5a3262b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `julia:1.0.5-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:6d1fcd8c3852d82ed2106a3864f1988f4c2b5abb9468d39c21949b747acc078a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2373324090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c557ea613ed973fefc9515f7d983425cb0aa38a06022753a4a33c4dfde3229c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 16:12:31 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Apr 2020 16:12:32 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 15 Apr 2020 16:14:40 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:14:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c87e61e215534fa0ea052587f742ba88472509be46c78a7cc75d7ed0053b17`  
		Last Modified: Wed, 15 Apr 2020 16:21:01 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bcde73013f768a9f44196664367e81b4f43c0b882e570853af0bf59948fe5a`  
		Last Modified: Wed, 15 Apr 2020 16:21:01 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb83cc8dbfc7bab88eb17aa225d5613c093fb8b5710136f27532a8c834b84c5`  
		Last Modified: Wed, 15 Apr 2020 16:21:24 GMT  
		Size: 102.6 MB (102612307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1827d03c2ba71b8c71cac7bdcc334d9a0ef28fa9f624767395c9ed6901f2189`  
		Last Modified: Wed, 15 Apr 2020 16:21:00 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:3d2e0ed851bee2a39078b39ae18888c57e7df5a1f782ba25f83a98d3efb3bde7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `julia:1.0.5-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:1674bdb64a13be8dd0ba1ed1ae5297600c359090114cf479e7ee78ad8a97c0a4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5835909745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38c7621840a1341adc13f5dc96a174c9049ae25e090a50762bbc848046035f7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 16:09:36 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Apr 2020 16:09:37 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 15 Apr 2020 16:12:19 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:12:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9783a626bfc6c492e88d93634cd51b0db5500193ddc79fec9e60483a136fd44f`  
		Last Modified: Wed, 15 Apr 2020 16:18:46 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f74b39daa13501d036cac058e6e9ba589ecf851154e194d38a0e5513398e5d5`  
		Last Modified: Wed, 15 Apr 2020 16:18:47 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8731473ab072a405f24c4d785b331ca3426e5a6ee4530c4a4c8db95238ab8f`  
		Last Modified: Wed, 15 Apr 2020 16:20:49 GMT  
		Size: 107.8 MB (107837593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e106b6892877a7ece24dc8a1b93d6558d7f4291002d73b115629e6468a367f`  
		Last Modified: Wed, 15 Apr 2020 16:18:46 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-buster`

```console
$ docker pull julia@sha256:c955f5236d77d2f7e64ef68db2e437339ce90bf02e5797c47e858e505e9da4a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:2a06370da23d782108c0732072af7f9bd8b7e4637fb3c566518eadab25ad1452
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127091567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2b45ef2aee5caef759cec3135a8fe45aadd3622a3b0f32b3a64ab1f5f8fcff`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:10:06 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 03:10:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 03:10:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47628d6c8460c838b670244642769e16d3fda363aaa38e3a15ace69770d32ae7`  
		Last Modified: Tue, 31 Mar 2020 03:12:47 GMT  
		Size: 95.6 MB (95563121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:75b7ce521343f133276fe003ec3f45049c28229c3917d2a87a04df5a11ee6e56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113617564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d520aea8b3e10328c36ed39bff20260c9a2c5f325dada3bee03825bdfd85b3`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:26:42 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 16 Apr 2020 04:27:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:27:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f84f27cb050c6c80eaa3f030e663d1f379434c7eb723ecd961960cca94ce23`  
		Last Modified: Thu, 16 Apr 2020 04:29:56 GMT  
		Size: 87.1 MB (87128757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:e51be36c62c43437e8545d96dca91a4d8ffcfa69de20ca8a194d2a188ce4f284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110058209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db7f8cac7240d993e5a99a10e525f4dbe9252c4fd0893af10a821803c0ff0a2f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:02:15 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 05:02:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 05:02:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0331b401a52b08506234031b6eee798966f847554f590eeeb5ecca88f452ee9d`  
		Last Modified: Tue, 31 Mar 2020 05:05:01 GMT  
		Size: 79.9 MB (79891054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; 386

```console
$ docker pull julia@sha256:4d1091e0130d722328e51323bd017ae3123bffb54c505947b83080016f58d5c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124832456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2a2be245b976227c78c02e70504f280bb9d531a8e7d23c72bc42d187240f32`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:50 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 01:06:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 01:06:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c736f77b2c39c0a7d673f69702b484cd32fd0ae06a2c41afbfdd09bd67a26a3f`  
		Last Modified: Tue, 31 Mar 2020 01:07:46 GMT  
		Size: 92.5 MB (92498433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-stretch`

```console
$ docker pull julia@sha256:707b42a3b6299cb939fb060e8c8b68d56b1809f81a09d813bbdb7dc0ade6b335
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-stretch` - linux; amd64

```console
$ docker pull julia@sha256:2b2bdfdbb79c80f4b6c5429255e030fc43a3c22bd9211da35451f1c401ab1bd9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150462359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab155a20c23e928df7f77391605a2dcb28b670fb8a69443fd76e58c3f66adc24`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:23:50 GMT
ADD file:774b5e2033bb42ad97daa64267a5f041124cc0b05ec0198f1b5578ceea5a48e4 in / 
# Tue, 31 Mar 2020 01:23:51 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:10:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:10:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:10:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:10:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:10:52 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 03:11:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 03:11:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:56da78ce36e97a8ba1f860575bb1422d1cb6ab4dade70b06ddf1651302dde955`  
		Last Modified: Tue, 31 Mar 2020 01:29:15 GMT  
		Size: 45.4 MB (45375928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caae116d1f2e04bd2bb34f461207f1678ffbd1055cac4261fc47c26bfd09ecec`  
		Last Modified: Tue, 31 Mar 2020 03:12:54 GMT  
		Size: 9.5 MB (9512490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc4ee952d08081e65a7a25f118cda93d54cd4e1095f51399fca929ce8af4ec7`  
		Last Modified: Tue, 31 Mar 2020 03:13:16 GMT  
		Size: 95.6 MB (95573941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:5b84a10f822b25848ea3fabc8bc6086581128ecd3b156c1f54b856ece255c213
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137475536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ed8e99447aa20809833a8be698edfaddce2888aa9b42cab044b3c7aca1beea`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 01:04:37 GMT
ADD file:b83ed4f9f7c8b10eba728f85030722a771b39336afd7ff9eef2eb6b94791533e in / 
# Thu, 16 Apr 2020 01:04:40 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:27:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:27:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:27:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:27:53 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:27:54 GMT
ENV JULIA_VERSION=1.0.5
# Thu, 16 Apr 2020 04:28:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:28:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:37d8a5aac9ec54f7757e1243cff051c8372be0cf907e086fba2607e08d2a4135`  
		Last Modified: Thu, 16 Apr 2020 01:12:16 GMT  
		Size: 42.1 MB (42101227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef7d5f25fea236330cff3e861fb0b9ba3fea72a068f04f41052cdf983b4b6ea`  
		Last Modified: Thu, 16 Apr 2020 04:30:04 GMT  
		Size: 8.2 MB (8236420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33e6e0c3d457486bd1bbaa1293f5284cae17e122303e00c6c0f3688c2682bef`  
		Last Modified: Thu, 16 Apr 2020 04:30:33 GMT  
		Size: 87.1 MB (87137889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:64780dcf9dde72ea1d13eeb38426159f503c66f5c8cb5fc89fb7e3b1dd03714b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131542888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50141ed73b125c08cdb905970f9814272b2233356ef817714b774e2b1ef434ad`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:08:11 GMT
ADD file:ab80e35f9496440fac439083c9c9c18cd80521039d4bc4f4082e8e84a5e9fcda in / 
# Tue, 31 Mar 2020 02:08:15 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:03:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:03:14 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:03:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:03:15 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:03:16 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 05:03:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 05:03:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:84582781a9f06ad84225307f9cf89d5f77f6e5610281e6ca088fc8c2e9a1d027`  
		Last Modified: Tue, 31 Mar 2020 02:14:13 GMT  
		Size: 43.2 MB (43158116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070099fd0c601859f7343963cb68e812f0a3f9d28f51692f4b6724163810f797`  
		Last Modified: Tue, 31 Mar 2020 05:05:12 GMT  
		Size: 8.5 MB (8475542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d14b70fb1b508a370e075af661c60d29bf03f87d88f83f12315aa274e5c93b`  
		Last Modified: Tue, 31 Mar 2020 05:05:35 GMT  
		Size: 79.9 MB (79909230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; 386

```console
$ docker pull julia@sha256:11951e55331a4ab948ae1d2251e1d4b984a80f51dc18e3deb4a13e7356082a91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148115515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:516139a7db9645d481dc83d3de07d0b66641a7be8d61f6feae38c167a4856902`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:42:34 GMT
ADD file:a2d15d4f5721611194d2e75c068cf76220a1fd273b28e60afc9d97c41920f37b in / 
# Tue, 31 Mar 2020 00:42:34 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:06:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:06:22 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:06:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:06:23 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:06:23 GMT
ENV JULIA_VERSION=1.0.5
# Tue, 31 Mar 2020 01:06:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 31 Mar 2020 01:06:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e23f42c0de4ea650702adc216b9d71349a24439e774c0bbbb00d2ad19aa304df`  
		Last Modified: Tue, 31 Mar 2020 00:48:31 GMT  
		Size: 46.1 MB (46095182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94b8e22825a1c08e3ff89c71100144c828d6ce65a471c0dbe8436d1bae4a95`  
		Last Modified: Tue, 31 Mar 2020 01:07:54 GMT  
		Size: 9.5 MB (9518564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de53669bf41db847593fe23c9add4ef17c241fc3907cf637acaf9b9856b9eac6`  
		Last Modified: Tue, 31 Mar 2020 01:08:13 GMT  
		Size: 92.5 MB (92501769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:fcf962fbc743de075477cea3ea12b929d74c96a66c2f81e3d5f7820e5a3262b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `julia:1.0-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:6d1fcd8c3852d82ed2106a3864f1988f4c2b5abb9468d39c21949b747acc078a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2373324090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c557ea613ed973fefc9515f7d983425cb0aa38a06022753a4a33c4dfde3229c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 16:12:31 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Apr 2020 16:12:32 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 15 Apr 2020 16:14:40 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:14:42 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c87e61e215534fa0ea052587f742ba88472509be46c78a7cc75d7ed0053b17`  
		Last Modified: Wed, 15 Apr 2020 16:21:01 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bcde73013f768a9f44196664367e81b4f43c0b882e570853af0bf59948fe5a`  
		Last Modified: Wed, 15 Apr 2020 16:21:01 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb83cc8dbfc7bab88eb17aa225d5613c093fb8b5710136f27532a8c834b84c5`  
		Last Modified: Wed, 15 Apr 2020 16:21:24 GMT  
		Size: 102.6 MB (102612307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1827d03c2ba71b8c71cac7bdcc334d9a0ef28fa9f624767395c9ed6901f2189`  
		Last Modified: Wed, 15 Apr 2020 16:21:00 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:3d2e0ed851bee2a39078b39ae18888c57e7df5a1f782ba25f83a98d3efb3bde7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `julia:1.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:1674bdb64a13be8dd0ba1ed1ae5297600c359090114cf479e7ee78ad8a97c0a4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5835909745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38c7621840a1341adc13f5dc96a174c9049ae25e090a50762bbc848046035f7`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 16:09:36 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 15 Apr 2020 16:09:37 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 15 Apr 2020 16:12:19 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/S', 			'/D=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:12:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9783a626bfc6c492e88d93634cd51b0db5500193ddc79fec9e60483a136fd44f`  
		Last Modified: Wed, 15 Apr 2020 16:18:46 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f74b39daa13501d036cac058e6e9ba589ecf851154e194d38a0e5513398e5d5`  
		Last Modified: Wed, 15 Apr 2020 16:18:47 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8731473ab072a405f24c4d785b331ca3426e5a6ee4530c4a4c8db95238ab8f`  
		Last Modified: Wed, 15 Apr 2020 16:20:49 GMT  
		Size: 107.8 MB (107837593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e106b6892877a7ece24dc8a1b93d6558d7f4291002d73b115629e6468a367f`  
		Last Modified: Wed, 15 Apr 2020 16:18:46 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4`

```console
$ docker pull julia@sha256:d041f4a94d00a7b0e2634045cd422b7fa97edef601a48894ab045c55b31f1ae9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `julia:1.4` - linux; amd64

```console
$ docker pull julia@sha256:98b9f4174aee469d83a3d6c8c46d0fd9c1a6ef95f7fcf0a3e8e1b20aa01d4988
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138323266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18183d0f0d8119399633e1baabfd1092b030b9b48d98290b15676c3cfa06b283`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:09:46 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:20:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364e671b6375d1b6ec0a9a1d40cdab37905fa8dfaa094127586381c6f867ae36`  
		Last Modified: Mon, 06 Apr 2020 23:20:50 GMT  
		Size: 106.8 MB (106794820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4` - linux; arm variant v7

```console
$ docker pull julia@sha256:0ac7eb3ba05168cd26791bb2e36436f2fa132b37f0776a9b39fb36214bb93f47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123503508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f5de0dda095868608104228885ffc09b658a247d7720b16fc63282f0f26238`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:25:49 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 04:26:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:26:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0230b466eb1f16bd472b786b23f9da3b9174ac5b23eab9e862321830d0c2d0e`  
		Last Modified: Thu, 16 Apr 2020 04:29:15 GMT  
		Size: 97.0 MB (97014701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a10a693db14af0d554aa7b98379fc4b4c8717d239186ea58c5f36f999e038229
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119875470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102fa2b9dd57d9ddb7762e531e4757d83f221990dee3606caa028c6839c2908f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:01:25 GMT
ENV JULIA_VERSION=1.4.0
# Tue, 07 Apr 2020 00:44:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Apr 2020 00:44:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e431814eaafc5d057cf00cdcafa51c860fb428bf78ff92489102a2e0f9712c8`  
		Last Modified: Tue, 07 Apr 2020 00:45:18 GMT  
		Size: 89.7 MB (89708315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4` - linux; 386

```console
$ docker pull julia@sha256:fb09607a2c0f0ff09e2ca51ffe314721d2708313b20bb41d05edbbad1b0285ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135745740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d0a3d12891fdd339b3bb182b7db7ecfc83e0979dc3ad4f6a914ae74a3f96f6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:27 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:38:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:38:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f23a5e87a61c1beb0e0fbcbd325e86d325f9d2737b674c120dd486c8699396`  
		Last Modified: Mon, 06 Apr 2020 23:39:33 GMT  
		Size: 103.4 MB (103411717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:73899dda58739417bedc7db11486dc30cdb3da1f37fb14d5b21473d11e609b13
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5862126325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a2078b38cb3b41f4a03539a1f6c4b3004fa67d2ca6b5594c396da81e1c2c0b`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:33:36 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:33:37 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 15:36:28 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 15:36:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f038398c36fe8c9f122b2c320286deb8340ad4bfb15151c7f0003b30a446a5`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc10fd05f63ed1f8c894e879f5b7e265e57eba8c14fd15dec49febcc9d9a4c50`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdbe481149c0c0461929bedd602d9e61479caa109e234b517e2b5ab9fe67a5`  
		Last Modified: Wed, 15 Apr 2020 16:17:45 GMT  
		Size: 134.1 MB (134054202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df348e63ef1f9d6be06ba680c38dd8277df605185deb68d67a49e0ae50436a1a`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:1e33b6e7007a2f411de49d7b1a0f7e803fb903c85fae39b26a499bd7627bb628
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2404042630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c55b7e7389c5a36e6037e0e789d97bef87e8e8036194f157e4a1848622b4c0c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:36:48 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:36:49 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 16:09:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:09:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef82f9deae85c127a0081ef3def77db201036d2e40fc3c59d76d5a9479ffe8`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2578c185ed18752b07b8d9a71d93a1fdb3707a17661f7e9aca7dc773371628a9`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb745a5e60aaa23fe0b0860d65adf83ee9f0415022f23f35d34dd993877b06`  
		Last Modified: Wed, 15 Apr 2020 16:18:29 GMT  
		Size: 133.3 MB (133330862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842173cc65f3b5379978f761a13c39c00bc69db010d3f1475329c69a8f6dec0`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0`

```console
$ docker pull julia@sha256:d041f4a94d00a7b0e2634045cd422b7fa97edef601a48894ab045c55b31f1ae9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `julia:1.4.0` - linux; amd64

```console
$ docker pull julia@sha256:98b9f4174aee469d83a3d6c8c46d0fd9c1a6ef95f7fcf0a3e8e1b20aa01d4988
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138323266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18183d0f0d8119399633e1baabfd1092b030b9b48d98290b15676c3cfa06b283`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:09:46 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:20:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364e671b6375d1b6ec0a9a1d40cdab37905fa8dfaa094127586381c6f867ae36`  
		Last Modified: Mon, 06 Apr 2020 23:20:50 GMT  
		Size: 106.8 MB (106794820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0` - linux; arm variant v7

```console
$ docker pull julia@sha256:0ac7eb3ba05168cd26791bb2e36436f2fa132b37f0776a9b39fb36214bb93f47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123503508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f5de0dda095868608104228885ffc09b658a247d7720b16fc63282f0f26238`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:25:49 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 04:26:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:26:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0230b466eb1f16bd472b786b23f9da3b9174ac5b23eab9e862321830d0c2d0e`  
		Last Modified: Thu, 16 Apr 2020 04:29:15 GMT  
		Size: 97.0 MB (97014701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a10a693db14af0d554aa7b98379fc4b4c8717d239186ea58c5f36f999e038229
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119875470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102fa2b9dd57d9ddb7762e531e4757d83f221990dee3606caa028c6839c2908f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:01:25 GMT
ENV JULIA_VERSION=1.4.0
# Tue, 07 Apr 2020 00:44:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Apr 2020 00:44:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e431814eaafc5d057cf00cdcafa51c860fb428bf78ff92489102a2e0f9712c8`  
		Last Modified: Tue, 07 Apr 2020 00:45:18 GMT  
		Size: 89.7 MB (89708315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0` - linux; 386

```console
$ docker pull julia@sha256:fb09607a2c0f0ff09e2ca51ffe314721d2708313b20bb41d05edbbad1b0285ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135745740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d0a3d12891fdd339b3bb182b7db7ecfc83e0979dc3ad4f6a914ae74a3f96f6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:27 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:38:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:38:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f23a5e87a61c1beb0e0fbcbd325e86d325f9d2737b674c120dd486c8699396`  
		Last Modified: Mon, 06 Apr 2020 23:39:33 GMT  
		Size: 103.4 MB (103411717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:73899dda58739417bedc7db11486dc30cdb3da1f37fb14d5b21473d11e609b13
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5862126325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a2078b38cb3b41f4a03539a1f6c4b3004fa67d2ca6b5594c396da81e1c2c0b`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:33:36 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:33:37 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 15:36:28 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 15:36:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f038398c36fe8c9f122b2c320286deb8340ad4bfb15151c7f0003b30a446a5`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc10fd05f63ed1f8c894e879f5b7e265e57eba8c14fd15dec49febcc9d9a4c50`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdbe481149c0c0461929bedd602d9e61479caa109e234b517e2b5ab9fe67a5`  
		Last Modified: Wed, 15 Apr 2020 16:17:45 GMT  
		Size: 134.1 MB (134054202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df348e63ef1f9d6be06ba680c38dd8277df605185deb68d67a49e0ae50436a1a`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:1e33b6e7007a2f411de49d7b1a0f7e803fb903c85fae39b26a499bd7627bb628
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2404042630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c55b7e7389c5a36e6037e0e789d97bef87e8e8036194f157e4a1848622b4c0c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:36:48 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:36:49 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 16:09:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:09:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef82f9deae85c127a0081ef3def77db201036d2e40fc3c59d76d5a9479ffe8`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2578c185ed18752b07b8d9a71d93a1fdb3707a17661f7e9aca7dc773371628a9`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb745a5e60aaa23fe0b0860d65adf83ee9f0415022f23f35d34dd993877b06`  
		Last Modified: Wed, 15 Apr 2020 16:18:29 GMT  
		Size: 133.3 MB (133330862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842173cc65f3b5379978f761a13c39c00bc69db010d3f1475329c69a8f6dec0`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0-buster`

```console
$ docker pull julia@sha256:85a0bb7cfc62976db640692c151c15840d47b825d76046b398e1cf941030b0b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.4.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:98b9f4174aee469d83a3d6c8c46d0fd9c1a6ef95f7fcf0a3e8e1b20aa01d4988
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138323266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18183d0f0d8119399633e1baabfd1092b030b9b48d98290b15676c3cfa06b283`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:09:46 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:20:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364e671b6375d1b6ec0a9a1d40cdab37905fa8dfaa094127586381c6f867ae36`  
		Last Modified: Mon, 06 Apr 2020 23:20:50 GMT  
		Size: 106.8 MB (106794820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:0ac7eb3ba05168cd26791bb2e36436f2fa132b37f0776a9b39fb36214bb93f47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123503508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f5de0dda095868608104228885ffc09b658a247d7720b16fc63282f0f26238`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:25:49 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 04:26:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:26:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0230b466eb1f16bd472b786b23f9da3b9174ac5b23eab9e862321830d0c2d0e`  
		Last Modified: Thu, 16 Apr 2020 04:29:15 GMT  
		Size: 97.0 MB (97014701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a10a693db14af0d554aa7b98379fc4b4c8717d239186ea58c5f36f999e038229
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119875470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102fa2b9dd57d9ddb7762e531e4757d83f221990dee3606caa028c6839c2908f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:01:25 GMT
ENV JULIA_VERSION=1.4.0
# Tue, 07 Apr 2020 00:44:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Apr 2020 00:44:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e431814eaafc5d057cf00cdcafa51c860fb428bf78ff92489102a2e0f9712c8`  
		Last Modified: Tue, 07 Apr 2020 00:45:18 GMT  
		Size: 89.7 MB (89708315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4.0-buster` - linux; 386

```console
$ docker pull julia@sha256:fb09607a2c0f0ff09e2ca51ffe314721d2708313b20bb41d05edbbad1b0285ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135745740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d0a3d12891fdd339b3bb182b7db7ecfc83e0979dc3ad4f6a914ae74a3f96f6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:27 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:38:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:38:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f23a5e87a61c1beb0e0fbcbd325e86d325f9d2737b674c120dd486c8699396`  
		Last Modified: Mon, 06 Apr 2020 23:39:33 GMT  
		Size: 103.4 MB (103411717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:68ed12481c16cccc92bc96490bedd9d624719211232264ae58afffa87edc079c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `julia:1.4.0-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:1e33b6e7007a2f411de49d7b1a0f7e803fb903c85fae39b26a499bd7627bb628
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2404042630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c55b7e7389c5a36e6037e0e789d97bef87e8e8036194f157e4a1848622b4c0c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:36:48 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:36:49 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 16:09:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:09:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef82f9deae85c127a0081ef3def77db201036d2e40fc3c59d76d5a9479ffe8`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2578c185ed18752b07b8d9a71d93a1fdb3707a17661f7e9aca7dc773371628a9`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb745a5e60aaa23fe0b0860d65adf83ee9f0415022f23f35d34dd993877b06`  
		Last Modified: Wed, 15 Apr 2020 16:18:29 GMT  
		Size: 133.3 MB (133330862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842173cc65f3b5379978f761a13c39c00bc69db010d3f1475329c69a8f6dec0`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:414c4d202386b41a8da6b5ea37fbb9416089f2ff701871c2e6b4530ad46fee65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `julia:1.4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:73899dda58739417bedc7db11486dc30cdb3da1f37fb14d5b21473d11e609b13
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5862126325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a2078b38cb3b41f4a03539a1f6c4b3004fa67d2ca6b5594c396da81e1c2c0b`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:33:36 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:33:37 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 15:36:28 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 15:36:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f038398c36fe8c9f122b2c320286deb8340ad4bfb15151c7f0003b30a446a5`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc10fd05f63ed1f8c894e879f5b7e265e57eba8c14fd15dec49febcc9d9a4c50`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdbe481149c0c0461929bedd602d9e61479caa109e234b517e2b5ab9fe67a5`  
		Last Modified: Wed, 15 Apr 2020 16:17:45 GMT  
		Size: 134.1 MB (134054202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df348e63ef1f9d6be06ba680c38dd8277df605185deb68d67a49e0ae50436a1a`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4-buster`

```console
$ docker pull julia@sha256:85a0bb7cfc62976db640692c151c15840d47b825d76046b398e1cf941030b0b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.4-buster` - linux; amd64

```console
$ docker pull julia@sha256:98b9f4174aee469d83a3d6c8c46d0fd9c1a6ef95f7fcf0a3e8e1b20aa01d4988
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138323266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18183d0f0d8119399633e1baabfd1092b030b9b48d98290b15676c3cfa06b283`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:09:46 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:20:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364e671b6375d1b6ec0a9a1d40cdab37905fa8dfaa094127586381c6f867ae36`  
		Last Modified: Mon, 06 Apr 2020 23:20:50 GMT  
		Size: 106.8 MB (106794820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:0ac7eb3ba05168cd26791bb2e36436f2fa132b37f0776a9b39fb36214bb93f47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123503508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f5de0dda095868608104228885ffc09b658a247d7720b16fc63282f0f26238`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:25:49 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 04:26:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:26:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0230b466eb1f16bd472b786b23f9da3b9174ac5b23eab9e862321830d0c2d0e`  
		Last Modified: Thu, 16 Apr 2020 04:29:15 GMT  
		Size: 97.0 MB (97014701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a10a693db14af0d554aa7b98379fc4b4c8717d239186ea58c5f36f999e038229
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119875470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102fa2b9dd57d9ddb7762e531e4757d83f221990dee3606caa028c6839c2908f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:01:25 GMT
ENV JULIA_VERSION=1.4.0
# Tue, 07 Apr 2020 00:44:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Apr 2020 00:44:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e431814eaafc5d057cf00cdcafa51c860fb428bf78ff92489102a2e0f9712c8`  
		Last Modified: Tue, 07 Apr 2020 00:45:18 GMT  
		Size: 89.7 MB (89708315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.4-buster` - linux; 386

```console
$ docker pull julia@sha256:fb09607a2c0f0ff09e2ca51ffe314721d2708313b20bb41d05edbbad1b0285ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135745740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d0a3d12891fdd339b3bb182b7db7ecfc83e0979dc3ad4f6a914ae74a3f96f6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:27 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:38:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:38:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f23a5e87a61c1beb0e0fbcbd325e86d325f9d2737b674c120dd486c8699396`  
		Last Modified: Mon, 06 Apr 2020 23:39:33 GMT  
		Size: 103.4 MB (103411717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4-windowsservercore-1809`

```console
$ docker pull julia@sha256:68ed12481c16cccc92bc96490bedd9d624719211232264ae58afffa87edc079c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `julia:1.4-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:1e33b6e7007a2f411de49d7b1a0f7e803fb903c85fae39b26a499bd7627bb628
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2404042630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c55b7e7389c5a36e6037e0e789d97bef87e8e8036194f157e4a1848622b4c0c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:36:48 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:36:49 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 16:09:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:09:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef82f9deae85c127a0081ef3def77db201036d2e40fc3c59d76d5a9479ffe8`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2578c185ed18752b07b8d9a71d93a1fdb3707a17661f7e9aca7dc773371628a9`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb745a5e60aaa23fe0b0860d65adf83ee9f0415022f23f35d34dd993877b06`  
		Last Modified: Wed, 15 Apr 2020 16:18:29 GMT  
		Size: 133.3 MB (133330862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842173cc65f3b5379978f761a13c39c00bc69db010d3f1475329c69a8f6dec0`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.4-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:414c4d202386b41a8da6b5ea37fbb9416089f2ff701871c2e6b4530ad46fee65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `julia:1.4-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:73899dda58739417bedc7db11486dc30cdb3da1f37fb14d5b21473d11e609b13
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5862126325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a2078b38cb3b41f4a03539a1f6c4b3004fa67d2ca6b5594c396da81e1c2c0b`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:33:36 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:33:37 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 15:36:28 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 15:36:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f038398c36fe8c9f122b2c320286deb8340ad4bfb15151c7f0003b30a446a5`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc10fd05f63ed1f8c894e879f5b7e265e57eba8c14fd15dec49febcc9d9a4c50`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdbe481149c0c0461929bedd602d9e61479caa109e234b517e2b5ab9fe67a5`  
		Last Modified: Wed, 15 Apr 2020 16:17:45 GMT  
		Size: 134.1 MB (134054202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df348e63ef1f9d6be06ba680c38dd8277df605185deb68d67a49e0ae50436a1a`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-buster`

```console
$ docker pull julia@sha256:85a0bb7cfc62976db640692c151c15840d47b825d76046b398e1cf941030b0b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-buster` - linux; amd64

```console
$ docker pull julia@sha256:98b9f4174aee469d83a3d6c8c46d0fd9c1a6ef95f7fcf0a3e8e1b20aa01d4988
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138323266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18183d0f0d8119399633e1baabfd1092b030b9b48d98290b15676c3cfa06b283`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:09:46 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:20:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364e671b6375d1b6ec0a9a1d40cdab37905fa8dfaa094127586381c6f867ae36`  
		Last Modified: Mon, 06 Apr 2020 23:20:50 GMT  
		Size: 106.8 MB (106794820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:0ac7eb3ba05168cd26791bb2e36436f2fa132b37f0776a9b39fb36214bb93f47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123503508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f5de0dda095868608104228885ffc09b658a247d7720b16fc63282f0f26238`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:25:49 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 04:26:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:26:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0230b466eb1f16bd472b786b23f9da3b9174ac5b23eab9e862321830d0c2d0e`  
		Last Modified: Thu, 16 Apr 2020 04:29:15 GMT  
		Size: 97.0 MB (97014701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a10a693db14af0d554aa7b98379fc4b4c8717d239186ea58c5f36f999e038229
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119875470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102fa2b9dd57d9ddb7762e531e4757d83f221990dee3606caa028c6839c2908f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:01:25 GMT
ENV JULIA_VERSION=1.4.0
# Tue, 07 Apr 2020 00:44:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Apr 2020 00:44:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e431814eaafc5d057cf00cdcafa51c860fb428bf78ff92489102a2e0f9712c8`  
		Last Modified: Tue, 07 Apr 2020 00:45:18 GMT  
		Size: 89.7 MB (89708315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; 386

```console
$ docker pull julia@sha256:fb09607a2c0f0ff09e2ca51ffe314721d2708313b20bb41d05edbbad1b0285ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135745740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d0a3d12891fdd339b3bb182b7db7ecfc83e0979dc3ad4f6a914ae74a3f96f6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:27 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:38:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:38:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f23a5e87a61c1beb0e0fbcbd325e86d325f9d2737b674c120dd486c8699396`  
		Last Modified: Mon, 06 Apr 2020 23:39:33 GMT  
		Size: 103.4 MB (103411717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:68ed12481c16cccc92bc96490bedd9d624719211232264ae58afffa87edc079c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:1e33b6e7007a2f411de49d7b1a0f7e803fb903c85fae39b26a499bd7627bb628
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2404042630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c55b7e7389c5a36e6037e0e789d97bef87e8e8036194f157e4a1848622b4c0c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:36:48 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:36:49 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 16:09:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:09:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef82f9deae85c127a0081ef3def77db201036d2e40fc3c59d76d5a9479ffe8`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2578c185ed18752b07b8d9a71d93a1fdb3707a17661f7e9aca7dc773371628a9`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb745a5e60aaa23fe0b0860d65adf83ee9f0415022f23f35d34dd993877b06`  
		Last Modified: Wed, 15 Apr 2020 16:18:29 GMT  
		Size: 133.3 MB (133330862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842173cc65f3b5379978f761a13c39c00bc69db010d3f1475329c69a8f6dec0`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:414c4d202386b41a8da6b5ea37fbb9416089f2ff701871c2e6b4530ad46fee65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `julia:1-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:73899dda58739417bedc7db11486dc30cdb3da1f37fb14d5b21473d11e609b13
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5862126325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a2078b38cb3b41f4a03539a1f6c4b3004fa67d2ca6b5594c396da81e1c2c0b`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:33:36 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:33:37 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 15:36:28 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 15:36:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f038398c36fe8c9f122b2c320286deb8340ad4bfb15151c7f0003b30a446a5`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc10fd05f63ed1f8c894e879f5b7e265e57eba8c14fd15dec49febcc9d9a4c50`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdbe481149c0c0461929bedd602d9e61479caa109e234b517e2b5ab9fe67a5`  
		Last Modified: Wed, 15 Apr 2020 16:17:45 GMT  
		Size: 134.1 MB (134054202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df348e63ef1f9d6be06ba680c38dd8277df605185deb68d67a49e0ae50436a1a`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:buster`

```console
$ docker pull julia@sha256:85a0bb7cfc62976db640692c151c15840d47b825d76046b398e1cf941030b0b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:98b9f4174aee469d83a3d6c8c46d0fd9c1a6ef95f7fcf0a3e8e1b20aa01d4988
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138323266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18183d0f0d8119399633e1baabfd1092b030b9b48d98290b15676c3cfa06b283`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:09:46 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:20:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364e671b6375d1b6ec0a9a1d40cdab37905fa8dfaa094127586381c6f867ae36`  
		Last Modified: Mon, 06 Apr 2020 23:20:50 GMT  
		Size: 106.8 MB (106794820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:0ac7eb3ba05168cd26791bb2e36436f2fa132b37f0776a9b39fb36214bb93f47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123503508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f5de0dda095868608104228885ffc09b658a247d7720b16fc63282f0f26238`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:25:49 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 04:26:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:26:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0230b466eb1f16bd472b786b23f9da3b9174ac5b23eab9e862321830d0c2d0e`  
		Last Modified: Thu, 16 Apr 2020 04:29:15 GMT  
		Size: 97.0 MB (97014701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a10a693db14af0d554aa7b98379fc4b4c8717d239186ea58c5f36f999e038229
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119875470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102fa2b9dd57d9ddb7762e531e4757d83f221990dee3606caa028c6839c2908f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:01:25 GMT
ENV JULIA_VERSION=1.4.0
# Tue, 07 Apr 2020 00:44:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Apr 2020 00:44:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e431814eaafc5d057cf00cdcafa51c860fb428bf78ff92489102a2e0f9712c8`  
		Last Modified: Tue, 07 Apr 2020 00:45:18 GMT  
		Size: 89.7 MB (89708315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:fb09607a2c0f0ff09e2ca51ffe314721d2708313b20bb41d05edbbad1b0285ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135745740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d0a3d12891fdd339b3bb182b7db7ecfc83e0979dc3ad4f6a914ae74a3f96f6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:27 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:38:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:38:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f23a5e87a61c1beb0e0fbcbd325e86d325f9d2737b674c120dd486c8699396`  
		Last Modified: Mon, 06 Apr 2020 23:39:33 GMT  
		Size: 103.4 MB (103411717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:d041f4a94d00a7b0e2634045cd422b7fa97edef601a48894ab045c55b31f1ae9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:98b9f4174aee469d83a3d6c8c46d0fd9c1a6ef95f7fcf0a3e8e1b20aa01d4988
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138323266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18183d0f0d8119399633e1baabfd1092b030b9b48d98290b15676c3cfa06b283`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:09:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 03:09:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 03:09:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 03:09:46 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:20:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:20:07 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b71d3134af3728e710f1dd85497919cd05a5f63d8732281a8f599f71252e6`  
		Last Modified: Tue, 31 Mar 2020 03:11:39 GMT  
		Size: 4.4 MB (4436584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364e671b6375d1b6ec0a9a1d40cdab37905fa8dfaa094127586381c6f867ae36`  
		Last Modified: Mon, 06 Apr 2020 23:20:50 GMT  
		Size: 106.8 MB (106794820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm variant v7

```console
$ docker pull julia@sha256:0ac7eb3ba05168cd26791bb2e36436f2fa132b37f0776a9b39fb36214bb93f47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123503508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f5de0dda095868608104228885ffc09b658a247d7720b16fc63282f0f26238`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:25:49 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 04:26:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:26:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0230b466eb1f16bd472b786b23f9da3b9174ac5b23eab9e862321830d0c2d0e`  
		Last Modified: Thu, 16 Apr 2020 04:29:15 GMT  
		Size: 97.0 MB (97014701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a10a693db14af0d554aa7b98379fc4b4c8717d239186ea58c5f36f999e038229
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119875470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102fa2b9dd57d9ddb7762e531e4757d83f221990dee3606caa028c6839c2908f`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:33 GMT
ADD file:47ab456123ae97a527249191ff2bc0014e7ef0ae186aec91bf6a63eb077ecb91 in / 
# Tue, 31 Mar 2020 02:05:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 05:01:19 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 05:01:21 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 05:01:24 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 05:01:25 GMT
ENV JULIA_VERSION=1.4.0
# Tue, 07 Apr 2020 00:44:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 07 Apr 2020 00:44:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a6c32b8bc1ce2b374630673ded1d5ef5a98936d045bf0632fcf599dc2229d493`  
		Last Modified: Tue, 31 Mar 2020 02:12:15 GMT  
		Size: 25.9 MB (25851645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2839d96f3fc4180c714a825b5c1a24f2f93217a76c3714bd55165a88e05d91`  
		Last Modified: Tue, 31 Mar 2020 05:04:00 GMT  
		Size: 4.3 MB (4315510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e431814eaafc5d057cf00cdcafa51c860fb428bf78ff92489102a2e0f9712c8`  
		Last Modified: Tue, 07 Apr 2020 00:45:18 GMT  
		Size: 89.7 MB (89708315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:fb09607a2c0f0ff09e2ca51ffe314721d2708313b20bb41d05edbbad1b0285ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135745740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d0a3d12891fdd339b3bb182b7db7ecfc83e0979dc3ad4f6a914ae74a3f96f6`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 31 Mar 2020 00:39:42 GMT
ADD file:a453117866661af4ddfa21203d65ce6661efeaeca2a1704e09747c83b4c58e47 in / 
# Tue, 31 Mar 2020 00:39:42 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:05:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 31 Mar 2020 01:05:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 01:05:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 31 Mar 2020 01:05:27 GMT
ENV JULIA_VERSION=1.4.0
# Mon, 06 Apr 2020 23:38:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 06 Apr 2020 23:38:50 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2314106a15e49c7908bebb2c697dcaf3d6a1626b70fe72bc0c0cb71eb216ddc3`  
		Last Modified: Tue, 31 Mar 2020 00:45:31 GMT  
		Size: 27.7 MB (27747648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fde8d7ec1bbaa2b4b31dceffabe4dc5a10339fbd48d0479f927f186ef0689`  
		Last Modified: Tue, 31 Mar 2020 01:06:55 GMT  
		Size: 4.6 MB (4586375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f23a5e87a61c1beb0e0fbcbd325e86d325f9d2737b674c120dd486c8699396`  
		Last Modified: Mon, 06 Apr 2020 23:39:33 GMT  
		Size: 103.4 MB (103411717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:73899dda58739417bedc7db11486dc30cdb3da1f37fb14d5b21473d11e609b13
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5862126325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a2078b38cb3b41f4a03539a1f6c4b3004fa67d2ca6b5594c396da81e1c2c0b`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:33:36 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:33:37 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 15:36:28 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 15:36:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f038398c36fe8c9f122b2c320286deb8340ad4bfb15151c7f0003b30a446a5`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc10fd05f63ed1f8c894e879f5b7e265e57eba8c14fd15dec49febcc9d9a4c50`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdbe481149c0c0461929bedd602d9e61479caa109e234b517e2b5ab9fe67a5`  
		Last Modified: Wed, 15 Apr 2020 16:17:45 GMT  
		Size: 134.1 MB (134054202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df348e63ef1f9d6be06ba680c38dd8277df605185deb68d67a49e0ae50436a1a`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:1e33b6e7007a2f411de49d7b1a0f7e803fb903c85fae39b26a499bd7627bb628
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2404042630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c55b7e7389c5a36e6037e0e789d97bef87e8e8036194f157e4a1848622b4c0c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:36:48 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:36:49 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 16:09:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:09:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef82f9deae85c127a0081ef3def77db201036d2e40fc3c59d76d5a9479ffe8`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2578c185ed18752b07b8d9a71d93a1fdb3707a17661f7e9aca7dc773371628a9`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb745a5e60aaa23fe0b0860d65adf83ee9f0415022f23f35d34dd993877b06`  
		Last Modified: Wed, 15 Apr 2020 16:18:29 GMT  
		Size: 133.3 MB (133330862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842173cc65f3b5379978f761a13c39c00bc69db010d3f1475329c69a8f6dec0`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:68ed12481c16cccc92bc96490bedd9d624719211232264ae58afffa87edc079c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull julia@sha256:1e33b6e7007a2f411de49d7b1a0f7e803fb903c85fae39b26a499bd7627bb628
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2404042630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c55b7e7389c5a36e6037e0e789d97bef87e8e8036194f157e4a1848622b4c0c`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:36:48 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:36:49 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 16:09:24 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 16:09:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef82f9deae85c127a0081ef3def77db201036d2e40fc3c59d76d5a9479ffe8`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2578c185ed18752b07b8d9a71d93a1fdb3707a17661f7e9aca7dc773371628a9`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb745a5e60aaa23fe0b0860d65adf83ee9f0415022f23f35d34dd993877b06`  
		Last Modified: Wed, 15 Apr 2020 16:18:29 GMT  
		Size: 133.3 MB (133330862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842173cc65f3b5379978f761a13c39c00bc69db010d3f1475329c69a8f6dec0`  
		Last Modified: Wed, 15 Apr 2020 16:18:01 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:414c4d202386b41a8da6b5ea37fbb9416089f2ff701871c2e6b4530ad46fee65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `julia:windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull julia@sha256:73899dda58739417bedc7db11486dc30cdb3da1f37fb14d5b21473d11e609b13
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5862126325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a2078b38cb3b41f4a03539a1f6c4b3004fa67d2ca6b5594c396da81e1c2c0b`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Apr 2020 15:33:36 GMT
ENV JULIA_VERSION=1.4.0
# Wed, 15 Apr 2020 15:33:37 GMT
ENV JULIA_SHA256=aa41a5c91eac5d34c7604cefd5cf8b619dbcfa35149b5de5381c2c8f06d6598c
# Wed, 15 Apr 2020 15:36:28 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 15 Apr 2020 15:36:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f038398c36fe8c9f122b2c320286deb8340ad4bfb15151c7f0003b30a446a5`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc10fd05f63ed1f8c894e879f5b7e265e57eba8c14fd15dec49febcc9d9a4c50`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbdbe481149c0c0461929bedd602d9e61479caa109e234b517e2b5ab9fe67a5`  
		Last Modified: Wed, 15 Apr 2020 16:17:45 GMT  
		Size: 134.1 MB (134054202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df348e63ef1f9d6be06ba680c38dd8277df605185deb68d67a49e0ae50436a1a`  
		Last Modified: Wed, 15 Apr 2020 16:15:15 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
