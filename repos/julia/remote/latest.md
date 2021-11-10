## `julia:latest`

```console
$ docker pull julia@sha256:25c989a1919efbc5d35fc9ded62549cf47a95f34af6dd93d7e61b0e013522063
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	windows version 10.0.20348.350; amd64
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:c38b3ce216b01d16bd1a1592392a8e024336859a7f8257b0dbf0a2e44177dcbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.3 MB (153329374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8cdc51824337548d42fe66c55ec5d8957d563d9212eeadddc594b680c9fd28`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:51:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:51:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Oct 2021 09:51:51 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 09:51:51 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Oct 2021 09:52:27 GMT
ENV JULIA_VERSION=1.6.3
# Tue, 12 Oct 2021 09:52:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='c7459c334cd7c3e4a297baf52535937c6bad640e60882f9201a73bab9394314b' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7cf08affbad206bd3c1ef8bc117bf0aa6ac95d1666bf4c06f9d530cff29b2067' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='df1a7e96f83b60fda54fd14713a373e37ac2d80fd11dbd708a77c8a22ab86e25' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='06e3d64813e4ba6019d8d79e918c48af4943700bd1eb689c481d82a64f8c280a' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='a3cb6f58ee93bbd3bd72ecd45b9f37bf5e16e9c0ef30ba17c809ec7cbb84ee96' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Oct 2021 09:52:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b8d869efaeb262f8cb654a2f48a3e342f88a5126dbb642f03e1a8bc2eb5dd1`  
		Last Modified: Tue, 12 Oct 2021 09:54:30 GMT  
		Size: 4.5 MB (4458487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bb6b59a0738627b87ccdf2470ea804c964349d3ed88380b5acb7ec3ce7776c`  
		Last Modified: Tue, 12 Oct 2021 09:55:29 GMT  
		Size: 121.7 MB (121731377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm variant v7

```console
$ docker pull julia@sha256:3c6a1d0af384f115d1889391c36df2f72f91b68399dac31b2728843f8ab6b782
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139347770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41946159713d6c99bda729d54dfd0830330ca603cc74b0c57f8d62a92ddcfacb`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:22:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:22:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Oct 2021 18:22:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 18:22:50 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Oct 2021 18:23:57 GMT
ENV JULIA_VERSION=1.6.3
# Tue, 12 Oct 2021 18:24:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='c7459c334cd7c3e4a297baf52535937c6bad640e60882f9201a73bab9394314b' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7cf08affbad206bd3c1ef8bc117bf0aa6ac95d1666bf4c06f9d530cff29b2067' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='df1a7e96f83b60fda54fd14713a373e37ac2d80fd11dbd708a77c8a22ab86e25' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='06e3d64813e4ba6019d8d79e918c48af4943700bd1eb689c481d82a64f8c280a' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='a3cb6f58ee93bbd3bd72ecd45b9f37bf5e16e9c0ef30ba17c809ec7cbb84ee96' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Oct 2021 18:24:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7094c2acb6418732c3212eda7f35443fe5b5879771194a48414da83badb9959`  
		Last Modified: Tue, 12 Oct 2021 18:28:48 GMT  
		Size: 3.8 MB (3806072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d07760a0aab18b5f5ee1ac473b6eaad4642c28d3b870decb63abfe61eae4a72`  
		Last Modified: Tue, 12 Oct 2021 18:31:13 GMT  
		Size: 112.8 MB (112802000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:7c397e721a70c4ae8de54b3a2d1b436d0f04d38bbe808e75e82f0c08ebb1ba6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145410667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd696c08a4301ab685d0d46df6e5333201126477771334f8475e3e9c0c713d1`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Mon, 25 Oct 2021 17:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 25 Oct 2021 17:41:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 25 Oct 2021 17:41:58 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Oct 2021 17:41:59 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 25 Oct 2021 17:42:35 GMT
ENV JULIA_VERSION=1.6.3
# Mon, 25 Oct 2021 17:42:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='c7459c334cd7c3e4a297baf52535937c6bad640e60882f9201a73bab9394314b' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7cf08affbad206bd3c1ef8bc117bf0aa6ac95d1666bf4c06f9d530cff29b2067' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='df1a7e96f83b60fda54fd14713a373e37ac2d80fd11dbd708a77c8a22ab86e25' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='06e3d64813e4ba6019d8d79e918c48af4943700bd1eb689c481d82a64f8c280a' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='a3cb6f58ee93bbd3bd72ecd45b9f37bf5e16e9c0ef30ba17c809ec7cbb84ee96' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Mon, 25 Oct 2021 17:42:59 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9399b25f47f0d86b127fa39eaf584ca9173c1768d2f0383377bfe5c0db19d9d2`  
		Last Modified: Mon, 25 Oct 2021 17:44:55 GMT  
		Size: 4.3 MB (4338197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213cedddfa2ebe35217951f615e9db98a1e437db086dc24e735aba8aee2a8592`  
		Last Modified: Mon, 25 Oct 2021 17:45:49 GMT  
		Size: 115.2 MB (115163991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:79f57ec489f4bdbe37cd7f5494f617379bb25b7fda9521e00de035517b85e013
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.7 MB (151745863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db891f22ad270fb2f05d1c9ad7727e2cb9e8a311cb32983ca55e8e36167aa191`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:13:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:13:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Oct 2021 02:13:17 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 02:13:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Oct 2021 02:13:57 GMT
ENV JULIA_VERSION=1.6.3
# Tue, 12 Oct 2021 02:14:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='c7459c334cd7c3e4a297baf52535937c6bad640e60882f9201a73bab9394314b' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7cf08affbad206bd3c1ef8bc117bf0aa6ac95d1666bf4c06f9d530cff29b2067' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='df1a7e96f83b60fda54fd14713a373e37ac2d80fd11dbd708a77c8a22ab86e25' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='06e3d64813e4ba6019d8d79e918c48af4943700bd1eb689c481d82a64f8c280a' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='a3cb6f58ee93bbd3bd72ecd45b9f37bf5e16e9c0ef30ba17c809ec7cbb84ee96' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Oct 2021 02:14:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3aaa4cbcacabf22501ccde8b2540b8dce4fa9b5722ee82168c66a8855a4c63`  
		Last Modified: Tue, 12 Oct 2021 02:16:38 GMT  
		Size: 4.6 MB (4610944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd66857956c78239cadcd50382f16705950ad5091c6ffa9cd11f7f41b32cf41`  
		Last Modified: Tue, 12 Oct 2021 02:18:01 GMT  
		Size: 119.3 MB (119343474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; ppc64le

```console
$ docker pull julia@sha256:edefd1e21ac467bc6f0456c9ece7f5a3598d9095a71c38908613a8a78f164802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142396250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f33d199503119b17096a792af8f45d9969eca45022213d2e03e2ba29f776eb4`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:46 GMT
ADD file:5526880c6f19a4b4231a8b2bd7cfc625d116764c4918eff6f0b55f8c1eb38e1a in / 
# Tue, 12 Oct 2021 01:26:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:51:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:51:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 12 Oct 2021 06:51:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 06:51:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 12 Oct 2021 06:53:18 GMT
ENV JULIA_VERSION=1.6.3
# Tue, 12 Oct 2021 06:54:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='c7459c334cd7c3e4a297baf52535937c6bad640e60882f9201a73bab9394314b' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7cf08affbad206bd3c1ef8bc117bf0aa6ac95d1666bf4c06f9d530cff29b2067' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='df1a7e96f83b60fda54fd14713a373e37ac2d80fd11dbd708a77c8a22ab86e25' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='06e3d64813e4ba6019d8d79e918c48af4943700bd1eb689c481d82a64f8c280a' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='a3cb6f58ee93bbd3bd72ecd45b9f37bf5e16e9c0ef30ba17c809ec7cbb84ee96' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Tue, 12 Oct 2021 06:54:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d69973af32573c07c8789c0f9c144a5c0b822a1e85b59db3ce9f8ebc489ce85d`  
		Last Modified: Tue, 12 Oct 2021 01:38:40 GMT  
		Size: 30.5 MB (30547197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6651b20c67f0204f1988da03e511f991ac21eeb0e84729f4676ef4984a7a6a3`  
		Last Modified: Tue, 12 Oct 2021 06:55:24 GMT  
		Size: 4.9 MB (4854320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422b813f1dcebc61860511e8c537ff6736ea1240878ed86921274fca19f8ae40`  
		Last Modified: Tue, 12 Oct 2021 06:56:22 GMT  
		Size: 107.0 MB (106994733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.20348.350; amd64

```console
$ docker pull julia@sha256:3bad5d8cfa752278e4154371301dfcc82bd5f7294ae4c76c73fbf5284e7df1b7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2318902439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc64a21674d1e2b60ccd81b23490df170b48f8c0821923e02733e7ef747bed47`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 03 Nov 2021 08:36:33 GMT
RUN Install update ltsc2022-amd64
# Wed, 10 Nov 2021 01:38:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 16:32:56 GMT
ENV JULIA_VERSION=1.6.3
# Wed, 10 Nov 2021 16:32:57 GMT
ENV JULIA_SHA256=bc43b8729dd2d95d9d148ada989c8582a66e99af89fcc91d8ed41ee2f13a9985
# Wed, 10 Nov 2021 16:34:17 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Nov 2021 16:34:18 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0eb404f1860fa8786ad09d1d9fe9fd580115f83cd38623bc4eb0c46abdaa0a3`  
		Size: 932.9 MB (932907933 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:27ded59d7006d9d7bffa7c253cd04a900a5d6b0d47b84d0edd624d12fd64cdc9`  
		Last Modified: Wed, 10 Nov 2021 02:07:39 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee76644db8eb4246fdd01f2cacd7a48532345847d7b2aed0b3720c2a85a9b51d`  
		Last Modified: Wed, 10 Nov 2021 16:50:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059c3e13eb3cfca2801bc98bcceca030c347c4e49d19debddc7491d5ba294bdb`  
		Last Modified: Wed, 10 Nov 2021 16:50:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3029ad0b3a7916a3c882f44a730118491c5b21cb9077691a6a0f115ddaad6346`  
		Last Modified: Wed, 10 Nov 2021 16:53:23 GMT  
		Size: 134.3 MB (134289777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde5b4194c1a95cc2039cdea514b2d475fafd03783b53d2fa61af5982ac790bc`  
		Last Modified: Wed, 10 Nov 2021 16:50:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.17763.2300; amd64

```console
$ docker pull julia@sha256:6106e2899affa48a30bb841df0ba463f6545a892a48b19bd30d7df72b3cb8ee8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2840164410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8790d663075e5e7f9c9749b63323cd693a85ba5b3ccd1541ceb531609a01abd6`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 16:34:37 GMT
ENV JULIA_VERSION=1.6.3
# Wed, 10 Nov 2021 16:34:38 GMT
ENV JULIA_SHA256=bc43b8729dd2d95d9d148ada989c8582a66e99af89fcc91d8ed41ee2f13a9985
# Wed, 10 Nov 2021 16:36:25 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Nov 2021 16:36:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36332ea76f6c664be25a30f2a99c6c81868dd4d34dd963db630bd1a93a148e2d`  
		Last Modified: Wed, 10 Nov 2021 16:53:38 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d9094b02d475a66b3ff52f1efbcf17bdc19ddfa0f2f0eda4d8edccbd6fe5ac`  
		Last Modified: Wed, 10 Nov 2021 16:53:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63a876deae804fb1ea34b7343c42da39e1cc9fa458fc8ae6aedd776b27a584b`  
		Last Modified: Wed, 10 Nov 2021 16:54:06 GMT  
		Size: 134.0 MB (134037564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f947f1cd8824e949ac5a58999b789cd7a0156f591d5ff393dc4b32b01c34fc2`  
		Last Modified: Wed, 10 Nov 2021 16:53:38 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.14393.4770; amd64

```console
$ docker pull julia@sha256:f1eee35edddd471b1e3c91f29b9f130eede2b9c76d1589f198774357fd9594ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6407127071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9978c7b0d641af96d374bc038d42bd3538573acaf6c0ca60dbe7aba2a5ba2d3`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 16:36:34 GMT
ENV JULIA_VERSION=1.6.3
# Wed, 10 Nov 2021 16:36:36 GMT
ENV JULIA_SHA256=bc43b8729dd2d95d9d148ada989c8582a66e99af89fcc91d8ed41ee2f13a9985
# Wed, 10 Nov 2021 16:38:35 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.')); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Complete.'
# Wed, 10 Nov 2021 16:38:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06bdbb04bf0f61b88448c676d3e27f99b26bf009d0cf818227fbd3f43acd5481`  
		Last Modified: Wed, 10 Nov 2021 16:54:20 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa7d91f9da5c7fa9cc985bc37ddda7b180692b64963def049ca71f20ca17deb`  
		Last Modified: Wed, 10 Nov 2021 16:54:20 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61c189e0e853fd0f99f4edabc1bbd62078ed753c0f07bec6633f844dd6cd90e`  
		Last Modified: Wed, 10 Nov 2021 16:56:46 GMT  
		Size: 134.0 MB (134030505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021cb037305b6323d94fa93b5ee4f992e8c8d0383b90525c083adf3d7a27ddc6`  
		Last Modified: Wed, 10 Nov 2021 16:54:20 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
