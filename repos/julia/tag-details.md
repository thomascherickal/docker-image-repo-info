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
-	[`julia:1.3`](#julia13)
-	[`julia:1.3.0`](#julia130)
-	[`julia:1.3.0-buster`](#julia130-buster)
-	[`julia:1.3.0-stretch`](#julia130-stretch)
-	[`julia:1.3.0-windowsservercore-1809`](#julia130-windowsservercore-1809)
-	[`julia:1.3.0-windowsservercore-ltsc2016`](#julia130-windowsservercore-ltsc2016)
-	[`julia:1.3-buster`](#julia13-buster)
-	[`julia:1.3-stretch`](#julia13-stretch)
-	[`julia:1.3-windowsservercore-1809`](#julia13-windowsservercore-1809)
-	[`julia:1.3-windowsservercore-ltsc2016`](#julia13-windowsservercore-ltsc2016)
-	[`julia:1-buster`](#julia1-buster)
-	[`julia:1-stretch`](#julia1-stretch)
-	[`julia:1-windowsservercore-1809`](#julia1-windowsservercore-1809)
-	[`julia:1-windowsservercore-ltsc2016`](#julia1-windowsservercore-ltsc2016)
-	[`julia:buster`](#juliabuster)
-	[`julia:latest`](#julialatest)
-	[`julia:stretch`](#juliastretch)
-	[`julia:windowsservercore-1809`](#juliawindowsservercore-1809)
-	[`julia:windowsservercore-ltsc2016`](#juliawindowsservercore-ltsc2016)

## `julia:1`

```console
$ docker pull julia@sha256:7b3bfe95ca06e9fd46b7ec19006ca3f7f310c3a8466a12881feda7f53a92c7da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3384; amd64

### `julia:1` - linux; amd64

```console
$ docker pull julia@sha256:855bfbdbbd5cc5f3cbaf8ff9fed2164bb0dc21e0035103fa188cc854320b3fb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134425125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ff4467bc504928bc38c4e9e0e1de1c3155e963b2e4740d343626ee4ac083ce`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:47:56 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d01f17cc027422f21aec33ea176681d1efdab3bb4ef423122498c2717f5229`  
		Last Modified: Wed, 27 Nov 2019 02:49:24 GMT  
		Size: 102.9 MB (102895931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm variant v7

```console
$ docker pull julia@sha256:58c396546e8f7d0005cbee44eae1314c21d8f9d56626eb8d2440a86d4bc41044
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120037403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16eabdac133e6048c7b1d30677cd49a95c4bbb583dd1d8c30d9b5549a421847e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:22:27 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:23:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:23:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150e3a89eccb7cf1cae73035f9715d06ddb4c2318064947cec1095e34d2a919f`  
		Last Modified: Wed, 27 Nov 2019 02:25:18 GMT  
		Size: 93.6 MB (93554747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:55d301874a87f3a4e3b91e8ac915a7faa66785af5d806387a2138f633c032052
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116157611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae46a568bc821bd44bbd953136fb4f48db84130146ed5dee611a910a25bd8c2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:14:47 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:15:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:15:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045010ca5f3dcd227e5c1abfe431dede8fda3193218869802c57c82513a3a54`  
		Last Modified: Wed, 27 Nov 2019 02:17:36 GMT  
		Size: 86.0 MB (85991353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - linux; 386

```console
$ docker pull julia@sha256:bbd19a90620c29fecab83cbd6643bbfbed5d5faafa50905bd436ac5994c2ec5b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131293685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d434f2968499dd9f4ffde133fce692acd78e9704fa041349f35d13a5a1c5139d`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:23 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:55:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:55:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1cce47ac70f88ccd84583d12913fad10934ed8afdd006d22005aef3a47a297`  
		Last Modified: Wed, 27 Nov 2019 01:57:04 GMT  
		Size: 99.0 MB (98960687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:4466de07b40c1ccef59af3ba9657c9bd0860ae48a5c64905996975fd98c36c8f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5851253362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e052b93d9ffa13c50ad0cc5a1adf4bc81224f0ecb84bf49897c21f470ff7ba2e`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:12:36 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 11 Dec 2019 18:12:37 GMT
ENV JULIA_SHA256=35af4b93188b2404a78026b583c7f010ecb17df2eabb9fc32de4737de28f31d5
# Wed, 11 Dec 2019 18:16:16 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:16:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bb6a227a3e35a2ac1412d7ce1f6d1fe0eb9ffef54d7fd0d942eda6a4a9e844`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895110186ac4672791f3312f5bb04163342b724e9e41e75ef5a12770627e6f6a`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87adc6544f789d6c8a086e47e9cd0e80a1fae0c26a74b3bd0c4362a9ba35ce65`  
		Last Modified: Wed, 11 Dec 2019 18:21:07 GMT  
		Size: 128.5 MB (128544729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a92f8fb56b5bcfe5c53c100e5ce668116c15207c92ed840adea2f14a0d6d60`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0`

```console
$ docker pull julia@sha256:cd9687230a6aee67f815ec32683702d5d71e6296b28dc11f00fd53e49efdd629
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3384; amd64

### `julia:1.0` - linux; amd64

```console
$ docker pull julia@sha256:9ad03e08b013aba7545c650b07f6625a473b43493703256ec15adc30dc521718
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127092291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab11de873a86b43efb6eca09952dc0a83ee6c822352cbf0838a094fc82e8d098`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 01:31:04 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 01:31:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 01:31:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4ac886c21129aae1538fe03fe56a08f9d25cb9a764d5e46a1b211642777bfa`  
		Last Modified: Sat, 23 Nov 2019 01:34:51 GMT  
		Size: 95.6 MB (95563097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm variant v7

```console
$ docker pull julia@sha256:26d5f550695d03996bb248b4771c4de22269825c22c0a05ed1fe771d62f63657
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113611474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9946549ea87aa6c30084a85de270d269cbaa75c2865d05226b300310122ff70e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 23:56:27 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 23:57:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 23:57:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0f61767947e22241a04725d196ecf79fdf9f10c86ddb7d70cff1de5c3f4200`  
		Last Modified: Sat, 23 Nov 2019 00:01:55 GMT  
		Size: 87.1 MB (87128818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ad49213c7d02d60e1b94e6c0924d2c908ec16978b337904ff7e15ee566ff0d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110057200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e1b9b43fbfb0944b0d3234cc91624bcda3b7caec546bbad3d901c336764a10`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 21:27:47 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 21:28:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 21:28:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181021cf7d4653f524f321a824cabc51935ae15ce6e528aedc03972080adaad0`  
		Last Modified: Fri, 22 Nov 2019 21:33:44 GMT  
		Size: 79.9 MB (79890942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - linux; 386

```console
$ docker pull julia@sha256:f2b82bc66aabb9c89aa3f552b79b39871a1c4568ea757eb93edab657e393e990
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124831416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57efbc14982c588a8213ee52a0b952f187562aef97e9bad18e50a17fbdd0a4de`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 07:06:51 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 07:07:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 07:07:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a88ce4ba772edcc0f3518d33ea4d1ce83f76afdb0a30d3d5047122492f99fd5`  
		Last Modified: Sat, 23 Nov 2019 07:11:16 GMT  
		Size: 92.5 MB (92498418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:22c1172c453f7e8ece28df589d51aba5e944310e0508a122d6765bb2dcd64ab6
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5830478533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39bcfbbf3e14b1a47a6b7e64af57a1cc26f18ff7a43ece0782b5c46dc1964932`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:16:43 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Dec 2019 18:16:44 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Dec 2019 18:19:57 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:20:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6271ad885fd8f6f6b2c5bf12b7aabd7c1053b92ded7f6c61e327f3d0061a05e`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48577290f463573a8ae98f04345be40d3e4dca180941891e38ee32242e4a6eb8`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f901d6225921a001a0801691d9e87227172011596c1be7d06c8a8e32d8a8ba9`  
		Last Modified: Wed, 11 Dec 2019 18:22:22 GMT  
		Size: 107.8 MB (107769860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30160e9a65d581c999e8058ddc00ed106d4d121278a191aa344d45efacb27fd`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5`

```console
$ docker pull julia@sha256:cd9687230a6aee67f815ec32683702d5d71e6296b28dc11f00fd53e49efdd629
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3384; amd64

### `julia:1.0.5` - linux; amd64

```console
$ docker pull julia@sha256:9ad03e08b013aba7545c650b07f6625a473b43493703256ec15adc30dc521718
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127092291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab11de873a86b43efb6eca09952dc0a83ee6c822352cbf0838a094fc82e8d098`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 01:31:04 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 01:31:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 01:31:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4ac886c21129aae1538fe03fe56a08f9d25cb9a764d5e46a1b211642777bfa`  
		Last Modified: Sat, 23 Nov 2019 01:34:51 GMT  
		Size: 95.6 MB (95563097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm variant v7

```console
$ docker pull julia@sha256:26d5f550695d03996bb248b4771c4de22269825c22c0a05ed1fe771d62f63657
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113611474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9946549ea87aa6c30084a85de270d269cbaa75c2865d05226b300310122ff70e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 23:56:27 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 23:57:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 23:57:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0f61767947e22241a04725d196ecf79fdf9f10c86ddb7d70cff1de5c3f4200`  
		Last Modified: Sat, 23 Nov 2019 00:01:55 GMT  
		Size: 87.1 MB (87128818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ad49213c7d02d60e1b94e6c0924d2c908ec16978b337904ff7e15ee566ff0d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110057200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e1b9b43fbfb0944b0d3234cc91624bcda3b7caec546bbad3d901c336764a10`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 21:27:47 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 21:28:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 21:28:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181021cf7d4653f524f321a824cabc51935ae15ce6e528aedc03972080adaad0`  
		Last Modified: Fri, 22 Nov 2019 21:33:44 GMT  
		Size: 79.9 MB (79890942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - linux; 386

```console
$ docker pull julia@sha256:f2b82bc66aabb9c89aa3f552b79b39871a1c4568ea757eb93edab657e393e990
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124831416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57efbc14982c588a8213ee52a0b952f187562aef97e9bad18e50a17fbdd0a4de`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 07:06:51 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 07:07:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 07:07:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a88ce4ba772edcc0f3518d33ea4d1ce83f76afdb0a30d3d5047122492f99fd5`  
		Last Modified: Sat, 23 Nov 2019 07:11:16 GMT  
		Size: 92.5 MB (92498418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:22c1172c453f7e8ece28df589d51aba5e944310e0508a122d6765bb2dcd64ab6
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5830478533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39bcfbbf3e14b1a47a6b7e64af57a1cc26f18ff7a43ece0782b5c46dc1964932`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:16:43 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Dec 2019 18:16:44 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Dec 2019 18:19:57 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:20:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6271ad885fd8f6f6b2c5bf12b7aabd7c1053b92ded7f6c61e327f3d0061a05e`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48577290f463573a8ae98f04345be40d3e4dca180941891e38ee32242e4a6eb8`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f901d6225921a001a0801691d9e87227172011596c1be7d06c8a8e32d8a8ba9`  
		Last Modified: Wed, 11 Dec 2019 18:22:22 GMT  
		Size: 107.8 MB (107769860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30160e9a65d581c999e8058ddc00ed106d4d121278a191aa344d45efacb27fd`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-buster`

```console
$ docker pull julia@sha256:5821e82d27b94b05afc44e65620711fc66ee6c3dfa83b6f47e1f511d907d9261
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-buster` - linux; amd64

```console
$ docker pull julia@sha256:9ad03e08b013aba7545c650b07f6625a473b43493703256ec15adc30dc521718
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127092291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab11de873a86b43efb6eca09952dc0a83ee6c822352cbf0838a094fc82e8d098`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 01:31:04 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 01:31:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 01:31:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4ac886c21129aae1538fe03fe56a08f9d25cb9a764d5e46a1b211642777bfa`  
		Last Modified: Sat, 23 Nov 2019 01:34:51 GMT  
		Size: 95.6 MB (95563097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:26d5f550695d03996bb248b4771c4de22269825c22c0a05ed1fe771d62f63657
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113611474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9946549ea87aa6c30084a85de270d269cbaa75c2865d05226b300310122ff70e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 23:56:27 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 23:57:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 23:57:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0f61767947e22241a04725d196ecf79fdf9f10c86ddb7d70cff1de5c3f4200`  
		Last Modified: Sat, 23 Nov 2019 00:01:55 GMT  
		Size: 87.1 MB (87128818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ad49213c7d02d60e1b94e6c0924d2c908ec16978b337904ff7e15ee566ff0d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110057200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e1b9b43fbfb0944b0d3234cc91624bcda3b7caec546bbad3d901c336764a10`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 21:27:47 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 21:28:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 21:28:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181021cf7d4653f524f321a824cabc51935ae15ce6e528aedc03972080adaad0`  
		Last Modified: Fri, 22 Nov 2019 21:33:44 GMT  
		Size: 79.9 MB (79890942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-buster` - linux; 386

```console
$ docker pull julia@sha256:f2b82bc66aabb9c89aa3f552b79b39871a1c4568ea757eb93edab657e393e990
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124831416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57efbc14982c588a8213ee52a0b952f187562aef97e9bad18e50a17fbdd0a4de`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 07:06:51 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 07:07:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 07:07:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a88ce4ba772edcc0f3518d33ea4d1ce83f76afdb0a30d3d5047122492f99fd5`  
		Last Modified: Sat, 23 Nov 2019 07:11:16 GMT  
		Size: 92.5 MB (92498418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-stretch`

```console
$ docker pull julia@sha256:43a9bd790b0ea2d095f11f85ef548e954d93ca0a748274ef7241bb313570cdfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0.5-stretch` - linux; amd64

```console
$ docker pull julia@sha256:73404c4c5ea9c3e69e8aa48e2ad0f973432f4c2e02cd1ee230e21e60f345e2aa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150466521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c998c934a90a3ba399d48c89dc1be32b51461732d8ffa9a770a55685dfeb6b9e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:31:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:31:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:31:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:31:40 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 01:31:40 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 01:32:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 01:32:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd717a013904df6230ae874b6de22ddd7a5c72a8937eb48101a8cd7e82150ce`  
		Last Modified: Sat, 23 Nov 2019 01:34:58 GMT  
		Size: 9.5 MB (9511878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db18cbd2232f9b7eced61448700b0f2f20a6f824fd0e65051c701e27633b52f`  
		Last Modified: Sat, 23 Nov 2019 01:35:16 GMT  
		Size: 95.6 MB (95573884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:5bb00d407c1588fdb57240c6b3a5c3a57ba13ff1bf7481fd7042781c92d6ee97
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137481489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78b15a0bd29332164b84c19edc85397b29a9570ca38c18a17b2565b351971d47`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:27:54 GMT
ADD file:3893b8a7336301b4a2a741f62c99805c3c7b2bee21e4f026b6885060becfc03d in / 
# Fri, 22 Nov 2019 13:27:57 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:57:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:57:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:57:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:57:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 23:57:38 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 23:58:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 23:58:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fb827ed75ba2d760675c1e0dfd2cef27b5120725860abe8870ee3842dfce2a08`  
		Last Modified: Fri, 22 Nov 2019 13:36:40 GMT  
		Size: 42.1 MB (42108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b39760398ccb4ebaae39d52d7f424dfdf4b3adfe97ad9688fa2c23b0d1a2f99`  
		Last Modified: Sat, 23 Nov 2019 00:02:04 GMT  
		Size: 8.2 MB (8235504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598a57db8c616fb5dc94995c3ab06a6e9c37bb9e2e5b06cac4ac647ac11816b3`  
		Last Modified: Sat, 23 Nov 2019 00:02:30 GMT  
		Size: 87.1 MB (87137916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c5bc435613b9a4c87b310d640a57cfbd32d6ae69a94bfdf7d96157e7f4e36ea9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131550642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e447fae692ad894b5903db53c29e205b0f0f609823e2e8396faa4b0c761844f3`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:17 GMT
ADD file:ad8ecaf59c4f4c76dd6d93f5efff4420e3b55b36937eb36df317c7cd9ba19aeb in / 
# Fri, 22 Nov 2019 13:45:20 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:28:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:28:55 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:28:55 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:28:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 21:28:56 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 21:29:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 21:29:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c0d6add7f35c078f38df34ebc5a91afab0ba514167d17ad24fd4582eb0880bf4`  
		Last Modified: Fri, 22 Nov 2019 13:51:57 GMT  
		Size: 43.2 MB (43166306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514ccdd36eea60f0ca3c94a5a9f9f3d7e245449173314333e7fad1a25c8d8e93`  
		Last Modified: Fri, 22 Nov 2019 21:33:55 GMT  
		Size: 8.5 MB (8475026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c51eee54bffef83150b0a60a51e7a2d3098f57e2409a53e3a0f0ba86e56fbf`  
		Last Modified: Fri, 22 Nov 2019 21:34:16 GMT  
		Size: 79.9 MB (79909310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0.5-stretch` - linux; 386

```console
$ docker pull julia@sha256:3b183418189ca34005aaa5738856f0262601096ab8f43bebe3f0e14c62999b7d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148119402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd69c9afa049f8e38424ef08916699866ebb08c89e7c9a3159184202883c87c1`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:23 GMT
ADD file:5c01b74109a8b04410a939b8bd31367bdef970268befe81e02e43ddc646d79bc in / 
# Fri, 22 Nov 2019 16:54:23 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:07:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:07:27 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:07:27 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:07:27 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 07:07:27 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 07:07:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 07:07:48 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5940e26a4f3cd4f9002a93c11a8590498495bd0f4ce3fe102e4ddaf7c06d3a`  
		Last Modified: Fri, 22 Nov 2019 17:02:42 GMT  
		Size: 46.1 MB (46100192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d6ee381e95c963c3bf0743c0644c71078fd756b8fc6ddb2132430496ff1d6a`  
		Last Modified: Sat, 23 Nov 2019 07:11:24 GMT  
		Size: 9.5 MB (9517454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4781788224cde870f5168b50bb828407ee66a3522558b28c340cef92e092e0`  
		Last Modified: Sat, 23 Nov 2019 07:11:47 GMT  
		Size: 92.5 MB (92501756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0.5-windowsservercore-1809`

```console
$ docker pull julia@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `julia:1.0.5-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:7805ea8bb62c712345b06da3dc052d887654a15baeec33450cf1519e8ae3a5dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `julia:1.0.5-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:22c1172c453f7e8ece28df589d51aba5e944310e0508a122d6765bb2dcd64ab6
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5830478533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39bcfbbf3e14b1a47a6b7e64af57a1cc26f18ff7a43ece0782b5c46dc1964932`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:16:43 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Dec 2019 18:16:44 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Dec 2019 18:19:57 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:20:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6271ad885fd8f6f6b2c5bf12b7aabd7c1053b92ded7f6c61e327f3d0061a05e`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48577290f463573a8ae98f04345be40d3e4dca180941891e38ee32242e4a6eb8`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f901d6225921a001a0801691d9e87227172011596c1be7d06c8a8e32d8a8ba9`  
		Last Modified: Wed, 11 Dec 2019 18:22:22 GMT  
		Size: 107.8 MB (107769860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30160e9a65d581c999e8058ddc00ed106d4d121278a191aa344d45efacb27fd`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-buster`

```console
$ docker pull julia@sha256:5821e82d27b94b05afc44e65620711fc66ee6c3dfa83b6f47e1f511d907d9261
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:9ad03e08b013aba7545c650b07f6625a473b43493703256ec15adc30dc521718
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127092291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab11de873a86b43efb6eca09952dc0a83ee6c822352cbf0838a094fc82e8d098`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 01:31:04 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 01:31:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 01:31:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4ac886c21129aae1538fe03fe56a08f9d25cb9a764d5e46a1b211642777bfa`  
		Last Modified: Sat, 23 Nov 2019 01:34:51 GMT  
		Size: 95.6 MB (95563097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:26d5f550695d03996bb248b4771c4de22269825c22c0a05ed1fe771d62f63657
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113611474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9946549ea87aa6c30084a85de270d269cbaa75c2865d05226b300310122ff70e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 23:56:27 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 23:57:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 23:57:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0f61767947e22241a04725d196ecf79fdf9f10c86ddb7d70cff1de5c3f4200`  
		Last Modified: Sat, 23 Nov 2019 00:01:55 GMT  
		Size: 87.1 MB (87128818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:8ad49213c7d02d60e1b94e6c0924d2c908ec16978b337904ff7e15ee566ff0d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110057200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e1b9b43fbfb0944b0d3234cc91624bcda3b7caec546bbad3d901c336764a10`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 21:27:47 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 21:28:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 21:28:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181021cf7d4653f524f321a824cabc51935ae15ce6e528aedc03972080adaad0`  
		Last Modified: Fri, 22 Nov 2019 21:33:44 GMT  
		Size: 79.9 MB (79890942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-buster` - linux; 386

```console
$ docker pull julia@sha256:f2b82bc66aabb9c89aa3f552b79b39871a1c4568ea757eb93edab657e393e990
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124831416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57efbc14982c588a8213ee52a0b952f187562aef97e9bad18e50a17fbdd0a4de`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 07:06:51 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 07:07:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 07:07:10 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a88ce4ba772edcc0f3518d33ea4d1ce83f76afdb0a30d3d5047122492f99fd5`  
		Last Modified: Sat, 23 Nov 2019 07:11:16 GMT  
		Size: 92.5 MB (92498418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-stretch`

```console
$ docker pull julia@sha256:43a9bd790b0ea2d095f11f85ef548e954d93ca0a748274ef7241bb313570cdfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.0-stretch` - linux; amd64

```console
$ docker pull julia@sha256:73404c4c5ea9c3e69e8aa48e2ad0f973432f4c2e02cd1ee230e21e60f345e2aa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150466521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c998c934a90a3ba399d48c89dc1be32b51461732d8ffa9a770a55685dfeb6b9e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:31:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:31:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:31:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:31:40 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 01:31:40 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 01:32:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 01:32:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd717a013904df6230ae874b6de22ddd7a5c72a8937eb48101a8cd7e82150ce`  
		Last Modified: Sat, 23 Nov 2019 01:34:58 GMT  
		Size: 9.5 MB (9511878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db18cbd2232f9b7eced61448700b0f2f20a6f824fd0e65051c701e27633b52f`  
		Last Modified: Sat, 23 Nov 2019 01:35:16 GMT  
		Size: 95.6 MB (95573884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:5bb00d407c1588fdb57240c6b3a5c3a57ba13ff1bf7481fd7042781c92d6ee97
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137481489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78b15a0bd29332164b84c19edc85397b29a9570ca38c18a17b2565b351971d47`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:27:54 GMT
ADD file:3893b8a7336301b4a2a741f62c99805c3c7b2bee21e4f026b6885060becfc03d in / 
# Fri, 22 Nov 2019 13:27:57 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:57:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:57:36 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:57:37 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:57:37 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 23:57:38 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 23:58:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 23:58:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:fb827ed75ba2d760675c1e0dfd2cef27b5120725860abe8870ee3842dfce2a08`  
		Last Modified: Fri, 22 Nov 2019 13:36:40 GMT  
		Size: 42.1 MB (42108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b39760398ccb4ebaae39d52d7f424dfdf4b3adfe97ad9688fa2c23b0d1a2f99`  
		Last Modified: Sat, 23 Nov 2019 00:02:04 GMT  
		Size: 8.2 MB (8235504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598a57db8c616fb5dc94995c3ab06a6e9c37bb9e2e5b06cac4ac647ac11816b3`  
		Last Modified: Sat, 23 Nov 2019 00:02:30 GMT  
		Size: 87.1 MB (87137916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:c5bc435613b9a4c87b310d640a57cfbd32d6ae69a94bfdf7d96157e7f4e36ea9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131550642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e447fae692ad894b5903db53c29e205b0f0f609823e2e8396faa4b0c761844f3`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:17 GMT
ADD file:ad8ecaf59c4f4c76dd6d93f5efff4420e3b55b36937eb36df317c7cd9ba19aeb in / 
# Fri, 22 Nov 2019 13:45:20 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:28:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:28:55 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:28:55 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:28:56 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 22 Nov 2019 21:28:56 GMT
ENV JULIA_VERSION=1.0.5
# Fri, 22 Nov 2019 21:29:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Fri, 22 Nov 2019 21:29:26 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c0d6add7f35c078f38df34ebc5a91afab0ba514167d17ad24fd4582eb0880bf4`  
		Last Modified: Fri, 22 Nov 2019 13:51:57 GMT  
		Size: 43.2 MB (43166306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514ccdd36eea60f0ca3c94a5a9f9f3d7e245449173314333e7fad1a25c8d8e93`  
		Last Modified: Fri, 22 Nov 2019 21:33:55 GMT  
		Size: 8.5 MB (8475026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c51eee54bffef83150b0a60a51e7a2d3098f57e2409a53e3a0f0ba86e56fbf`  
		Last Modified: Fri, 22 Nov 2019 21:34:16 GMT  
		Size: 79.9 MB (79909310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.0-stretch` - linux; 386

```console
$ docker pull julia@sha256:3b183418189ca34005aaa5738856f0262601096ab8f43bebe3f0e14c62999b7d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148119402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd69c9afa049f8e38424ef08916699866ebb08c89e7c9a3159184202883c87c1`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:23 GMT
ADD file:5c01b74109a8b04410a939b8bd31367bdef970268befe81e02e43ddc646d79bc in / 
# Fri, 22 Nov 2019 16:54:23 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:07:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:07:27 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:07:27 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:07:27 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 23 Nov 2019 07:07:27 GMT
ENV JULIA_VERSION=1.0.5
# Sat, 23 Nov 2019 07:07:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9dedd613777ba6ebd8aee5796915ff50aa6188ea03ed143cb687fc2aefd76b03' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='cfb2712765db90f0e4fa27e57a88c6d994ebcf1781f8673ebb17b5df7962d0c5' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='41cea1336ed8861413bb945740e567360e26f241eb3e10b3bb0fccd25655ed28' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='67c8f31699b79df96ce95926a363cd24ffa5bb4d9a814e071b1e8c8ff33e5a8f' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Sat, 23 Nov 2019 07:07:48 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:0f5940e26a4f3cd4f9002a93c11a8590498495bd0f4ce3fe102e4ddaf7c06d3a`  
		Last Modified: Fri, 22 Nov 2019 17:02:42 GMT  
		Size: 46.1 MB (46100192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d6ee381e95c963c3bf0743c0644c71078fd756b8fc6ddb2132430496ff1d6a`  
		Last Modified: Sat, 23 Nov 2019 07:11:24 GMT  
		Size: 9.5 MB (9517454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4781788224cde870f5168b50bb828407ee66a3522558b28c340cef92e092e0`  
		Last Modified: Sat, 23 Nov 2019 07:11:47 GMT  
		Size: 92.5 MB (92501756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `julia:1.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:7805ea8bb62c712345b06da3dc052d887654a15baeec33450cf1519e8ae3a5dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `julia:1.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:22c1172c453f7e8ece28df589d51aba5e944310e0508a122d6765bb2dcd64ab6
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5830478533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39bcfbbf3e14b1a47a6b7e64af57a1cc26f18ff7a43ece0782b5c46dc1964932`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:16:43 GMT
ENV JULIA_VERSION=1.0.5
# Wed, 11 Dec 2019 18:16:44 GMT
ENV JULIA_SHA256=83c04bdc264e7ab87f4e22be9f3dff8c5a62a49c8edea6a0c85f4645d4cbac7a
# Wed, 11 Dec 2019 18:19:57 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:20:00 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6271ad885fd8f6f6b2c5bf12b7aabd7c1053b92ded7f6c61e327f3d0061a05e`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48577290f463573a8ae98f04345be40d3e4dca180941891e38ee32242e4a6eb8`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f901d6225921a001a0801691d9e87227172011596c1be7d06c8a8e32d8a8ba9`  
		Last Modified: Wed, 11 Dec 2019 18:22:22 GMT  
		Size: 107.8 MB (107769860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30160e9a65d581c999e8058ddc00ed106d4d121278a191aa344d45efacb27fd`  
		Last Modified: Wed, 11 Dec 2019 18:21:45 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3`

```console
$ docker pull julia@sha256:7b3bfe95ca06e9fd46b7ec19006ca3f7f310c3a8466a12881feda7f53a92c7da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3384; amd64

### `julia:1.3` - linux; amd64

```console
$ docker pull julia@sha256:855bfbdbbd5cc5f3cbaf8ff9fed2164bb0dc21e0035103fa188cc854320b3fb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134425125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ff4467bc504928bc38c4e9e0e1de1c3155e963b2e4740d343626ee4ac083ce`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:47:56 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d01f17cc027422f21aec33ea176681d1efdab3bb4ef423122498c2717f5229`  
		Last Modified: Wed, 27 Nov 2019 02:49:24 GMT  
		Size: 102.9 MB (102895931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3` - linux; arm variant v7

```console
$ docker pull julia@sha256:58c396546e8f7d0005cbee44eae1314c21d8f9d56626eb8d2440a86d4bc41044
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120037403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16eabdac133e6048c7b1d30677cd49a95c4bbb583dd1d8c30d9b5549a421847e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:22:27 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:23:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:23:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150e3a89eccb7cf1cae73035f9715d06ddb4c2318064947cec1095e34d2a919f`  
		Last Modified: Wed, 27 Nov 2019 02:25:18 GMT  
		Size: 93.6 MB (93554747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:55d301874a87f3a4e3b91e8ac915a7faa66785af5d806387a2138f633c032052
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116157611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae46a568bc821bd44bbd953136fb4f48db84130146ed5dee611a910a25bd8c2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:14:47 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:15:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:15:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045010ca5f3dcd227e5c1abfe431dede8fda3193218869802c57c82513a3a54`  
		Last Modified: Wed, 27 Nov 2019 02:17:36 GMT  
		Size: 86.0 MB (85991353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3` - linux; 386

```console
$ docker pull julia@sha256:bbd19a90620c29fecab83cbd6643bbfbed5d5faafa50905bd436ac5994c2ec5b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131293685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d434f2968499dd9f4ffde133fce692acd78e9704fa041349f35d13a5a1c5139d`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:23 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:55:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:55:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1cce47ac70f88ccd84583d12913fad10934ed8afdd006d22005aef3a47a297`  
		Last Modified: Wed, 27 Nov 2019 01:57:04 GMT  
		Size: 99.0 MB (98960687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:4466de07b40c1ccef59af3ba9657c9bd0860ae48a5c64905996975fd98c36c8f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5851253362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e052b93d9ffa13c50ad0cc5a1adf4bc81224f0ecb84bf49897c21f470ff7ba2e`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:12:36 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 11 Dec 2019 18:12:37 GMT
ENV JULIA_SHA256=35af4b93188b2404a78026b583c7f010ecb17df2eabb9fc32de4737de28f31d5
# Wed, 11 Dec 2019 18:16:16 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:16:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bb6a227a3e35a2ac1412d7ce1f6d1fe0eb9ffef54d7fd0d942eda6a4a9e844`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895110186ac4672791f3312f5bb04163342b724e9e41e75ef5a12770627e6f6a`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87adc6544f789d6c8a086e47e9cd0e80a1fae0c26a74b3bd0c4362a9ba35ce65`  
		Last Modified: Wed, 11 Dec 2019 18:21:07 GMT  
		Size: 128.5 MB (128544729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a92f8fb56b5bcfe5c53c100e5ce668116c15207c92ed840adea2f14a0d6d60`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3.0`

```console
$ docker pull julia@sha256:7b3bfe95ca06e9fd46b7ec19006ca3f7f310c3a8466a12881feda7f53a92c7da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3384; amd64

### `julia:1.3.0` - linux; amd64

```console
$ docker pull julia@sha256:855bfbdbbd5cc5f3cbaf8ff9fed2164bb0dc21e0035103fa188cc854320b3fb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134425125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ff4467bc504928bc38c4e9e0e1de1c3155e963b2e4740d343626ee4ac083ce`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:47:56 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d01f17cc027422f21aec33ea176681d1efdab3bb4ef423122498c2717f5229`  
		Last Modified: Wed, 27 Nov 2019 02:49:24 GMT  
		Size: 102.9 MB (102895931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.0` - linux; arm variant v7

```console
$ docker pull julia@sha256:58c396546e8f7d0005cbee44eae1314c21d8f9d56626eb8d2440a86d4bc41044
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120037403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16eabdac133e6048c7b1d30677cd49a95c4bbb583dd1d8c30d9b5549a421847e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:22:27 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:23:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:23:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150e3a89eccb7cf1cae73035f9715d06ddb4c2318064947cec1095e34d2a919f`  
		Last Modified: Wed, 27 Nov 2019 02:25:18 GMT  
		Size: 93.6 MB (93554747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.0` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:55d301874a87f3a4e3b91e8ac915a7faa66785af5d806387a2138f633c032052
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116157611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae46a568bc821bd44bbd953136fb4f48db84130146ed5dee611a910a25bd8c2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:14:47 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:15:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:15:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045010ca5f3dcd227e5c1abfe431dede8fda3193218869802c57c82513a3a54`  
		Last Modified: Wed, 27 Nov 2019 02:17:36 GMT  
		Size: 86.0 MB (85991353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.0` - linux; 386

```console
$ docker pull julia@sha256:bbd19a90620c29fecab83cbd6643bbfbed5d5faafa50905bd436ac5994c2ec5b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131293685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d434f2968499dd9f4ffde133fce692acd78e9704fa041349f35d13a5a1c5139d`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:23 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:55:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:55:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1cce47ac70f88ccd84583d12913fad10934ed8afdd006d22005aef3a47a297`  
		Last Modified: Wed, 27 Nov 2019 01:57:04 GMT  
		Size: 99.0 MB (98960687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.0` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:4466de07b40c1ccef59af3ba9657c9bd0860ae48a5c64905996975fd98c36c8f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5851253362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e052b93d9ffa13c50ad0cc5a1adf4bc81224f0ecb84bf49897c21f470ff7ba2e`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:12:36 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 11 Dec 2019 18:12:37 GMT
ENV JULIA_SHA256=35af4b93188b2404a78026b583c7f010ecb17df2eabb9fc32de4737de28f31d5
# Wed, 11 Dec 2019 18:16:16 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:16:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bb6a227a3e35a2ac1412d7ce1f6d1fe0eb9ffef54d7fd0d942eda6a4a9e844`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895110186ac4672791f3312f5bb04163342b724e9e41e75ef5a12770627e6f6a`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87adc6544f789d6c8a086e47e9cd0e80a1fae0c26a74b3bd0c4362a9ba35ce65`  
		Last Modified: Wed, 11 Dec 2019 18:21:07 GMT  
		Size: 128.5 MB (128544729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a92f8fb56b5bcfe5c53c100e5ce668116c15207c92ed840adea2f14a0d6d60`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3.0-buster`

```console
$ docker pull julia@sha256:f58fa348609fd9cf10359792b1241365bc14390490c598c557b8e23108b31a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.3.0-buster` - linux; amd64

```console
$ docker pull julia@sha256:855bfbdbbd5cc5f3cbaf8ff9fed2164bb0dc21e0035103fa188cc854320b3fb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134425125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ff4467bc504928bc38c4e9e0e1de1c3155e963b2e4740d343626ee4ac083ce`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:47:56 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d01f17cc027422f21aec33ea176681d1efdab3bb4ef423122498c2717f5229`  
		Last Modified: Wed, 27 Nov 2019 02:49:24 GMT  
		Size: 102.9 MB (102895931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.0-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:58c396546e8f7d0005cbee44eae1314c21d8f9d56626eb8d2440a86d4bc41044
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120037403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16eabdac133e6048c7b1d30677cd49a95c4bbb583dd1d8c30d9b5549a421847e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:22:27 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:23:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:23:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150e3a89eccb7cf1cae73035f9715d06ddb4c2318064947cec1095e34d2a919f`  
		Last Modified: Wed, 27 Nov 2019 02:25:18 GMT  
		Size: 93.6 MB (93554747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.0-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:55d301874a87f3a4e3b91e8ac915a7faa66785af5d806387a2138f633c032052
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116157611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae46a568bc821bd44bbd953136fb4f48db84130146ed5dee611a910a25bd8c2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:14:47 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:15:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:15:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045010ca5f3dcd227e5c1abfe431dede8fda3193218869802c57c82513a3a54`  
		Last Modified: Wed, 27 Nov 2019 02:17:36 GMT  
		Size: 86.0 MB (85991353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.0-buster` - linux; 386

```console
$ docker pull julia@sha256:bbd19a90620c29fecab83cbd6643bbfbed5d5faafa50905bd436ac5994c2ec5b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131293685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d434f2968499dd9f4ffde133fce692acd78e9704fa041349f35d13a5a1c5139d`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:23 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:55:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:55:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1cce47ac70f88ccd84583d12913fad10934ed8afdd006d22005aef3a47a297`  
		Last Modified: Wed, 27 Nov 2019 01:57:04 GMT  
		Size: 99.0 MB (98960687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3.0-stretch`

```console
$ docker pull julia@sha256:62dd3e54b72b91579a3a3c47abac8c3e1c4c650870e6d36b014ab55f3dddfab6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.3.0-stretch` - linux; amd64

```console
$ docker pull julia@sha256:3b3d8b12fd4e4651f1f4fcb2f509bedb460efd90d6ec80621599f5826c7bc5ad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.0 MB (132968291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc66946c2f9a9f577616099d7940bdc7a2ece67de840b3fc220247ff698cb474`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:48:20 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaedd87a38ec22b96ab4effc5c4424e4b77a803a72b4ddb0161f5f9a19a9b83`  
		Last Modified: Sat, 23 Nov 2019 01:33:03 GMT  
		Size: 7.6 MB (7555516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0c10e0170e5622c7fbf906bc9d2ef71ed34623ff9e9b08370d56e59f314897`  
		Last Modified: Wed, 27 Nov 2019 02:49:49 GMT  
		Size: 102.9 MB (102888203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.0-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:91af6770b199cbbc68cca5694d05921abd7f1a188120c91f992911899d407343
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119163171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f503dd2a573a76cc88b828e38ad9b5ea48795272dbab3aecad6fc56479de45f`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:28:28 GMT
ADD file:9fcbe16260f606fbea9a4811e693312434fbc4b300e974d33dcac84808f2323c in / 
# Fri, 22 Nov 2019 13:28:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:54:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:54:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:54:15 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:23:31 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:24:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:24:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d721220e5446968b6d6c8c3cd477d7deaadfd7f3ea7070342828f151408cbc93`  
		Last Modified: Fri, 22 Nov 2019 13:36:57 GMT  
		Size: 19.3 MB (19311578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18c33863683af64036006c88f0c10de16277a86e0b64377395dc562229459db`  
		Last Modified: Fri, 22 Nov 2019 23:59:23 GMT  
		Size: 6.3 MB (6292069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38492a6a3562f22c872fe1d132133268e0865c7e7c40a82bcd3717085388de4`  
		Last Modified: Wed, 27 Nov 2019 02:26:00 GMT  
		Size: 93.6 MB (93559524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.0-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:941a65e5fcae3f19414eb77024f9c5b0f56a7ab7095949dc26f0efac8ffc7063
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.9 MB (112909753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c42f11c3a72c2a3c1a087684e203dea7ede550f456d7cb8bcbeb3758b1bd5ab`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:25:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:15:52 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:16:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:16:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d607c5cf53fc2fd360b3b9db3ec4f913a3464c9638a99792a4773eb8747897f`  
		Last Modified: Fri, 22 Nov 2019 21:30:36 GMT  
		Size: 6.5 MB (6526773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5421be62477a6f10881a9300a993af4a45a56462518f608090af6fab3a82e0`  
		Last Modified: Wed, 27 Nov 2019 02:18:13 GMT  
		Size: 86.0 MB (85997221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3.0-stretch` - linux; 386

```console
$ docker pull julia@sha256:dbb14be9b1d9fff64e0168a478d5cb78db80886aff5f2d06816bed18456fcb59
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129699923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c385dbc091479a349913c9dc921da40d38b67b57afc097489117c574ff9bdd5`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:05:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:05:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:05:28 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:51 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:56:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:56:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3add3465288c564759514e6470533c98709e4eb220ecc997d63cf40d0b38f05f`  
		Last Modified: Sat, 23 Nov 2019 07:08:45 GMT  
		Size: 7.6 MB (7582351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10d4a74ea93b5c5847256f5589a9666625162ffe17bfef1187878cfb978a299`  
		Last Modified: Wed, 27 Nov 2019 01:57:49 GMT  
		Size: 99.0 MB (98965502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3.0-windowsservercore-1809`

```console
$ docker pull julia@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `julia:1.3.0-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:fcc13ec2a4deabaf456332de57a4deb15d8de966d654c531dc259215595aa7a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `julia:1.3.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:4466de07b40c1ccef59af3ba9657c9bd0860ae48a5c64905996975fd98c36c8f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5851253362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e052b93d9ffa13c50ad0cc5a1adf4bc81224f0ecb84bf49897c21f470ff7ba2e`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:12:36 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 11 Dec 2019 18:12:37 GMT
ENV JULIA_SHA256=35af4b93188b2404a78026b583c7f010ecb17df2eabb9fc32de4737de28f31d5
# Wed, 11 Dec 2019 18:16:16 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:16:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bb6a227a3e35a2ac1412d7ce1f6d1fe0eb9ffef54d7fd0d942eda6a4a9e844`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895110186ac4672791f3312f5bb04163342b724e9e41e75ef5a12770627e6f6a`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87adc6544f789d6c8a086e47e9cd0e80a1fae0c26a74b3bd0c4362a9ba35ce65`  
		Last Modified: Wed, 11 Dec 2019 18:21:07 GMT  
		Size: 128.5 MB (128544729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a92f8fb56b5bcfe5c53c100e5ce668116c15207c92ed840adea2f14a0d6d60`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3-buster`

```console
$ docker pull julia@sha256:f58fa348609fd9cf10359792b1241365bc14390490c598c557b8e23108b31a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.3-buster` - linux; amd64

```console
$ docker pull julia@sha256:855bfbdbbd5cc5f3cbaf8ff9fed2164bb0dc21e0035103fa188cc854320b3fb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134425125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ff4467bc504928bc38c4e9e0e1de1c3155e963b2e4740d343626ee4ac083ce`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:47:56 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d01f17cc027422f21aec33ea176681d1efdab3bb4ef423122498c2717f5229`  
		Last Modified: Wed, 27 Nov 2019 02:49:24 GMT  
		Size: 102.9 MB (102895931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:58c396546e8f7d0005cbee44eae1314c21d8f9d56626eb8d2440a86d4bc41044
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120037403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16eabdac133e6048c7b1d30677cd49a95c4bbb583dd1d8c30d9b5549a421847e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:22:27 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:23:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:23:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150e3a89eccb7cf1cae73035f9715d06ddb4c2318064947cec1095e34d2a919f`  
		Last Modified: Wed, 27 Nov 2019 02:25:18 GMT  
		Size: 93.6 MB (93554747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:55d301874a87f3a4e3b91e8ac915a7faa66785af5d806387a2138f633c032052
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116157611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae46a568bc821bd44bbd953136fb4f48db84130146ed5dee611a910a25bd8c2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:14:47 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:15:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:15:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045010ca5f3dcd227e5c1abfe431dede8fda3193218869802c57c82513a3a54`  
		Last Modified: Wed, 27 Nov 2019 02:17:36 GMT  
		Size: 86.0 MB (85991353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-buster` - linux; 386

```console
$ docker pull julia@sha256:bbd19a90620c29fecab83cbd6643bbfbed5d5faafa50905bd436ac5994c2ec5b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131293685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d434f2968499dd9f4ffde133fce692acd78e9704fa041349f35d13a5a1c5139d`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:23 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:55:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:55:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1cce47ac70f88ccd84583d12913fad10934ed8afdd006d22005aef3a47a297`  
		Last Modified: Wed, 27 Nov 2019 01:57:04 GMT  
		Size: 99.0 MB (98960687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3-stretch`

```console
$ docker pull julia@sha256:62dd3e54b72b91579a3a3c47abac8c3e1c4c650870e6d36b014ab55f3dddfab6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1.3-stretch` - linux; amd64

```console
$ docker pull julia@sha256:3b3d8b12fd4e4651f1f4fcb2f509bedb460efd90d6ec80621599f5826c7bc5ad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.0 MB (132968291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc66946c2f9a9f577616099d7940bdc7a2ece67de840b3fc220247ff698cb474`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:48:20 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaedd87a38ec22b96ab4effc5c4424e4b77a803a72b4ddb0161f5f9a19a9b83`  
		Last Modified: Sat, 23 Nov 2019 01:33:03 GMT  
		Size: 7.6 MB (7555516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0c10e0170e5622c7fbf906bc9d2ef71ed34623ff9e9b08370d56e59f314897`  
		Last Modified: Wed, 27 Nov 2019 02:49:49 GMT  
		Size: 102.9 MB (102888203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:91af6770b199cbbc68cca5694d05921abd7f1a188120c91f992911899d407343
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119163171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f503dd2a573a76cc88b828e38ad9b5ea48795272dbab3aecad6fc56479de45f`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:28:28 GMT
ADD file:9fcbe16260f606fbea9a4811e693312434fbc4b300e974d33dcac84808f2323c in / 
# Fri, 22 Nov 2019 13:28:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:54:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:54:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:54:15 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:23:31 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:24:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:24:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d721220e5446968b6d6c8c3cd477d7deaadfd7f3ea7070342828f151408cbc93`  
		Last Modified: Fri, 22 Nov 2019 13:36:57 GMT  
		Size: 19.3 MB (19311578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18c33863683af64036006c88f0c10de16277a86e0b64377395dc562229459db`  
		Last Modified: Fri, 22 Nov 2019 23:59:23 GMT  
		Size: 6.3 MB (6292069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38492a6a3562f22c872fe1d132133268e0865c7e7c40a82bcd3717085388de4`  
		Last Modified: Wed, 27 Nov 2019 02:26:00 GMT  
		Size: 93.6 MB (93559524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:941a65e5fcae3f19414eb77024f9c5b0f56a7ab7095949dc26f0efac8ffc7063
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.9 MB (112909753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c42f11c3a72c2a3c1a087684e203dea7ede550f456d7cb8bcbeb3758b1bd5ab`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:25:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:15:52 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:16:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:16:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d607c5cf53fc2fd360b3b9db3ec4f913a3464c9638a99792a4773eb8747897f`  
		Last Modified: Fri, 22 Nov 2019 21:30:36 GMT  
		Size: 6.5 MB (6526773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5421be62477a6f10881a9300a993af4a45a56462518f608090af6fab3a82e0`  
		Last Modified: Wed, 27 Nov 2019 02:18:13 GMT  
		Size: 86.0 MB (85997221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1.3-stretch` - linux; 386

```console
$ docker pull julia@sha256:dbb14be9b1d9fff64e0168a478d5cb78db80886aff5f2d06816bed18456fcb59
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129699923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c385dbc091479a349913c9dc921da40d38b67b57afc097489117c574ff9bdd5`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:05:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:05:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:05:28 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:51 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:56:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:56:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3add3465288c564759514e6470533c98709e4eb220ecc997d63cf40d0b38f05f`  
		Last Modified: Sat, 23 Nov 2019 07:08:45 GMT  
		Size: 7.6 MB (7582351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10d4a74ea93b5c5847256f5589a9666625162ffe17bfef1187878cfb978a299`  
		Last Modified: Wed, 27 Nov 2019 01:57:49 GMT  
		Size: 99.0 MB (98965502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1.3-windowsservercore-1809`

```console
$ docker pull julia@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `julia:1.3-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:fcc13ec2a4deabaf456332de57a4deb15d8de966d654c531dc259215595aa7a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `julia:1.3-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:4466de07b40c1ccef59af3ba9657c9bd0860ae48a5c64905996975fd98c36c8f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5851253362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e052b93d9ffa13c50ad0cc5a1adf4bc81224f0ecb84bf49897c21f470ff7ba2e`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:12:36 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 11 Dec 2019 18:12:37 GMT
ENV JULIA_SHA256=35af4b93188b2404a78026b583c7f010ecb17df2eabb9fc32de4737de28f31d5
# Wed, 11 Dec 2019 18:16:16 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:16:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bb6a227a3e35a2ac1412d7ce1f6d1fe0eb9ffef54d7fd0d942eda6a4a9e844`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895110186ac4672791f3312f5bb04163342b724e9e41e75ef5a12770627e6f6a`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87adc6544f789d6c8a086e47e9cd0e80a1fae0c26a74b3bd0c4362a9ba35ce65`  
		Last Modified: Wed, 11 Dec 2019 18:21:07 GMT  
		Size: 128.5 MB (128544729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a92f8fb56b5bcfe5c53c100e5ce668116c15207c92ed840adea2f14a0d6d60`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-buster`

```console
$ docker pull julia@sha256:f58fa348609fd9cf10359792b1241365bc14390490c598c557b8e23108b31a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-buster` - linux; amd64

```console
$ docker pull julia@sha256:855bfbdbbd5cc5f3cbaf8ff9fed2164bb0dc21e0035103fa188cc854320b3fb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134425125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ff4467bc504928bc38c4e9e0e1de1c3155e963b2e4740d343626ee4ac083ce`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:47:56 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d01f17cc027422f21aec33ea176681d1efdab3bb4ef423122498c2717f5229`  
		Last Modified: Wed, 27 Nov 2019 02:49:24 GMT  
		Size: 102.9 MB (102895931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:58c396546e8f7d0005cbee44eae1314c21d8f9d56626eb8d2440a86d4bc41044
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120037403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16eabdac133e6048c7b1d30677cd49a95c4bbb583dd1d8c30d9b5549a421847e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:22:27 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:23:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:23:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150e3a89eccb7cf1cae73035f9715d06ddb4c2318064947cec1095e34d2a919f`  
		Last Modified: Wed, 27 Nov 2019 02:25:18 GMT  
		Size: 93.6 MB (93554747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:55d301874a87f3a4e3b91e8ac915a7faa66785af5d806387a2138f633c032052
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116157611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae46a568bc821bd44bbd953136fb4f48db84130146ed5dee611a910a25bd8c2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:14:47 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:15:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:15:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045010ca5f3dcd227e5c1abfe431dede8fda3193218869802c57c82513a3a54`  
		Last Modified: Wed, 27 Nov 2019 02:17:36 GMT  
		Size: 86.0 MB (85991353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-buster` - linux; 386

```console
$ docker pull julia@sha256:bbd19a90620c29fecab83cbd6643bbfbed5d5faafa50905bd436ac5994c2ec5b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131293685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d434f2968499dd9f4ffde133fce692acd78e9704fa041349f35d13a5a1c5139d`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:23 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:55:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:55:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1cce47ac70f88ccd84583d12913fad10934ed8afdd006d22005aef3a47a297`  
		Last Modified: Wed, 27 Nov 2019 01:57:04 GMT  
		Size: 99.0 MB (98960687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-stretch`

```console
$ docker pull julia@sha256:62dd3e54b72b91579a3a3c47abac8c3e1c4c650870e6d36b014ab55f3dddfab6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:1-stretch` - linux; amd64

```console
$ docker pull julia@sha256:3b3d8b12fd4e4651f1f4fcb2f509bedb460efd90d6ec80621599f5826c7bc5ad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.0 MB (132968291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc66946c2f9a9f577616099d7940bdc7a2ece67de840b3fc220247ff698cb474`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:48:20 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaedd87a38ec22b96ab4effc5c4424e4b77a803a72b4ddb0161f5f9a19a9b83`  
		Last Modified: Sat, 23 Nov 2019 01:33:03 GMT  
		Size: 7.6 MB (7555516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0c10e0170e5622c7fbf906bc9d2ef71ed34623ff9e9b08370d56e59f314897`  
		Last Modified: Wed, 27 Nov 2019 02:49:49 GMT  
		Size: 102.9 MB (102888203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:91af6770b199cbbc68cca5694d05921abd7f1a188120c91f992911899d407343
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119163171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f503dd2a573a76cc88b828e38ad9b5ea48795272dbab3aecad6fc56479de45f`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:28:28 GMT
ADD file:9fcbe16260f606fbea9a4811e693312434fbc4b300e974d33dcac84808f2323c in / 
# Fri, 22 Nov 2019 13:28:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:54:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:54:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:54:15 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:23:31 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:24:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:24:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d721220e5446968b6d6c8c3cd477d7deaadfd7f3ea7070342828f151408cbc93`  
		Last Modified: Fri, 22 Nov 2019 13:36:57 GMT  
		Size: 19.3 MB (19311578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18c33863683af64036006c88f0c10de16277a86e0b64377395dc562229459db`  
		Last Modified: Fri, 22 Nov 2019 23:59:23 GMT  
		Size: 6.3 MB (6292069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38492a6a3562f22c872fe1d132133268e0865c7e7c40a82bcd3717085388de4`  
		Last Modified: Wed, 27 Nov 2019 02:26:00 GMT  
		Size: 93.6 MB (93559524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:941a65e5fcae3f19414eb77024f9c5b0f56a7ab7095949dc26f0efac8ffc7063
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.9 MB (112909753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c42f11c3a72c2a3c1a087684e203dea7ede550f456d7cb8bcbeb3758b1bd5ab`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:25:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:15:52 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:16:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:16:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d607c5cf53fc2fd360b3b9db3ec4f913a3464c9638a99792a4773eb8747897f`  
		Last Modified: Fri, 22 Nov 2019 21:30:36 GMT  
		Size: 6.5 MB (6526773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5421be62477a6f10881a9300a993af4a45a56462518f608090af6fab3a82e0`  
		Last Modified: Wed, 27 Nov 2019 02:18:13 GMT  
		Size: 86.0 MB (85997221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:1-stretch` - linux; 386

```console
$ docker pull julia@sha256:dbb14be9b1d9fff64e0168a478d5cb78db80886aff5f2d06816bed18456fcb59
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129699923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c385dbc091479a349913c9dc921da40d38b67b57afc097489117c574ff9bdd5`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:05:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:05:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:05:28 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:51 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:56:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:56:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3add3465288c564759514e6470533c98709e4eb220ecc997d63cf40d0b38f05f`  
		Last Modified: Sat, 23 Nov 2019 07:08:45 GMT  
		Size: 7.6 MB (7582351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10d4a74ea93b5c5847256f5589a9666625162ffe17bfef1187878cfb978a299`  
		Last Modified: Wed, 27 Nov 2019 01:57:49 GMT  
		Size: 99.0 MB (98965502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `julia:1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:fcc13ec2a4deabaf456332de57a4deb15d8de966d654c531dc259215595aa7a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `julia:1-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:4466de07b40c1ccef59af3ba9657c9bd0860ae48a5c64905996975fd98c36c8f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5851253362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e052b93d9ffa13c50ad0cc5a1adf4bc81224f0ecb84bf49897c21f470ff7ba2e`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:12:36 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 11 Dec 2019 18:12:37 GMT
ENV JULIA_SHA256=35af4b93188b2404a78026b583c7f010ecb17df2eabb9fc32de4737de28f31d5
# Wed, 11 Dec 2019 18:16:16 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:16:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bb6a227a3e35a2ac1412d7ce1f6d1fe0eb9ffef54d7fd0d942eda6a4a9e844`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895110186ac4672791f3312f5bb04163342b724e9e41e75ef5a12770627e6f6a`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87adc6544f789d6c8a086e47e9cd0e80a1fae0c26a74b3bd0c4362a9ba35ce65`  
		Last Modified: Wed, 11 Dec 2019 18:21:07 GMT  
		Size: 128.5 MB (128544729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a92f8fb56b5bcfe5c53c100e5ce668116c15207c92ed840adea2f14a0d6d60`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:buster`

```console
$ docker pull julia@sha256:f58fa348609fd9cf10359792b1241365bc14390490c598c557b8e23108b31a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:855bfbdbbd5cc5f3cbaf8ff9fed2164bb0dc21e0035103fa188cc854320b3fb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134425125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ff4467bc504928bc38c4e9e0e1de1c3155e963b2e4740d343626ee4ac083ce`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:47:56 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d01f17cc027422f21aec33ea176681d1efdab3bb4ef423122498c2717f5229`  
		Last Modified: Wed, 27 Nov 2019 02:49:24 GMT  
		Size: 102.9 MB (102895931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:58c396546e8f7d0005cbee44eae1314c21d8f9d56626eb8d2440a86d4bc41044
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120037403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16eabdac133e6048c7b1d30677cd49a95c4bbb583dd1d8c30d9b5549a421847e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:22:27 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:23:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:23:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150e3a89eccb7cf1cae73035f9715d06ddb4c2318064947cec1095e34d2a919f`  
		Last Modified: Wed, 27 Nov 2019 02:25:18 GMT  
		Size: 93.6 MB (93554747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:55d301874a87f3a4e3b91e8ac915a7faa66785af5d806387a2138f633c032052
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116157611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae46a568bc821bd44bbd953136fb4f48db84130146ed5dee611a910a25bd8c2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:14:47 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:15:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:15:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045010ca5f3dcd227e5c1abfe431dede8fda3193218869802c57c82513a3a54`  
		Last Modified: Wed, 27 Nov 2019 02:17:36 GMT  
		Size: 86.0 MB (85991353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:bbd19a90620c29fecab83cbd6643bbfbed5d5faafa50905bd436ac5994c2ec5b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131293685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d434f2968499dd9f4ffde133fce692acd78e9704fa041349f35d13a5a1c5139d`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:23 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:55:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:55:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1cce47ac70f88ccd84583d12913fad10934ed8afdd006d22005aef3a47a297`  
		Last Modified: Wed, 27 Nov 2019 01:57:04 GMT  
		Size: 99.0 MB (98960687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:latest`

```console
$ docker pull julia@sha256:7b3bfe95ca06e9fd46b7ec19006ca3f7f310c3a8466a12881feda7f53a92c7da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.14393.3384; amd64

### `julia:latest` - linux; amd64

```console
$ docker pull julia@sha256:855bfbdbbd5cc5f3cbaf8ff9fed2164bb0dc21e0035103fa188cc854320b3fb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134425125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ff4467bc504928bc38c4e9e0e1de1c3155e963b2e4740d343626ee4ac083ce`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:47:56 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf7370ec9cf6dd32e21f979f25a7484f0bc1af5e22af8d4063f783bbd1e7be`  
		Last Modified: Sat, 23 Nov 2019 01:32:27 GMT  
		Size: 4.4 MB (4436540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d01f17cc027422f21aec33ea176681d1efdab3bb4ef423122498c2717f5229`  
		Last Modified: Wed, 27 Nov 2019 02:49:24 GMT  
		Size: 102.9 MB (102895931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm variant v7

```console
$ docker pull julia@sha256:58c396546e8f7d0005cbee44eae1314c21d8f9d56626eb8d2440a86d4bc41044
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120037403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16eabdac133e6048c7b1d30677cd49a95c4bbb583dd1d8c30d9b5549a421847e`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:53:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:53:05 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:53:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:53:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:22:27 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:23:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:23:23 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6f78638d63b84e65a5f75357e3cdcff753023b3685213651477ca68a5a892`  
		Last Modified: Fri, 22 Nov 2019 23:58:38 GMT  
		Size: 3.8 MB (3783603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150e3a89eccb7cf1cae73035f9715d06ddb4c2318064947cec1095e34d2a919f`  
		Last Modified: Wed, 27 Nov 2019 02:25:18 GMT  
		Size: 93.6 MB (93554747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:55d301874a87f3a4e3b91e8ac915a7faa66785af5d806387a2138f633c032052
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116157611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae46a568bc821bd44bbd953136fb4f48db84130146ed5dee611a910a25bd8c2`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:24:32 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:24:33 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:24:35 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:14:47 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:15:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:15:37 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbe62516314248297d1613ea61c38305f5e6a36196a17280158d9738d2883`  
		Last Modified: Fri, 22 Nov 2019 21:30:07 GMT  
		Size: 4.3 MB (4315456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6045010ca5f3dcd227e5c1abfe431dede8fda3193218869802c57c82513a3a54`  
		Last Modified: Wed, 27 Nov 2019 02:17:36 GMT  
		Size: 86.0 MB (85991353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - linux; 386

```console
$ docker pull julia@sha256:bbd19a90620c29fecab83cbd6643bbfbed5d5faafa50905bd436ac5994c2ec5b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131293685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d434f2968499dd9f4ffde133fce692acd78e9704fa041349f35d13a5a1c5139d`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:04:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:04:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:04:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:04:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:23 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:55:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:55:46 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d44d8c03d6f82d00a5e5b2dc75e39b34f145e796595d0f3a2a304ac7c53a53`  
		Last Modified: Sat, 23 Nov 2019 07:08:11 GMT  
		Size: 4.6 MB (4586238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1cce47ac70f88ccd84583d12913fad10934ed8afdd006d22005aef3a47a297`  
		Last Modified: Wed, 27 Nov 2019 01:57:04 GMT  
		Size: 99.0 MB (98960687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:latest` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:4466de07b40c1ccef59af3ba9657c9bd0860ae48a5c64905996975fd98c36c8f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5851253362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e052b93d9ffa13c50ad0cc5a1adf4bc81224f0ecb84bf49897c21f470ff7ba2e`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:12:36 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 11 Dec 2019 18:12:37 GMT
ENV JULIA_SHA256=35af4b93188b2404a78026b583c7f010ecb17df2eabb9fc32de4737de28f31d5
# Wed, 11 Dec 2019 18:16:16 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:16:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bb6a227a3e35a2ac1412d7ce1f6d1fe0eb9ffef54d7fd0d942eda6a4a9e844`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895110186ac4672791f3312f5bb04163342b724e9e41e75ef5a12770627e6f6a`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87adc6544f789d6c8a086e47e9cd0e80a1fae0c26a74b3bd0c4362a9ba35ce65`  
		Last Modified: Wed, 11 Dec 2019 18:21:07 GMT  
		Size: 128.5 MB (128544729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a92f8fb56b5bcfe5c53c100e5ce668116c15207c92ed840adea2f14a0d6d60`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:stretch`

```console
$ docker pull julia@sha256:62dd3e54b72b91579a3a3c47abac8c3e1c4c650870e6d36b014ab55f3dddfab6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:stretch` - linux; amd64

```console
$ docker pull julia@sha256:3b3d8b12fd4e4651f1f4fcb2f509bedb460efd90d6ec80621599f5826c7bc5ad
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.0 MB (132968291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc66946c2f9a9f577616099d7940bdc7a2ece67de840b3fc220247ff698cb474`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:29:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 01:29:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 01:29:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 01:29:47 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:48:20 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:48:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:48:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaedd87a38ec22b96ab4effc5c4424e4b77a803a72b4ddb0161f5f9a19a9b83`  
		Last Modified: Sat, 23 Nov 2019 01:33:03 GMT  
		Size: 7.6 MB (7555516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0c10e0170e5622c7fbf906bc9d2ef71ed34623ff9e9b08370d56e59f314897`  
		Last Modified: Wed, 27 Nov 2019 02:49:49 GMT  
		Size: 102.9 MB (102888203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:stretch` - linux; arm variant v7

```console
$ docker pull julia@sha256:91af6770b199cbbc68cca5694d05921abd7f1a188120c91f992911899d407343
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119163171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f503dd2a573a76cc88b828e38ad9b5ea48795272dbab3aecad6fc56479de45f`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:28:28 GMT
ADD file:9fcbe16260f606fbea9a4811e693312434fbc4b300e974d33dcac84808f2323c in / 
# Fri, 22 Nov 2019 13:28:29 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 23:54:13 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 23:54:14 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 23:54:15 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:23:31 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:24:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:24:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:d721220e5446968b6d6c8c3cd477d7deaadfd7f3ea7070342828f151408cbc93`  
		Last Modified: Fri, 22 Nov 2019 13:36:57 GMT  
		Size: 19.3 MB (19311578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18c33863683af64036006c88f0c10de16277a86e0b64377395dc562229459db`  
		Last Modified: Fri, 22 Nov 2019 23:59:23 GMT  
		Size: 6.3 MB (6292069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38492a6a3562f22c872fe1d132133268e0865c7e7c40a82bcd3717085388de4`  
		Last Modified: Wed, 27 Nov 2019 02:26:00 GMT  
		Size: 93.6 MB (93559524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:stretch` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:941a65e5fcae3f19414eb77024f9c5b0f56a7ab7095949dc26f0efac8ffc7063
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.9 MB (112909753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c42f11c3a72c2a3c1a087684e203dea7ede550f456d7cb8bcbeb3758b1bd5ab`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 21:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 21:25:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Fri, 22 Nov 2019 21:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 21:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 02:15:52 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 02:16:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 02:16:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d607c5cf53fc2fd360b3b9db3ec4f913a3464c9638a99792a4773eb8747897f`  
		Last Modified: Fri, 22 Nov 2019 21:30:36 GMT  
		Size: 6.5 MB (6526773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5421be62477a6f10881a9300a993af4a45a56462518f608090af6fab3a82e0`  
		Last Modified: Wed, 27 Nov 2019 02:18:13 GMT  
		Size: 86.0 MB (85997221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:stretch` - linux; 386

```console
$ docker pull julia@sha256:dbb14be9b1d9fff64e0168a478d5cb78db80886aff5f2d06816bed18456fcb59
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129699923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c385dbc091479a349913c9dc921da40d38b67b57afc097489117c574ff9bdd5`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 07:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 07:05:28 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 23 Nov 2019 07:05:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 07:05:28 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 27 Nov 2019 01:55:51 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 27 Nov 2019 01:56:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='9ec9e8076f65bef9ba1fb3c58037743c5abb3b53d845b827e44a37e7bcacffe8' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='7739a318f371250faf10befd5636008fbb84992cc90ee88b3a753b1ad408ad7c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='8557c86cb4f65e8d8c2b1da376e759548cb35942a63820a6d20bc1448c45ec1b' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='e43339e72b2e71f8df343e6f542bf3a48cbbf7e9c135b076d5d651d9153615c9' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 27 Nov 2019 01:56:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3add3465288c564759514e6470533c98709e4eb220ecc997d63cf40d0b38f05f`  
		Last Modified: Sat, 23 Nov 2019 07:08:45 GMT  
		Size: 7.6 MB (7582351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10d4a74ea93b5c5847256f5589a9666625162ffe17bfef1187878cfb978a299`  
		Last Modified: Wed, 27 Nov 2019 01:57:49 GMT  
		Size: 99.0 MB (98965502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `julia:windowsservercore-1809`

```console
$ docker pull julia@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `julia:windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:fcc13ec2a4deabaf456332de57a4deb15d8de966d654c531dc259215595aa7a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `julia:windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:4466de07b40c1ccef59af3ba9657c9bd0860ae48a5c64905996975fd98c36c8f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5851253362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e052b93d9ffa13c50ad0cc5a1adf4bc81224f0ecb84bf49897c21f470ff7ba2e`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:12:36 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 11 Dec 2019 18:12:37 GMT
ENV JULIA_SHA256=35af4b93188b2404a78026b583c7f010ecb17df2eabb9fc32de4737de28f31d5
# Wed, 11 Dec 2019 18:16:16 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:16:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bb6a227a3e35a2ac1412d7ce1f6d1fe0eb9ffef54d7fd0d942eda6a4a9e844`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895110186ac4672791f3312f5bb04163342b724e9e41e75ef5a12770627e6f6a`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87adc6544f789d6c8a086e47e9cd0e80a1fae0c26a74b3bd0c4362a9ba35ce65`  
		Last Modified: Wed, 11 Dec 2019 18:21:07 GMT  
		Size: 128.5 MB (128544729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a92f8fb56b5bcfe5c53c100e5ce668116c15207c92ed840adea2f14a0d6d60`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
