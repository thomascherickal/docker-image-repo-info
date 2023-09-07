## `julia:rc-bookworm`

```console
$ docker pull julia@sha256:29d4ec7946aca6bf0235115738e098fbbcb1a5255f6acd1a7f8855bcb3db2f9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:rc-bookworm` - linux; amd64

```console
$ docker pull julia@sha256:bd958a0c33a969c59853434c9e1f880ae6fcf49c9ef44eee8c39a31c27b93bbc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.5 MB (204490423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17d3b665e36e1e4f71688eb56f3e27469e56e0859bb7a01e27bf16b7aed4a8a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 07 Sep 2023 00:20:51 GMT
ADD file:3a8cd4de7f163d93718670f4db1de49045f5e04af3a8aa27d81c0f14647db707 in / 
# Thu, 07 Sep 2023 00:20:51 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 11:41:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 11:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 07 Sep 2023 11:41:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 11:41:44 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 07 Sep 2023 11:41:44 GMT
ENV JULIA_VERSION=1.10.0-beta2
# Thu, 07 Sep 2023 11:42:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta2-linux-x86_64.tar.gz'; 			sha256='f1a17f5a52980c167416cbe4eda14419d818f3b76985401154a3a567879d6477'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta2-linux-aarch64.tar.gz'; 			sha256='38e7c07a0c3f124497da62d81dc6bf58dbce8a6a3f0542ba52aaac54ed238351'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta2-linux-i686.tar.gz'; 			sha256='adc781af2ee5981988f0551672170b1610c4af1262495f4ecf19602da0ed579f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta2-linux-ppc64le.tar.gz'; 			sha256='4b51efbdfe958e754f982c618825cd95b5c3421da3486ef8bc4c83b90270e06c'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 07 Sep 2023 11:42:06 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 07 Sep 2023 11:42:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 11:42:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:360eba32fa65016e0d558c6af176db31a202e9a6071666f9b629cb8ba6ccedf0`  
		Last Modified: Thu, 07 Sep 2023 00:25:22 GMT  
		Size: 29.1 MB (29124494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61bb0e5fa43b4c9306bc15df84a1ae72148dd0426ee15110d56bd0ee91e3b25`  
		Last Modified: Thu, 07 Sep 2023 11:44:58 GMT  
		Size: 5.7 MB (5695768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201d13c2c3fa3828e4a46771072da486694682a0fb44f3fd88fee32773dd4520`  
		Last Modified: Thu, 07 Sep 2023 11:45:22 GMT  
		Size: 169.7 MB (169669788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfc12b2ec468f3a6fb934da46958881ac57050499d49e777e8361bb1a365809`  
		Last Modified: Thu, 07 Sep 2023 11:44:57 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:58d200d483fbda5c94f52f1a3af2dadec4d253ba462af9504d1f581f6e177e03
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.8 MB (198784012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a9dd439098b111a597a5011e82ab51b6653b5e073be38fc276a31d46da63e2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:39 GMT
ADD file:fb5c8f411c4a1e06c25ac32455221938386907d0b4782fc228ca67de63a7e9de in / 
# Thu, 07 Sep 2023 00:39:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:40:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:40:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 07 Sep 2023 06:40:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 06:40:40 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 07 Sep 2023 06:40:40 GMT
ENV JULIA_VERSION=1.10.0-beta2
# Thu, 07 Sep 2023 06:41:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta2-linux-x86_64.tar.gz'; 			sha256='f1a17f5a52980c167416cbe4eda14419d818f3b76985401154a3a567879d6477'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta2-linux-aarch64.tar.gz'; 			sha256='38e7c07a0c3f124497da62d81dc6bf58dbce8a6a3f0542ba52aaac54ed238351'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta2-linux-i686.tar.gz'; 			sha256='adc781af2ee5981988f0551672170b1610c4af1262495f4ecf19602da0ed579f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta2-linux-ppc64le.tar.gz'; 			sha256='4b51efbdfe958e754f982c618825cd95b5c3421da3486ef8bc4c83b90270e06c'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 07 Sep 2023 06:41:06 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 07 Sep 2023 06:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 06:41:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:155eab17d86c47443adc8cebe7fc62c847c03db8cfb1ca53aa6276564fff23ef`  
		Last Modified: Thu, 07 Sep 2023 00:43:02 GMT  
		Size: 29.2 MB (29157149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2f400666de2f95466cb32743ac8c47703241fb90551f13071d892df707065c`  
		Last Modified: Thu, 07 Sep 2023 06:43:34 GMT  
		Size: 5.5 MB (5527097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcbf3e5540e9280bb81653c97a5dea1915e7d23291ac491d87ecb816448e0e1`  
		Last Modified: Thu, 07 Sep 2023 06:43:53 GMT  
		Size: 164.1 MB (164099392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf52a93b2d17e9352e2e4a518b95d247f724dab4760a857770daa59a2f57e10`  
		Last Modified: Thu, 07 Sep 2023 06:43:33 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bookworm` - linux; 386

```console
$ docker pull julia@sha256:517fc3368f6ab3bdfd810819508c0da1f240da19aeb9742e9c69810a2ebcde2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192061580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad624e74fb3676686e9e284685cff5ac5f5f9564ddc19c092ebb40314831296`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:01 GMT
ADD file:ffdb2f26091492ac2e82793b461bb70da9ce1d68d219ec0db182b4510e82586b in / 
# Tue, 15 Aug 2023 23:39:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 09:28:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 09:28:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 09:28:46 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 09:28:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 26 Aug 2023 05:59:32 GMT
ENV JULIA_VERSION=1.10.0-beta2
# Sat, 26 Aug 2023 06:00:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta2-linux-x86_64.tar.gz'; 			sha256='f1a17f5a52980c167416cbe4eda14419d818f3b76985401154a3a567879d6477'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta2-linux-aarch64.tar.gz'; 			sha256='38e7c07a0c3f124497da62d81dc6bf58dbce8a6a3f0542ba52aaac54ed238351'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta2-linux-i686.tar.gz'; 			sha256='adc781af2ee5981988f0551672170b1610c4af1262495f4ecf19602da0ed579f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta2-linux-ppc64le.tar.gz'; 			sha256='4b51efbdfe958e754f982c618825cd95b5c3421da3486ef8bc4c83b90270e06c'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 26 Aug 2023 06:00:02 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Sat, 26 Aug 2023 06:00:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Aug 2023 06:00:03 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a12cc43de7614ac71c57865601eb4cedd27ce910b66c5091e07781b8547d5b0b`  
		Last Modified: Tue, 15 Aug 2023 23:43:26 GMT  
		Size: 30.1 MB (30141823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac45508e354104caec85eedf213ac7fda6a301c8b3dcc8f54624f48dc743b73d`  
		Last Modified: Wed, 16 Aug 2023 09:32:17 GMT  
		Size: 5.9 MB (5854584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e786f9b252739b4cf33ae6f08f2aae0b928edbc11ec1fa2943627523e5169abf`  
		Last Modified: Sat, 26 Aug 2023 06:02:48 GMT  
		Size: 156.1 MB (156064799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb1073cba594132527966548473110dbcde0fd3724e98801a96bee5c927fb8a`  
		Last Modified: Sat, 26 Aug 2023 06:02:09 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bookworm` - linux; ppc64le

```console
$ docker pull julia@sha256:621991e9329c3ee00f3a60468ca3f9187efa942bc400c0624dc6a0401787be7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.0 MB (193036823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba915f89d20c1522e1f2546ebf25033a708860a3178df21a62ad94fe7338e50a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:29 GMT
ADD file:c5cce4a01995fb11fea5067fdf342af046481b4869e8e858a85986686f68ef2a in / 
# Thu, 07 Sep 2023 00:17:32 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:06:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:06:50 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 07 Sep 2023 01:06:51 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Sep 2023 01:06:51 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 07 Sep 2023 01:06:52 GMT
ENV JULIA_VERSION=1.10.0-beta2
# Thu, 07 Sep 2023 01:07:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta2-linux-x86_64.tar.gz'; 			sha256='f1a17f5a52980c167416cbe4eda14419d818f3b76985401154a3a567879d6477'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta2-linux-aarch64.tar.gz'; 			sha256='38e7c07a0c3f124497da62d81dc6bf58dbce8a6a3f0542ba52aaac54ed238351'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta2-linux-i686.tar.gz'; 			sha256='adc781af2ee5981988f0551672170b1610c4af1262495f4ecf19602da0ed579f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta2-linux-ppc64le.tar.gz'; 			sha256='4b51efbdfe958e754f982c618825cd95b5c3421da3486ef8bc4c83b90270e06c'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 07 Sep 2023 01:07:57 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:07:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 01:07:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1db76043538a495ac265ef61277e1a2137637bebdc1ffa7712108b3efe4a4d33`  
		Last Modified: Thu, 07 Sep 2023 00:23:29 GMT  
		Size: 33.1 MB (33119207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c764a3bfda2b550902ea9e8e6211753ab495e60e25d51e4a63cf60e2734c4e`  
		Last Modified: Thu, 07 Sep 2023 01:12:39 GMT  
		Size: 6.2 MB (6229781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bc9eb2fb323b3b7e4e262293a19112088783fe1d185bc6a8dbcd228387fc49`  
		Last Modified: Thu, 07 Sep 2023 01:13:19 GMT  
		Size: 153.7 MB (153687459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdbb4b9b4fa6a10c12f89a2028d078a290d0bf34a2987d295a1f8c8be3c1d24`  
		Last Modified: Thu, 07 Sep 2023 01:12:37 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
