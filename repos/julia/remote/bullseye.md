## `julia:bullseye`

```console
$ docker pull julia@sha256:179168a4665b432cee0c0a377c410eeec060f98db5ceb6820fac93fd4f1dd1b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:bullseye` - linux; amd64

```console
$ docker pull julia@sha256:7a57877428af4f89aeadff7c471c73f3930f353febe4303c9817a54a0ad93773
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.5 MB (155469648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82f237302a983426375f0aa600b167180f7132b24384c8a67635947632c5eb7`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:42:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:42:08 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 02 Dec 2021 09:42:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 09:42:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 02 Dec 2021 09:43:28 GMT
ENV JULIA_VERSION=1.6.4
# Thu, 02 Dec 2021 09:43:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='52244ae47697e8073dfbc9d1251b0422f0dbd1fbe1a41da4b9f7ddf0506b2132' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='9ad3f6bd71eb6840d4cef1569855da20c0b4931a2bdf77703a64df672b0702a1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='072daac7229c15fa41d0c1b65b8a3d6ee747323d02f5943da3846b075291b48b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='9d43d642174cf22cf0fde18dc2578c84f357d2c619b9d846d3a6da4192ba48cf' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Dec 2021 09:43:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55e18473ecc625d930f2f4852d4fb5fcd720e0f41240db5bee9d0f9b2841d65`  
		Last Modified: Thu, 02 Dec 2021 09:46:07 GMT  
		Size: 2.4 MB (2425640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911a91489626fba4b10ff5cada14b5e09bccee3c981c0b944c9b5f505d31758a`  
		Last Modified: Thu, 02 Dec 2021 09:47:55 GMT  
		Size: 121.7 MB (121673787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; arm variant v7

```console
$ docker pull julia@sha256:c5c9d02932e3e83576a6122165a128cac63de4be93ca2a3b446368b5d32b4a00
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141695808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d217e292a19c22e92bbad35434383535335858a34564f2f9898f81bf6b8c5b4`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:43 GMT
ADD file:cd2ac52107a2ea6657f23850a4b29366309eb39fa177321e0a9fd6d58562ae80 in / 
# Wed, 17 Nov 2021 01:59:44 GMT
CMD ["bash"]
# Wed, 01 Dec 2021 02:04:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Dec 2021 02:04:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:04:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:04:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 01 Dec 2021 02:06:08 GMT
ENV JULIA_VERSION=1.6.4
# Wed, 01 Dec 2021 02:06:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='52244ae47697e8073dfbc9d1251b0422f0dbd1fbe1a41da4b9f7ddf0506b2132' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='9ad3f6bd71eb6840d4cef1569855da20c0b4931a2bdf77703a64df672b0702a1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='072daac7229c15fa41d0c1b65b8a3d6ee747323d02f5943da3846b075291b48b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='9d43d642174cf22cf0fde18dc2578c84f357d2c619b9d846d3a6da4192ba48cf' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 01 Dec 2021 02:07:01 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b6e5ca4da96841e58eb27c88695a059e5105fad5a066de803f4b94ae4002ba66`  
		Last Modified: Wed, 17 Nov 2021 02:15:13 GMT  
		Size: 26.6 MB (26573160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ac930351005d3628be9a87b90b75988bede2483da49a4e0049ea4b4877dfe1`  
		Last Modified: Wed, 01 Dec 2021 02:10:29 GMT  
		Size: 2.2 MB (2227537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b959a7cad35d65afd80f2ab034b8904464b8f23023856ad64e69da05f4f3a12`  
		Last Modified: Wed, 01 Dec 2021 02:13:27 GMT  
		Size: 112.9 MB (112895111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:128856024316843d89f872b5240121fc9c7b86541bdca107e54897349ce513ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.5 MB (147543941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fb06a7b45388502f2ebb481a36ed97e96c46d79429f47342e4ac8c56de60b79`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 01 Dec 2021 01:44:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Dec 2021 01:44:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 01:44:17 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 01:44:18 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 01 Dec 2021 01:45:00 GMT
ENV JULIA_VERSION=1.6.4
# Wed, 01 Dec 2021 01:45:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='52244ae47697e8073dfbc9d1251b0422f0dbd1fbe1a41da4b9f7ddf0506b2132' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='9ad3f6bd71eb6840d4cef1569855da20c0b4931a2bdf77703a64df672b0702a1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='072daac7229c15fa41d0c1b65b8a3d6ee747323d02f5943da3846b075291b48b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='9d43d642174cf22cf0fde18dc2578c84f357d2c619b9d846d3a6da4192ba48cf' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 01 Dec 2021 01:45:28 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65b6cab17a910a7b2a7279c9ef37810345bd378f4144976db2f0356d2ec558d`  
		Last Modified: Wed, 01 Dec 2021 01:47:04 GMT  
		Size: 2.2 MB (2208789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bdf211aab2dad6aeb89c9628138a21660946fdc3ec46d5b26fb95361644052b`  
		Last Modified: Wed, 01 Dec 2021 01:48:02 GMT  
		Size: 115.3 MB (115278631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:bullseye` - linux; 386

```console
$ docker pull julia@sha256:7d54d3afa67fb997455f39abefc4de9c6b29e1bec88d13614ae138ea630e8afe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.2 MB (154239879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5411de5769045ce0bfdc2ad6b60c8d58b4fec936ee351616a9e409b296d33d1c`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:19:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:19:15 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 02 Dec 2021 09:19:16 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 09:19:16 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 02 Dec 2021 09:20:28 GMT
ENV JULIA_VERSION=1.6.4
# Thu, 02 Dec 2021 09:20:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='52244ae47697e8073dfbc9d1251b0422f0dbd1fbe1a41da4b9f7ddf0506b2132' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='9ad3f6bd71eb6840d4cef1569855da20c0b4931a2bdf77703a64df672b0702a1' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='072daac7229c15fa41d0c1b65b8a3d6ee747323d02f5943da3846b075291b48b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='9d43d642174cf22cf0fde18dc2578c84f357d2c619b9d846d3a6da4192ba48cf' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 02 Dec 2021 09:20:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c26dd9e12ca161e0d08bf5b14bcb1f80a4ae55a052739f8a0eb7cc36628df37`  
		Last Modified: Thu, 02 Dec 2021 09:23:26 GMT  
		Size: 2.5 MB (2529574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275f24d59e1528dbf9ecba59b2fcc919cf7cf09c176d0d96e8391db0223aa720`  
		Last Modified: Thu, 02 Dec 2021 09:25:21 GMT  
		Size: 119.3 MB (119329491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
