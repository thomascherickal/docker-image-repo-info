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
$ docker pull julia@sha256:a20da039d52d95c761b4b13875c94fb8318b17d9d448e735ecf925c905958ac5
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
$ docker pull julia@sha256:bfc01a9df4e1be3008f340eab05b24bdb7d9bafef34566bc3a27f1ac596d5d44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152642145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b56ebea4641ef6a66716d80dae4979419c982386cd92264acd8c28b929a2b5`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:42:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3590b2fdcfc2bff47fd0c3ae89549beb8c8a27bab9de7bb1f9fc161edf28e401`  
		Last Modified: Wed, 12 May 2021 07:44:23 GMT  
		Size: 121.0 MB (121038263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm variant v7

```console
$ docker pull julia@sha256:4fb94cb34d3a511286e0e645179bb01e291c16fdff61b25f34e7f36fe5fe904a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138674871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d195bc8607141c75d0a40c7ed04754cc2b63225bdedd2cec2b0617544fdaf347`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:24:06 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:25:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721055864112278de1c7e26fbd0a8a9090981b88c3ef7294973e2eca6d7de330`  
		Last Modified: Wed, 12 May 2021 05:29:40 GMT  
		Size: 112.1 MB (112123281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:73fb59a680664d8ba99433475b95823cf25c563bb31d8390a8425d5bcb93fadd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145166128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:315cacb65d56c0681885dd17934b6afe099870cfd7e8ad6694ef735a42a0ce0a`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:08:46 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:09:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1339845483c4b85ae6d79082f459ef0023a6fa182eb828b2d985dfb5e3c17`  
		Last Modified: Wed, 12 May 2021 05:12:07 GMT  
		Size: 114.9 MB (114916462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:a222b4e13a08bf81f7cde50e794da65bf73cd25776ebd0a93099ec585ec7435b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151027028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0560700b3f76fc2c16ff5c6563bf596ecd43892ea1f04772bc2190ec6c6bd073`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 06:25:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807190c575f727580cbfe8cc5bde2310c0e471738d5a64441791c6b967cd15f8`  
		Last Modified: Wed, 12 May 2021 06:27:38 GMT  
		Size: 118.6 MB (118621307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; ppc64le

```console
$ docker pull julia@sha256:1e89bd0a20a23ef683e7e2d4b1ce0cae1f0e78ed4f548220371a23ee6e7c9961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141804364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4655b4ce98fa467eba91dc56101179c125c5f76f5f21e28f70be0046aa3c08`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:42:03 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:10 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:45:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:45:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b9d6c62221de71df69574d32fbcaf65a789b858134d92f4cee0fc7bf6961a`  
		Last Modified: Wed, 12 May 2021 07:46:12 GMT  
		Size: 4.9 MB (4853531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8df68540a8fff3c9c01c3e8e83bf0327e0ca6ce233231e2f5c96519e4506cf`  
		Last Modified: Wed, 12 May 2021 07:46:33 GMT  
		Size: 106.4 MB (106398439 bytes)  
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
$ docker pull julia@sha256:1bb2491f1db9c9963fd9f5a1c5e3c766010fc38f609c060bca0ef0be319729c2
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
$ docker pull julia@sha256:bfc01a9df4e1be3008f340eab05b24bdb7d9bafef34566bc3a27f1ac596d5d44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152642145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b56ebea4641ef6a66716d80dae4979419c982386cd92264acd8c28b929a2b5`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:42:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3590b2fdcfc2bff47fd0c3ae89549beb8c8a27bab9de7bb1f9fc161edf28e401`  
		Last Modified: Wed, 12 May 2021 07:44:23 GMT  
		Size: 121.0 MB (121038263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:4fb94cb34d3a511286e0e645179bb01e291c16fdff61b25f34e7f36fe5fe904a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138674871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d195bc8607141c75d0a40c7ed04754cc2b63225bdedd2cec2b0617544fdaf347`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:24:06 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:25:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721055864112278de1c7e26fbd0a8a9090981b88c3ef7294973e2eca6d7de330`  
		Last Modified: Wed, 12 May 2021 05:29:40 GMT  
		Size: 112.1 MB (112123281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:73fb59a680664d8ba99433475b95823cf25c563bb31d8390a8425d5bcb93fadd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145166128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:315cacb65d56c0681885dd17934b6afe099870cfd7e8ad6694ef735a42a0ce0a`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:08:46 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:09:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1339845483c4b85ae6d79082f459ef0023a6fa182eb828b2d985dfb5e3c17`  
		Last Modified: Wed, 12 May 2021 05:12:07 GMT  
		Size: 114.9 MB (114916462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; 386

```console
$ docker pull julia@sha256:a222b4e13a08bf81f7cde50e794da65bf73cd25776ebd0a93099ec585ec7435b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151027028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0560700b3f76fc2c16ff5c6563bf596ecd43892ea1f04772bc2190ec6c6bd073`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 06:25:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807190c575f727580cbfe8cc5bde2310c0e471738d5a64441791c6b967cd15f8`  
		Last Modified: Wed, 12 May 2021 06:27:38 GMT  
		Size: 118.6 MB (118621307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:1e89bd0a20a23ef683e7e2d4b1ce0cae1f0e78ed4f548220371a23ee6e7c9961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141804364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4655b4ce98fa467eba91dc56101179c125c5f76f5f21e28f70be0046aa3c08`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:42:03 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:10 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:45:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:45:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b9d6c62221de71df69574d32fbcaf65a789b858134d92f4cee0fc7bf6961a`  
		Last Modified: Wed, 12 May 2021 07:46:12 GMT  
		Size: 4.9 MB (4853531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8df68540a8fff3c9c01c3e8e83bf0327e0ca6ce233231e2f5c96519e4506cf`  
		Last Modified: Wed, 12 May 2021 07:46:33 GMT  
		Size: 106.4 MB (106398439 bytes)  
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
$ docker pull julia@sha256:92cbbf515425538f7cbb8cd76bcbdd970d19a85e6ba37e6e4b0d3821e69ceeff
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
$ docker pull julia@sha256:4e3abbfb7997b874d0c072f0d87f095ead72277c9696ffdc892d0acd9b68f034
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127167343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e703ba5244a2b5791434090b0cdf4744865f04da4a9cc06637ffe149e8617ef4`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 07:42:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef49001e91b7412b4fe416d3e59c973035b0878dad235c6f904ca10ea3a579f0`  
		Last Modified: Wed, 12 May 2021 07:44:59 GMT  
		Size: 95.6 MB (95563461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm variant v7

```console
$ docker pull julia@sha256:99e2202438834b15f9af2a20c722b9454f49a8c61d5340079d65e33f82875f44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113680540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b2eb5a20ef9de1f7b04ed25da8b18b661c21cc6732fc7258e446cb025c0acda`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:25:33 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:26:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:26:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0172e7367d606799747ab244ec699332195e953ff15b9cfdee409edad3b5e4f5`  
		Last Modified: Wed, 12 May 2021 05:30:21 GMT  
		Size: 87.1 MB (87128950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c022ee68654e450062e88550327499d7cdf0e8988f788d6f9de9a72a5d86b59d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110140808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9b42ecba10533a17b7b8ce785a36040c020089726e21044c292eb01e370e31`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:09:27 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:09:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7132a18129ef30dd1365f0a243d47d06fbb2226c788b14580e9f4f637c1497d3`  
		Last Modified: Wed, 12 May 2021 05:12:37 GMT  
		Size: 79.9 MB (79891142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; 386

```console
$ docker pull julia@sha256:57e5cd7991e9301a4202037db199a226a38b1bdd29aa99f4e742a8555bfbefc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124904797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a74462823cc1c7263121827e593327fe8ace4b44af522cb7ef86f054e68b7c`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:25:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 06:25:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c81391664817920efda67219799c15979d42b6259bb2d6f94c8f08472e7c78e`  
		Last Modified: Wed, 12 May 2021 06:28:28 GMT  
		Size: 92.5 MB (92499076 bytes)  
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
$ docker pull julia@sha256:d673e09eb113ab3481fe067dd3dca99863903a308e4241f0bd668d95b6dabf1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:4e3abbfb7997b874d0c072f0d87f095ead72277c9696ffdc892d0acd9b68f034
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127167343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e703ba5244a2b5791434090b0cdf4744865f04da4a9cc06637ffe149e8617ef4`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 07:42:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef49001e91b7412b4fe416d3e59c973035b0878dad235c6f904ca10ea3a579f0`  
		Last Modified: Wed, 12 May 2021 07:44:59 GMT  
		Size: 95.6 MB (95563461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:99e2202438834b15f9af2a20c722b9454f49a8c61d5340079d65e33f82875f44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113680540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b2eb5a20ef9de1f7b04ed25da8b18b661c21cc6732fc7258e446cb025c0acda`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:25:33 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:26:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:26:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0172e7367d606799747ab244ec699332195e953ff15b9cfdee409edad3b5e4f5`  
		Last Modified: Wed, 12 May 2021 05:30:21 GMT  
		Size: 87.1 MB (87128950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c022ee68654e450062e88550327499d7cdf0e8988f788d6f9de9a72a5d86b59d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110140808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9b42ecba10533a17b7b8ce785a36040c020089726e21044c292eb01e370e31`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:09:27 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:09:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7132a18129ef30dd1365f0a243d47d06fbb2226c788b14580e9f4f637c1497d3`  
		Last Modified: Wed, 12 May 2021 05:12:37 GMT  
		Size: 79.9 MB (79891142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; 386

```console
$ docker pull julia@sha256:57e5cd7991e9301a4202037db199a226a38b1bdd29aa99f4e742a8555bfbefc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124904797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a74462823cc1c7263121827e593327fe8ace4b44af522cb7ef86f054e68b7c`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:25:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 06:25:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c81391664817920efda67219799c15979d42b6259bb2d6f94c8f08472e7c78e`  
		Last Modified: Wed, 12 May 2021 06:28:28 GMT  
		Size: 92.5 MB (92499076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-stretch`

```console
$ docker pull julia@sha256:a34a92bb45c65c7f49ce4c4d7d741065033bc498e44f0a0b10a8d5cb5ab07062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-stretch` - linux; amd64

```console
$ docker pull julia@sha256:15ed05d5089a0798eab11f0a6b4f70b2161d22ac5bd347bd9b2f8c54d5076aef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150445548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7325e286df9e036090a0cd87f061d844bd6ec0874e176b6ed6f150007af5f6d7`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:42:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:42:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:42:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:42:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:54 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 07:43:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:43:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cfb94db574b9f9fd071f5977536120b564935fbfdd7c185a4125eb4b594175`  
		Last Modified: Wed, 12 May 2021 07:45:12 GMT  
		Size: 9.5 MB (9491707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7867a4b095ebaffd05af1180fb4015f1f06c055d56d97c6e458a73625bad41c1`  
		Last Modified: Wed, 12 May 2021 07:45:28 GMT  
		Size: 95.6 MB (95573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:d43511b724a45c5d755420a38ac720ca683478df729202ef6618d83a30bb0684
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137464196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b936ff8e198dcbf0a321ec78982bbfbef1e621c3fcc60c4761db0fe65b8d9f`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:11:51 GMT
ADD file:81cfd4e746bdfcc19847240b77012487652be22dbd5741ccb2485a4207f2b73f in / 
# Wed, 12 May 2021 01:11:56 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:27:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:27:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:27:30 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:27:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:27:41 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:28:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:28:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:55b9a6b6b2552c5b2eac0a316e75a7bc18092819ee25c4f1d4d54700bcc1d3dc`  
		Last Modified: Wed, 12 May 2021 01:21:23 GMT  
		Size: 42.1 MB (42120307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6827c3cf09f2d4679be84b0459a5d1c6768fc46ef9eb9ecd131c82502367c0c7`  
		Last Modified: Wed, 12 May 2021 05:30:32 GMT  
		Size: 8.2 MB (8206188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824f8194f92835fce202057961485275aabda2d341c5560fe61e945f2b987025`  
		Last Modified: Wed, 12 May 2021 05:30:59 GMT  
		Size: 87.1 MB (87137701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:6ca47cbd25adadc424cdbc1d64759c22209a706f2fcfee397cb9fbfd1a3ac273
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131538174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eee7ae41bcfb9c9eb037b97a62f7d5f1f2ade7d3494a116e96f22801241ffe42`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:56:12 GMT
ADD file:9582243afc9973a3708fda530270ae8f23796b20a532a9f07e4faaf245e2cdc0 in / 
# Wed, 12 May 2021 00:56:18 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:10:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:10:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:10:27 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:10:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:10:30 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:11:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:11:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:41f38ce3010a5142300d74e5e19db4dea7694f4771471c330fff27c633f8ba32`  
		Last Modified: Wed, 12 May 2021 01:04:15 GMT  
		Size: 43.2 MB (43177820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2f9cf036df066305fd9eb9603c4d8eb5e707e4fa1bbdf5565b37a59962685b`  
		Last Modified: Wed, 12 May 2021 05:12:46 GMT  
		Size: 8.5 MB (8451245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b43704452a96bec2bbf628200ee815a4bd0a8896a9433134acbcfec03d63ff1`  
		Last Modified: Wed, 12 May 2021 05:13:07 GMT  
		Size: 79.9 MB (79909109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; 386

```console
$ docker pull julia@sha256:bd10277bb14a9d36bfd75c31fc1a0a89ab9ac7519c521002a25e0fb7c761b1de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148093854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db5ff238a1290970bdc27378cb0b8dca4addc200e08f689a426d040b978e34f`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:41:41 GMT
ADD file:3b26e2f83a0edf42ea62d20102b47011ee41cd2ab349c9da7487f62ff21b8471 in / 
# Wed, 12 May 2021 00:41:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:26:00 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:26:00 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:26:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:26:01 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 06:26:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:26:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2a179d76df60628ca372acea241dbf24d4039a86b7dc2ba920d26f64bded15a1`  
		Last Modified: Wed, 12 May 2021 00:49:13 GMT  
		Size: 46.1 MB (46098744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cb1d8105074193c3b0923e01b4e259db0ca62727276144bf4240d4a8e1d49b`  
		Last Modified: Wed, 12 May 2021 06:28:45 GMT  
		Size: 9.5 MB (9493223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e95206e112ea371512ab725ba2d8b8554508e492a03563916817453debf0c`  
		Last Modified: Wed, 12 May 2021 06:29:08 GMT  
		Size: 92.5 MB (92501887 bytes)  
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
$ docker pull julia@sha256:92cbbf515425538f7cbb8cd76bcbdd970d19a85e6ba37e6e4b0d3821e69ceeff
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
$ docker pull julia@sha256:4e3abbfb7997b874d0c072f0d87f095ead72277c9696ffdc892d0acd9b68f034
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127167343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e703ba5244a2b5791434090b0cdf4744865f04da4a9cc06637ffe149e8617ef4`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 07:42:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef49001e91b7412b4fe416d3e59c973035b0878dad235c6f904ca10ea3a579f0`  
		Last Modified: Wed, 12 May 2021 07:44:59 GMT  
		Size: 95.6 MB (95563461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm variant v7

```console
$ docker pull julia@sha256:99e2202438834b15f9af2a20c722b9454f49a8c61d5340079d65e33f82875f44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113680540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b2eb5a20ef9de1f7b04ed25da8b18b661c21cc6732fc7258e446cb025c0acda`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:25:33 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:26:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:26:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0172e7367d606799747ab244ec699332195e953ff15b9cfdee409edad3b5e4f5`  
		Last Modified: Wed, 12 May 2021 05:30:21 GMT  
		Size: 87.1 MB (87128950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c022ee68654e450062e88550327499d7cdf0e8988f788d6f9de9a72a5d86b59d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110140808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9b42ecba10533a17b7b8ce785a36040c020089726e21044c292eb01e370e31`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:09:27 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:09:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7132a18129ef30dd1365f0a243d47d06fbb2226c788b14580e9f4f637c1497d3`  
		Last Modified: Wed, 12 May 2021 05:12:37 GMT  
		Size: 79.9 MB (79891142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; 386

```console
$ docker pull julia@sha256:57e5cd7991e9301a4202037db199a226a38b1bdd29aa99f4e742a8555bfbefc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124904797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a74462823cc1c7263121827e593327fe8ace4b44af522cb7ef86f054e68b7c`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:25:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 06:25:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c81391664817920efda67219799c15979d42b6259bb2d6f94c8f08472e7c78e`  
		Last Modified: Wed, 12 May 2021 06:28:28 GMT  
		Size: 92.5 MB (92499076 bytes)  
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
$ docker pull julia@sha256:d673e09eb113ab3481fe067dd3dca99863903a308e4241f0bd668d95b6dabf1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-buster` - linux; amd64

```console
$ docker pull julia@sha256:4e3abbfb7997b874d0c072f0d87f095ead72277c9696ffdc892d0acd9b68f034
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127167343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e703ba5244a2b5791434090b0cdf4744865f04da4a9cc06637ffe149e8617ef4`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 07:42:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:40 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef49001e91b7412b4fe416d3e59c973035b0878dad235c6f904ca10ea3a579f0`  
		Last Modified: Wed, 12 May 2021 07:44:59 GMT  
		Size: 95.6 MB (95563461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:99e2202438834b15f9af2a20c722b9454f49a8c61d5340079d65e33f82875f44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113680540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b2eb5a20ef9de1f7b04ed25da8b18b661c21cc6732fc7258e446cb025c0acda`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:25:33 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:26:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:26:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0172e7367d606799747ab244ec699332195e953ff15b9cfdee409edad3b5e4f5`  
		Last Modified: Wed, 12 May 2021 05:30:21 GMT  
		Size: 87.1 MB (87128950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c022ee68654e450062e88550327499d7cdf0e8988f788d6f9de9a72a5d86b59d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110140808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9b42ecba10533a17b7b8ce785a36040c020089726e21044c292eb01e370e31`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:09:27 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:09:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7132a18129ef30dd1365f0a243d47d06fbb2226c788b14580e9f4f637c1497d3`  
		Last Modified: Wed, 12 May 2021 05:12:37 GMT  
		Size: 79.9 MB (79891142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; 386

```console
$ docker pull julia@sha256:57e5cd7991e9301a4202037db199a226a38b1bdd29aa99f4e742a8555bfbefc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124904797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a74462823cc1c7263121827e593327fe8ace4b44af522cb7ef86f054e68b7c`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:25:24 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 06:25:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c81391664817920efda67219799c15979d42b6259bb2d6f94c8f08472e7c78e`  
		Last Modified: Wed, 12 May 2021 06:28:28 GMT  
		Size: 92.5 MB (92499076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-stretch`

```console
$ docker pull julia@sha256:a34a92bb45c65c7f49ce4c4d7d741065033bc498e44f0a0b10a8d5cb5ab07062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-stretch` - linux; amd64

```console
$ docker pull julia@sha256:15ed05d5089a0798eab11f0a6b4f70b2161d22ac5bd347bd9b2f8c54d5076aef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150445548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7325e286df9e036090a0cd87f061d844bd6ec0874e176b6ed6f150007af5f6d7`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:42:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:42:54 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:42:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:42:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:54 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 07:43:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:43:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cfb94db574b9f9fd071f5977536120b564935fbfdd7c185a4125eb4b594175`  
		Last Modified: Wed, 12 May 2021 07:45:12 GMT  
		Size: 9.5 MB (9491707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7867a4b095ebaffd05af1180fb4015f1f06c055d56d97c6e458a73625bad41c1`  
		Last Modified: Wed, 12 May 2021 07:45:28 GMT  
		Size: 95.6 MB (95573758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:d43511b724a45c5d755420a38ac720ca683478df729202ef6618d83a30bb0684
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137464196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b936ff8e198dcbf0a321ec78982bbfbef1e621c3fcc60c4761db0fe65b8d9f`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:11:51 GMT
ADD file:81cfd4e746bdfcc19847240b77012487652be22dbd5741ccb2485a4207f2b73f in / 
# Wed, 12 May 2021 01:11:56 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:27:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:27:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:27:30 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:27:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:27:41 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:28:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:28:33 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:55b9a6b6b2552c5b2eac0a316e75a7bc18092819ee25c4f1d4d54700bcc1d3dc`  
		Last Modified: Wed, 12 May 2021 01:21:23 GMT  
		Size: 42.1 MB (42120307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6827c3cf09f2d4679be84b0459a5d1c6768fc46ef9eb9ecd131c82502367c0c7`  
		Last Modified: Wed, 12 May 2021 05:30:32 GMT  
		Size: 8.2 MB (8206188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824f8194f92835fce202057961485275aabda2d341c5560fe61e945f2b987025`  
		Last Modified: Wed, 12 May 2021 05:30:59 GMT  
		Size: 87.1 MB (87137701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:6ca47cbd25adadc424cdbc1d64759c22209a706f2fcfee397cb9fbfd1a3ac273
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131538174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eee7ae41bcfb9c9eb037b97a62f7d5f1f2ade7d3494a116e96f22801241ffe42`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:56:12 GMT
ADD file:9582243afc9973a3708fda530270ae8f23796b20a532a9f07e4faaf245e2cdc0 in / 
# Wed, 12 May 2021 00:56:18 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:10:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:10:26 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:10:27 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:10:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:10:30 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 05:11:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:11:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:41f38ce3010a5142300d74e5e19db4dea7694f4771471c330fff27c633f8ba32`  
		Last Modified: Wed, 12 May 2021 01:04:15 GMT  
		Size: 43.2 MB (43177820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2f9cf036df066305fd9eb9603c4d8eb5e707e4fa1bbdf5565b37a59962685b`  
		Last Modified: Wed, 12 May 2021 05:12:46 GMT  
		Size: 8.5 MB (8451245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b43704452a96bec2bbf628200ee815a4bd0a8896a9433134acbcfec03d63ff1`  
		Last Modified: Wed, 12 May 2021 05:13:07 GMT  
		Size: 79.9 MB (79909109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; 386

```console
$ docker pull julia@sha256:bd10277bb14a9d36bfd75c31fc1a0a89ab9ac7519c521002a25e0fb7c761b1de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148093854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db5ff238a1290970bdc27378cb0b8dca4addc200e08f689a426d040b978e34f`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:41:41 GMT
ADD file:3b26e2f83a0edf42ea62d20102b47011ee41cd2ab349c9da7487f62ff21b8471 in / 
# Wed, 12 May 2021 00:41:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:26:00 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:26:00 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:26:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:26:01 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 12 May 2021 06:26:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:26:21 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2a179d76df60628ca372acea241dbf24d4039a86b7dc2ba920d26f64bded15a1`  
		Last Modified: Wed, 12 May 2021 00:49:13 GMT  
		Size: 46.1 MB (46098744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cb1d8105074193c3b0923e01b4e259db0ca62727276144bf4240d4a8e1d49b`  
		Last Modified: Wed, 12 May 2021 06:28:45 GMT  
		Size: 9.5 MB (9493223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e95206e112ea371512ab725ba2d8b8554508e492a03563916817453debf0c`  
		Last Modified: Wed, 12 May 2021 06:29:08 GMT  
		Size: 92.5 MB (92501887 bytes)  
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
$ docker pull julia@sha256:a20da039d52d95c761b4b13875c94fb8318b17d9d448e735ecf925c905958ac5
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
$ docker pull julia@sha256:bfc01a9df4e1be3008f340eab05b24bdb7d9bafef34566bc3a27f1ac596d5d44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152642145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b56ebea4641ef6a66716d80dae4979419c982386cd92264acd8c28b929a2b5`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:42:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3590b2fdcfc2bff47fd0c3ae89549beb8c8a27bab9de7bb1f9fc161edf28e401`  
		Last Modified: Wed, 12 May 2021 07:44:23 GMT  
		Size: 121.0 MB (121038263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm variant v7

```console
$ docker pull julia@sha256:4fb94cb34d3a511286e0e645179bb01e291c16fdff61b25f34e7f36fe5fe904a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138674871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d195bc8607141c75d0a40c7ed04754cc2b63225bdedd2cec2b0617544fdaf347`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:24:06 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:25:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721055864112278de1c7e26fbd0a8a9090981b88c3ef7294973e2eca6d7de330`  
		Last Modified: Wed, 12 May 2021 05:29:40 GMT  
		Size: 112.1 MB (112123281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:73fb59a680664d8ba99433475b95823cf25c563bb31d8390a8425d5bcb93fadd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145166128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:315cacb65d56c0681885dd17934b6afe099870cfd7e8ad6694ef735a42a0ce0a`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:08:46 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:09:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1339845483c4b85ae6d79082f459ef0023a6fa182eb828b2d985dfb5e3c17`  
		Last Modified: Wed, 12 May 2021 05:12:07 GMT  
		Size: 114.9 MB (114916462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; 386

```console
$ docker pull julia@sha256:a222b4e13a08bf81f7cde50e794da65bf73cd25776ebd0a93099ec585ec7435b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151027028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0560700b3f76fc2c16ff5c6563bf596ecd43892ea1f04772bc2190ec6c6bd073`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 06:25:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807190c575f727580cbfe8cc5bde2310c0e471738d5a64441791c6b967cd15f8`  
		Last Modified: Wed, 12 May 2021 06:27:38 GMT  
		Size: 118.6 MB (118621307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6` - linux; ppc64le

```console
$ docker pull julia@sha256:1e89bd0a20a23ef683e7e2d4b1ce0cae1f0e78ed4f548220371a23ee6e7c9961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141804364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4655b4ce98fa467eba91dc56101179c125c5f76f5f21e28f70be0046aa3c08`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:42:03 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:10 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:45:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:45:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b9d6c62221de71df69574d32fbcaf65a789b858134d92f4cee0fc7bf6961a`  
		Last Modified: Wed, 12 May 2021 07:46:12 GMT  
		Size: 4.9 MB (4853531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8df68540a8fff3c9c01c3e8e83bf0327e0ca6ce233231e2f5c96519e4506cf`  
		Last Modified: Wed, 12 May 2021 07:46:33 GMT  
		Size: 106.4 MB (106398439 bytes)  
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
$ docker pull julia@sha256:1bb2491f1db9c9963fd9f5a1c5e3c766010fc38f609c060bca0ef0be319729c2
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
$ docker pull julia@sha256:bfc01a9df4e1be3008f340eab05b24bdb7d9bafef34566bc3a27f1ac596d5d44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152642145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b56ebea4641ef6a66716d80dae4979419c982386cd92264acd8c28b929a2b5`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:42:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3590b2fdcfc2bff47fd0c3ae89549beb8c8a27bab9de7bb1f9fc161edf28e401`  
		Last Modified: Wed, 12 May 2021 07:44:23 GMT  
		Size: 121.0 MB (121038263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:4fb94cb34d3a511286e0e645179bb01e291c16fdff61b25f34e7f36fe5fe904a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138674871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d195bc8607141c75d0a40c7ed04754cc2b63225bdedd2cec2b0617544fdaf347`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:24:06 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:25:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721055864112278de1c7e26fbd0a8a9090981b88c3ef7294973e2eca6d7de330`  
		Last Modified: Wed, 12 May 2021 05:29:40 GMT  
		Size: 112.1 MB (112123281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:73fb59a680664d8ba99433475b95823cf25c563bb31d8390a8425d5bcb93fadd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145166128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:315cacb65d56c0681885dd17934b6afe099870cfd7e8ad6694ef735a42a0ce0a`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:08:46 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:09:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1339845483c4b85ae6d79082f459ef0023a6fa182eb828b2d985dfb5e3c17`  
		Last Modified: Wed, 12 May 2021 05:12:07 GMT  
		Size: 114.9 MB (114916462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; 386

```console
$ docker pull julia@sha256:a222b4e13a08bf81f7cde50e794da65bf73cd25776ebd0a93099ec585ec7435b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151027028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0560700b3f76fc2c16ff5c6563bf596ecd43892ea1f04772bc2190ec6c6bd073`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 06:25:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807190c575f727580cbfe8cc5bde2310c0e471738d5a64441791c6b967cd15f8`  
		Last Modified: Wed, 12 May 2021 06:27:38 GMT  
		Size: 118.6 MB (118621307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:1e89bd0a20a23ef683e7e2d4b1ce0cae1f0e78ed4f548220371a23ee6e7c9961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141804364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4655b4ce98fa467eba91dc56101179c125c5f76f5f21e28f70be0046aa3c08`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:42:03 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:10 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:45:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:45:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b9d6c62221de71df69574d32fbcaf65a789b858134d92f4cee0fc7bf6961a`  
		Last Modified: Wed, 12 May 2021 07:46:12 GMT  
		Size: 4.9 MB (4853531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8df68540a8fff3c9c01c3e8e83bf0327e0ca6ce233231e2f5c96519e4506cf`  
		Last Modified: Wed, 12 May 2021 07:46:33 GMT  
		Size: 106.4 MB (106398439 bytes)  
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
$ docker pull julia@sha256:a20da039d52d95c761b4b13875c94fb8318b17d9d448e735ecf925c905958ac5
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
$ docker pull julia@sha256:bfc01a9df4e1be3008f340eab05b24bdb7d9bafef34566bc3a27f1ac596d5d44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152642145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b56ebea4641ef6a66716d80dae4979419c982386cd92264acd8c28b929a2b5`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:42:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3590b2fdcfc2bff47fd0c3ae89549beb8c8a27bab9de7bb1f9fc161edf28e401`  
		Last Modified: Wed, 12 May 2021 07:44:23 GMT  
		Size: 121.0 MB (121038263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1` - linux; arm variant v7

```console
$ docker pull julia@sha256:4fb94cb34d3a511286e0e645179bb01e291c16fdff61b25f34e7f36fe5fe904a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138674871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d195bc8607141c75d0a40c7ed04754cc2b63225bdedd2cec2b0617544fdaf347`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:24:06 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:25:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721055864112278de1c7e26fbd0a8a9090981b88c3ef7294973e2eca6d7de330`  
		Last Modified: Wed, 12 May 2021 05:29:40 GMT  
		Size: 112.1 MB (112123281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:73fb59a680664d8ba99433475b95823cf25c563bb31d8390a8425d5bcb93fadd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145166128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:315cacb65d56c0681885dd17934b6afe099870cfd7e8ad6694ef735a42a0ce0a`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:08:46 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:09:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1339845483c4b85ae6d79082f459ef0023a6fa182eb828b2d985dfb5e3c17`  
		Last Modified: Wed, 12 May 2021 05:12:07 GMT  
		Size: 114.9 MB (114916462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1` - linux; 386

```console
$ docker pull julia@sha256:a222b4e13a08bf81f7cde50e794da65bf73cd25776ebd0a93099ec585ec7435b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151027028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0560700b3f76fc2c16ff5c6563bf596ecd43892ea1f04772bc2190ec6c6bd073`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 06:25:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807190c575f727580cbfe8cc5bde2310c0e471738d5a64441791c6b967cd15f8`  
		Last Modified: Wed, 12 May 2021 06:27:38 GMT  
		Size: 118.6 MB (118621307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1` - linux; ppc64le

```console
$ docker pull julia@sha256:1e89bd0a20a23ef683e7e2d4b1ce0cae1f0e78ed4f548220371a23ee6e7c9961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141804364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4655b4ce98fa467eba91dc56101179c125c5f76f5f21e28f70be0046aa3c08`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:42:03 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:10 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:45:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:45:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b9d6c62221de71df69574d32fbcaf65a789b858134d92f4cee0fc7bf6961a`  
		Last Modified: Wed, 12 May 2021 07:46:12 GMT  
		Size: 4.9 MB (4853531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8df68540a8fff3c9c01c3e8e83bf0327e0ca6ce233231e2f5c96519e4506cf`  
		Last Modified: Wed, 12 May 2021 07:46:33 GMT  
		Size: 106.4 MB (106398439 bytes)  
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
$ docker pull julia@sha256:1bb2491f1db9c9963fd9f5a1c5e3c766010fc38f609c060bca0ef0be319729c2
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
$ docker pull julia@sha256:bfc01a9df4e1be3008f340eab05b24bdb7d9bafef34566bc3a27f1ac596d5d44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152642145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b56ebea4641ef6a66716d80dae4979419c982386cd92264acd8c28b929a2b5`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:42:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3590b2fdcfc2bff47fd0c3ae89549beb8c8a27bab9de7bb1f9fc161edf28e401`  
		Last Modified: Wed, 12 May 2021 07:44:23 GMT  
		Size: 121.0 MB (121038263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:4fb94cb34d3a511286e0e645179bb01e291c16fdff61b25f34e7f36fe5fe904a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138674871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d195bc8607141c75d0a40c7ed04754cc2b63225bdedd2cec2b0617544fdaf347`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:24:06 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:25:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721055864112278de1c7e26fbd0a8a9090981b88c3ef7294973e2eca6d7de330`  
		Last Modified: Wed, 12 May 2021 05:29:40 GMT  
		Size: 112.1 MB (112123281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:73fb59a680664d8ba99433475b95823cf25c563bb31d8390a8425d5bcb93fadd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145166128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:315cacb65d56c0681885dd17934b6afe099870cfd7e8ad6694ef735a42a0ce0a`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:08:46 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:09:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1339845483c4b85ae6d79082f459ef0023a6fa182eb828b2d985dfb5e3c17`  
		Last Modified: Wed, 12 May 2021 05:12:07 GMT  
		Size: 114.9 MB (114916462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1-buster` - linux; 386

```console
$ docker pull julia@sha256:a222b4e13a08bf81f7cde50e794da65bf73cd25776ebd0a93099ec585ec7435b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151027028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0560700b3f76fc2c16ff5c6563bf596ecd43892ea1f04772bc2190ec6c6bd073`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 06:25:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807190c575f727580cbfe8cc5bde2310c0e471738d5a64441791c6b967cd15f8`  
		Last Modified: Wed, 12 May 2021 06:27:38 GMT  
		Size: 118.6 MB (118621307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.6.1-buster` - linux; ppc64le

```console
$ docker pull julia@sha256:1e89bd0a20a23ef683e7e2d4b1ce0cae1f0e78ed4f548220371a23ee6e7c9961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141804364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4655b4ce98fa467eba91dc56101179c125c5f76f5f21e28f70be0046aa3c08`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:42:03 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:10 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:45:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:45:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b9d6c62221de71df69574d32fbcaf65a789b858134d92f4cee0fc7bf6961a`  
		Last Modified: Wed, 12 May 2021 07:46:12 GMT  
		Size: 4.9 MB (4853531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8df68540a8fff3c9c01c3e8e83bf0327e0ca6ce233231e2f5c96519e4506cf`  
		Last Modified: Wed, 12 May 2021 07:46:33 GMT  
		Size: 106.4 MB (106398439 bytes)  
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
$ docker pull julia@sha256:1bb2491f1db9c9963fd9f5a1c5e3c766010fc38f609c060bca0ef0be319729c2
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
$ docker pull julia@sha256:bfc01a9df4e1be3008f340eab05b24bdb7d9bafef34566bc3a27f1ac596d5d44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152642145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b56ebea4641ef6a66716d80dae4979419c982386cd92264acd8c28b929a2b5`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:42:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3590b2fdcfc2bff47fd0c3ae89549beb8c8a27bab9de7bb1f9fc161edf28e401`  
		Last Modified: Wed, 12 May 2021 07:44:23 GMT  
		Size: 121.0 MB (121038263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:4fb94cb34d3a511286e0e645179bb01e291c16fdff61b25f34e7f36fe5fe904a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138674871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d195bc8607141c75d0a40c7ed04754cc2b63225bdedd2cec2b0617544fdaf347`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:24:06 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:25:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721055864112278de1c7e26fbd0a8a9090981b88c3ef7294973e2eca6d7de330`  
		Last Modified: Wed, 12 May 2021 05:29:40 GMT  
		Size: 112.1 MB (112123281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:73fb59a680664d8ba99433475b95823cf25c563bb31d8390a8425d5bcb93fadd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145166128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:315cacb65d56c0681885dd17934b6afe099870cfd7e8ad6694ef735a42a0ce0a`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:08:46 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:09:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1339845483c4b85ae6d79082f459ef0023a6fa182eb828b2d985dfb5e3c17`  
		Last Modified: Wed, 12 May 2021 05:12:07 GMT  
		Size: 114.9 MB (114916462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:a222b4e13a08bf81f7cde50e794da65bf73cd25776ebd0a93099ec585ec7435b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151027028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0560700b3f76fc2c16ff5c6563bf596ecd43892ea1f04772bc2190ec6c6bd073`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 06:25:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807190c575f727580cbfe8cc5bde2310c0e471738d5a64441791c6b967cd15f8`  
		Last Modified: Wed, 12 May 2021 06:27:38 GMT  
		Size: 118.6 MB (118621307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; ppc64le

```console
$ docker pull julia@sha256:1e89bd0a20a23ef683e7e2d4b1ce0cae1f0e78ed4f548220371a23ee6e7c9961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141804364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4655b4ce98fa467eba91dc56101179c125c5f76f5f21e28f70be0046aa3c08`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:42:03 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:10 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:45:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:45:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b9d6c62221de71df69574d32fbcaf65a789b858134d92f4cee0fc7bf6961a`  
		Last Modified: Wed, 12 May 2021 07:46:12 GMT  
		Size: 4.9 MB (4853531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8df68540a8fff3c9c01c3e8e83bf0327e0ca6ce233231e2f5c96519e4506cf`  
		Last Modified: Wed, 12 May 2021 07:46:33 GMT  
		Size: 106.4 MB (106398439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:a20da039d52d95c761b4b13875c94fb8318b17d9d448e735ecf925c905958ac5
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
$ docker pull julia@sha256:bfc01a9df4e1be3008f340eab05b24bdb7d9bafef34566bc3a27f1ac596d5d44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.6 MB (152642145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b56ebea4641ef6a66716d80dae4979419c982386cd92264acd8c28b929a2b5`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:56 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:41:57 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:42:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:42:14 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f547a6826c90d8e31258244b6bb64fd967e5dbdaf8bed0c7712c0269f81efa`  
		Last Modified: Wed, 12 May 2021 07:43:57 GMT  
		Size: 4.5 MB (4457967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3590b2fdcfc2bff47fd0c3ae89549beb8c8a27bab9de7bb1f9fc161edf28e401`  
		Last Modified: Wed, 12 May 2021 07:44:23 GMT  
		Size: 121.0 MB (121038263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm variant v7

```console
$ docker pull julia@sha256:4fb94cb34d3a511286e0e645179bb01e291c16fdff61b25f34e7f36fe5fe904a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138674871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d195bc8607141c75d0a40c7ed04754cc2b63225bdedd2cec2b0617544fdaf347`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:23:49 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:23:56 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:24:01 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:24:06 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:25:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fac5422993ec7963ee4e886e056cd1de63597b4a034c948dedfdc2255c1ebc3`  
		Last Modified: Wed, 12 May 2021 05:29:05 GMT  
		Size: 3.8 MB (3805324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721055864112278de1c7e26fbd0a8a9090981b88c3ef7294973e2eca6d7de330`  
		Last Modified: Wed, 12 May 2021 05:29:40 GMT  
		Size: 112.1 MB (112123281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:73fb59a680664d8ba99433475b95823cf25c563bb31d8390a8425d5bcb93fadd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145166128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:315cacb65d56c0681885dd17934b6afe099870cfd7e8ad6694ef735a42a0ce0a`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 05:08:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 05:08:45 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 05:08:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 05:08:46 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 05:09:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 05:09:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a26428527d17de6f793835329fb56ff5d006bce4689329f3f0a82af75e239d`  
		Last Modified: Wed, 12 May 2021 05:11:35 GMT  
		Size: 4.3 MB (4338416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e1339845483c4b85ae6d79082f459ef0023a6fa182eb828b2d985dfb5e3c17`  
		Last Modified: Wed, 12 May 2021 05:12:07 GMT  
		Size: 114.9 MB (114916462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:a222b4e13a08bf81f7cde50e794da65bf73cd25776ebd0a93099ec585ec7435b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (151027028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0560700b3f76fc2c16ff5c6563bf596ecd43892ea1f04772bc2190ec6c6bd073`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:24:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:24:53 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 06:24:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 06:24:54 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 06:25:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 06:25:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded8ee5a5cacc938dde888f7ef76c634f79f3f7b2e3de3fa58083d7f6e16932`  
		Last Modified: Wed, 12 May 2021 06:27:02 GMT  
		Size: 4.6 MB (4610647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807190c575f727580cbfe8cc5bde2310c0e471738d5a64441791c6b967cd15f8`  
		Last Modified: Wed, 12 May 2021 06:27:38 GMT  
		Size: 118.6 MB (118621307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; ppc64le

```console
$ docker pull julia@sha256:1e89bd0a20a23ef683e7e2d4b1ce0cae1f0e78ed4f548220371a23ee6e7c9961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141804364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4655b4ce98fa467eba91dc56101179c125c5f76f5f21e28f70be0046aa3c08`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 07:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 12 May 2021 07:41:54 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 07:42:03 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 12 May 2021 07:42:10 GMT
ENV JULIA_VERSION=1.6.1
# Wed, 12 May 2021 07:45:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='7c888adec3ea42afbfed2ce756ce1164a570d50fa7506c3f2e1e2cbc49d52506' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='4fcdbd35334788ad6c2a5e79270a126496a01e1834de1e6895441a0aec8c8a55' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='e6c6a0eba5546b6f8b9cdd4d303517f94e0892056c20d89faf86ee1678aab917' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='b65f3e4288279d214f5a1fb98aafc16fd6dfae7225833b5fb34cfbb5e1651b15' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='c5732c8777e302f01751314314006fba4e80eb3118cba15ef2858ede1f6d23e2' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 12 May 2021 07:45:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b9d6c62221de71df69574d32fbcaf65a789b858134d92f4cee0fc7bf6961a`  
		Last Modified: Wed, 12 May 2021 07:46:12 GMT  
		Size: 4.9 MB (4853531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8df68540a8fff3c9c01c3e8e83bf0327e0ca6ce233231e2f5c96519e4506cf`  
		Last Modified: Wed, 12 May 2021 07:46:33 GMT  
		Size: 106.4 MB (106398439 bytes)  
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
