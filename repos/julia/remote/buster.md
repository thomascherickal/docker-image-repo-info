## `julia:buster`

```console
$ docker pull julia@sha256:00d3fc012534d8f1f07c458a7c07c816a87f8f70e6a16d07eb202eb2a42e4415
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
$ docker pull julia@sha256:48a445a78f4460a8f0c7daf8f6ca376bc190485a092f681a4f24b4fb4c57bdf7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.8 MB (152842860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa1a7d560fa80d378d794a75ccc4a2df1e3e7ddf6ef397787a4bc9189383cc38`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:00:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:00:37 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 03 Sep 2021 07:00:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 07:00:38 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Sep 2021 07:01:19 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 03 Sep 2021 07:01:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 03 Sep 2021 07:01:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cf10713026e0c75134ff3211c7f5385f2c4c544992d08b46a84fb3418a1a57`  
		Last Modified: Fri, 03 Sep 2021 07:03:57 GMT  
		Size: 4.5 MB (4458852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83704fc4fa73b4aba748725dcb4d27d4746e9ebcbc335b9090fa458e3edc9507`  
		Last Modified: Fri, 03 Sep 2021 07:04:57 GMT  
		Size: 121.2 MB (121238164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:1f2f7284c892ff11eea4667ef5444c1f888f73efa2357a3c2fe7e312ce55143e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138996814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a69e5f6723d79bad3780ba327234e113cf5d7aea99ea4fb8d5b19bde6b73d975`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:40 GMT
ADD file:4754bbccf4c59f77dd54f3888871f0635a2f9655cda53f50e63237f1580286e0 in / 
# Fri, 03 Sep 2021 01:00:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:02:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:02:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 03 Sep 2021 07:02:13 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 07:02:14 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Sep 2021 07:03:19 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 03 Sep 2021 07:03:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 03 Sep 2021 07:04:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2215ad7863d95c38f1f794f1d5b4d6c5ca4ca7e921e4bb7218b803f7ed270675`  
		Last Modified: Fri, 03 Sep 2021 01:16:23 GMT  
		Size: 22.7 MB (22746151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62658c2a7964a84f18d8c4baa82ecb94b63035d526b66a3c70092c4fb8ab392b`  
		Last Modified: Fri, 03 Sep 2021 07:07:49 GMT  
		Size: 3.8 MB (3806098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf1d8c4bfcf4fc4fbc06ff3f8ea6ff1a535667a38431105db711671da78ad4`  
		Last Modified: Fri, 03 Sep 2021 07:10:24 GMT  
		Size: 112.4 MB (112444565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:a11fa8ad8260a4377cb0addafbc60d92a864dc31f913398a16d9a155fabb64e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145412761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd5c1f359d6de9693fc683335e881581e8ff28bef6484e9c2f4e07c9acef9ccb`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:08:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:08:27 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 03 Sep 2021 04:08:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 04:08:28 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Sep 2021 04:09:02 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 03 Sep 2021 04:09:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 03 Sep 2021 04:09:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74f0afdeb041314bf07f654c5ad98c93ac4e458cf116d71b974bb8c37497d19`  
		Last Modified: Fri, 03 Sep 2021 04:11:08 GMT  
		Size: 4.3 MB (4339030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e5c526fa81dcc602377f203b409418914b824132b19b864c35d44ec614f18e`  
		Last Modified: Fri, 03 Sep 2021 04:12:07 GMT  
		Size: 115.2 MB (115158871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:d8d137549c5d01a6cf196b7436012991b62aaf1d952b5dae25fe6c981e206543
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151312662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b275d1430ce05e2974ed471f101d31a66b7a87ce2d4095ee32f7d66c12bd52e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:49:23 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 03 Sep 2021 01:49:23 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 01:49:23 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Sep 2021 01:49:56 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 03 Sep 2021 01:50:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 03 Sep 2021 01:50:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882724d438ad078694d63f99e810a933ef88a7123e243da22826c51fedd6526d`  
		Last Modified: Fri, 03 Sep 2021 01:52:48 GMT  
		Size: 4.6 MB (4610980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1395d6672b512b9f0ee705939e996b31c6582c5e4c7c0368c29f01f7ede3c1`  
		Last Modified: Fri, 03 Sep 2021 01:54:04 GMT  
		Size: 118.9 MB (118904169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; ppc64le

```console
$ docker pull julia@sha256:cce46284039293b46262a58b3ccb53edb538f22646b15dbe10f1b205f2c5f3e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142010578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af72e79428f27e1796ad6030c9cc0254e1832b2f9e8d20369be28d5243fca3ef`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:16:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:16:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 03 Sep 2021 08:16:41 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:16:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Sep 2021 08:18:48 GMT
ENV JULIA_VERSION=1.6.2
# Fri, 03 Sep 2021 08:20:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='3eb4b5775b0df1ad38f6c409e989501ab445c95bcb01ab02bd60f5bd1e823240' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='76229a04fc259c3d70a7bbf28f80c248f9891bd85d154df7cc67bcbdc3350c4f' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='fe487892b2e960698de467741330e0754b8ff80bb63b66c31451685be3f348cd' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='360f6ca9bb39eafda135ae0c943f9c336af843445e14aa5d60581433362ea286' ;; 		ppc64el) tarArch='ppc64le'; dirArch='ppc64le'; sha256='84c1c0aa3bbc229192e17d16d5da9d6bb0daa791a78dd40480b09528fb50648a' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 03 Sep 2021 08:20:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a54f94c4773f149e324c9485ac146a921c9f496490b95eaf3f2ad044038c1f`  
		Last Modified: Fri, 03 Sep 2021 08:21:17 GMT  
		Size: 4.9 MB (4854342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc9792ae633ab78f340f708e1ae6819fea98048006ecb49bd43f61272b93a22`  
		Last Modified: Fri, 03 Sep 2021 08:22:16 GMT  
		Size: 106.6 MB (106602561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
