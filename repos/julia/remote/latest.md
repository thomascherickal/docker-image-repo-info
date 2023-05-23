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
