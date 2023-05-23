<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `julia`

-	[`julia:1`](#julia1)
-	[`julia:1-alpine`](#julia1-alpine)
-	[`julia:1-alpine3.17`](#julia1-alpine317)
-	[`julia:1-alpine3.18`](#julia1-alpine318)
-	[`julia:1-bullseye`](#julia1-bullseye)
-	[`julia:1-buster`](#julia1-buster)
-	[`julia:1-windowsservercore`](#julia1-windowsservercore)
-	[`julia:1-windowsservercore-1809`](#julia1-windowsservercore-1809)
-	[`julia:1-windowsservercore-ltsc2022`](#julia1-windowsservercore-ltsc2022)
-	[`julia:1.6`](#julia16)
-	[`julia:1.6-alpine`](#julia16-alpine)
-	[`julia:1.6-alpine3.17`](#julia16-alpine317)
-	[`julia:1.6-alpine3.18`](#julia16-alpine318)
-	[`julia:1.6-bullseye`](#julia16-bullseye)
-	[`julia:1.6-buster`](#julia16-buster)
-	[`julia:1.6-windowsservercore`](#julia16-windowsservercore)
-	[`julia:1.6-windowsservercore-1809`](#julia16-windowsservercore-1809)
-	[`julia:1.6-windowsservercore-ltsc2022`](#julia16-windowsservercore-ltsc2022)
-	[`julia:1.6.7`](#julia167)
-	[`julia:1.6.7-alpine`](#julia167-alpine)
-	[`julia:1.6.7-alpine3.17`](#julia167-alpine317)
-	[`julia:1.6.7-alpine3.18`](#julia167-alpine318)
-	[`julia:1.6.7-bullseye`](#julia167-bullseye)
-	[`julia:1.6.7-buster`](#julia167-buster)
-	[`julia:1.6.7-windowsservercore`](#julia167-windowsservercore)
-	[`julia:1.6.7-windowsservercore-1809`](#julia167-windowsservercore-1809)
-	[`julia:1.6.7-windowsservercore-ltsc2022`](#julia167-windowsservercore-ltsc2022)
-	[`julia:1.9`](#julia19)
-	[`julia:1.9-alpine`](#julia19-alpine)
-	[`julia:1.9-alpine3.17`](#julia19-alpine317)
-	[`julia:1.9-alpine3.18`](#julia19-alpine318)
-	[`julia:1.9-bullseye`](#julia19-bullseye)
-	[`julia:1.9-buster`](#julia19-buster)
-	[`julia:1.9-windowsservercore`](#julia19-windowsservercore)
-	[`julia:1.9-windowsservercore-1809`](#julia19-windowsservercore-1809)
-	[`julia:1.9-windowsservercore-ltsc2022`](#julia19-windowsservercore-ltsc2022)
-	[`julia:1.9.0`](#julia190)
-	[`julia:1.9.0-alpine`](#julia190-alpine)
-	[`julia:1.9.0-alpine3.17`](#julia190-alpine317)
-	[`julia:1.9.0-alpine3.18`](#julia190-alpine318)
-	[`julia:1.9.0-bullseye`](#julia190-bullseye)
-	[`julia:1.9.0-buster`](#julia190-buster)
-	[`julia:1.9.0-windowsservercore`](#julia190-windowsservercore)
-	[`julia:1.9.0-windowsservercore-1809`](#julia190-windowsservercore-1809)
-	[`julia:1.9.0-windowsservercore-ltsc2022`](#julia190-windowsservercore-ltsc2022)
-	[`julia:alpine`](#juliaalpine)
-	[`julia:alpine3.17`](#juliaalpine317)
-	[`julia:alpine3.18`](#juliaalpine318)
-	[`julia:bullseye`](#juliabullseye)
-	[`julia:buster`](#juliabuster)
-	[`julia:latest`](#julialatest)
-	[`julia:windowsservercore`](#juliawindowsservercore)
-	[`julia:windowsservercore-1809`](#juliawindowsservercore-1809)
-	[`julia:windowsservercore-ltsc2022`](#juliawindowsservercore-ltsc2022)

## `julia:1`

```console
$ docker pull julia@sha256:36902255c08939b511a37508150a2883abd51afacbeab0d461635d7f5f644e6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:1` - linux; amd64

```console
$ docker pull julia@sha256:1baf0ab6fb6c474d216468d960333ffde38ccb3c76bb7f830c416d0d024412e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182524441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0394c94147bb57936f72c3b7d0ff8f2bdf98d7adc929d5fe3fa528b7339c4d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:58:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:58:41 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:58:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:58:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c421a694ca3262d6955441bf869575152e027f158a67a5fca1069ca8806102`  
		Last Modified: Tue, 23 May 2023 04:00:55 GMT  
		Size: 148.7 MB (148693723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4d7795ec1ad44b7fb4ee919ddeb55611a858900c4d78219ec62c0518711be9`  
		Last Modified: Tue, 23 May 2023 04:00:33 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5e2977123b1cfe0518c291316ab3931d4b194fb628e97df6062a8067b1d35328
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.4 MB (175390009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ce886a6f78d5c7d285a05c16e8d159ea755355ed2843492a291bc61382736e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:20 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:44:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:44:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:44:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2616bb8cca402291d62dd06f67f3c3597f3042a4e8304a488e7db91581127cdf`  
		Last Modified: Wed, 10 May 2023 17:45:38 GMT  
		Size: 142.9 MB (142922569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc3b0ff727d110588d9b4875a9023116e1bc994d1b0dc5043d3ee86d66b1413`  
		Last Modified: Wed, 10 May 2023 17:45:21 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:7abf4e29ba01e1411695848991b2db643582481665fbefb816e49a5b70e9cb2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.7 MB (180735444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82a6bcb39c5b8202e58fc03ec47e602516000881cf4a2cb2f99998dc76d2603`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:02 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:29:26 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:29:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:29:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c55db0a6af6b3d85fb7c5a15e0d4c95f7e806ffa98208ce7ef735b7fc6725`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 145.8 MB (145814394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1668b9c92f4ae6e6ae9db09e901b457cce51b2a4ad763d409af5acd1499a971`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; ppc64le

```console
$ docker pull julia@sha256:fb992d3e811683d5a7acb40e070aa5cf48e0c551496021b7a3b986619326fb59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171094683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c12da7cffc9305381fb6312a99958195846c536f37834527c9e4ef8b94b61e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:07:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:07:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:08:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:08:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:08:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:08:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a7cd9dea84bb9d934231269410340992f182978f4edef2332551db9339895`  
		Last Modified: Tue, 23 May 2023 02:08:20 GMT  
		Size: 2.6 MB (2627396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b277918387795ff9e75af87373fb080fc7e519c3608df2d74dbbdaa2ad80c9`  
		Last Modified: Tue, 23 May 2023 02:08:55 GMT  
		Size: 133.2 MB (133185997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c2c74cab468cff7d8a1904dc5d697186d7ef6fe72b630d69ad8a14624a37b`  
		Last Modified: Tue, 23 May 2023 02:08:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine`

```console
$ docker pull julia@sha256:9df2dbe2638111d1133a5d401f981c46e7c98ae2c8fd2d21961a5e5ee13156f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine` - linux; amd64

```console
$ docker pull julia@sha256:9ed027843d8b3172d329dc5c1d2c6a6e587e748c42148cef8760a8fccbb83b85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153983502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82888c0d329cf435c73c43c4d89b154f6c0aaeb5468851cdf4364ae43472fec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_VERSION=1.9.0
# Mon, 15 May 2023 22:24:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:28 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3362ee69b9e183770605ef4b78cc162da6ed0150fa898768ebcb885a75ad3`  
		Last Modified: Mon, 15 May 2023 22:25:39 GMT  
		Size: 150.6 MB (150585641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee82d7382bfddf890d4621823ade41cd9210f9d81b1e38b44b6696272338b8`  
		Last Modified: Mon, 15 May 2023 22:25:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.17`

```console
$ docker pull julia@sha256:7f878f474243a69885585625807077d702d3c9a4c45af3bcb6620cbd5c59b503
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:f7b02fd0227eea383b76adac8f09121d3ce02fd4e2478d1422c2cdc851b79080
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153960395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea35812b9c8ce031bdf4d24d5cc14f53019dfe24d654cc51b06ba88beebee658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 29 Mar 2023 22:04:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:53:52 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:54:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 10 May 2023 17:54:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:54:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b199db89e2a6dd5f8f853e5b18e6e77a15d775d9158e7880a86156b68e361e`  
		Last Modified: Wed, 10 May 2023 17:56:36 GMT  
		Size: 150.6 MB (150585459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0840a682c27557acbad940eaff83e57fd9fd217b43b6f2de6bafd7c0fee7b04`  
		Last Modified: Wed, 10 May 2023 17:56:14 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-alpine3.18`

```console
$ docker pull julia@sha256:9df2dbe2638111d1133a5d401f981c46e7c98ae2c8fd2d21961a5e5ee13156f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:9ed027843d8b3172d329dc5c1d2c6a6e587e748c42148cef8760a8fccbb83b85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153983502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82888c0d329cf435c73c43c4d89b154f6c0aaeb5468851cdf4364ae43472fec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_VERSION=1.9.0
# Mon, 15 May 2023 22:24:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:28 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3362ee69b9e183770605ef4b78cc162da6ed0150fa898768ebcb885a75ad3`  
		Last Modified: Mon, 15 May 2023 22:25:39 GMT  
		Size: 150.6 MB (150585641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee82d7382bfddf890d4621823ade41cd9210f9d81b1e38b44b6696272338b8`  
		Last Modified: Mon, 15 May 2023 22:25:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-bullseye`

```console
$ docker pull julia@sha256:b031ec96e64d1a0a90b48ced4bc4a4fdaba9e13f61c199809289ace462695178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:1baf0ab6fb6c474d216468d960333ffde38ccb3c76bb7f830c416d0d024412e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182524441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0394c94147bb57936f72c3b7d0ff8f2bdf98d7adc929d5fe3fa528b7339c4d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:58:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:58:41 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:58:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:58:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c421a694ca3262d6955441bf869575152e027f158a67a5fca1069ca8806102`  
		Last Modified: Tue, 23 May 2023 04:00:55 GMT  
		Size: 148.7 MB (148693723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4d7795ec1ad44b7fb4ee919ddeb55611a858900c4d78219ec62c0518711be9`  
		Last Modified: Tue, 23 May 2023 04:00:33 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5e2977123b1cfe0518c291316ab3931d4b194fb628e97df6062a8067b1d35328
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.4 MB (175390009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ce886a6f78d5c7d285a05c16e8d159ea755355ed2843492a291bc61382736e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:20 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:44:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:44:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:44:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2616bb8cca402291d62dd06f67f3c3597f3042a4e8304a488e7db91581127cdf`  
		Last Modified: Wed, 10 May 2023 17:45:38 GMT  
		Size: 142.9 MB (142922569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc3b0ff727d110588d9b4875a9023116e1bc994d1b0dc5043d3ee86d66b1413`  
		Last Modified: Wed, 10 May 2023 17:45:21 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bullseye` - linux; 386

```console
$ docker pull julia@sha256:7abf4e29ba01e1411695848991b2db643582481665fbefb816e49a5b70e9cb2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.7 MB (180735444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82a6bcb39c5b8202e58fc03ec47e602516000881cf4a2cb2f99998dc76d2603`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:02 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:29:26 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:29:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:29:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c55db0a6af6b3d85fb7c5a15e0d4c95f7e806ffa98208ce7ef735b7fc6725`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 145.8 MB (145814394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1668b9c92f4ae6e6ae9db09e901b457cce51b2a4ad763d409af5acd1499a971`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:fb992d3e811683d5a7acb40e070aa5cf48e0c551496021b7a3b986619326fb59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171094683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c12da7cffc9305381fb6312a99958195846c536f37834527c9e4ef8b94b61e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:07:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:07:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:08:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:08:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:08:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:08:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a7cd9dea84bb9d934231269410340992f182978f4edef2332551db9339895`  
		Last Modified: Tue, 23 May 2023 02:08:20 GMT  
		Size: 2.6 MB (2627396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b277918387795ff9e75af87373fb080fc7e519c3608df2d74dbbdaa2ad80c9`  
		Last Modified: Tue, 23 May 2023 02:08:55 GMT  
		Size: 133.2 MB (133185997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c2c74cab468cff7d8a1904dc5d697186d7ef6fe72b630d69ad8a14624a37b`  
		Last Modified: Tue, 23 May 2023 02:08:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-buster`

```console
$ docker pull julia@sha256:ef4f187da55bd84a6e754aa15bbd8b293cc8746c224cad2e522907d23f7f24d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-buster` - linux; amd64

```console
$ docker pull julia@sha256:a616d9ed55df3b4e5943dfc9794af3cd60f86f05dda5e0bafed5bf3bacbb203b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180302639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c1122d78b068c53d117c09b5ca780be1391bab12f89990c84ea547db7272bc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:59:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:59:14 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:59:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add0b47570fa87476e546a69dfdf17243a2bdfe9059e797eaa71e66a594c750`  
		Last Modified: Tue, 23 May 2023 04:01:08 GMT  
		Size: 4.5 MB (4472118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3dfa17601b0c6337c1d87a32b4533f1bf5d06ccb3cd50ccf3c60d135b9418d`  
		Last Modified: Tue, 23 May 2023 04:01:30 GMT  
		Size: 148.7 MB (148691569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e65c1f2b4a861c50f9070a5ec00ccad08d555f838567262169d38f4da444b6`  
		Last Modified: Tue, 23 May 2023 04:01:07 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1c318c6cf16dc00c022b64202164701af68203394f1f7a7368396b2fc684b172
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173191012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c396b9151522a26e360c8ff6c077cdc17cd73edc217f556c96bb4052c09f52f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:23:05 GMT
ADD file:1d8cf95f550bb4b86ad82b22e7195179335fa3b327fd1f1ba1e6c8357ee15c94 in / 
# Wed, 03 May 2023 00:23:05 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:38:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:38:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:43 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:45:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:45:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:45:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:45:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5627aec4010af613408c2ee78d5d32b9ecac22cb396d702906fb1160721f0011`  
		Last Modified: Wed, 03 May 2023 00:26:29 GMT  
		Size: 25.9 MB (25922039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4bb136449e53562b21b648a615cf43907af192446ee7d880c05b3a8254c8af`  
		Last Modified: Wed, 03 May 2023 03:40:39 GMT  
		Size: 4.4 MB (4350609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ca056492e3a7e4b3c199f8a889b9183b1a75edb249a08e1d8786c7b4d8cad8`  
		Last Modified: Wed, 10 May 2023 17:46:07 GMT  
		Size: 142.9 MB (142917988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee770aa11ecd8ad59c9dfc316a7ce4b28e594d1bf3d5467b6a85ed956a3863c`  
		Last Modified: Wed, 10 May 2023 17:45:50 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; 386

```console
$ docker pull julia@sha256:255f7543d0e6dba32bffdc3ae60e70270c061eb49973957af547ba0e6261139a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178248531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:056069102655d640917bef51c63d30efa8aac4fecf2bb3f8da960cee2a11c3f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:40:01 GMT
ADD file:96715cff0e3569a2a1d7e203f0797ed4880da7714d455e25f032c67bff27221f in / 
# Tue, 23 May 2023 00:40:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:37 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:30:00 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:30:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:30:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3c2058520f8e2dee0c8d97a0e68335849888066e5d0d1b82b6ef302541b5c874`  
		Last Modified: Tue, 23 May 2023 00:45:13 GMT  
		Size: 27.8 MB (27797210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678dd0b30ea1ab93eb8bcc35bcf334b795b36c9b74173148a7dbb8d70fab701`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 4.6 MB (4623824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83a140272f2611b1f4445691bb0ac4abbb87dd9d4ac6f5f9d505bf97ece32fe`  
		Last Modified: Tue, 23 May 2023 02:32:21 GMT  
		Size: 145.8 MB (145827125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01965ecc75242364a50d7ecb78bc7ae189013003af9f27b68e7bbdff182061b7`  
		Last Modified: Tue, 23 May 2023 02:31:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore`

```console
$ docker pull julia@sha256:51427d8cfaf9d87867929fe0bcf0652465c5618261c3c24e482d35e62084c6d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:1-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:30526016f4cdb9c4c5c531ce9e9955b2328b495c64587b2767af1ad1561439b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:604ba14a26f6b140f5e4e281daa12fa2b1f4ef444781bf3b30b3d4aeaf404417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `julia:1-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6`

```console
$ docker pull julia@sha256:65b17bcb5e9b0e15fee247d043bb1cc396bba9749747d117ccfa54e3b3d0a19e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:1.6` - linux; amd64

```console
$ docker pull julia@sha256:c8f6b96ab6b715c766a6485a7a499e39e4f233a85204024255417495db4b364b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156470773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede005e31b348b6d9c57ae4140e3b1cc4169876aa04d550d982acbc3fb60b513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:59:25 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 03:59:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:59:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:59:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:59:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8556cf9795a1ce12713f8dbb5b9ea6f9bb70b1003a60254a03f14a5fdb762`  
		Last Modified: Tue, 23 May 2023 04:02:01 GMT  
		Size: 122.6 MB (122640058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865f8dc690e0bceabb40c6e5a2a9436c0dcad7ecc7dc3e21a5d3e49ad9ccd71`  
		Last Modified: Tue, 23 May 2023 04:01:44 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm variant v7

```console
$ docker pull julia@sha256:f4697aca57403f3be030882823cc9269406a647fa56986c1937f6447f546f246
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142481887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34f62617e30af6cbf895d9c8b3af1109b3deb4517124543e42c8b907843b041`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 02 May 2023 23:47:57 GMT
ADD file:69d82e947b50a0f0ec610822ffe7c23ec1f6eb41bc17068502380f827cbcce40 in / 
# Tue, 02 May 2023 23:47:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 05:54:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 05:54:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 05:54:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 05:54:54 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 05:54:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 05:54:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9c7c4e67baad3ce38491ce8c1ffaa9ca9ce37409270ce53ab3472054f35d097e`  
		Last Modified: Tue, 02 May 2023 23:51:30 GMT  
		Size: 26.6 MB (26564648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34a33ab1e3a66dc8f0d8f561e66108ac58b4d4dced41b1bd2c872d21b7fd1b4`  
		Last Modified: Wed, 03 May 2023 05:55:43 GMT  
		Size: 2.2 MB (2228960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c904682ccefca56baca0005cbaaa7e757f77bbb19df1e168c78bec2671b8df06`  
		Last Modified: Wed, 03 May 2023 05:56:02 GMT  
		Size: 113.7 MB (113687904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c25c2e61ceda75e6ec1dcfe9627b74e93d7cb99b12ca5452055c0cc0873dc2b`  
		Last Modified: Wed, 03 May 2023 05:55:43 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f0cb7640adf95bc3fc6c603c6eb9a7b76fba164454f4c3563143e0a11af7b136
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148895758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e9f7ff436a74ae2954bf396b8ae0edfc80e22b3d74fce5daef4b5b3157238b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 03:39:14 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 03:39:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 03:39:29 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 03:39:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 03:39:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c52e1f143cd7e48eb844907c2e25b5aa95cbcb28062c943320016844e57d2a`  
		Last Modified: Wed, 03 May 2023 03:42:10 GMT  
		Size: 116.4 MB (116428323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c7d1277473b3cc0fba07efbcccaa604023f1a4ea9ab523a2ef39ab96829404`  
		Last Modified: Wed, 03 May 2023 03:41:56 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; 386

```console
$ docker pull julia@sha256:09f1b083664b7248342acd21dc07e793666bc552b73646cc7ee87796b85e24c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155228544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c6dda947fb24429f880c766fa4bc11e9ab8ab982113dd790cbb6b69b9ef71a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:30:08 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 02:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:30:33 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:30:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:30:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0790b481c61582d040d8872b94795f195b2b3d9ffcd0c8c5d33c0683de187fd9`  
		Last Modified: Tue, 23 May 2023 02:32:58 GMT  
		Size: 120.3 MB (120307491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3193caf127fe61f2d393bacbef592a17eb9e78ab512d6df7c47353b14513a`  
		Last Modified: Tue, 23 May 2023 02:32:33 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:7e0f50fd9c88c790c64e9a40c1c29981368e3ed8cc215601bd5637711c5a6669
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1909494956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb15ee4828117c07bfff86c99bcf233ed017c6f34a308642192fca99d613691`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:32:31 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:32:32 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:32:33 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:33:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:33:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf0017a529e60f82e02af855e1112c244642471771c3c99f5164ce11b0ee914`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a1096533c4db5806a3e5c7f3a69faedb409a6c8733191a7e10d627aa7b325a`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711ca30bcfd5af661b63bc4e1db9b888fcaa14152a30456492180598e970317`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73d254af54574ed3afe72fa5364772638c1b4735649aec0b2807fc10d57084b`  
		Last Modified: Wed, 10 May 2023 05:39:24 GMT  
		Size: 134.5 MB (134506457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b268c90d009c976bb609f1dc060f3372d12418141823d93d2d29db14f5625cf3`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:9054874fbc0f9140b744f296fbdeaf6f28d08c40e7df71f667da8e54c33a5e6e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2206535515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d8896f4558089bbbe91431f87562b48db06f036e265127069eb0740a47f5378`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:33:44 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:33:45 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:33:46 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:35:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:35:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8c72398896ca187419ddbd67e44c1bdcedeba1015bae412c3b223da75bda4`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7de3df320f1d8ecdb0c694655ff678d826cb3cef6bff41a1fa354d3d4e598b7`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd9611b45abc0b498af22640b0dfbccb2244bbeac43b79c1f4b902a92553c38`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71abe049a8b13047f1b307a884567c6d629e6a88a2e42ec2bd1c43779091f46b`  
		Last Modified: Wed, 10 May 2023 05:40:01 GMT  
		Size: 134.5 MB (134493294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6d28206483adb96781bbe2372dfbdc2bc14b263df9e6ed2bc316ef471709b5`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine`

```console
$ docker pull julia@sha256:da0a327e7be2f7885df3d1dd655c8cc6aa3a836aea8ba8201879b91c54cb8f11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine` - linux; amd64

```console
$ docker pull julia@sha256:09f04cc2650688a0b1f09fa5b00d7ca2aa6dfdc1c1fc56d43df1c7b5994d7264
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125227359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c573f93d537fc748719d3c445941b2980266c9040453fd503bdab2140f9316c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:35 GMT
ENV JULIA_VERSION=1.6.7
# Mon, 15 May 2023 22:24:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:49 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dedadc624819670ffd0e049086d2f48d10406f443b69833b1c2a05b9489ccf03`  
		Last Modified: Mon, 15 May 2023 22:26:19 GMT  
		Size: 121.8 MB (121829496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b15a60b7a9333ccc46110b56abd98b9e489a72aacade80363bf922904b591c4`  
		Last Modified: Mon, 15 May 2023 22:26:02 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine3.17`

```console
$ docker pull julia@sha256:238ae7ae38c3fc6dc98079321bdf1b65079fc2dacd07ee070b704d8dd48bfc1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:7394c3e48e48b3f58565a94afb0bfbc83927f2b5d4dca1ac71fe3dd8aac3f13b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125204596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718b69ebed2b925dbce3d235d056968d4609f2ba2c71035aa818c460f7250a30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 29 Mar 2023 22:04:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 29 Mar 2023 22:06:12 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 04:18:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 03 May 2023 04:18:22 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 04:18:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 04:18:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed41d38c57b45602d3262f4def55c6dbefa6af04c92d86f23e99415807374f47`  
		Last Modified: Wed, 03 May 2023 04:24:46 GMT  
		Size: 121.8 MB (121829659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98547d2af32156d63952e8e82bfb935a225048964a3796385d68e5e8b6d5ddc7`  
		Last Modified: Wed, 03 May 2023 04:24:28 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-alpine3.18`

```console
$ docker pull julia@sha256:da0a327e7be2f7885df3d1dd655c8cc6aa3a836aea8ba8201879b91c54cb8f11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6-alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:09f04cc2650688a0b1f09fa5b00d7ca2aa6dfdc1c1fc56d43df1c7b5994d7264
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125227359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c573f93d537fc748719d3c445941b2980266c9040453fd503bdab2140f9316c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:35 GMT
ENV JULIA_VERSION=1.6.7
# Mon, 15 May 2023 22:24:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:49 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dedadc624819670ffd0e049086d2f48d10406f443b69833b1c2a05b9489ccf03`  
		Last Modified: Mon, 15 May 2023 22:26:19 GMT  
		Size: 121.8 MB (121829496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b15a60b7a9333ccc46110b56abd98b9e489a72aacade80363bf922904b591c4`  
		Last Modified: Mon, 15 May 2023 22:26:02 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-bullseye`

```console
$ docker pull julia@sha256:39a9ee53836fd23a8506c39bfb7b1c558fa72b7870c04878718891bc0bcaffc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:c8f6b96ab6b715c766a6485a7a499e39e4f233a85204024255417495db4b364b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156470773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede005e31b348b6d9c57ae4140e3b1cc4169876aa04d550d982acbc3fb60b513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:59:25 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 03:59:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:59:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:59:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:59:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8556cf9795a1ce12713f8dbb5b9ea6f9bb70b1003a60254a03f14a5fdb762`  
		Last Modified: Tue, 23 May 2023 04:02:01 GMT  
		Size: 122.6 MB (122640058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865f8dc690e0bceabb40c6e5a2a9436c0dcad7ecc7dc3e21a5d3e49ad9ccd71`  
		Last Modified: Tue, 23 May 2023 04:01:44 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull julia@sha256:f4697aca57403f3be030882823cc9269406a647fa56986c1937f6447f546f246
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142481887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34f62617e30af6cbf895d9c8b3af1109b3deb4517124543e42c8b907843b041`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 02 May 2023 23:47:57 GMT
ADD file:69d82e947b50a0f0ec610822ffe7c23ec1f6eb41bc17068502380f827cbcce40 in / 
# Tue, 02 May 2023 23:47:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 05:54:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 05:54:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 05:54:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 05:54:54 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 05:54:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 05:54:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9c7c4e67baad3ce38491ce8c1ffaa9ca9ce37409270ce53ab3472054f35d097e`  
		Last Modified: Tue, 02 May 2023 23:51:30 GMT  
		Size: 26.6 MB (26564648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34a33ab1e3a66dc8f0d8f561e66108ac58b4d4dced41b1bd2c872d21b7fd1b4`  
		Last Modified: Wed, 03 May 2023 05:55:43 GMT  
		Size: 2.2 MB (2228960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c904682ccefca56baca0005cbaaa7e757f77bbb19df1e168c78bec2671b8df06`  
		Last Modified: Wed, 03 May 2023 05:56:02 GMT  
		Size: 113.7 MB (113687904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c25c2e61ceda75e6ec1dcfe9627b74e93d7cb99b12ca5452055c0cc0873dc2b`  
		Last Modified: Wed, 03 May 2023 05:55:43 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f0cb7640adf95bc3fc6c603c6eb9a7b76fba164454f4c3563143e0a11af7b136
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148895758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e9f7ff436a74ae2954bf396b8ae0edfc80e22b3d74fce5daef4b5b3157238b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 03:39:14 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 03:39:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 03:39:29 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 03:39:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 03:39:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c52e1f143cd7e48eb844907c2e25b5aa95cbcb28062c943320016844e57d2a`  
		Last Modified: Wed, 03 May 2023 03:42:10 GMT  
		Size: 116.4 MB (116428323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c7d1277473b3cc0fba07efbcccaa604023f1a4ea9ab523a2ef39ab96829404`  
		Last Modified: Wed, 03 May 2023 03:41:56 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-bullseye` - linux; 386

```console
$ docker pull julia@sha256:09f1b083664b7248342acd21dc07e793666bc552b73646cc7ee87796b85e24c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155228544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c6dda947fb24429f880c766fa4bc11e9ab8ab982113dd790cbb6b69b9ef71a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:30:08 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 02:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:30:33 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:30:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:30:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0790b481c61582d040d8872b94795f195b2b3d9ffcd0c8c5d33c0683de187fd9`  
		Last Modified: Tue, 23 May 2023 02:32:58 GMT  
		Size: 120.3 MB (120307491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3193caf127fe61f2d393bacbef592a17eb9e78ab512d6df7c47353b14513a`  
		Last Modified: Tue, 23 May 2023 02:32:33 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-buster`

```console
$ docker pull julia@sha256:20d01af23da6e6a2eb6a800be737ba40d508e9d2edbfbd52a554c45ddae5f253
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6-buster` - linux; amd64

```console
$ docker pull julia@sha256:b129894fbfe5a482db6f7ac2c684ef07e46a0523d39f23a8b157f6c4b45a95e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.3 MB (154261836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1db6637bde6a1ce46560f8470e142047c1749aa2bf38181bb8b1dc7d98fc1968`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:59:44 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 03:59:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:59:58 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:59:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:59:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add0b47570fa87476e546a69dfdf17243a2bdfe9059e797eaa71e66a594c750`  
		Last Modified: Tue, 23 May 2023 04:01:08 GMT  
		Size: 4.5 MB (4472118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17692a645d52ee2258dbcaf3c89ea254a8083182621f8477cf0cd4ce424c5163`  
		Last Modified: Tue, 23 May 2023 04:02:27 GMT  
		Size: 122.7 MB (122650766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bf363d78e34a9aa14726ea83b6dbc224edd234370618c3f950230d3ea9ed09`  
		Last Modified: Tue, 23 May 2023 04:02:09 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:b24936c2be84556a762df86fb53df061a47a8801dad8536b210863c99980bb69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.3 MB (140261465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a21da53aac044df7709949a58a4183a3d47238cdf1e2058388c9c9aad022284`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 02 May 2023 23:48:16 GMT
ADD file:b8cf5ec32175731f2e4d1320020ed59d77bffe001218886fdd42e5aa3d5eda22 in / 
# Tue, 02 May 2023 23:48:16 GMT
CMD ["bash"]
# Wed, 03 May 2023 05:55:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 05:55:08 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 05:55:08 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 05:55:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 05:55:09 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 05:55:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 05:55:29 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 05:55:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 05:55:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:238786c487af66dadc8fb598b41ed76a08602b2a8a746d9c0cea9574cd9c9774`  
		Last Modified: Tue, 02 May 2023 23:52:11 GMT  
		Size: 22.7 MB (22747671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d2da501cd2ba273f52ced0ce21e157286e93568f69124c2f4a123c97a23b4`  
		Last Modified: Wed, 03 May 2023 05:56:11 GMT  
		Size: 3.8 MB (3816282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7bed06a017fc39cecd0f1b4ec51e71471fe97e6dc79c92b9408647209797c18`  
		Last Modified: Wed, 03 May 2023 05:56:31 GMT  
		Size: 113.7 MB (113697137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a2739a797aea02168f607d950eeb025b14584f5f6606626d82a18e74db9628`  
		Last Modified: Wed, 03 May 2023 05:56:10 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:587e2d5d60f716cac12d3a840768b923fd6576f7aa7677c93dafb3ec902c7496
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146709159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59587caa4eaebdb3283b317c3b97680d28d0c4b9dc06f37939b0324987639cba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:23:05 GMT
ADD file:1d8cf95f550bb4b86ad82b22e7195179335fa3b327fd1f1ba1e6c8357ee15c94 in / 
# Wed, 03 May 2023 00:23:05 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:38:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:38:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 03:39:33 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 03:39:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 03:39:48 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 03:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 03:39:48 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5627aec4010af613408c2ee78d5d32b9ecac22cb396d702906fb1160721f0011`  
		Last Modified: Wed, 03 May 2023 00:26:29 GMT  
		Size: 25.9 MB (25922039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4bb136449e53562b21b648a615cf43907af192446ee7d880c05b3a8254c8af`  
		Last Modified: Wed, 03 May 2023 03:40:39 GMT  
		Size: 4.4 MB (4350609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec161b9b02f469bf254b49088cf01496b66209e0502e98323f1993e179a6956`  
		Last Modified: Wed, 03 May 2023 03:42:30 GMT  
		Size: 116.4 MB (116436136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc47aac8ede1fa21feadfb93759f58fa2781773e628a2b828e8d148d609986ee`  
		Last Modified: Wed, 03 May 2023 03:42:17 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; 386

```console
$ docker pull julia@sha256:be141ab28104a9b6bd4c643eef6c4d0038bd49e344b7341c82a8bc43903e9a2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152735514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc9eb1a81e666b39c73e68e226bb01e62c9ce278b7edf6200ca471cf8790027c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:40:01 GMT
ADD file:96715cff0e3569a2a1d7e203f0797ed4880da7714d455e25f032c67bff27221f in / 
# Tue, 23 May 2023 00:40:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:30:36 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 02:30:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:30:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:30:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:30:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3c2058520f8e2dee0c8d97a0e68335849888066e5d0d1b82b6ef302541b5c874`  
		Last Modified: Tue, 23 May 2023 00:45:13 GMT  
		Size: 27.8 MB (27797210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678dd0b30ea1ab93eb8bcc35bcf334b795b36c9b74173148a7dbb8d70fab701`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 4.6 MB (4623824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266a72865041ef1eed5f176498c96078ac607a0398bf1de9a7209c1fad170e0a`  
		Last Modified: Tue, 23 May 2023 02:33:29 GMT  
		Size: 120.3 MB (120314104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d92df80f7e1512fa111860c7220ac566752cc28dfcb04bdbaa0dec0cfe0f9e9`  
		Last Modified: Tue, 23 May 2023 02:33:06 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore`

```console
$ docker pull julia@sha256:f12deffb3a2268bff161c8d459c4e815c65b9f31b5bd652ed070ec2ef37b7e9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:1.6-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:7e0f50fd9c88c790c64e9a40c1c29981368e3ed8cc215601bd5637711c5a6669
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1909494956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb15ee4828117c07bfff86c99bcf233ed017c6f34a308642192fca99d613691`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:32:31 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:32:32 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:32:33 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:33:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:33:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf0017a529e60f82e02af855e1112c244642471771c3c99f5164ce11b0ee914`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a1096533c4db5806a3e5c7f3a69faedb409a6c8733191a7e10d627aa7b325a`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711ca30bcfd5af661b63bc4e1db9b888fcaa14152a30456492180598e970317`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73d254af54574ed3afe72fa5364772638c1b4735649aec0b2807fc10d57084b`  
		Last Modified: Wed, 10 May 2023 05:39:24 GMT  
		Size: 134.5 MB (134506457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b268c90d009c976bb609f1dc060f3372d12418141823d93d2d29db14f5625cf3`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:9054874fbc0f9140b744f296fbdeaf6f28d08c40e7df71f667da8e54c33a5e6e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2206535515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d8896f4558089bbbe91431f87562b48db06f036e265127069eb0740a47f5378`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:33:44 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:33:45 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:33:46 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:35:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:35:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8c72398896ca187419ddbd67e44c1bdcedeba1015bae412c3b223da75bda4`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7de3df320f1d8ecdb0c694655ff678d826cb3cef6bff41a1fa354d3d4e598b7`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd9611b45abc0b498af22640b0dfbccb2244bbeac43b79c1f4b902a92553c38`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71abe049a8b13047f1b307a884567c6d629e6a88a2e42ec2bd1c43779091f46b`  
		Last Modified: Wed, 10 May 2023 05:40:01 GMT  
		Size: 134.5 MB (134493294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6d28206483adb96781bbe2372dfbdc2bc14b263df9e6ed2bc316ef471709b5`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-1809`

```console
$ docker pull julia@sha256:85588bb3893e999913f74c591fe0ae82acc9da116f7dc0160e6267b29475c237
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `julia:1.6-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:9054874fbc0f9140b744f296fbdeaf6f28d08c40e7df71f667da8e54c33a5e6e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2206535515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d8896f4558089bbbe91431f87562b48db06f036e265127069eb0740a47f5378`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:33:44 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:33:45 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:33:46 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:35:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:35:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8c72398896ca187419ddbd67e44c1bdcedeba1015bae412c3b223da75bda4`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7de3df320f1d8ecdb0c694655ff678d826cb3cef6bff41a1fa354d3d4e598b7`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd9611b45abc0b498af22640b0dfbccb2244bbeac43b79c1f4b902a92553c38`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71abe049a8b13047f1b307a884567c6d629e6a88a2e42ec2bd1c43779091f46b`  
		Last Modified: Wed, 10 May 2023 05:40:01 GMT  
		Size: 134.5 MB (134493294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6d28206483adb96781bbe2372dfbdc2bc14b263df9e6ed2bc316ef471709b5`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:347d7a805c07c435afdf3976dd6629f86a463acf8117afd1d3cc683a764e4636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `julia:1.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:7e0f50fd9c88c790c64e9a40c1c29981368e3ed8cc215601bd5637711c5a6669
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1909494956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb15ee4828117c07bfff86c99bcf233ed017c6f34a308642192fca99d613691`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:32:31 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:32:32 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:32:33 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:33:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:33:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf0017a529e60f82e02af855e1112c244642471771c3c99f5164ce11b0ee914`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a1096533c4db5806a3e5c7f3a69faedb409a6c8733191a7e10d627aa7b325a`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711ca30bcfd5af661b63bc4e1db9b888fcaa14152a30456492180598e970317`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73d254af54574ed3afe72fa5364772638c1b4735649aec0b2807fc10d57084b`  
		Last Modified: Wed, 10 May 2023 05:39:24 GMT  
		Size: 134.5 MB (134506457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b268c90d009c976bb609f1dc060f3372d12418141823d93d2d29db14f5625cf3`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7`

```console
$ docker pull julia@sha256:65b17bcb5e9b0e15fee247d043bb1cc396bba9749747d117ccfa54e3b3d0a19e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:1.6.7` - linux; amd64

```console
$ docker pull julia@sha256:c8f6b96ab6b715c766a6485a7a499e39e4f233a85204024255417495db4b364b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156470773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede005e31b348b6d9c57ae4140e3b1cc4169876aa04d550d982acbc3fb60b513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:59:25 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 03:59:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:59:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:59:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:59:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8556cf9795a1ce12713f8dbb5b9ea6f9bb70b1003a60254a03f14a5fdb762`  
		Last Modified: Tue, 23 May 2023 04:02:01 GMT  
		Size: 122.6 MB (122640058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865f8dc690e0bceabb40c6e5a2a9436c0dcad7ecc7dc3e21a5d3e49ad9ccd71`  
		Last Modified: Tue, 23 May 2023 04:01:44 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - linux; arm variant v7

```console
$ docker pull julia@sha256:f4697aca57403f3be030882823cc9269406a647fa56986c1937f6447f546f246
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142481887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34f62617e30af6cbf895d9c8b3af1109b3deb4517124543e42c8b907843b041`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 02 May 2023 23:47:57 GMT
ADD file:69d82e947b50a0f0ec610822ffe7c23ec1f6eb41bc17068502380f827cbcce40 in / 
# Tue, 02 May 2023 23:47:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 05:54:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 05:54:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 05:54:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 05:54:54 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 05:54:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 05:54:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9c7c4e67baad3ce38491ce8c1ffaa9ca9ce37409270ce53ab3472054f35d097e`  
		Last Modified: Tue, 02 May 2023 23:51:30 GMT  
		Size: 26.6 MB (26564648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34a33ab1e3a66dc8f0d8f561e66108ac58b4d4dced41b1bd2c872d21b7fd1b4`  
		Last Modified: Wed, 03 May 2023 05:55:43 GMT  
		Size: 2.2 MB (2228960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c904682ccefca56baca0005cbaaa7e757f77bbb19df1e168c78bec2671b8df06`  
		Last Modified: Wed, 03 May 2023 05:56:02 GMT  
		Size: 113.7 MB (113687904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c25c2e61ceda75e6ec1dcfe9627b74e93d7cb99b12ca5452055c0cc0873dc2b`  
		Last Modified: Wed, 03 May 2023 05:55:43 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f0cb7640adf95bc3fc6c603c6eb9a7b76fba164454f4c3563143e0a11af7b136
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148895758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e9f7ff436a74ae2954bf396b8ae0edfc80e22b3d74fce5daef4b5b3157238b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 03:39:14 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 03:39:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 03:39:29 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 03:39:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 03:39:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c52e1f143cd7e48eb844907c2e25b5aa95cbcb28062c943320016844e57d2a`  
		Last Modified: Wed, 03 May 2023 03:42:10 GMT  
		Size: 116.4 MB (116428323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c7d1277473b3cc0fba07efbcccaa604023f1a4ea9ab523a2ef39ab96829404`  
		Last Modified: Wed, 03 May 2023 03:41:56 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - linux; 386

```console
$ docker pull julia@sha256:09f1b083664b7248342acd21dc07e793666bc552b73646cc7ee87796b85e24c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155228544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c6dda947fb24429f880c766fa4bc11e9ab8ab982113dd790cbb6b69b9ef71a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:30:08 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 02:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:30:33 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:30:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:30:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0790b481c61582d040d8872b94795f195b2b3d9ffcd0c8c5d33c0683de187fd9`  
		Last Modified: Tue, 23 May 2023 02:32:58 GMT  
		Size: 120.3 MB (120307491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3193caf127fe61f2d393bacbef592a17eb9e78ab512d6df7c47353b14513a`  
		Last Modified: Tue, 23 May 2023 02:32:33 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:7e0f50fd9c88c790c64e9a40c1c29981368e3ed8cc215601bd5637711c5a6669
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1909494956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb15ee4828117c07bfff86c99bcf233ed017c6f34a308642192fca99d613691`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:32:31 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:32:32 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:32:33 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:33:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:33:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf0017a529e60f82e02af855e1112c244642471771c3c99f5164ce11b0ee914`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a1096533c4db5806a3e5c7f3a69faedb409a6c8733191a7e10d627aa7b325a`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711ca30bcfd5af661b63bc4e1db9b888fcaa14152a30456492180598e970317`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73d254af54574ed3afe72fa5364772638c1b4735649aec0b2807fc10d57084b`  
		Last Modified: Wed, 10 May 2023 05:39:24 GMT  
		Size: 134.5 MB (134506457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b268c90d009c976bb609f1dc060f3372d12418141823d93d2d29db14f5625cf3`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:9054874fbc0f9140b744f296fbdeaf6f28d08c40e7df71f667da8e54c33a5e6e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2206535515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d8896f4558089bbbe91431f87562b48db06f036e265127069eb0740a47f5378`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:33:44 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:33:45 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:33:46 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:35:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:35:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8c72398896ca187419ddbd67e44c1bdcedeba1015bae412c3b223da75bda4`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7de3df320f1d8ecdb0c694655ff678d826cb3cef6bff41a1fa354d3d4e598b7`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd9611b45abc0b498af22640b0dfbccb2244bbeac43b79c1f4b902a92553c38`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71abe049a8b13047f1b307a884567c6d629e6a88a2e42ec2bd1c43779091f46b`  
		Last Modified: Wed, 10 May 2023 05:40:01 GMT  
		Size: 134.5 MB (134493294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6d28206483adb96781bbe2372dfbdc2bc14b263df9e6ed2bc316ef471709b5`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-alpine`

```console
$ docker pull julia@sha256:da0a327e7be2f7885df3d1dd655c8cc6aa3a836aea8ba8201879b91c54cb8f11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.7-alpine` - linux; amd64

```console
$ docker pull julia@sha256:09f04cc2650688a0b1f09fa5b00d7ca2aa6dfdc1c1fc56d43df1c7b5994d7264
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125227359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c573f93d537fc748719d3c445941b2980266c9040453fd503bdab2140f9316c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:35 GMT
ENV JULIA_VERSION=1.6.7
# Mon, 15 May 2023 22:24:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:49 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dedadc624819670ffd0e049086d2f48d10406f443b69833b1c2a05b9489ccf03`  
		Last Modified: Mon, 15 May 2023 22:26:19 GMT  
		Size: 121.8 MB (121829496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b15a60b7a9333ccc46110b56abd98b9e489a72aacade80363bf922904b591c4`  
		Last Modified: Mon, 15 May 2023 22:26:02 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-alpine3.17`

```console
$ docker pull julia@sha256:238ae7ae38c3fc6dc98079321bdf1b65079fc2dacd07ee070b704d8dd48bfc1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.7-alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:7394c3e48e48b3f58565a94afb0bfbc83927f2b5d4dca1ac71fe3dd8aac3f13b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125204596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718b69ebed2b925dbce3d235d056968d4609f2ba2c71035aa818c460f7250a30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 29 Mar 2023 22:04:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 29 Mar 2023 22:06:12 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 04:18:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 03 May 2023 04:18:22 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 04:18:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 04:18:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed41d38c57b45602d3262f4def55c6dbefa6af04c92d86f23e99415807374f47`  
		Last Modified: Wed, 03 May 2023 04:24:46 GMT  
		Size: 121.8 MB (121829659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98547d2af32156d63952e8e82bfb935a225048964a3796385d68e5e8b6d5ddc7`  
		Last Modified: Wed, 03 May 2023 04:24:28 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-alpine3.18`

```console
$ docker pull julia@sha256:da0a327e7be2f7885df3d1dd655c8cc6aa3a836aea8ba8201879b91c54cb8f11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.6.7-alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:09f04cc2650688a0b1f09fa5b00d7ca2aa6dfdc1c1fc56d43df1c7b5994d7264
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125227359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c573f93d537fc748719d3c445941b2980266c9040453fd503bdab2140f9316c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:35 GMT
ENV JULIA_VERSION=1.6.7
# Mon, 15 May 2023 22:24:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.6/julia-1.6.7-musl-x86_64.tar.gz'; 			sha256='d71ccc5aa36cf691616a40bf6fb960fac5620ce53d2f90a95947b90dec509433'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:49 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dedadc624819670ffd0e049086d2f48d10406f443b69833b1c2a05b9489ccf03`  
		Last Modified: Mon, 15 May 2023 22:26:19 GMT  
		Size: 121.8 MB (121829496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b15a60b7a9333ccc46110b56abd98b9e489a72aacade80363bf922904b591c4`  
		Last Modified: Mon, 15 May 2023 22:26:02 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-bullseye`

```console
$ docker pull julia@sha256:39a9ee53836fd23a8506c39bfb7b1c558fa72b7870c04878718891bc0bcaffc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6.7-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:c8f6b96ab6b715c766a6485a7a499e39e4f233a85204024255417495db4b364b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156470773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede005e31b348b6d9c57ae4140e3b1cc4169876aa04d550d982acbc3fb60b513`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:59:25 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 03:59:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:59:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:59:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:59:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a8556cf9795a1ce12713f8dbb5b9ea6f9bb70b1003a60254a03f14a5fdb762`  
		Last Modified: Tue, 23 May 2023 04:02:01 GMT  
		Size: 122.6 MB (122640058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865f8dc690e0bceabb40c6e5a2a9436c0dcad7ecc7dc3e21a5d3e49ad9ccd71`  
		Last Modified: Tue, 23 May 2023 04:01:44 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bullseye` - linux; arm variant v7

```console
$ docker pull julia@sha256:f4697aca57403f3be030882823cc9269406a647fa56986c1937f6447f546f246
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142481887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c34f62617e30af6cbf895d9c8b3af1109b3deb4517124543e42c8b907843b041`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 02 May 2023 23:47:57 GMT
ADD file:69d82e947b50a0f0ec610822ffe7c23ec1f6eb41bc17068502380f827cbcce40 in / 
# Tue, 02 May 2023 23:47:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 05:54:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 05:54:31 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 05:54:31 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 05:54:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 05:54:54 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 05:54:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 05:54:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9c7c4e67baad3ce38491ce8c1ffaa9ca9ce37409270ce53ab3472054f35d097e`  
		Last Modified: Tue, 02 May 2023 23:51:30 GMT  
		Size: 26.6 MB (26564648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34a33ab1e3a66dc8f0d8f561e66108ac58b4d4dced41b1bd2c872d21b7fd1b4`  
		Last Modified: Wed, 03 May 2023 05:55:43 GMT  
		Size: 2.2 MB (2228960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c904682ccefca56baca0005cbaaa7e757f77bbb19df1e168c78bec2671b8df06`  
		Last Modified: Wed, 03 May 2023 05:56:02 GMT  
		Size: 113.7 MB (113687904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c25c2e61ceda75e6ec1dcfe9627b74e93d7cb99b12ca5452055c0cc0873dc2b`  
		Last Modified: Wed, 03 May 2023 05:55:43 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f0cb7640adf95bc3fc6c603c6eb9a7b76fba164454f4c3563143e0a11af7b136
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148895758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e9f7ff436a74ae2954bf396b8ae0edfc80e22b3d74fce5daef4b5b3157238b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 03:39:14 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 03:39:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 03:39:29 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 03:39:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 03:39:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c52e1f143cd7e48eb844907c2e25b5aa95cbcb28062c943320016844e57d2a`  
		Last Modified: Wed, 03 May 2023 03:42:10 GMT  
		Size: 116.4 MB (116428323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c7d1277473b3cc0fba07efbcccaa604023f1a4ea9ab523a2ef39ab96829404`  
		Last Modified: Wed, 03 May 2023 03:41:56 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-bullseye` - linux; 386

```console
$ docker pull julia@sha256:09f1b083664b7248342acd21dc07e793666bc552b73646cc7ee87796b85e24c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155228544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c6dda947fb24429f880c766fa4bc11e9ab8ab982113dd790cbb6b69b9ef71a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:30:08 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 02:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:30:33 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:30:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:30:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0790b481c61582d040d8872b94795f195b2b3d9ffcd0c8c5d33c0683de187fd9`  
		Last Modified: Tue, 23 May 2023 02:32:58 GMT  
		Size: 120.3 MB (120307491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a3193caf127fe61f2d393bacbef592a17eb9e78ab512d6df7c47353b14513a`  
		Last Modified: Tue, 23 May 2023 02:32:33 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-buster`

```console
$ docker pull julia@sha256:20d01af23da6e6a2eb6a800be737ba40d508e9d2edbfbd52a554c45ddae5f253
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.6.7-buster` - linux; amd64

```console
$ docker pull julia@sha256:b129894fbfe5a482db6f7ac2c684ef07e46a0523d39f23a8b157f6c4b45a95e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.3 MB (154261836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1db6637bde6a1ce46560f8470e142047c1749aa2bf38181bb8b1dc7d98fc1968`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:59:44 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 03:59:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:59:58 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:59:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:59:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add0b47570fa87476e546a69dfdf17243a2bdfe9059e797eaa71e66a594c750`  
		Last Modified: Tue, 23 May 2023 04:01:08 GMT  
		Size: 4.5 MB (4472118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17692a645d52ee2258dbcaf3c89ea254a8083182621f8477cf0cd4ce424c5163`  
		Last Modified: Tue, 23 May 2023 04:02:27 GMT  
		Size: 122.7 MB (122650766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bf363d78e34a9aa14726ea83b6dbc224edd234370618c3f950230d3ea9ed09`  
		Last Modified: Tue, 23 May 2023 04:02:09 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:b24936c2be84556a762df86fb53df061a47a8801dad8536b210863c99980bb69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.3 MB (140261465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a21da53aac044df7709949a58a4183a3d47238cdf1e2058388c9c9aad022284`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 02 May 2023 23:48:16 GMT
ADD file:b8cf5ec32175731f2e4d1320020ed59d77bffe001218886fdd42e5aa3d5eda22 in / 
# Tue, 02 May 2023 23:48:16 GMT
CMD ["bash"]
# Wed, 03 May 2023 05:55:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 05:55:08 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 05:55:08 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 05:55:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 05:55:09 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 05:55:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 05:55:29 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 05:55:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 05:55:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:238786c487af66dadc8fb598b41ed76a08602b2a8a746d9c0cea9574cd9c9774`  
		Last Modified: Tue, 02 May 2023 23:52:11 GMT  
		Size: 22.7 MB (22747671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d2da501cd2ba273f52ced0ce21e157286e93568f69124c2f4a123c97a23b4`  
		Last Modified: Wed, 03 May 2023 05:56:11 GMT  
		Size: 3.8 MB (3816282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7bed06a017fc39cecd0f1b4ec51e71471fe97e6dc79c92b9408647209797c18`  
		Last Modified: Wed, 03 May 2023 05:56:31 GMT  
		Size: 113.7 MB (113697137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a2739a797aea02168f607d950eeb025b14584f5f6606626d82a18e74db9628`  
		Last Modified: Wed, 03 May 2023 05:56:10 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:587e2d5d60f716cac12d3a840768b923fd6576f7aa7677c93dafb3ec902c7496
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146709159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59587caa4eaebdb3283b317c3b97680d28d0c4b9dc06f37939b0324987639cba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:23:05 GMT
ADD file:1d8cf95f550bb4b86ad82b22e7195179335fa3b327fd1f1ba1e6c8357ee15c94 in / 
# Wed, 03 May 2023 00:23:05 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:38:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:38:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 03:39:33 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 03 May 2023 03:39:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 03 May 2023 03:39:48 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 03:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 03:39:48 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5627aec4010af613408c2ee78d5d32b9ecac22cb396d702906fb1160721f0011`  
		Last Modified: Wed, 03 May 2023 00:26:29 GMT  
		Size: 25.9 MB (25922039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4bb136449e53562b21b648a615cf43907af192446ee7d880c05b3a8254c8af`  
		Last Modified: Wed, 03 May 2023 03:40:39 GMT  
		Size: 4.4 MB (4350609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec161b9b02f469bf254b49088cf01496b66209e0502e98323f1993e179a6956`  
		Last Modified: Wed, 03 May 2023 03:42:30 GMT  
		Size: 116.4 MB (116436136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc47aac8ede1fa21feadfb93759f58fa2781773e628a2b828e8d148d609986ee`  
		Last Modified: Wed, 03 May 2023 03:42:17 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-buster` - linux; 386

```console
$ docker pull julia@sha256:be141ab28104a9b6bd4c643eef6c4d0038bd49e344b7341c82a8bc43903e9a2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152735514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc9eb1a81e666b39c73e68e226bb01e62c9ce278b7edf6200ca471cf8790027c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:40:01 GMT
ADD file:96715cff0e3569a2a1d7e203f0797ed4880da7714d455e25f032c67bff27221f in / 
# Tue, 23 May 2023 00:40:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:30:36 GMT
ENV JULIA_VERSION=1.6.7
# Tue, 23 May 2023 02:30:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.6/julia-1.6.7-linux-x86_64.tar.gz'; 			sha256='6c4522d595e4cbcd00157ac458a72f8aec01757053d2073f99daa39e442b2a36'; 			;; 		'armhf') 			url='https://julialang-s3.julialang.org/bin/linux/armv7l/1.6/julia-1.6.7-linux-armv7l.tar.gz'; 			sha256='67db7e1f4ad4b9676c26a4659ede8bb9a174346fe22b236f568028c63f02ed2a'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.6/julia-1.6.7-linux-aarch64.tar.gz'; 			sha256='8746d561cbe35e1b83739a84b2637a1d2348728b1d94d76629ad98ff76da6cea'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.6/julia-1.6.7-linux-i686.tar.gz'; 			sha256='d11edad41d2cf4784647e2ac9e304c189bed914cbf38ce4008c668ba789e6df9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:30:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:30:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:30:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3c2058520f8e2dee0c8d97a0e68335849888066e5d0d1b82b6ef302541b5c874`  
		Last Modified: Tue, 23 May 2023 00:45:13 GMT  
		Size: 27.8 MB (27797210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678dd0b30ea1ab93eb8bcc35bcf334b795b36c9b74173148a7dbb8d70fab701`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 4.6 MB (4623824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266a72865041ef1eed5f176498c96078ac607a0398bf1de9a7209c1fad170e0a`  
		Last Modified: Tue, 23 May 2023 02:33:29 GMT  
		Size: 120.3 MB (120314104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d92df80f7e1512fa111860c7220ac566752cc28dfcb04bdbaa0dec0cfe0f9e9`  
		Last Modified: Tue, 23 May 2023 02:33:06 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-windowsservercore`

```console
$ docker pull julia@sha256:f12deffb3a2268bff161c8d459c4e815c65b9f31b5bd652ed070ec2ef37b7e9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:1.6.7-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:7e0f50fd9c88c790c64e9a40c1c29981368e3ed8cc215601bd5637711c5a6669
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1909494956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb15ee4828117c07bfff86c99bcf233ed017c6f34a308642192fca99d613691`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:32:31 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:32:32 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:32:33 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:33:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:33:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf0017a529e60f82e02af855e1112c244642471771c3c99f5164ce11b0ee914`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a1096533c4db5806a3e5c7f3a69faedb409a6c8733191a7e10d627aa7b325a`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711ca30bcfd5af661b63bc4e1db9b888fcaa14152a30456492180598e970317`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73d254af54574ed3afe72fa5364772638c1b4735649aec0b2807fc10d57084b`  
		Last Modified: Wed, 10 May 2023 05:39:24 GMT  
		Size: 134.5 MB (134506457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b268c90d009c976bb609f1dc060f3372d12418141823d93d2d29db14f5625cf3`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.7-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:9054874fbc0f9140b744f296fbdeaf6f28d08c40e7df71f667da8e54c33a5e6e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2206535515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d8896f4558089bbbe91431f87562b48db06f036e265127069eb0740a47f5378`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:33:44 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:33:45 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:33:46 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:35:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:35:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8c72398896ca187419ddbd67e44c1bdcedeba1015bae412c3b223da75bda4`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7de3df320f1d8ecdb0c694655ff678d826cb3cef6bff41a1fa354d3d4e598b7`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd9611b45abc0b498af22640b0dfbccb2244bbeac43b79c1f4b902a92553c38`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71abe049a8b13047f1b307a884567c6d629e6a88a2e42ec2bd1c43779091f46b`  
		Last Modified: Wed, 10 May 2023 05:40:01 GMT  
		Size: 134.5 MB (134493294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6d28206483adb96781bbe2372dfbdc2bc14b263df9e6ed2bc316ef471709b5`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-windowsservercore-1809`

```console
$ docker pull julia@sha256:85588bb3893e999913f74c591fe0ae82acc9da116f7dc0160e6267b29475c237
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `julia:1.6.7-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:9054874fbc0f9140b744f296fbdeaf6f28d08c40e7df71f667da8e54c33a5e6e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2206535515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d8896f4558089bbbe91431f87562b48db06f036e265127069eb0740a47f5378`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:33:44 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:33:45 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:33:46 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:35:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:35:32 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8c72398896ca187419ddbd67e44c1bdcedeba1015bae412c3b223da75bda4`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7de3df320f1d8ecdb0c694655ff678d826cb3cef6bff41a1fa354d3d4e598b7`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd9611b45abc0b498af22640b0dfbccb2244bbeac43b79c1f4b902a92553c38`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71abe049a8b13047f1b307a884567c6d629e6a88a2e42ec2bd1c43779091f46b`  
		Last Modified: Wed, 10 May 2023 05:40:01 GMT  
		Size: 134.5 MB (134493294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6d28206483adb96781bbe2372dfbdc2bc14b263df9e6ed2bc316ef471709b5`  
		Last Modified: Wed, 10 May 2023 05:39:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.6.7-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:347d7a805c07c435afdf3976dd6629f86a463acf8117afd1d3cc683a764e4636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `julia:1.6.7-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:7e0f50fd9c88c790c64e9a40c1c29981368e3ed8cc215601bd5637711c5a6669
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1909494956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb15ee4828117c07bfff86c99bcf233ed017c6f34a308642192fca99d613691`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 05:32:31 GMT
ENV JULIA_VERSION=1.6.7
# Wed, 10 May 2023 05:32:32 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.6/julia-1.6.7-win64.exe
# Wed, 10 May 2023 05:32:33 GMT
ENV JULIA_SHA256=20a4bdca8314a6193472ee29f470ba02a1f8ffd7a803342896fcbbf61bf3d4c8
# Wed, 10 May 2023 05:33:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 05:33:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf0017a529e60f82e02af855e1112c244642471771c3c99f5164ce11b0ee914`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a1096533c4db5806a3e5c7f3a69faedb409a6c8733191a7e10d627aa7b325a`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711ca30bcfd5af661b63bc4e1db9b888fcaa14152a30456492180598e970317`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73d254af54574ed3afe72fa5364772638c1b4735649aec0b2807fc10d57084b`  
		Last Modified: Wed, 10 May 2023 05:39:24 GMT  
		Size: 134.5 MB (134506457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b268c90d009c976bb609f1dc060f3372d12418141823d93d2d29db14f5625cf3`  
		Last Modified: Wed, 10 May 2023 05:38:59 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9`

```console
$ docker pull julia@sha256:36902255c08939b511a37508150a2883abd51afacbeab0d461635d7f5f644e6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:1.9` - linux; amd64

```console
$ docker pull julia@sha256:1baf0ab6fb6c474d216468d960333ffde38ccb3c76bb7f830c416d0d024412e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182524441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0394c94147bb57936f72c3b7d0ff8f2bdf98d7adc929d5fe3fa528b7339c4d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:58:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:58:41 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:58:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:58:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c421a694ca3262d6955441bf869575152e027f158a67a5fca1069ca8806102`  
		Last Modified: Tue, 23 May 2023 04:00:55 GMT  
		Size: 148.7 MB (148693723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4d7795ec1ad44b7fb4ee919ddeb55611a858900c4d78219ec62c0518711be9`  
		Last Modified: Tue, 23 May 2023 04:00:33 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5e2977123b1cfe0518c291316ab3931d4b194fb628e97df6062a8067b1d35328
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.4 MB (175390009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ce886a6f78d5c7d285a05c16e8d159ea755355ed2843492a291bc61382736e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:20 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:44:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:44:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:44:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2616bb8cca402291d62dd06f67f3c3597f3042a4e8304a488e7db91581127cdf`  
		Last Modified: Wed, 10 May 2023 17:45:38 GMT  
		Size: 142.9 MB (142922569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc3b0ff727d110588d9b4875a9023116e1bc994d1b0dc5043d3ee86d66b1413`  
		Last Modified: Wed, 10 May 2023 17:45:21 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9` - linux; 386

```console
$ docker pull julia@sha256:7abf4e29ba01e1411695848991b2db643582481665fbefb816e49a5b70e9cb2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.7 MB (180735444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82a6bcb39c5b8202e58fc03ec47e602516000881cf4a2cb2f99998dc76d2603`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:02 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:29:26 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:29:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:29:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c55db0a6af6b3d85fb7c5a15e0d4c95f7e806ffa98208ce7ef735b7fc6725`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 145.8 MB (145814394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1668b9c92f4ae6e6ae9db09e901b457cce51b2a4ad763d409af5acd1499a971`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9` - linux; ppc64le

```console
$ docker pull julia@sha256:fb992d3e811683d5a7acb40e070aa5cf48e0c551496021b7a3b986619326fb59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171094683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c12da7cffc9305381fb6312a99958195846c536f37834527c9e4ef8b94b61e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:07:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:07:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:08:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:08:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:08:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:08:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a7cd9dea84bb9d934231269410340992f182978f4edef2332551db9339895`  
		Last Modified: Tue, 23 May 2023 02:08:20 GMT  
		Size: 2.6 MB (2627396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b277918387795ff9e75af87373fb080fc7e519c3608df2d74dbbdaa2ad80c9`  
		Last Modified: Tue, 23 May 2023 02:08:55 GMT  
		Size: 133.2 MB (133185997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c2c74cab468cff7d8a1904dc5d697186d7ef6fe72b630d69ad8a14624a37b`  
		Last Modified: Tue, 23 May 2023 02:08:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-alpine`

```console
$ docker pull julia@sha256:9df2dbe2638111d1133a5d401f981c46e7c98ae2c8fd2d21961a5e5ee13156f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9-alpine` - linux; amd64

```console
$ docker pull julia@sha256:9ed027843d8b3172d329dc5c1d2c6a6e587e748c42148cef8760a8fccbb83b85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153983502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82888c0d329cf435c73c43c4d89b154f6c0aaeb5468851cdf4364ae43472fec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_VERSION=1.9.0
# Mon, 15 May 2023 22:24:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:28 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3362ee69b9e183770605ef4b78cc162da6ed0150fa898768ebcb885a75ad3`  
		Last Modified: Mon, 15 May 2023 22:25:39 GMT  
		Size: 150.6 MB (150585641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee82d7382bfddf890d4621823ade41cd9210f9d81b1e38b44b6696272338b8`  
		Last Modified: Mon, 15 May 2023 22:25:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-alpine3.17`

```console
$ docker pull julia@sha256:7f878f474243a69885585625807077d702d3c9a4c45af3bcb6620cbd5c59b503
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9-alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:f7b02fd0227eea383b76adac8f09121d3ce02fd4e2478d1422c2cdc851b79080
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153960395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea35812b9c8ce031bdf4d24d5cc14f53019dfe24d654cc51b06ba88beebee658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 29 Mar 2023 22:04:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:53:52 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:54:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 10 May 2023 17:54:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:54:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b199db89e2a6dd5f8f853e5b18e6e77a15d775d9158e7880a86156b68e361e`  
		Last Modified: Wed, 10 May 2023 17:56:36 GMT  
		Size: 150.6 MB (150585459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0840a682c27557acbad940eaff83e57fd9fd217b43b6f2de6bafd7c0fee7b04`  
		Last Modified: Wed, 10 May 2023 17:56:14 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-alpine3.18`

```console
$ docker pull julia@sha256:9df2dbe2638111d1133a5d401f981c46e7c98ae2c8fd2d21961a5e5ee13156f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9-alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:9ed027843d8b3172d329dc5c1d2c6a6e587e748c42148cef8760a8fccbb83b85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153983502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82888c0d329cf435c73c43c4d89b154f6c0aaeb5468851cdf4364ae43472fec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_VERSION=1.9.0
# Mon, 15 May 2023 22:24:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:28 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3362ee69b9e183770605ef4b78cc162da6ed0150fa898768ebcb885a75ad3`  
		Last Modified: Mon, 15 May 2023 22:25:39 GMT  
		Size: 150.6 MB (150585641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee82d7382bfddf890d4621823ade41cd9210f9d81b1e38b44b6696272338b8`  
		Last Modified: Mon, 15 May 2023 22:25:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-bullseye`

```console
$ docker pull julia@sha256:b031ec96e64d1a0a90b48ced4bc4a4fdaba9e13f61c199809289ace462695178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.9-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:1baf0ab6fb6c474d216468d960333ffde38ccb3c76bb7f830c416d0d024412e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182524441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0394c94147bb57936f72c3b7d0ff8f2bdf98d7adc929d5fe3fa528b7339c4d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:58:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:58:41 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:58:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:58:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c421a694ca3262d6955441bf869575152e027f158a67a5fca1069ca8806102`  
		Last Modified: Tue, 23 May 2023 04:00:55 GMT  
		Size: 148.7 MB (148693723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4d7795ec1ad44b7fb4ee919ddeb55611a858900c4d78219ec62c0518711be9`  
		Last Modified: Tue, 23 May 2023 04:00:33 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5e2977123b1cfe0518c291316ab3931d4b194fb628e97df6062a8067b1d35328
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.4 MB (175390009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ce886a6f78d5c7d285a05c16e8d159ea755355ed2843492a291bc61382736e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:20 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:44:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:44:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:44:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2616bb8cca402291d62dd06f67f3c3597f3042a4e8304a488e7db91581127cdf`  
		Last Modified: Wed, 10 May 2023 17:45:38 GMT  
		Size: 142.9 MB (142922569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc3b0ff727d110588d9b4875a9023116e1bc994d1b0dc5043d3ee86d66b1413`  
		Last Modified: Wed, 10 May 2023 17:45:21 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-bullseye` - linux; 386

```console
$ docker pull julia@sha256:7abf4e29ba01e1411695848991b2db643582481665fbefb816e49a5b70e9cb2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.7 MB (180735444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82a6bcb39c5b8202e58fc03ec47e602516000881cf4a2cb2f99998dc76d2603`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:02 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:29:26 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:29:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:29:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c55db0a6af6b3d85fb7c5a15e0d4c95f7e806ffa98208ce7ef735b7fc6725`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 145.8 MB (145814394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1668b9c92f4ae6e6ae9db09e901b457cce51b2a4ad763d409af5acd1499a971`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:fb992d3e811683d5a7acb40e070aa5cf48e0c551496021b7a3b986619326fb59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171094683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c12da7cffc9305381fb6312a99958195846c536f37834527c9e4ef8b94b61e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:07:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:07:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:08:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:08:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:08:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:08:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a7cd9dea84bb9d934231269410340992f182978f4edef2332551db9339895`  
		Last Modified: Tue, 23 May 2023 02:08:20 GMT  
		Size: 2.6 MB (2627396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b277918387795ff9e75af87373fb080fc7e519c3608df2d74dbbdaa2ad80c9`  
		Last Modified: Tue, 23 May 2023 02:08:55 GMT  
		Size: 133.2 MB (133185997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c2c74cab468cff7d8a1904dc5d697186d7ef6fe72b630d69ad8a14624a37b`  
		Last Modified: Tue, 23 May 2023 02:08:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-buster`

```console
$ docker pull julia@sha256:ef4f187da55bd84a6e754aa15bbd8b293cc8746c224cad2e522907d23f7f24d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.9-buster` - linux; amd64

```console
$ docker pull julia@sha256:a616d9ed55df3b4e5943dfc9794af3cd60f86f05dda5e0bafed5bf3bacbb203b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180302639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c1122d78b068c53d117c09b5ca780be1391bab12f89990c84ea547db7272bc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:59:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:59:14 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:59:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add0b47570fa87476e546a69dfdf17243a2bdfe9059e797eaa71e66a594c750`  
		Last Modified: Tue, 23 May 2023 04:01:08 GMT  
		Size: 4.5 MB (4472118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3dfa17601b0c6337c1d87a32b4533f1bf5d06ccb3cd50ccf3c60d135b9418d`  
		Last Modified: Tue, 23 May 2023 04:01:30 GMT  
		Size: 148.7 MB (148691569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e65c1f2b4a861c50f9070a5ec00ccad08d555f838567262169d38f4da444b6`  
		Last Modified: Tue, 23 May 2023 04:01:07 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1c318c6cf16dc00c022b64202164701af68203394f1f7a7368396b2fc684b172
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173191012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c396b9151522a26e360c8ff6c077cdc17cd73edc217f556c96bb4052c09f52f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:23:05 GMT
ADD file:1d8cf95f550bb4b86ad82b22e7195179335fa3b327fd1f1ba1e6c8357ee15c94 in / 
# Wed, 03 May 2023 00:23:05 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:38:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:38:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:43 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:45:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:45:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:45:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:45:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5627aec4010af613408c2ee78d5d32b9ecac22cb396d702906fb1160721f0011`  
		Last Modified: Wed, 03 May 2023 00:26:29 GMT  
		Size: 25.9 MB (25922039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4bb136449e53562b21b648a615cf43907af192446ee7d880c05b3a8254c8af`  
		Last Modified: Wed, 03 May 2023 03:40:39 GMT  
		Size: 4.4 MB (4350609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ca056492e3a7e4b3c199f8a889b9183b1a75edb249a08e1d8786c7b4d8cad8`  
		Last Modified: Wed, 10 May 2023 17:46:07 GMT  
		Size: 142.9 MB (142917988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee770aa11ecd8ad59c9dfc316a7ce4b28e594d1bf3d5467b6a85ed956a3863c`  
		Last Modified: Wed, 10 May 2023 17:45:50 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-buster` - linux; 386

```console
$ docker pull julia@sha256:255f7543d0e6dba32bffdc3ae60e70270c061eb49973957af547ba0e6261139a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178248531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:056069102655d640917bef51c63d30efa8aac4fecf2bb3f8da960cee2a11c3f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:40:01 GMT
ADD file:96715cff0e3569a2a1d7e203f0797ed4880da7714d455e25f032c67bff27221f in / 
# Tue, 23 May 2023 00:40:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:37 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:30:00 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:30:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:30:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3c2058520f8e2dee0c8d97a0e68335849888066e5d0d1b82b6ef302541b5c874`  
		Last Modified: Tue, 23 May 2023 00:45:13 GMT  
		Size: 27.8 MB (27797210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678dd0b30ea1ab93eb8bcc35bcf334b795b36c9b74173148a7dbb8d70fab701`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 4.6 MB (4623824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83a140272f2611b1f4445691bb0ac4abbb87dd9d4ac6f5f9d505bf97ece32fe`  
		Last Modified: Tue, 23 May 2023 02:32:21 GMT  
		Size: 145.8 MB (145827125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01965ecc75242364a50d7ecb78bc7ae189013003af9f27b68e7bbdff182061b7`  
		Last Modified: Tue, 23 May 2023 02:31:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-windowsservercore`

```console
$ docker pull julia@sha256:51427d8cfaf9d87867929fe0bcf0652465c5618261c3c24e482d35e62084c6d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:1.9-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-windowsservercore-1809`

```console
$ docker pull julia@sha256:30526016f4cdb9c4c5c531ce9e9955b2328b495c64587b2767af1ad1561439b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `julia:1.9-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:604ba14a26f6b140f5e4e281daa12fa2b1f4ef444781bf3b30b3d4aeaf404417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `julia:1.9-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.0`

```console
$ docker pull julia@sha256:36902255c08939b511a37508150a2883abd51afacbeab0d461635d7f5f644e6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:1.9.0` - linux; amd64

```console
$ docker pull julia@sha256:1baf0ab6fb6c474d216468d960333ffde38ccb3c76bb7f830c416d0d024412e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182524441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0394c94147bb57936f72c3b7d0ff8f2bdf98d7adc929d5fe3fa528b7339c4d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:58:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:58:41 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:58:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:58:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c421a694ca3262d6955441bf869575152e027f158a67a5fca1069ca8806102`  
		Last Modified: Tue, 23 May 2023 04:00:55 GMT  
		Size: 148.7 MB (148693723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4d7795ec1ad44b7fb4ee919ddeb55611a858900c4d78219ec62c0518711be9`  
		Last Modified: Tue, 23 May 2023 04:00:33 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5e2977123b1cfe0518c291316ab3931d4b194fb628e97df6062a8067b1d35328
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.4 MB (175390009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ce886a6f78d5c7d285a05c16e8d159ea755355ed2843492a291bc61382736e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:20 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:44:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:44:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:44:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2616bb8cca402291d62dd06f67f3c3597f3042a4e8304a488e7db91581127cdf`  
		Last Modified: Wed, 10 May 2023 17:45:38 GMT  
		Size: 142.9 MB (142922569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc3b0ff727d110588d9b4875a9023116e1bc994d1b0dc5043d3ee86d66b1413`  
		Last Modified: Wed, 10 May 2023 17:45:21 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.0` - linux; 386

```console
$ docker pull julia@sha256:7abf4e29ba01e1411695848991b2db643582481665fbefb816e49a5b70e9cb2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.7 MB (180735444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82a6bcb39c5b8202e58fc03ec47e602516000881cf4a2cb2f99998dc76d2603`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:02 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:29:26 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:29:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:29:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c55db0a6af6b3d85fb7c5a15e0d4c95f7e806ffa98208ce7ef735b7fc6725`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 145.8 MB (145814394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1668b9c92f4ae6e6ae9db09e901b457cce51b2a4ad763d409af5acd1499a971`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.0` - linux; ppc64le

```console
$ docker pull julia@sha256:fb992d3e811683d5a7acb40e070aa5cf48e0c551496021b7a3b986619326fb59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171094683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c12da7cffc9305381fb6312a99958195846c536f37834527c9e4ef8b94b61e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:07:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:07:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:08:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:08:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:08:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:08:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a7cd9dea84bb9d934231269410340992f182978f4edef2332551db9339895`  
		Last Modified: Tue, 23 May 2023 02:08:20 GMT  
		Size: 2.6 MB (2627396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b277918387795ff9e75af87373fb080fc7e519c3608df2d74dbbdaa2ad80c9`  
		Last Modified: Tue, 23 May 2023 02:08:55 GMT  
		Size: 133.2 MB (133185997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c2c74cab468cff7d8a1904dc5d697186d7ef6fe72b630d69ad8a14624a37b`  
		Last Modified: Tue, 23 May 2023 02:08:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.0` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.0` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.0-alpine`

```console
$ docker pull julia@sha256:9df2dbe2638111d1133a5d401f981c46e7c98ae2c8fd2d21961a5e5ee13156f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9.0-alpine` - linux; amd64

```console
$ docker pull julia@sha256:9ed027843d8b3172d329dc5c1d2c6a6e587e748c42148cef8760a8fccbb83b85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153983502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82888c0d329cf435c73c43c4d89b154f6c0aaeb5468851cdf4364ae43472fec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_VERSION=1.9.0
# Mon, 15 May 2023 22:24:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:28 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3362ee69b9e183770605ef4b78cc162da6ed0150fa898768ebcb885a75ad3`  
		Last Modified: Mon, 15 May 2023 22:25:39 GMT  
		Size: 150.6 MB (150585641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee82d7382bfddf890d4621823ade41cd9210f9d81b1e38b44b6696272338b8`  
		Last Modified: Mon, 15 May 2023 22:25:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.0-alpine3.17`

```console
$ docker pull julia@sha256:7f878f474243a69885585625807077d702d3c9a4c45af3bcb6620cbd5c59b503
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9.0-alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:f7b02fd0227eea383b76adac8f09121d3ce02fd4e2478d1422c2cdc851b79080
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153960395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea35812b9c8ce031bdf4d24d5cc14f53019dfe24d654cc51b06ba88beebee658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 29 Mar 2023 22:04:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:53:52 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:54:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 10 May 2023 17:54:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:54:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b199db89e2a6dd5f8f853e5b18e6e77a15d775d9158e7880a86156b68e361e`  
		Last Modified: Wed, 10 May 2023 17:56:36 GMT  
		Size: 150.6 MB (150585459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0840a682c27557acbad940eaff83e57fd9fd217b43b6f2de6bafd7c0fee7b04`  
		Last Modified: Wed, 10 May 2023 17:56:14 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.0-alpine3.18`

```console
$ docker pull julia@sha256:9df2dbe2638111d1133a5d401f981c46e7c98ae2c8fd2d21961a5e5ee13156f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1.9.0-alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:9ed027843d8b3172d329dc5c1d2c6a6e587e748c42148cef8760a8fccbb83b85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153983502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82888c0d329cf435c73c43c4d89b154f6c0aaeb5468851cdf4364ae43472fec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_VERSION=1.9.0
# Mon, 15 May 2023 22:24:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:28 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3362ee69b9e183770605ef4b78cc162da6ed0150fa898768ebcb885a75ad3`  
		Last Modified: Mon, 15 May 2023 22:25:39 GMT  
		Size: 150.6 MB (150585641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee82d7382bfddf890d4621823ade41cd9210f9d81b1e38b44b6696272338b8`  
		Last Modified: Mon, 15 May 2023 22:25:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.0-bullseye`

```console
$ docker pull julia@sha256:b031ec96e64d1a0a90b48ced4bc4a4fdaba9e13f61c199809289ace462695178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:1.9.0-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:1baf0ab6fb6c474d216468d960333ffde38ccb3c76bb7f830c416d0d024412e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182524441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0394c94147bb57936f72c3b7d0ff8f2bdf98d7adc929d5fe3fa528b7339c4d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:58:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:58:41 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:58:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:58:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c421a694ca3262d6955441bf869575152e027f158a67a5fca1069ca8806102`  
		Last Modified: Tue, 23 May 2023 04:00:55 GMT  
		Size: 148.7 MB (148693723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4d7795ec1ad44b7fb4ee919ddeb55611a858900c4d78219ec62c0518711be9`  
		Last Modified: Tue, 23 May 2023 04:00:33 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5e2977123b1cfe0518c291316ab3931d4b194fb628e97df6062a8067b1d35328
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.4 MB (175390009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ce886a6f78d5c7d285a05c16e8d159ea755355ed2843492a291bc61382736e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:20 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:44:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:44:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:44:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2616bb8cca402291d62dd06f67f3c3597f3042a4e8304a488e7db91581127cdf`  
		Last Modified: Wed, 10 May 2023 17:45:38 GMT  
		Size: 142.9 MB (142922569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc3b0ff727d110588d9b4875a9023116e1bc994d1b0dc5043d3ee86d66b1413`  
		Last Modified: Wed, 10 May 2023 17:45:21 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.0-bullseye` - linux; 386

```console
$ docker pull julia@sha256:7abf4e29ba01e1411695848991b2db643582481665fbefb816e49a5b70e9cb2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.7 MB (180735444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82a6bcb39c5b8202e58fc03ec47e602516000881cf4a2cb2f99998dc76d2603`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:02 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:29:26 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:29:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:29:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c55db0a6af6b3d85fb7c5a15e0d4c95f7e806ffa98208ce7ef735b7fc6725`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 145.8 MB (145814394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1668b9c92f4ae6e6ae9db09e901b457cce51b2a4ad763d409af5acd1499a971`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.0-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:fb992d3e811683d5a7acb40e070aa5cf48e0c551496021b7a3b986619326fb59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171094683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c12da7cffc9305381fb6312a99958195846c536f37834527c9e4ef8b94b61e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:07:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:07:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:08:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:08:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:08:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:08:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a7cd9dea84bb9d934231269410340992f182978f4edef2332551db9339895`  
		Last Modified: Tue, 23 May 2023 02:08:20 GMT  
		Size: 2.6 MB (2627396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b277918387795ff9e75af87373fb080fc7e519c3608df2d74dbbdaa2ad80c9`  
		Last Modified: Tue, 23 May 2023 02:08:55 GMT  
		Size: 133.2 MB (133185997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c2c74cab468cff7d8a1904dc5d697186d7ef6fe72b630d69ad8a14624a37b`  
		Last Modified: Tue, 23 May 2023 02:08:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.0-buster`

```console
$ docker pull julia@sha256:ef4f187da55bd84a6e754aa15bbd8b293cc8746c224cad2e522907d23f7f24d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.9.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:a616d9ed55df3b4e5943dfc9794af3cd60f86f05dda5e0bafed5bf3bacbb203b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180302639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c1122d78b068c53d117c09b5ca780be1391bab12f89990c84ea547db7272bc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:59:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:59:14 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:59:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add0b47570fa87476e546a69dfdf17243a2bdfe9059e797eaa71e66a594c750`  
		Last Modified: Tue, 23 May 2023 04:01:08 GMT  
		Size: 4.5 MB (4472118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3dfa17601b0c6337c1d87a32b4533f1bf5d06ccb3cd50ccf3c60d135b9418d`  
		Last Modified: Tue, 23 May 2023 04:01:30 GMT  
		Size: 148.7 MB (148691569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e65c1f2b4a861c50f9070a5ec00ccad08d555f838567262169d38f4da444b6`  
		Last Modified: Tue, 23 May 2023 04:01:07 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1c318c6cf16dc00c022b64202164701af68203394f1f7a7368396b2fc684b172
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173191012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c396b9151522a26e360c8ff6c077cdc17cd73edc217f556c96bb4052c09f52f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:23:05 GMT
ADD file:1d8cf95f550bb4b86ad82b22e7195179335fa3b327fd1f1ba1e6c8357ee15c94 in / 
# Wed, 03 May 2023 00:23:05 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:38:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:38:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:43 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:45:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:45:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:45:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:45:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5627aec4010af613408c2ee78d5d32b9ecac22cb396d702906fb1160721f0011`  
		Last Modified: Wed, 03 May 2023 00:26:29 GMT  
		Size: 25.9 MB (25922039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4bb136449e53562b21b648a615cf43907af192446ee7d880c05b3a8254c8af`  
		Last Modified: Wed, 03 May 2023 03:40:39 GMT  
		Size: 4.4 MB (4350609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ca056492e3a7e4b3c199f8a889b9183b1a75edb249a08e1d8786c7b4d8cad8`  
		Last Modified: Wed, 10 May 2023 17:46:07 GMT  
		Size: 142.9 MB (142917988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee770aa11ecd8ad59c9dfc316a7ce4b28e594d1bf3d5467b6a85ed956a3863c`  
		Last Modified: Wed, 10 May 2023 17:45:50 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.0-buster` - linux; 386

```console
$ docker pull julia@sha256:255f7543d0e6dba32bffdc3ae60e70270c061eb49973957af547ba0e6261139a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178248531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:056069102655d640917bef51c63d30efa8aac4fecf2bb3f8da960cee2a11c3f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:40:01 GMT
ADD file:96715cff0e3569a2a1d7e203f0797ed4880da7714d455e25f032c67bff27221f in / 
# Tue, 23 May 2023 00:40:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:37 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:30:00 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:30:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:30:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3c2058520f8e2dee0c8d97a0e68335849888066e5d0d1b82b6ef302541b5c874`  
		Last Modified: Tue, 23 May 2023 00:45:13 GMT  
		Size: 27.8 MB (27797210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678dd0b30ea1ab93eb8bcc35bcf334b795b36c9b74173148a7dbb8d70fab701`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 4.6 MB (4623824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83a140272f2611b1f4445691bb0ac4abbb87dd9d4ac6f5f9d505bf97ece32fe`  
		Last Modified: Tue, 23 May 2023 02:32:21 GMT  
		Size: 145.8 MB (145827125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01965ecc75242364a50d7ecb78bc7ae189013003af9f27b68e7bbdff182061b7`  
		Last Modified: Tue, 23 May 2023 02:31:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.0-windowsservercore`

```console
$ docker pull julia@sha256:51427d8cfaf9d87867929fe0bcf0652465c5618261c3c24e482d35e62084c6d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:1.9.0-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.9.0-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:30526016f4cdb9c4c5c531ce9e9955b2328b495c64587b2767af1ad1561439b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `julia:1.9.0-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.9.0-windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:604ba14a26f6b140f5e4e281daa12fa2b1f4ef444781bf3b30b3d4aeaf404417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `julia:1.9.0-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine`

```console
$ docker pull julia@sha256:9df2dbe2638111d1133a5d401f981c46e7c98ae2c8fd2d21961a5e5ee13156f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine` - linux; amd64

```console
$ docker pull julia@sha256:9ed027843d8b3172d329dc5c1d2c6a6e587e748c42148cef8760a8fccbb83b85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153983502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82888c0d329cf435c73c43c4d89b154f6c0aaeb5468851cdf4364ae43472fec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_VERSION=1.9.0
# Mon, 15 May 2023 22:24:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:28 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3362ee69b9e183770605ef4b78cc162da6ed0150fa898768ebcb885a75ad3`  
		Last Modified: Mon, 15 May 2023 22:25:39 GMT  
		Size: 150.6 MB (150585641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee82d7382bfddf890d4621823ade41cd9210f9d81b1e38b44b6696272338b8`  
		Last Modified: Mon, 15 May 2023 22:25:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.17`

```console
$ docker pull julia@sha256:7f878f474243a69885585625807077d702d3c9a4c45af3bcb6620cbd5c59b503
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:f7b02fd0227eea383b76adac8f09121d3ce02fd4e2478d1422c2cdc851b79080
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153960395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea35812b9c8ce031bdf4d24d5cc14f53019dfe24d654cc51b06ba88beebee658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 29 Mar 2023 22:04:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 22:04:46 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:53:52 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:54:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 10 May 2023 17:54:11 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:54:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b199db89e2a6dd5f8f853e5b18e6e77a15d775d9158e7880a86156b68e361e`  
		Last Modified: Wed, 10 May 2023 17:56:36 GMT  
		Size: 150.6 MB (150585459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0840a682c27557acbad940eaff83e57fd9fd217b43b6f2de6bafd7c0fee7b04`  
		Last Modified: Wed, 10 May 2023 17:56:14 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:alpine3.18`

```console
$ docker pull julia@sha256:9df2dbe2638111d1133a5d401f981c46e7c98ae2c8fd2d21961a5e5ee13156f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.18` - linux; amd64

```console
$ docker pull julia@sha256:9ed027843d8b3172d329dc5c1d2c6a6e587e748c42148cef8760a8fccbb83b85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153983502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82888c0d329cf435c73c43c4d89b154f6c0aaeb5468851cdf4364ae43472fec1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 15 May 2023 22:24:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 15 May 2023 22:24:11 GMT
ENV JULIA_VERSION=1.9.0
# Mon, 15 May 2023 22:24:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-musl-x86_64.tar.gz'; 			sha256='2594ff9a69d86415faae2e2e218ec3a5abbeb41ab3590b646b75824221adcb5b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 15 May 2023 22:24:28 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Mon, 15 May 2023 22:24:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 May 2023 22:24:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c3362ee69b9e183770605ef4b78cc162da6ed0150fa898768ebcb885a75ad3`  
		Last Modified: Mon, 15 May 2023 22:25:39 GMT  
		Size: 150.6 MB (150585641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ee82d7382bfddf890d4621823ade41cd9210f9d81b1e38b44b6696272338b8`  
		Last Modified: Mon, 15 May 2023 22:25:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:bullseye`

```console
$ docker pull julia@sha256:b031ec96e64d1a0a90b48ced4bc4a4fdaba9e13f61c199809289ace462695178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:bullseye` - linux; amd64

```console
$ docker pull julia@sha256:1baf0ab6fb6c474d216468d960333ffde38ccb3c76bb7f830c416d0d024412e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182524441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0394c94147bb57936f72c3b7d0ff8f2bdf98d7adc929d5fe3fa528b7339c4d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:58:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:58:41 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:58:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:58:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c421a694ca3262d6955441bf869575152e027f158a67a5fca1069ca8806102`  
		Last Modified: Tue, 23 May 2023 04:00:55 GMT  
		Size: 148.7 MB (148693723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4d7795ec1ad44b7fb4ee919ddeb55611a858900c4d78219ec62c0518711be9`  
		Last Modified: Tue, 23 May 2023 04:00:33 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5e2977123b1cfe0518c291316ab3931d4b194fb628e97df6062a8067b1d35328
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.4 MB (175390009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ce886a6f78d5c7d285a05c16e8d159ea755355ed2843492a291bc61382736e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:20 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:44:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:44:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:44:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2616bb8cca402291d62dd06f67f3c3597f3042a4e8304a488e7db91581127cdf`  
		Last Modified: Wed, 10 May 2023 17:45:38 GMT  
		Size: 142.9 MB (142922569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc3b0ff727d110588d9b4875a9023116e1bc994d1b0dc5043d3ee86d66b1413`  
		Last Modified: Wed, 10 May 2023 17:45:21 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; 386

```console
$ docker pull julia@sha256:7abf4e29ba01e1411695848991b2db643582481665fbefb816e49a5b70e9cb2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.7 MB (180735444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82a6bcb39c5b8202e58fc03ec47e602516000881cf4a2cb2f99998dc76d2603`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:02 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:29:26 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:29:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:29:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c55db0a6af6b3d85fb7c5a15e0d4c95f7e806ffa98208ce7ef735b7fc6725`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 145.8 MB (145814394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1668b9c92f4ae6e6ae9db09e901b457cce51b2a4ad763d409af5acd1499a971`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:fb992d3e811683d5a7acb40e070aa5cf48e0c551496021b7a3b986619326fb59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171094683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c12da7cffc9305381fb6312a99958195846c536f37834527c9e4ef8b94b61e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:07:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:07:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:08:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:08:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:08:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:08:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a7cd9dea84bb9d934231269410340992f182978f4edef2332551db9339895`  
		Last Modified: Tue, 23 May 2023 02:08:20 GMT  
		Size: 2.6 MB (2627396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b277918387795ff9e75af87373fb080fc7e519c3608df2d74dbbdaa2ad80c9`  
		Last Modified: Tue, 23 May 2023 02:08:55 GMT  
		Size: 133.2 MB (133185997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c2c74cab468cff7d8a1904dc5d697186d7ef6fe72b630d69ad8a14624a37b`  
		Last Modified: Tue, 23 May 2023 02:08:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:buster`

```console
$ docker pull julia@sha256:ef4f187da55bd84a6e754aa15bbd8b293cc8746c224cad2e522907d23f7f24d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:a616d9ed55df3b4e5943dfc9794af3cd60f86f05dda5e0bafed5bf3bacbb203b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.3 MB (180302639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c1122d78b068c53d117c09b5ca780be1391bab12f89990c84ea547db7272bc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:56 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:59:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:59:14 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:59:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add0b47570fa87476e546a69dfdf17243a2bdfe9059e797eaa71e66a594c750`  
		Last Modified: Tue, 23 May 2023 04:01:08 GMT  
		Size: 4.5 MB (4472118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3dfa17601b0c6337c1d87a32b4533f1bf5d06ccb3cd50ccf3c60d135b9418d`  
		Last Modified: Tue, 23 May 2023 04:01:30 GMT  
		Size: 148.7 MB (148691569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e65c1f2b4a861c50f9070a5ec00ccad08d555f838567262169d38f4da444b6`  
		Last Modified: Tue, 23 May 2023 04:01:07 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:1c318c6cf16dc00c022b64202164701af68203394f1f7a7368396b2fc684b172
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173191012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c396b9151522a26e360c8ff6c077cdc17cd73edc217f556c96bb4052c09f52f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:23:05 GMT
ADD file:1d8cf95f550bb4b86ad82b22e7195179335fa3b327fd1f1ba1e6c8357ee15c94 in / 
# Wed, 03 May 2023 00:23:05 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:38:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:38:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:38:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:43 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:45:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:45:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:45:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:45:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5627aec4010af613408c2ee78d5d32b9ecac22cb396d702906fb1160721f0011`  
		Last Modified: Wed, 03 May 2023 00:26:29 GMT  
		Size: 25.9 MB (25922039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4bb136449e53562b21b648a615cf43907af192446ee7d880c05b3a8254c8af`  
		Last Modified: Wed, 03 May 2023 03:40:39 GMT  
		Size: 4.4 MB (4350609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ca056492e3a7e4b3c199f8a889b9183b1a75edb249a08e1d8786c7b4d8cad8`  
		Last Modified: Wed, 10 May 2023 17:46:07 GMT  
		Size: 142.9 MB (142917988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee770aa11ecd8ad59c9dfc316a7ce4b28e594d1bf3d5467b6a85ed956a3863c`  
		Last Modified: Wed, 10 May 2023 17:45:50 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:255f7543d0e6dba32bffdc3ae60e70270c061eb49973957af547ba0e6261139a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178248531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:056069102655d640917bef51c63d30efa8aac4fecf2bb3f8da960cee2a11c3f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:40:01 GMT
ADD file:96715cff0e3569a2a1d7e203f0797ed4880da7714d455e25f032c67bff27221f in / 
# Tue, 23 May 2023 00:40:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:36 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:36 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:37 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:30:00 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:30:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:30:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3c2058520f8e2dee0c8d97a0e68335849888066e5d0d1b82b6ef302541b5c874`  
		Last Modified: Tue, 23 May 2023 00:45:13 GMT  
		Size: 27.8 MB (27797210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678dd0b30ea1ab93eb8bcc35bcf334b795b36c9b74173148a7dbb8d70fab701`  
		Last Modified: Tue, 23 May 2023 02:31:53 GMT  
		Size: 4.6 MB (4623824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83a140272f2611b1f4445691bb0ac4abbb87dd9d4ac6f5f9d505bf97ece32fe`  
		Last Modified: Tue, 23 May 2023 02:32:21 GMT  
		Size: 145.8 MB (145827125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01965ecc75242364a50d7ecb78bc7ae189013003af9f27b68e7bbdff182061b7`  
		Last Modified: Tue, 23 May 2023 02:31:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:36902255c08939b511a37508150a2883abd51afacbeab0d461635d7f5f644e6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:1baf0ab6fb6c474d216468d960333ffde38ccb3c76bb7f830c416d0d024412e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182524441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0394c94147bb57936f72c3b7d0ff8f2bdf98d7adc929d5fe3fa528b7339c4d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:58:20 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 03:58:20 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 03:58:21 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 03:58:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 03:58:41 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 03:58:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:58:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee1ad552555ac3b6bbcf73cf8e0a74753f824def74a2d74f5f8c177787b12a4`  
		Last Modified: Tue, 23 May 2023 04:00:34 GMT  
		Size: 2.4 MB (2426756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c421a694ca3262d6955441bf869575152e027f158a67a5fca1069ca8806102`  
		Last Modified: Tue, 23 May 2023 04:00:55 GMT  
		Size: 148.7 MB (148693723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4d7795ec1ad44b7fb4ee919ddeb55611a858900c4d78219ec62c0518711be9`  
		Last Modified: Tue, 23 May 2023 04:00:33 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5e2977123b1cfe0518c291316ab3931d4b194fb628e97df6062a8067b1d35328
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.4 MB (175390009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ce886a6f78d5c7d285a05c16e8d159ea755355ed2843492a291bc61382736e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:37:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 03 May 2023 03:37:35 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 03:37:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 10 May 2023 17:44:20 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:44:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 10 May 2023 17:44:40 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 10 May 2023 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 17:44:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85508fa2e82b98bf1b3609774366f78b99f51510455f0f0448dbf02e8fc2842`  
		Last Modified: Wed, 03 May 2023 03:40:09 GMT  
		Size: 2.4 MB (2414328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2616bb8cca402291d62dd06f67f3c3597f3042a4e8304a488e7db91581127cdf`  
		Last Modified: Wed, 10 May 2023 17:45:38 GMT  
		Size: 142.9 MB (142922569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc3b0ff727d110588d9b4875a9023116e1bc994d1b0dc5043d3ee86d66b1413`  
		Last Modified: Wed, 10 May 2023 17:45:21 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:7abf4e29ba01e1411695848991b2db643582481665fbefb816e49a5b70e9cb2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.7 MB (180735444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82a6bcb39c5b8202e58fc03ec47e602516000881cf4a2cb2f99998dc76d2603`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:29:01 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:29:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:29:02 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:29:26 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:29:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:29:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b599b0eed4b38a60f7217762f640670549cadeaa6d779a9ab6cde6f79affaf`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 2.5 MB (2532511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c55db0a6af6b3d85fb7c5a15e0d4c95f7e806ffa98208ce7ef735b7fc6725`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 145.8 MB (145814394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1668b9c92f4ae6e6ae9db09e901b457cce51b2a4ad763d409af5acd1499a971`  
		Last Modified: Tue, 23 May 2023 02:31:10 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; ppc64le

```console
$ docker pull julia@sha256:fb992d3e811683d5a7acb40e070aa5cf48e0c551496021b7a3b986619326fb59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171094683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c12da7cffc9305381fb6312a99958195846c536f37834527c9e4ef8b94b61e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:07:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 23 May 2023 02:07:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 23 May 2023 02:07:13 GMT
ENV JULIA_VERSION=1.9.0
# Tue, 23 May 2023 02:08:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.0-linux-x86_64.tar.gz'; 			sha256='00c614466ef9809c2eb23480e38d196a2c577fff2730c4f83d135b913d473359'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.0-linux-aarch64.tar.gz'; 			sha256='0a14315b53acd97f22d26d4a8fd2c237e524e95c3bec98d2d78b54d80c2bc364'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.0-linux-i686.tar.gz'; 			sha256='add391830b50df8d84f11ecf9e0fdd3d0fd420ba08737640094696fde64a22be'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.0-linux-ppc64le.tar.gz'; 			sha256='f32197fdd7b8e34d26d91cc46fc2fa040e07b02e61d22c0cedbc5e7e3d0363d5'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 23 May 2023 02:08:04 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Tue, 23 May 2023 02:08:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 02:08:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73a7cd9dea84bb9d934231269410340992f182978f4edef2332551db9339895`  
		Last Modified: Tue, 23 May 2023 02:08:20 GMT  
		Size: 2.6 MB (2627396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b277918387795ff9e75af87373fb080fc7e519c3608df2d74dbbdaa2ad80c9`  
		Last Modified: Tue, 23 May 2023 02:08:55 GMT  
		Size: 133.2 MB (133185997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c2c74cab468cff7d8a1904dc5d697186d7ef6fe72b630d69ad8a14624a37b`  
		Last Modified: Tue, 23 May 2023 02:08:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore`

```console
$ docker pull julia@sha256:51427d8cfaf9d87867929fe0bcf0652465c5618261c3c24e482d35e62084c6d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `julia:windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:30526016f4cdb9c4c5c531ce9e9955b2328b495c64587b2767af1ad1561439b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `julia:windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull julia@sha256:25ab1a544fb2ce3fd59e5fbaf47ad242e28c63c4bbf2d0b0e4dc47cd55b3d225
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2233512867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76648ae4ac059222749064fa8c307f696e203873d350d53c97f553cc997c583a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:18:35 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:18:36 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:18:37 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:20:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:20:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d785f01b4ee99c7ba82c3b5b935ca2f788a3def4e57145b304e7d1d3c9728ded`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d291d304af7e0c57143faa61f0eda518c4bfb4ff210d19e47a0abb77e0914f`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cccccf4b0bbca7afcd352d1b472c323ca99fe17eeab8dea3eb1146b926687`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a64a1eda873b1cea949cfe88cda836dcb34d676ca7d6f01bfc0862e9e518880`  
		Last Modified: Wed, 10 May 2023 17:22:38 GMT  
		Size: 161.5 MB (161470633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae670d86aeef0dedbb6d00c9207edde78d7c2fea34b1b2245633ed9f724c9ad`  
		Last Modified: Wed, 10 May 2023 17:22:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-ltsc2022`

```console
$ docker pull julia@sha256:604ba14a26f6b140f5e4e281daa12fa2b1f4ef444781bf3b30b3d4aeaf404417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `julia:windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull julia@sha256:28121afd72ac219147a96abf2a079ba909a8146a2024bf18648f77871dd88792
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1936481566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d731d7190d9df75b0fb7e8bbc3c8d85092c0ef5cb86019abd55bba22ee8b5656`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 17:17:08 GMT
ENV JULIA_VERSION=1.9.0
# Wed, 10 May 2023 17:17:09 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.9/julia-1.9.0-win64.exe
# Wed, 10 May 2023 17:17:10 GMT
ENV JULIA_SHA256=096ed36b1bc1fd7d00abc47d9e9f339d051961c2d0c5021005bb8f7e7a93ef0e
# Wed, 10 May 2023 17:18:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 10 May 2023 17:18:24 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce704eb4d2eee608dd704627d552207b9194ec68eee1e468a36b6b30c30eac`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02905013f0ea97ad3491cfeaed3b954c50aeb738cbfc326f86f2342b104c4eb`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2132f59a86b83ce1611ab2bf14903b2186efa7777b435e6f4ad1322c570d8328`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ca5036ec568d0820d327e34572098f4bf3741d316ce11ad0ff3aec3dd712df`  
		Last Modified: Wed, 10 May 2023 17:21:53 GMT  
		Size: 161.5 MB (161493116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751cc4a131c3078089bc7a991c8e978f0bdebcf426d7912e8e95b42a7276695`  
		Last Modified: Wed, 10 May 2023 17:21:20 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
