## `julia:rc-bullseye`

```console
$ docker pull julia@sha256:87e835cb791721f5c951f20e3b36cd04598311a67093b5249ab19abd95e9eed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:rc-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:ad82d0ac1eeb7fb0bdad81e3b7a9eced8b4c5126aa053c70ab2f112961959681
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.5 MB (178534442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3428f73ccfe1dde3e61a77375bd1ff94d1a679585ae76d8e544a7094d78817`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:22:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:22:07 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 May 2022 05:22:07 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 05:22:07 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 02 Jun 2022 18:32:59 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 02 Jun 2022 18:33:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-rc1-linux-x86_64.tar.gz'; 			sha256='a47efddaaccb424dad6499f870ab7f792c50827d23cc64cb9873280318337966'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-rc1-linux-aarch64.tar.gz'; 			sha256='15dd553754aa15e514f28ed00ed4cfdb1f8cf883f3398b803ef5cf05e767a2fb'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-rc1-linux-i686.tar.gz'; 			sha256='bed81bb5e2cd60abb824b40cbb1ed2f27c9f974dfd7fbc43ce1684e5462bae2b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Jun 2022 18:33:29 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eda415c0e29e6a7b2336cfb8d64af2edf15ca42f3035042e9e9dc9d04e67740`  
		Last Modified: Sat, 28 May 2022 05:25:21 GMT  
		Size: 2.4 MB (2425947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a4bef474e869bc28914d4786d69fd9fa4088aa23e5d2b074560a3cbfd78e84`  
		Last Modified: Thu, 02 Jun 2022 18:36:10 GMT  
		Size: 144.7 MB (144729219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:09f65d856c6df826ce585dbba8b7475a8dc88ee449e4ca7ab1ccb6175acecb3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.5 MB (170489028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d883eb693437a964875bd8e29c6c109a529525aa317fe04ae7a92054f651fc32`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:34:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:34:15 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 May 2022 02:34:16 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 02:34:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 02 Jun 2022 17:57:00 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 02 Jun 2022 17:57:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-rc1-linux-x86_64.tar.gz'; 			sha256='a47efddaaccb424dad6499f870ab7f792c50827d23cc64cb9873280318337966'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-rc1-linux-aarch64.tar.gz'; 			sha256='15dd553754aa15e514f28ed00ed4cfdb1f8cf883f3398b803ef5cf05e767a2fb'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-rc1-linux-i686.tar.gz'; 			sha256='bed81bb5e2cd60abb824b40cbb1ed2f27c9f974dfd7fbc43ce1684e5462bae2b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Jun 2022 17:57:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5009ca1e06d69bfe9ec7e7c510ef3712bb224c97f82fdaaa98effd93fabbe0e`  
		Last Modified: Sat, 28 May 2022 02:37:44 GMT  
		Size: 2.2 MB (2208675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b6c4dc27f85e1fddabdb5c0a9b4b4a06ffdde59264380ad6fbd27e325f9374`  
		Last Modified: Thu, 02 Jun 2022 17:59:19 GMT  
		Size: 138.2 MB (138214625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; 386

```console
$ docker pull julia@sha256:29841149a017c980e42b57ebac48b4f3045cc23ac3896bbb7ea5926898d932e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.4 MB (174444854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cb31251963c7cb2e40d156cdd944962f9ff47f92f3aec0f1cdc2873faa9e606`
-	Default Command: `["julia"]`

```dockerfile
# Sat, 28 May 2022 00:39:33 GMT
ADD file:8320d7b95b9f68313e086faff974bb38977e0c9da4984afb6382eb0405742bde in / 
# Sat, 28 May 2022 00:39:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:34:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:34:04 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 28 May 2022 03:34:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 03:34:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 02 Jun 2022 17:42:37 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 02 Jun 2022 17:43:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-rc1-linux-x86_64.tar.gz'; 			sha256='a47efddaaccb424dad6499f870ab7f792c50827d23cc64cb9873280318337966'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-rc1-linux-aarch64.tar.gz'; 			sha256='15dd553754aa15e514f28ed00ed4cfdb1f8cf883f3398b803ef5cf05e767a2fb'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-rc1-linux-i686.tar.gz'; 			sha256='bed81bb5e2cd60abb824b40cbb1ed2f27c9f974dfd7fbc43ce1684e5462bae2b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Jun 2022 17:43:01 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:5e7494d2ee6c81c73ce32f8bde3ea8658c6224c2cc22d7bb01df4bc3d42949aa`  
		Last Modified: Sat, 28 May 2022 00:46:43 GMT  
		Size: 32.4 MB (32390321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ab24c5119b700891a3f447f29ac0960077800cc5f71e2353786b09cc525fca`  
		Last Modified: Sat, 28 May 2022 03:37:42 GMT  
		Size: 2.3 MB (2324352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99633d9d235882e94a53348f4724fc8b7ab74e0c90b9439441fb4c64c02e336`  
		Last Modified: Thu, 02 Jun 2022 17:45:06 GMT  
		Size: 139.7 MB (139730181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
