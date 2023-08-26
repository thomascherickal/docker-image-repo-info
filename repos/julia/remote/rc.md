## `julia:rc`

```console
$ docker pull julia@sha256:7152b2c25ac5f6dfc30f8747dec19878efe92dde5b03c7f5bf214e4be2d88c4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.1906; amd64
	-	windows version 10.0.17763.4737; amd64

### `julia:rc` - linux; amd64

```console
$ docker pull julia@sha256:76bc10e44a4667579f8db64fb3c36c78c72952e65b88f7aa9a876d9383266a7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.5 MB (204490534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3916663b02f1a5670641cd0933adc955f0e189c7186dabd93fe90c21de00f43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:46 GMT
ADD file:997f5a9b32407d96efac41a1cfafb318f77de077c8b5cd7065b6ec9796b4bf5e in / 
# Wed, 16 Aug 2023 00:59:47 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 09:57:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 09:57:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 09:57:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 09:57:28 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 26 Aug 2023 04:03:24 GMT
ENV JULIA_VERSION=1.10.0-beta2
# Sat, 26 Aug 2023 04:03:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta2-linux-x86_64.tar.gz'; 			sha256='f1a17f5a52980c167416cbe4eda14419d818f3b76985401154a3a567879d6477'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta2-linux-aarch64.tar.gz'; 			sha256='38e7c07a0c3f124497da62d81dc6bf58dbce8a6a3f0542ba52aaac54ed238351'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta2-linux-i686.tar.gz'; 			sha256='adc781af2ee5981988f0551672170b1610c4af1262495f4ecf19602da0ed579f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta2-linux-ppc64le.tar.gz'; 			sha256='4b51efbdfe958e754f982c618825cd95b5c3421da3486ef8bc4c83b90270e06c'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 26 Aug 2023 04:03:45 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Sat, 26 Aug 2023 04:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Aug 2023 04:03:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:52d2b7f179e32b4cbd579ee3c4958027988f9a8274850ab0c7c24661e3adaac5`  
		Last Modified: Wed, 16 Aug 2023 01:04:30 GMT  
		Size: 29.1 MB (29124563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8721124fc215962745673ef73dc19e3e00368bee1b4da37bc61b6832d5c29735`  
		Last Modified: Wed, 16 Aug 2023 10:00:40 GMT  
		Size: 5.7 MB (5695794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fafd635b8881457a3d7ca50a1256e783f41c4fb6080aa3bc95b5b4e41b7af5f`  
		Last Modified: Sat, 26 Aug 2023 04:07:24 GMT  
		Size: 169.7 MB (169669806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7575c924380084de91e364518effe5a8f4f19d61b9ea9f2d13aa3728b40c03f6`  
		Last Modified: Sat, 26 Aug 2023 04:06:59 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5825aa5da29f59b8ab2b4cea718e81124aa730beac98caa81c32c288f46aeeac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.8 MB (198784050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc41462e7d9d41651f613943eb11b5b7cfc90e8f1a5de85733ff5a5f29e49cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:57 GMT
ADD file:bc58956fa3d1aff2efb0264655d039fedfff28dc4ff19a65a235e82754ee1cfa in / 
# Tue, 15 Aug 2023 23:39:57 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:29:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:29:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 03:29:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:29:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 26 Aug 2023 03:12:33 GMT
ENV JULIA_VERSION=1.10.0-beta2
# Sat, 26 Aug 2023 03:12:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta2-linux-x86_64.tar.gz'; 			sha256='f1a17f5a52980c167416cbe4eda14419d818f3b76985401154a3a567879d6477'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta2-linux-aarch64.tar.gz'; 			sha256='38e7c07a0c3f124497da62d81dc6bf58dbce8a6a3f0542ba52aaac54ed238351'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta2-linux-i686.tar.gz'; 			sha256='adc781af2ee5981988f0551672170b1610c4af1262495f4ecf19602da0ed579f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta2-linux-ppc64le.tar.gz'; 			sha256='4b51efbdfe958e754f982c618825cd95b5c3421da3486ef8bc4c83b90270e06c'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 26 Aug 2023 03:12:55 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Sat, 26 Aug 2023 03:12:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Aug 2023 03:12:55 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4ee097f9a36616fddb52e45aba72142c4bc6f2e594f0a746e406acfde4f02f51`  
		Last Modified: Tue, 15 Aug 2023 23:43:21 GMT  
		Size: 29.2 MB (29157256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9ec7a2dd557caa143329ea7f6b0082a7529fe353e771325fc91731ef6a525`  
		Last Modified: Wed, 16 Aug 2023 03:32:10 GMT  
		Size: 5.5 MB (5527026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6edeaeb5e2af4608491bd48a9122b568f5d4f85613ac402fd63d13e2e4e5ea`  
		Last Modified: Sat, 26 Aug 2023 03:14:51 GMT  
		Size: 164.1 MB (164099394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f1a6a8b7e386bdc363b344c3dac6469114a87ca0100f402e2e67451708cbf4`  
		Last Modified: Sat, 26 Aug 2023 03:14:31 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - linux; 386

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

### `julia:rc` - linux; ppc64le

```console
$ docker pull julia@sha256:e428d3e40ea2ca975f976f91137ba46c7822e035e6a3f82a121c82918c0b42ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.0 MB (193036935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6c2f09a4af6c2a79ef625375527920f990fd33b6a4851e8913625fb6953f91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:33 GMT
ADD file:9578bf6d6b33f2ba960ab9309642d1c9dcc131d7b9e6f818b8cc4b843fe3aec8 in / 
# Wed, 16 Aug 2023 01:09:35 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:47:59 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 03:48:00 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:48:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 26 Aug 2023 07:17:48 GMT
ENV JULIA_VERSION=1.10.0-beta2
# Sat, 26 Aug 2023 07:19:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta2-linux-x86_64.tar.gz'; 			sha256='f1a17f5a52980c167416cbe4eda14419d818f3b76985401154a3a567879d6477'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta2-linux-aarch64.tar.gz'; 			sha256='38e7c07a0c3f124497da62d81dc6bf58dbce8a6a3f0542ba52aaac54ed238351'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta2-linux-i686.tar.gz'; 			sha256='adc781af2ee5981988f0551672170b1610c4af1262495f4ecf19602da0ed579f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta2-linux-ppc64le.tar.gz'; 			sha256='4b51efbdfe958e754f982c618825cd95b5c3421da3486ef8bc4c83b90270e06c'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 26 Aug 2023 07:19:08 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Sat, 26 Aug 2023 07:19:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Aug 2023 07:19:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0500920b409f06d69819525676ebf090702285435050f7b1f973c8c7b034ea7c`  
		Last Modified: Wed, 16 Aug 2023 01:15:59 GMT  
		Size: 33.1 MB (33119300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f30a0c06039c467cf0e1b6990bc9fe73f6347c0a9a3762abb5def24e2e8086b`  
		Last Modified: Wed, 16 Aug 2023 03:53:55 GMT  
		Size: 6.2 MB (6229794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ce1caed476f428dda5c199f1064c2ac52ed8e3fb1eadbaa9ee8530b2895fe8`  
		Last Modified: Sat, 26 Aug 2023 07:24:05 GMT  
		Size: 153.7 MB (153687464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3981fb2f1c95205d6ea476650c9e4df580498e6b0928a6dd47b671a32f29fa`  
		Last Modified: Sat, 26 Aug 2023 07:23:23 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - windows version 10.0.20348.1906; amd64

```console
$ docker pull julia@sha256:eae3106ec917974ad7d970d3cfd85aeba38894769cf5279681dda6578551b132
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978646138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c0a8c4429a8c764c3ca19aba4941fa75fefc0600af45901bd915e5c8d455306`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 26 Aug 2023 00:15:03 GMT
ENV JULIA_VERSION=1.10.0-beta2
# Sat, 26 Aug 2023 00:15:03 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.10/julia-1.10.0-beta2-win64.exe
# Sat, 26 Aug 2023 00:15:04 GMT
ENV JULIA_SHA256=21fcab0815ce738bb268daa154dccbf0532b7c27196586ce677d43164114474b
# Sat, 26 Aug 2023 00:16:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 26 Aug 2023 00:16:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4f392a93291aea3332a6629560f8b7982884485253af5cbbacd0b6e3a29b81`  
		Last Modified: Sat, 26 Aug 2023 00:24:30 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2f69fe7ffd434751fcbcf85ca0c9714fc3ea2d5f0589b80c94433234f9bb98`  
		Last Modified: Sat, 26 Aug 2023 00:24:30 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9b628f4c2cd9171779da934c630e94f824aec126feee2f6ff8c99d8d10a14a`  
		Last Modified: Sat, 26 Aug 2023 00:24:30 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc4e6376f2281bc6e5a55e8308a395e975a5c656596ea19177ab1f81b4e3bef`  
		Last Modified: Sat, 26 Aug 2023 00:25:10 GMT  
		Size: 181.3 MB (181275166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acc4f0d2b3e6a3b43e0ea785bbc61ac0513491b08d26d6b4cc701fe403f5faf`  
		Last Modified: Sat, 26 Aug 2023 00:24:30 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc` - windows version 10.0.17763.4737; amd64

```console
$ docker pull julia@sha256:6f84553294fb90710609622d4f829462d89ae25d0fe26f8125d05d4392da3897
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2177248053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db393aaec81277578d95e4dc782158b9e6da44389b7fa4ba33c914a9818cb135`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 26 Aug 2023 00:16:46 GMT
ENV JULIA_VERSION=1.10.0-beta2
# Sat, 26 Aug 2023 00:16:47 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.10/julia-1.10.0-beta2-win64.exe
# Sat, 26 Aug 2023 00:16:48 GMT
ENV JULIA_SHA256=21fcab0815ce738bb268daa154dccbf0532b7c27196586ce677d43164114474b
# Sat, 26 Aug 2023 00:19:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Sat, 26 Aug 2023 00:19:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d0381b7df0d91b892d604b4d43fdfe1b55a00fb6131bc4c886f332528a3366`  
		Last Modified: Sat, 26 Aug 2023 00:25:22 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf1c547752ba7eabdc8d03ffbb3f8f2443baf14ceb9905a040949053c6fc32`  
		Last Modified: Sat, 26 Aug 2023 00:25:22 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0879d3a3c36a90c775847740af299deb2d3d7fb61919c77d8e7a6105039f084`  
		Last Modified: Sat, 26 Aug 2023 00:25:22 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85d9967671a58c967766d7528e88e22f21088923a5fb07c54117d340d33b85b`  
		Last Modified: Sat, 26 Aug 2023 00:26:03 GMT  
		Size: 181.3 MB (181285569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7d4596cd290efb34ddcaa3bf6bcebff4c7fbfc5b3754e6fd4c67e2032525bb`  
		Last Modified: Sat, 26 Aug 2023 00:25:22 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
